# Comparing `tmp/configuraptor-1.0.2.tar.gz` & `tmp/configuraptor-1.0.3.tar.gz`

## Comparing `configuraptor-1.0.2.tar` & `configuraptor-1.0.3.tar`

### file list

```diff
@@ -1,59 +1,71 @@
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 configuraptor-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.0.2/coverage.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 configuraptor-1.0.2/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.0.2/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.0.2/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.0.2/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.0.2/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 configuraptor-1.0.2/examples/dataclass.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 configuraptor-1.0.2/examples/main.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.0.2/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.0.2/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.0.2/pytest_examples/empty.toml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.0.2/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.0.2/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.0.2/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/cls.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/core.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_about.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_core.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_singleton.py
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.0.2/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 configuraptor-1.0.2/README.md
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 configuraptor-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 configuraptor-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 configuraptor-1.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.0.3/coverage.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 configuraptor-1.0.3/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.0.3/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.0.3/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.0.3/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.0.3/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/dataclass.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/example_from_docs.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/example_from_docs.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/main.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   119587 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.0.3/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.0.3/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.0.3/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.0.3/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    13973 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_about.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_core.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 configuraptor-1.0.3/README.md
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 configuraptor-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 configuraptor-1.0.3/PKG-INFO
```

### Comparing `configuraptor-1.0.2/CHANGELOG.md` & `configuraptor-1.0.3/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.0.3 (2023-06-14)
+### Fix
+* **core:** Checking for a required parameterized type (e.g. list[str]) crashed for a missing key (with the wrong error) ([`68ccc1c`](https://github.com/trialandsuccess/configuraptor/commit/68ccc1c44e29c940d14acd6ce6b49e9885eaa03a))
+
+### Documentation
+* **readme:** Added first example code ([`da0b13d`](https://github.com/trialandsuccess/configuraptor/commit/da0b13d6e90fb0d26b1f33d804657a21304be745))
+* **changelog:** Manually added changes ([`c1c40ef`](https://github.com/trialandsuccess/configuraptor/commit/c1c40efb568abec30578d38a0a92d97f398fc23b))
+* **image:** Set height ([`78896b8`](https://github.com/trialandsuccess/configuraptor/commit/78896b8a53109c22e8c0875195dd486667a432f0))
+
 ## v1.0.2 (2023-06-14)
 ### Documentation
 * set image size
 
 ### Build
 * added `hatch` as dev dependency
```

### Comparing `configuraptor-1.0.2/coverage.svg` & `configuraptor-1.0.3/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/_static/configuraptor_circle.png` & `configuraptor-1.0.3/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/_static/configuraptor_original.jpeg` & `configuraptor-1.0.3/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/_static/configuraptor_round.png` & `configuraptor-1.0.3/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/_static/configuraptor_transparent.png` & `configuraptor-1.0.3/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/examples/dataclass.py` & `configuraptor-1.0.3/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/examples/main.py` & `configuraptor-1.0.3/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/examples/typedconfig_class.py` & `configuraptor-1.0.3/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/coverage_html.js` & `configuraptor-1.0.3/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/favicon_32.png` & `configuraptor-1.0.3/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/index.html` & `configuraptor-1.0.3/htmlcov/index.html`

 * *Files 17% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-13 19:33 +0200
+            created at 2023-06-14 11:44 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -58,108 +58,108 @@
                 <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing</th>
                 <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded</th>
                 <th class="right" aria-sort="none" data-shortcut="c">coverage</th>
             </tr>
         </thead>
         <tbody>
             <tr class="file">
-                <td class="name left"><a href="d_47560703719c1d9e___about___py.html">src/typedconfig/__about__.py</a></td>
+                <td class="name left"><a href="d_eb75b6cf8f5eab40___about___py.html">src/configuraptor/__about__.py</a></td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_47560703719c1d9e___init___py.html">src/typedconfig/__init__.py</a></td>
+                <td class="name left"><a href="d_eb75b6cf8f5eab40___init___py.html">src/configuraptor/__init__.py</a></td>
                 <td>3</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="3 3">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_47560703719c1d9e_cls_py.html">src/typedconfig/cls.py</a></td>
+                <td class="name left"><a href="d_eb75b6cf8f5eab40_cls_py.html">src/configuraptor/cls.py</a></td>
                 <td>7</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="7 7">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_47560703719c1d9e_core_py.html">src/typedconfig/core.py</a></td>
-                <td>142</td>
+                <td class="name left"><a href="d_eb75b6cf8f5eab40_core_py.html">src/configuraptor/core.py</a></td>
+                <td>144</td>
                 <td>0</td>
                 <td>3</td>
-                <td class="right" data-ratio="142 142">100%</td>
+                <td class="right" data-ratio="144 144">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_47560703719c1d9e_errors_py.html">src/typedconfig/errors.py</a></td>
+                <td class="name left"><a href="d_eb75b6cf8f5eab40_errors_py.html">src/configuraptor/errors.py</a></td>
                 <td>26</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="26 26">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_47560703719c1d9e_helpers_py.html">src/typedconfig/helpers.py</a></td>
+                <td class="name left"><a href="d_eb75b6cf8f5eab40_helpers_py.html">src/configuraptor/helpers.py</a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_31a2a1dc9b603870___init___py.html">src/typedconfig/loaders/__init__.py</a></td>
+                <td class="name left"><a href="d_6c7dc8b73849fb97___init___py.html">src/configuraptor/loaders/__init__.py</a></td>
                 <td>4</td>
                 <td>0</td>
                 <td>2</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_31a2a1dc9b603870_loaders_310_py.html">src/typedconfig/loaders/loaders_310.py</a></td>
+                <td class="name left"><a href="d_6c7dc8b73849fb97_loaders_310_py.html">src/configuraptor/loaders/loaders_310.py</a></td>
                 <td>5</td>
                 <td>0</td>
                 <td>6</td>
                 <td class="right" data-ratio="5 5">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_31a2a1dc9b603870_loaders_311_py.html">src/typedconfig/loaders/loaders_311.py</a></td>
+                <td class="name left"><a href="d_6c7dc8b73849fb97_loaders_311_py.html">src/configuraptor/loaders/loaders_311.py</a></td>
                 <td>6</td>
                 <td>0</td>
                 <td>2</td>
                 <td class="right" data-ratio="6 6">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_47560703719c1d9e_singleton_py.html">src/typedconfig/singleton.py</a></td>
+                <td class="name left"><a href="d_eb75b6cf8f5eab40_singleton_py.html">src/configuraptor/singleton.py</a></td>
                 <td>13</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="13 13">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>209</td>
+                <td>211</td>
                 <td>0</td>
                 <td>13</td>
-                <td class="right" data-ratio="209 209">100%</td>
+                <td class="right" data-ratio="211 211">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-13 19:33 +0200
+            created at 2023-06-14 11:44 +0200
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="d_47560703719c1d9e_singleton_py.html"/>
-        <a id="nextFileLink" class="nav" href="d_47560703719c1d9e___about___py.html"/>
+        <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html"/>
+        <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
         <button type="button" class="button_show_hide_help" data-shortcut="?"/>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -2,25 +2,25 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-06-13 19:33 +0200
+coverage.py_v7.2.7, created at 2023-06-14 11:44 +0200
 
-Module                                 statements missing excluded coverage
-src/typedconfig/__about__.py           1          0       0        100%
-src/typedconfig/__init__.py            3          0       0        100%
-src/typedconfig/cls.py                 7          0       0        100%
-src/typedconfig/core.py                142        0       3        100%
-src/typedconfig/errors.py              26         0       0        100%
-src/typedconfig/helpers.py             2          0       0        100%
-src/typedconfig/loaders/__init__.py    4          0       2        100%
-src/typedconfig/loaders/loaders_310.py 5          0       6        100%
-src/typedconfig/loaders/loaders_311.py 6          0       2        100%
-src/typedconfig/singleton.py           13         0       0        100%
-Total                                  209        0       13       100%
+Module                                   statements missing excluded coverage
+src/configuraptor/__about__.py           1          0       0        100%
+src/configuraptor/__init__.py            3          0       0        100%
+src/configuraptor/cls.py                 7          0       0        100%
+src/configuraptor/core.py                144        0       3        100%
+src/configuraptor/errors.py              26         0       0        100%
+src/configuraptor/helpers.py             2          0       0        100%
+src/configuraptor/loaders/__init__.py    4          0       2        100%
+src/configuraptor/loaders/loaders_310.py 5          0       6        100%
+src/configuraptor/loaders/loaders_311.py 6          0       2        100%
+src/configuraptor/singleton.py           13         0       0        100%
+Total                                    211        0       13       100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-06-13 19:33 +0200
+coverage.py_v7.2.7, created at 2023-06-14 11:44 +0200
  ____
```

### Comparing `configuraptor-1.0.2/htmlcov/keybd_closed.png` & `configuraptor-1.0.3/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/keybd_open.png` & `configuraptor-1.0.3/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/htmlcov/style.css` & `configuraptor-1.0.3/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/pytest_examples/some.toml` & `configuraptor-1.0.3/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/src/configuraptor/cls.py` & `configuraptor-1.0.3/src/configuraptor/cls.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/src/configuraptor/core.py` & `configuraptor-1.0.3/src/configuraptor/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,19 @@
         None -> True
         NoneType -> True
         typing.Union[str, None] -> True
         str | None -> True
         list[str | None] -> False
         list[str] -> False
     """
+    if _type and is_parameterized(_type) and typing.get_origin(_type) in (dict, list):
+        # e.g. list[str]
+        # will crash issubclass to test it first here
+        return False
+
     return (
         _type is None
         or issubclass(types.NoneType, _type)
         or issubclass(types.NoneType, type(_type))  # no type  # Nonetype
         or type(None) in typing.get_args(_type)  # union with Nonetype
     )
```

### Comparing `configuraptor-1.0.2/src/configuraptor/errors.py` & `configuraptor-1.0.3/src/configuraptor/errors.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/src/configuraptor/singleton.py` & `configuraptor-1.0.3/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/tests/test_singleton.py` & `configuraptor-1.0.3/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/tests/test_toml_basic.py` & `configuraptor-1.0.3/tests/test_toml_basic.py`

 * *Files 20% similar despite different names*

```diff
@@ -184,7 +184,19 @@
 def test_dict_of_custom():
     file = PYTEST_EXAMPLES / "with_dict_of_custom.toml"
 
     structure = configuraptor.load_into(Structure, file)
     for key, value in structure.contents.items():
         assert isinstance(key, str)
         assert isinstance(value, Point)
+
+
+class ShouldHaveListOfString:
+    required: list[str]
+    not_required: typing.Optional[list[str]]
+
+
+def test_missing_required_parameterized():
+    # should go through is_optional -> is_parameterized -> typing.get_origin(_type) in (dict, list) -> False -> Error
+    data = {"not_required": ["list", "of", "string"]}
+    with pytest.raises(ConfigErrorMissingKey):
+        configuraptor.load_into(ShouldHaveListOfString, data, key='')  # empty key to indicate data exists top-level
```

### Comparing `configuraptor-1.0.2/tests/test_toml_dataclass.py` & `configuraptor-1.0.3/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/tests/test_toml_existing.py` & `configuraptor-1.0.3/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/tests/test_toml_typedconfig_class.py` & `configuraptor-1.0.3/tests/test_toml_typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/LICENSE.txt` & `configuraptor-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.2/README.md` & `configuraptor-1.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -91,22 +91,99 @@
 000005a0: 7361 6765 290a 2d20 5b4c 6963 656e 7365  sage).- [License
 000005b0: 5d28 236c 6963 656e 7365 290a 2d20 5b43  ](#license).- [C
 000005c0: 6861 6e67 656c 6f67 5d28 2363 6861 6e67  hangelog](#chang
 000005d0: 656c 6f67 290a 0a23 2320 496e 7374 616c  elog)..## Instal
 000005e0: 6c61 7469 6f6e 0a0a 6060 6063 6f6e 736f  lation..```conso
 000005f0: 6c65 0a70 6970 2069 6e73 7461 6c6c 2063  le.pip install c
 00000600: 6f6e 6669 6775 7261 7074 6f72 0a60 6060  onfiguraptor.```
-00000610: 0a0a 2323 2055 7361 6765 0a0a 2323 204c  ..## Usage..## L
-00000620: 6963 656e 7365 0a0a 6065 6477 6860 2069  icense..`edwh` i
-00000630: 7320 6469 7374 7269 6275 7465 6420 756e  s distributed un
-00000640: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
-00000650: 2074 6865 205b 4d49 545d 2868 7474 7073   the [MIT](https
-00000660: 3a2f 2f73 7064 782e 6f72 672f 6c69 6365  ://spdx.org/lice
-00000670: 6e73 6573 2f4d 4954 2e68 746d 6c29 206c  nses/MIT.html) l
-00000680: 6963 656e 7365 2e0a 0a23 2320 4368 616e  icense...## Chan
-00000690: 6765 6c6f 670a 0a5b 5365 6520 4348 414e  gelog..[See CHAN
-000006a0: 4745 4c4f 472e 6d64 5d28 6874 7470 733a  GELOG.md](https:
-000006b0: 2f2f 6769 7468 7562 2e63 6f6d 2f74 7269  //github.com/tri
-000006c0: 616c 616e 6473 7563 6365 7373 2f63 6f6e  alandsuccess/con
-000006d0: 6669 6775 7261 7074 6f72 2f62 6c6f 622f  figuraptor/blob/
-000006e0: 6d61 7374 6572 2f43 4841 4e47 454c 4f47  master/CHANGELOG
-000006f0: 2e6d 6429 0a                             .md).
+00000610: 0a0a 2323 2055 7361 6765 0a0a 436f 6e66  ..## Usage..Conf
+00000620: 6967 7572 6170 746f 7220 6361 6e20 6265  iguraptor can be
+00000630: 2075 7365 6420 746f 206c 6f61 6420 796f   used to load yo
+00000640: 7572 2063 6f6e 6669 6720 6669 6c65 7320  ur config files 
+00000650: 696e 746f 2073 7472 7563 7475 7265 6420  into structured 
+00000660: 5079 7468 6f6e 2063 6c61 7373 6573 2e0a  Python classes..
+00000670: 0a60 6060 746f 6d6c 0a23 2065 7861 6d70  .```toml.# examp
+00000680: 6c65 5f66 726f 6d5f 646f 6373 2e74 6f6d  le_from_docs.tom
+00000690: 6c0a 5b63 6f6e 6669 675d 0a6e 616d 6520  l.[config].name 
+000006a0: 3d20 2248 656c 6c6f 2057 6f72 6c64 2122  = "Hello World!"
+000006b0: 0a0a 5b63 6f6e 6669 672e 7265 6665 7265  ..[config.refere
+000006c0: 6e63 655d 0a6e 756d 6265 7220 3d20 3432  nce].number = 42
+000006d0: 0a6e 756d 6265 7273 203d 205b 3431 2c20  .numbers = [41, 
+000006e0: 3433 5d0a 7374 7269 6e67 203d 2022 3432  43].string = "42
+000006f0: 220a 6060 600a 0a43 6f75 6c64 2062 6520  ".```..Could be 
+00000700: 6c6f 6164 6564 2069 6e74 6f20 5079 7468  loaded into Pyth
+00000710: 6f6e 2063 6c61 7373 6573 2075 7369 6e67  on classes using
+00000720: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00000730: 6f64 653a 0a60 6060 7079 7468 6f6e 0a23  ode:.```python.#
+00000740: 2065 7861 6d70 6c65 5f66 726f 6d5f 646f   example_from_do
+00000750: 6373 2e70 790a 6672 6f6d 2063 6f6e 6669  cs.py.from confi
+00000760: 6775 7261 7074 6f72 2069 6d70 6f72 7420  guraptor import 
+00000770: 6c6f 6164 5f69 6e74 6f2c 2054 7970 6564  load_into, Typed
+00000780: 436f 6e66 6967 0a0a 2323 2323 2323 2323  Config..########
+00000790: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
+000007a0: 2077 6974 6820 6261 7369 6320 636c 6173   with basic clas
+000007b0: 7365 7320 230a 2323 2323 2323 2323 2323  ses #.##########
+000007c0: 2323 2323 2323 2323 2323 2323 0a0a 636c  ############..cl
+000007d0: 6173 7320 536f 6d65 5265 6775 6c61 7243  ass SomeRegularC
+000007e0: 6c61 7373 3a0a 2020 2020 6e75 6d62 6572  lass:.    number
+000007f0: 3a20 696e 740a 2020 2020 6e75 6d62 6572  : int.    number
+00000800: 733a 206c 6973 745b 696e 745d 0a20 2020  s: list[int].   
+00000810: 2073 7472 696e 673a 2073 7472 0a0a 0a63   string: str...c
+00000820: 6c61 7373 2043 6f6e 6669 673a 0a20 2020  lass Config:.   
+00000830: 206e 616d 653a 2073 7472 0a20 2020 2072   name: str.    r
+00000840: 6566 6572 656e 6365 3a20 536f 6d65 5265  eference: SomeRe
+00000850: 6775 6c61 7243 6c61 7373 0a0a 0a69 6620  gularClass...if 
+00000860: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+00000870: 6169 6e5f 5f27 3a0a 2020 2020 6d79 5f63  ain__':.    my_c
+00000880: 6f6e 6669 6720 3d20 6c6f 6164 5f69 6e74  onfig = load_int
+00000890: 6f28 436f 6e66 6967 2c20 2265 7861 6d70  o(Config, "examp
+000008a0: 6c65 5f66 726f 6d5f 646f 6373 2e74 6f6d  le_from_docs.tom
+000008b0: 6c22 290a 0a20 2020 2070 7269 6e74 286d  l")..    print(m
+000008c0: 795f 636f 6e66 6967 2e6e 616d 6529 0a20  y_config.name). 
+000008d0: 2020 2023 2048 656c 6c6f 2057 6f72 6c64     # Hello World
+000008e0: 210a 2020 2020 7072 696e 7428 6d79 5f63  !.    print(my_c
+000008f0: 6f6e 6669 672e 7265 6665 7265 6e63 652e  onfig.reference.
+00000900: 6e75 6d62 6572 7329 0a20 2020 2023 205b  numbers).    # [
+00000910: 3431 2c20 3433 5d0a 0a0a 2323 2323 2323  41, 43]...######
+00000920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000930: 2323 0a23 2061 6c74 6572 6e61 7469 7665  ##.# alternative
+00000940: 206e 6f74 6174 696f 6e20 230a 2323 2323   notation #.####
+00000950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000960: 2323 2323 0a0a 636c 6173 7320 536f 6d65  ####..class Some
+00000970: 4f74 6865 7252 6567 756c 6172 436c 6173  OtherRegularClas
+00000980: 733a 0a20 2020 206e 756d 6265 723a 2069  s:.    number: i
+00000990: 6e74 0a20 2020 206e 756d 6265 7273 3a20  nt.    numbers: 
+000009a0: 6c69 7374 5b69 6e74 5d0a 2020 2020 7374  list[int].    st
+000009b0: 7269 6e67 3a20 7374 720a 0a0a 636c 6173  ring: str...clas
+000009c0: 7320 4f74 6865 7243 6f6e 6669 6728 5479  s OtherConfig(Ty
+000009d0: 7065 6443 6f6e 6669 6729 3a0a 2020 2020  pedConfig):.    
+000009e0: 6e61 6d65 3a20 7374 720a 2020 2020 7265  name: str.    re
+000009f0: 6665 7265 6e63 653a 2053 6f6d 6552 6567  ference: SomeReg
+00000a00: 756c 6172 436c 6173 730a 0a0a 6966 205f  ularClass...if _
+00000a10: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
+00000a20: 696e 5f5f 273a 0a20 2020 206d 795f 636f  in__':.    my_co
+00000a30: 6e66 6967 203d 204f 7468 6572 436f 6e66  nfig = OtherConf
+00000a40: 6967 2e6c 6f61 6428 2265 7861 6d70 6c65  ig.load("example
+00000a50: 5f66 726f 6d5f 646f 6373 2e74 6f6d 6c22  _from_docs.toml"
+00000a60: 290a 0a20 2020 2070 7269 6e74 286d 795f  )..    print(my_
+00000a70: 636f 6e66 6967 2e6e 616d 6529 0a20 2020  config.name).   
+00000a80: 2023 2048 656c 6c6f 2057 6f72 6c64 210a   # Hello World!.
+00000a90: 2020 2020 7072 696e 7428 6d79 5f63 6f6e      print(my_con
+00000aa0: 6669 672e 7265 6665 7265 6e63 652e 6e75  fig.reference.nu
+00000ab0: 6d62 6572 7329 0a20 2020 2023 205b 3431  mbers).    # [41
+00000ac0: 2c20 3433 5d0a 6060 600a 0a4d 6f72 6520  , 43].```..More 
+00000ad0: 6578 616d 706c 6573 2077 696c 6c20 6265  examples will be
+00000ae0: 2061 7661 696c 6162 6c65 2073 6f6f 6e2e   available soon.
+00000af0: 0a0a 2323 204c 6963 656e 7365 0a0a 6065  ..## License..`e
+00000b00: 6477 6860 2069 7320 6469 7374 7269 6275  dwh` is distribu
+00000b10: 7465 6420 756e 6465 7220 7468 6520 7465  ted under the te
+00000b20: 726d 7320 6f66 2074 6865 205b 4d49 545d  rms of the [MIT]
+00000b30: 2868 7474 7073 3a2f 2f73 7064 782e 6f72  (https://spdx.or
+00000b40: 672f 6c69 6365 6e73 6573 2f4d 4954 2e68  g/licenses/MIT.h
+00000b50: 746d 6c29 206c 6963 656e 7365 2e0a 0a23  tml) license...#
+00000b60: 2320 4368 616e 6765 6c6f 670a 0a5b 5365  # Changelog..[Se
+00000b70: 6520 4348 414e 4745 4c4f 472e 6d64 5d28  e CHANGELOG.md](
+00000b80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000b90: 6f6d 2f74 7269 616c 616e 6473 7563 6365  om/trialandsucce
+00000ba0: 7373 2f63 6f6e 6669 6775 7261 7074 6f72  ss/configuraptor
+00000bb0: 2f62 6c6f 622f 6d61 7374 6572 2f43 4841  /blob/master/CHA
+00000bc0: 4e47 454c 4f47 2e6d 6429 0a              NGELOG.md).
```

### Comparing `configuraptor-1.0.2/pyproject.toml` & `configuraptor-1.0.3/pyproject.toml`

 * *Files identical despite different names*

