# Comparing `tmp/configuraptor-1.0.1.tar.gz` & `tmp/configuraptor-1.0.2.tar.gz`

## Comparing `configuraptor-1.0.1.tar` & `configuraptor-1.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 configuraptor-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.0.1/coverage.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 configuraptor-1.0.1/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.0.1/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.0.1/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.0.1/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.0.1/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 configuraptor-1.0.1/examples/dataclass.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 configuraptor-1.0.1/examples/main.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.0.1/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.0.1/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.0.1/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.0.1/pytest_examples/empty.toml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.0.1/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.0.1/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.0.1/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/cls.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/core.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 configuraptor-1.0.1/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.0.1/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.0.1/tests/test_about.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 configuraptor-1.0.1/tests/test_core.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.0.1/tests/test_singleton.py
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 configuraptor-1.0.1/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 configuraptor-1.0.1/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.0.1/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.0.1/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.0.1/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 configuraptor-1.0.1/README.md
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 configuraptor-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 configuraptor-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 configuraptor-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.0.2/coverage.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 configuraptor-1.0.2/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.0.2/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.0.2/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.0.2/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.0.2/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 configuraptor-1.0.2/examples/dataclass.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 configuraptor-1.0.2/examples/main.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.0.2/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.0.2/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.0.2/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.0.2/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.0.2/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.0.2/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.0.2/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 configuraptor-1.0.2/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_about.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_core.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_singleton.py
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.0.2/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 configuraptor-1.0.2/README.md
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 configuraptor-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 configuraptor-1.0.2/PKG-INFO
```

### Comparing `configuraptor-1.0.1/CHANGELOG.md` & `configuraptor-1.0.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.0.2 (2023-06-14)
+### Documentation
+* set image size
+
+### Build
+* added `hatch` as dev dependency
+
 ## v1.0.1 (2023-06-14)
 ### Documentation
 * Fix changelog and url in readme ([`59bc18b`](https://github.com/trialandsuccess/configuraptor/commit/59bc18ba5d968b5275253d1637d4f5ef3aa3182b))
 
 ## v1.0.0 (2023-06-14)
 ### BREAKING CHANGE
 * renamed to 'configuraptor'
```

### Comparing `configuraptor-1.0.1/coverage.svg` & `configuraptor-1.0.2/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/_static/configuraptor_circle.png` & `configuraptor-1.0.2/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/_static/configuraptor_original.jpeg` & `configuraptor-1.0.2/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/_static/configuraptor_round.png` & `configuraptor-1.0.2/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/_static/configuraptor_transparent.png` & `configuraptor-1.0.2/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/examples/dataclass.py` & `configuraptor-1.0.2/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/examples/main.py` & `configuraptor-1.0.2/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/examples/typedconfig_class.py` & `configuraptor-1.0.2/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/coverage_html.js` & `configuraptor-1.0.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.0.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.0.2/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/favicon_32.png` & `configuraptor-1.0.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/index.html` & `configuraptor-1.0.2/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/keybd_closed.png` & `configuraptor-1.0.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/keybd_open.png` & `configuraptor-1.0.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/status.json` & `configuraptor-1.0.2/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/htmlcov/style.css` & `configuraptor-1.0.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/pytest_examples/some.toml` & `configuraptor-1.0.2/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/src/configuraptor/cls.py` & `configuraptor-1.0.2/src/configuraptor/cls.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/src/configuraptor/core.py` & `configuraptor-1.0.2/src/configuraptor/core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/src/configuraptor/errors.py` & `configuraptor-1.0.2/src/configuraptor/errors.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/src/configuraptor/singleton.py` & `configuraptor-1.0.2/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/tests/test_singleton.py` & `configuraptor-1.0.2/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/tests/test_toml_basic.py` & `configuraptor-1.0.2/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/tests/test_toml_dataclass.py` & `configuraptor-1.0.2/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/tests/test_toml_existing.py` & `configuraptor-1.0.2/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/tests/test_toml_typedconfig_class.py` & `configuraptor-1.0.2/tests/test_toml_typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/LICENSE.txt` & `configuraptor-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/README.md` & `configuraptor-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 <div align="center">
-    <img align="center" src="https://raw.githubusercontent.com/trialandsuccess/configuraptor/master/_static/configuraptor_circle.png" alt="Classy Configuraptor">
+    <img 
+        align="center" 
+        src="https://raw.githubusercontent.com/trialandsuccess/configuraptor/master/_static/configuraptor_circle.png" 
+        alt="Classy Configuraptor"
+        height="400px"
+        />
     <h1 align="center">Configuraptor</h1>
 </div>
 
 <div align="center">
     Load toml/yaml/json config files into classes for a typed config (type hinting etc.).
 </div>
 
@@ -39,8 +44,8 @@
 
 ## License
 
 `edwh` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Changelog
 
-[See CHANGELOG.md](https://github.com/trialandsuccess/configuraptor/blob/master/CHANGELOG.md)
+[See CHANGELOG.md](https://github.com/trialandsuccess/configuraptor/blob/master/CHANGELOG.md)
```

### Comparing `configuraptor-1.0.1/pyproject.toml` & `configuraptor-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.1/PKG-INFO` & `configuraptor-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.0.1
+Version: 1.0.2
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -20,15 +20,20 @@
 Requires-Dist: typeguard
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: su6[all]; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <div align="center">
-    <img align="center" src="https://raw.githubusercontent.com/trialandsuccess/configuraptor/master/_static/configuraptor_circle.png" alt="Classy Configuraptor">
+    <img 
+        align="center" 
+        src="https://raw.githubusercontent.com/trialandsuccess/configuraptor/master/_static/configuraptor_circle.png" 
+        alt="Classy Configuraptor"
+        height="400px"
+        />
     <h1 align="center">Configuraptor</h1>
 </div>
 
 <div align="center">
     Load toml/yaml/json config files into classes for a typed config (type hinting etc.).
 </div>
 
@@ -64,8 +69,8 @@
 
 ## License
 
 `edwh` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Changelog
 
-[See CHANGELOG.md](https://github.com/trialandsuccess/configuraptor/blob/master/CHANGELOG.md)
+[See CHANGELOG.md](https://github.com/trialandsuccess/configuraptor/blob/master/CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: configuraptor Version: 1.0.1 Summary: Load toml/
+Metadata-Version: 2.1 Name: configuraptor Version: 1.0.2 Summary: Load toml/
 yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/
 configuraptor#readme Project-URL: Issues, https://github.com/trialandsuccess/
 configuraptor/issues Project-URL: Source, https://github.com/trialandsuccess/
 configuraptor Author-email: Robin van der Noord
 trialandsuccess.nl> License-Expression: MIT License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
```

