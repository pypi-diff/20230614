# Comparing `tmp/configuraptor-1.1.2.tar.gz` & `tmp/configuraptor-1.2.0.tar.gz`

## Comparing `configuraptor-1.1.2.tar` & `configuraptor-1.2.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 configuraptor-1.1.2/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.1.2/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.1.2/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.1.2/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.1.2/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.1.2/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.1.2/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/dataclass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/example_from_docs.json
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/example_from_docs.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/example_from_docs.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/example_from_docs.yaml
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/main.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   124672 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/cls.py
--rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/core.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_about.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_core.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_json_yaml.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.1.2/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 configuraptor-1.1.2/README.md
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 configuraptor-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 configuraptor-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.2.0/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.2.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.2.0/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.2.0/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.2.0/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.2.0/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 configuraptor-1.2.0/examples/dataclass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.2.0/examples/example_from_docs.json
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.2.0/examples/example_from_docs.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.2.0/examples/example_from_docs.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.2.0/examples/example_from_docs.yaml
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.2.0/examples/main.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.2.0/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.2.0/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   124666 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.2.0/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.2.0/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.2.0/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.2.0/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.2.0/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.2.0/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.2.0/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.2.0/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    14512 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.2.0/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.2.0/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.2.0/tests/test_about.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 configuraptor-1.2.0/tests/test_core.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.2.0/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.2.0/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.2.0/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.2.0/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.2.0/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.2.0/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 configuraptor-1.2.0/README.md
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 configuraptor-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 configuraptor-1.2.0/PKG-INFO
```

### Comparing `configuraptor-1.1.2/CHANGELOG.md` & `configuraptor-1.2.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.2.0 (2023-06-14)
+### Feature
+* **lib:** Expose more methods externally + make second arg of all_annotations optional ([`63605ba`](https://github.com/trialandsuccess/configuraptor/commit/63605babb48ac2313e063def86608f82628688b7))
+
 ## v1.1.2 (2023-06-14)
 ### Fix
 * **dataclass:** Support for default_factory ([`031c68d`](https://github.com/trialandsuccess/configuraptor/commit/031c68d676fd59529e41debc480235a29f206405))
 
 ### Documentation
 * **readme:** Wrong package name oops ([`a9f7fad`](https://github.com/trialandsuccess/configuraptor/commit/a9f7fad7483dd55ff76655ec3a8feda9d55beef8))
```

### Comparing `configuraptor-1.1.2/coverage.svg` & `configuraptor-1.2.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/_static/configuraptor_circle.png` & `configuraptor-1.2.0/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/_static/configuraptor_original.jpeg` & `configuraptor-1.2.0/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/_static/configuraptor_round.png` & `configuraptor-1.2.0/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/_static/configuraptor_transparent.png` & `configuraptor-1.2.0/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/examples/dataclass.py` & `configuraptor-1.2.0/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/examples/example_from_docs.py` & `configuraptor-1.2.0/examples/example_from_docs.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/examples/main.py` & `configuraptor-1.2.0/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/examples/typedconfig_class.py` & `configuraptor-1.2.0/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/coverage_html.js` & `configuraptor-1.2.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.2.0/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.2.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.2.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.2.0/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.2.0/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.2.0/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.2.0/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.2.0/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.2.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.2.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.2.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 15:56 +0200
+            created at 2023-06-14 16:09 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,23 +83,23 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This file contains the module version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.1.1"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.1.2"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 15:56 +0200
+            created at 2023-06-14 16:09 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,22 +7,22 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   1 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 15:56 +0200
+at 2023-06-14 16:09 +0200
 
 
 1""" 
 2This file contains the module version. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "1.1.1" 
+8__version__ = "1.1.2" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 15:56 +0200
+at 2023-06-14 16:09 +0200
```

### Comparing `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/__init__.py: 100%</title>
+    <title>Coverage for src/configuraptor/helpers.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/__init__.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/helpers.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,23 +50,23 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">3 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">3<span class="text"> run</span></button>
+            <span class="text">2 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
             created at 2023-06-14 11:42 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
@@ -77,33 +77,33 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Exposes TypedConfig and load_into for this library.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Contains stand-alone helper functions.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">cls</span> <span class="key">import</span> <span class="nam">TypedConfig</span>  <span class="com"># noqa: F401 imported for library reasons</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">load_into</span>  <span class="com"># noqa: F401 imported for library reasons</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">singleton</span> <span class="key">import</span> <span class="op">(</span>  <span class="com"># noqa: F401 imported for library reasons</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">Singleton</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">SingletonMeta</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">def</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">s</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="str">    Convert CamelCase to snake_case.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    Source:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">        https://stackoverflow.com/questions/1175208/elegant-python-function-to-convert-camelcase-to-snake-case</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">return</span> <span class="str">""</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="op">[</span><span class="str">f"_{c.lower()}"</span> <span class="key">if</span> <span class="nam">c</span><span class="op">.</span><span class="nam">isupper</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">c</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">s</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
             created at 2023-06-14 11:42 +0200
         </p>
     </div>
 </footer>
 </body>
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
 
-****** Coverage for src/configuraptor/__init__.py: 100% ******
+****** Coverage for src/configuraptor/helpers.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 3 statements   3 run 0 missing 0 excluded *****
+***** 2 statements   2 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
 at 2023-06-14 11:42 +0200
 
 
 1""" 
-2Exposes TypedConfig and load_into for this library. 
+2Contains stand-alone helper functions. 
 3""" 
 4 
-5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
-<robinvandernoord@gmail.com> 
-6# 
-7# SPDX-License-Identifier: MIT 
-8from .cls import TypedConfig # noqa: F401 imported for library reasons 
-9from .core import load_into # noqa: F401 imported for library reasons 
-10from .singleton import ( # noqa: F401 imported for library reasons 
-11 Singleton, 
-12 SingletonMeta, 
-13) 
+5 
+6def camel_to_snake(s: str) -> str: 
+7 """ 
+8 Convert CamelCase to snake_case. 
+9 
+10 Source: 
+11 https://stackoverflow.com/questions/1175208/elegant-python-function-to-
+convert-camelcase-to-snake-case 
+12 """ 
+13 return "".join([f"_{c.lower()}" if c.isupper() else c for c in s]).lstrip
+("_") 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
 at 2023-06-14 11:42 +0200
```

### Comparing `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">150 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">150<span class="text"> run</span></button>
+            <span class="text">152 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">152<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">3<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 15:57 +0200
+            created at 2023-06-14 16:11 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,19 +80,19 @@
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Contains most of the loading logic.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">types</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">warnings</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">ChainMap</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">dataclasses</span> <span class="key">as</span> <span class="nam">dc</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">dataclasses</span> <span class="key">as</span> <span class="nam">dc</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">types</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">warnings</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">ChainMap</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">typeguard</span> <span class="key">import</span> <span class="nam">TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">typeguard</span> <span class="key">import</span> <span class="nam">check_type</span> <span class="key">as</span> <span class="nam">_check_type</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">loaders</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">,</span> <span class="nam">ConfigErrorMissingKey</span>&nbsp;</span><span class="r"></span></p>
@@ -292,15 +292,15 @@
     <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="nam">_type</span> <span class="key">is</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>  <span class="com"># no type  # Nonetype</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">        <span class="key">or</span> <span class="nam">type</span><span class="op">(</span><span class="key">None</span><span class="op">)</span> <span class="key">in</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>  <span class="com"># union with Nonetype</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="key">def</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">dc</span><span class="op">.</span><span class="nam">Field</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="key">def</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">dc</span><span class="op">.</span><span class="nam">Field</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">    Get Field info for a dataclass cls.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__dataclass_fields__"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">    <span class="key">return</span> <span class="nam">fields</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
@@ -329,231 +329,228 @@
     <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="str">        # step 2</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t"><span class="str">        cls = First</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">        data = {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="str">        annotations: {"key": str}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">    <span class="nam">updated</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="key">for</span> <span class="nam">_key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="key">if</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">            <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span> <span class="op">=</span> <span class="nam">data</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>  <span class="com"># value can change so define it as any instead of T</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">            <span class="key">if</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">                <span class="nam">origin</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">                <span class="key">if</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">list</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">                    <span class="nam">subtype</span> <span class="op">=</span> <span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">subtype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">dict</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">                    <span class="com"># e.g. dict[str, Point]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">                    <span class="nam">subkeytype</span><span class="op">,</span> <span class="nam">subvaluetype</span> <span class="op">=</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">                    <span class="com"># subkey(type) is not a custom class, so don't try to convert it:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">subkey</span><span class="op">:</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">subvaluetype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subkey</span><span class="op">,</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">                <span class="com"># elif origin is dict:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">                <span class="com"># keep data the same</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span> <span class="key">and</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">                    <span class="key">for</span> <span class="nam">arg</span> <span class="key">in</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">                        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">                            <span class="nam">value</span> <span class="op">=</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">arg</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">                            <span class="com"># print(_type, arg, value)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">                            <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">    <span class="nam">updated</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">    <span class="key">for</span> <span class="nam">_key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">        <span class="key">if</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">            <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span> <span class="op">=</span> <span class="nam">data</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>  <span class="com"># value can change so define it as any instead of T</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">            <span class="key">if</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">                <span class="nam">origin</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">                <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">                <span class="key">if</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">list</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                    <span class="nam">subtype</span> <span class="op">=</span> <span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">subtype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">dict</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">                    <span class="com"># e.g. dict[str, Point]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">                    <span class="nam">subkeytype</span><span class="op">,</span> <span class="nam">subvaluetype</span> <span class="op">=</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">                    <span class="com"># subkey(type) is not a custom class, so don't try to convert it:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">subkey</span><span class="op">:</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">subvaluetype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subkey</span><span class="op">,</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">                <span class="com"># elif origin is dict:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">                <span class="com"># keep data the same</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span> <span class="key">and</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">                    <span class="key">for</span> <span class="nam">arg</span> <span class="key">in</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">                        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">                            <span class="nam">value</span> <span class="op">=</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">arg</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">                            <span class="com"># print(_type, arg, value)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">                            <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">                <span class="com"># todo: other parameterized/unions/typing.Optional</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">                <span class="com"># todo: other parameterized/unions/typing.Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">            <span class="key">elif</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">                <span class="com"># type must be C (custom class) at this point</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">                    <span class="com"># make mypy and pycharm happy by telling it _type is of type C...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">                    <span class="com"># actually just passing _type as first arg!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">                    <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">Type_C</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">                    <span class="nam">value</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">        <span class="key">elif</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">            <span class="com"># property has default, use that instead.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">            <span class="com"># type is optional and not found in __dict__ -> default is None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">        <span class="key">elif</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">            <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">            <span class="key">and</span> <span class="op">(</span><span class="nam">field</span> <span class="op">:=</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_key</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">            <span class="key">and</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span> <span class="key">is</span> <span class="key">not</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">MISSING</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">        <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">            <span class="com"># could have a default factory</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">            <span class="com"># todo: do something with field.default?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">            <span class="com"># todo: exception group?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">        <span class="nam">updated</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="key">return</span> <span class="nam">updated</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t"><span class="key">def</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="str">    Based on class annotations, this prepares the data for `load_into_recurse`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">    1. convert config-keys to python compatible config_keys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="str">    2. loads custom class type annotations with the same logic (see also `load_recursive`)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t"><span class="str">    3. ensures the annotated types match the actual types after loading the config file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">_except</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="key">return</span> <span class="nam">to_load</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t"><span class="str">    Loads an instance of `cls` filled with `data`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t"><span class="str">    Uses `load_recursive` to load any fillable annotated properties (see that method for an example).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t"><span class="str">    `init` can be used to optionally pass extra __init__ arguments. \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t"><span class="str">        NOTE: This will overwrite a config key with the same name!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">        <span class="nam">init</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">    <span class="com"># fixme: cls.__init__ can set other keys than the name is in kwargs!!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">    <span class="key">if</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">init</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">|=</span> <span class="nam">init</span>  <span class="com"># add extra init variables (should not happen for a dataclass but whatev)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">        <span class="com"># ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">C</span><span class="op">,</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">        <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">            <span class="key">elif</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">                <span class="com"># type must be C (custom class) at this point</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">                    <span class="com"># make mypy and pycharm happy by telling it _type is of type C...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">                    <span class="com"># actually just passing _type as first arg!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">                    <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">Type_C</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">                    <span class="nam">value</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">        <span class="key">elif</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">            <span class="com"># property has default, use that instead.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">            <span class="com"># type is optional and not found in __dict__ -> default is None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">        <span class="key">elif</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span> <span class="key">and</span> <span class="op">(</span><span class="nam">field</span> <span class="op">:=</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_key</span><span class="op">)</span><span class="op">)</span> <span class="key">and</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span> <span class="key">is</span> <span class="key">not</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">MISSING</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">            <span class="com"># could have a default factory</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">            <span class="com"># todo: do something with field.default?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">            <span class="com"># todo: exception group?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">        <span class="nam">updated</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">    <span class="key">return</span> <span class="nam">updated</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">    <span class="key">if</span> <span class="nam">_except</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">        <span class="nam">_except</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t"><span class="key">def</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">    <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t"><span class="str">    Based on class annotations, this prepares the data for `load_into_recurse`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t"><span class="str">    1. convert config-keys to python compatible config_keys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="str">    2. loads custom class type annotations with the same logic (see also `load_recursive`)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t"><span class="str">    3. ensures the annotated types match the actual types after loading the config file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">_except</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="key">return</span> <span class="nam">to_load</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t"><span class="str">    Loads an instance of `cls` filled with `data`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t"><span class="str">    Uses `load_recursive` to load any fillable annotated properties (see that method for an example).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t"><span class="str">    `init` can be used to optionally pass extra __init__ arguments. \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t"><span class="str">        NOTE: This will overwrite a config key with the same name!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">        <span class="nam">init</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">    <span class="com"># fixme: cls.__init__ can set other keys than the name is in kwargs!!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">if</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">init</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">|=</span> <span class="nam">init</span>  <span class="com"># add extra init variables (should not happen for a dataclass but whatev)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">        <span class="com"># ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">C</span><span class="op">,</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">        <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_existing</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t"><span class="str">    Similar to `load_into_recurse` but uses an existing instance of a class (so after __init__) \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t"><span class="str">    and thus does not support init.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Can not init an existing instance!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">    <span class="nam">existing_data</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">existing_data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">    <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_existing</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t"><span class="str">    Similar to `load_into_recurse` but uses an existing instance of a class (so after __init__) \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t"><span class="str">    and thus does not support init.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Can not init an existing instance!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="nam">existing_data</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">existing_data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">    <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_class</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_recurse.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_existing.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">    <span class="nam">cls</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_existing</span><span class="op">(</span><span class="nam">inst</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span> <span class="op">|</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t"><span class="str">    Load your config into a class (instance).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t"><span class="str">        cls: either a class or an existing instance of that class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t"><span class="str">        data: can be a dictionary or a path to a file to load (as pathlib.Path or str)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t"><span class="str">        key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t"><span class="str">        init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into_instance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">    <span class="com"># make mypy and pycharm happy by telling it cls is of type C and not just 'type'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">    <span class="nam">_cls</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span> <span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_class</span><span class="op">(</span><span class="nam">_cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_class</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_recurse.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_existing.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t">    <span class="nam">cls</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_existing</span><span class="op">(</span><span class="nam">inst</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span> <span class="op">|</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t"><span class="str">    Load your config into a class (instance).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t"><span class="str">        cls: either a class or an existing instance of that class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t"><span class="str">        data: can be a dictionary or a path to a file to load (as pathlib.Path or str)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t"><span class="str">        key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t"><span class="str">        init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into_instance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">    <span class="com"># make mypy and pycharm happy by telling it cls is of type C and not just 'type'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">    <span class="nam">_cls</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span> <span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_class</span><span class="op">(</span><span class="nam">_cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 15:57 +0200
+            created at 2023-06-14 16:11 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,28 +5,28 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 150 statements   150 run 0 missing 3 excluded *****
+***** 152 statements   152 run 0 missing 3 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 15:57 +0200
+at 2023-06-14 16:11 +0200
 
 
 1""" 
 2Contains most of the loading logic. 
 3""" 
 4 
-5import types 
-6import typing 
-7import warnings 
-8from collections import ChainMap 
-9import dataclasses as dc 
+5import dataclasses as dc 
+6import types 
+7import typing 
+8import warnings 
+9from collections import ChainMap 
 10from pathlib import Path 
 11 
 12from typeguard import TypeCheckError 
 13from typeguard import check_type as _check_type 
 14 
 15from . import loaders 
 16from .errors import ConfigErrorInvalidType, ConfigErrorMissingKey 
@@ -240,15 +240,16 @@
 210 _type is None 
 211 or issubclass(types.NoneType, _type) 
 212 or issubclass(types.NoneType, type(_type)) # no type # Nonetype 
 213 or type(None) in typing.get_args(_type) # union with Nonetype 
 214 ) 
 215 
 216 
-217def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field]: 
+217def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field
+[typing.Any]]: 
 218 """ 
 219 Get Field info for a dataclass cls. 
 220 """ 
 221 fields = getattr(cls, "__dataclass_fields__", {}) 
 222 return fields.get(key) 
 223 
 224 
@@ -279,234 +280,232 @@
 247 
 248 # step 2 
 249 cls = First 
 250 data = {"key": "anything"} 
 251 annotations: {"key": str} 
 252 
 253 """ 
-254 
-255 updated = {} 
-256 for _key, _type in annotations.items(): 
-257 
-258 if _key in data: 
-259 value: typing.Any = data[_key] # value can change so define it as any
+254 updated = {} 
+255 for _key, _type in annotations.items(): 
+256 if _key in data: 
+257 value: typing.Any = data[_key] # value can change so define it as any
 instead of T 
-260 if is_parameterized(_type): 
-261 origin = typing.get_origin(_type) 
-262 arguments = typing.get_args(_type) 
-263 if origin is list and arguments and is_custom_class(arguments[0]): 
-264 subtype = arguments[0] 
-265 value = [load_into_recurse(subtype, subvalue) for subvalue in value] 
-266 
-267 elif origin is dict and arguments and is_custom_class(arguments[1]): 
-268 # e.g. dict[str, Point] 
-269 subkeytype, subvaluetype = arguments 
-270 # subkey(type) is not a custom class, so don't try to convert it: 
-271 value = {subkey: load_into_recurse(subvaluetype, subvalue) for subkey,
+258 if is_parameterized(_type): 
+259 origin = typing.get_origin(_type) 
+260 arguments = typing.get_args(_type) 
+261 if origin is list and arguments and is_custom_class(arguments[0]): 
+262 subtype = arguments[0] 
+263 value = [load_into_recurse(subtype, subvalue) for subvalue in value] 
+264 
+265 elif origin is dict and arguments and is_custom_class(arguments[1]): 
+266 # e.g. dict[str, Point] 
+267 subkeytype, subvaluetype = arguments 
+268 # subkey(type) is not a custom class, so don't try to convert it: 
+269 value = {subkey: load_into_recurse(subvaluetype, subvalue) for subkey,
 subvalue in value.items()} 
-272 # elif origin is dict: 
-273 # keep data the same 
-274 elif origin is typing.Union and arguments: 
-275 for arg in arguments: 
-276 if is_custom_class(arg): 
-277 value = load_into_recurse(arg, value) 
-278 else: 
-279 # print(_type, arg, value) 
-280 ... 
+270 # elif origin is dict: 
+271 # keep data the same 
+272 elif origin is typing.Union and arguments: 
+273 for arg in arguments: 
+274 if is_custom_class(arg): 
+275 value = load_into_recurse(arg, value) 
+276 else: 
+277 # print(_type, arg, value) 
+278 ... 
+279 
+280 # todo: other parameterized/unions/typing.Optional 
 281 
-282 # todo: other parameterized/unions/typing.Optional 
-283 
-284 elif is_custom_class(_type): 
-285 # type must be C (custom class) at this point 
-286 value = load_into_recurse( 
-287 # make mypy and pycharm happy by telling it _type is of type C... 
-288 # actually just passing _type as first arg! 
-289 typing.cast(Type_C[typing.Any], _type), 
-290 value, 
-291 ) 
-292 
-293 elif _key in cls.__dict__: 
-294 # property has default, use that instead. 
-295 value = cls.__dict__[_key] 
-296 elif is_optional(_type): 
-297 # type is optional and not found in __dict__ -> default is None 
-298 value = None 
-299 elif ( 
-300 dc.is_dataclass(cls) 
-301 and (field := dataclass_field(cls, _key)) 
-302 and field.default_factory is not dc.MISSING 
-303 ): 
-304 # could have a default factory 
-305 # todo: do something with field.default? 
-306 value = field.default_factory() 
-307 else: 
-308 # todo: exception group? 
-309 raise ConfigErrorMissingKey(_key, cls, _type) 
-310 
-311 updated[_key] = value 
-312 
-313 return updated 
-314 
-315 
-316def _all_annotations(cls: Type) -> ChainMap[str, Type]: 
-317 """ 
-318 Returns a dictionary-like ChainMap that includes annotations for all \ 
-319 attributes defined in cls or inherited from superclasses. 
-320 """ 
-321 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
+282 elif is_custom_class(_type): 
+283 # type must be C (custom class) at this point 
+284 value = load_into_recurse( 
+285 # make mypy and pycharm happy by telling it _type is of type C... 
+286 # actually just passing _type as first arg! 
+287 typing.cast(Type_C[typing.Any], _type), 
+288 value, 
+289 ) 
+290 
+291 elif _key in cls.__dict__: 
+292 # property has default, use that instead. 
+293 value = cls.__dict__[_key] 
+294 elif is_optional(_type): 
+295 # type is optional and not found in __dict__ -> default is None 
+296 value = None 
+297 elif dc.is_dataclass(cls) and (field := dataclass_field(cls, _key)) and
+field.default_factory is not dc.MISSING: 
+298 # could have a default factory 
+299 # todo: do something with field.default? 
+300 value = field.default_factory() 
+301 else: 
+302 # todo: exception group? 
+303 raise ConfigErrorMissingKey(_key, cls, _type) 
+304 
+305 updated[_key] = value 
+306 
+307 return updated 
+308 
+309 
+310def _all_annotations(cls: Type) -> ChainMap[str, Type]: 
+311 """ 
+312 Returns a dictionary-like ChainMap that includes annotations for all \ 
+313 attributes defined in cls or inherited from superclasses. 
+314 """ 
+315 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
 "__annotations__" in c.__dict__)) 
-322 
-323 
-324def all_annotations(cls: Type, _except: typing.Iterable[str]) -> dict[str,
-Type]: 
-325 """ 
-326 Wrapper around `_all_annotations` that filters away any keys in _except. 
-327 
-328 It also flattens the ChainMap to a regular dict. 
-329 """ 
-330 _all = _all_annotations(cls) 
-331 return {k: v for k, v in _all.items() if k not in _except} 
-332 
-333 
-334def _check_and_convert_data( 
-335 cls: typing.Type[C], 
-336 data: dict[str, typing.Any], 
-337 _except: typing.Iterable[str], 
-338) -> dict[str, typing.Any]: 
-339 """ 
-340 Based on class annotations, this prepares the data for
+316 
+317 
+318def all_annotations(cls: Type, _except: typing.Iterable[str] = None) -> dict
+[str, Type]: 
+319 """ 
+320 Wrapper around `_all_annotations` that filters away any keys in _except. 
+321 
+322 It also flattens the ChainMap to a regular dict. 
+323 """ 
+324 if _except is None: 
+325 _except = set() 
+326 
+327 _all = _all_annotations(cls) 
+328 return {k: v for k, v in _all.items() if k not in _except} 
+329 
+330 
+331def _check_and_convert_data( 
+332 cls: typing.Type[C], 
+333 data: dict[str, typing.Any], 
+334 _except: typing.Iterable[str], 
+335) -> dict[str, typing.Any]: 
+336 """ 
+337 Based on class annotations, this prepares the data for
 `load_into_recurse`. 
-341 
-342 1. convert config-keys to python compatible config_keys 
-343 2. loads custom class type annotations with the same logic (see also
+338 
+339 1. convert config-keys to python compatible config_keys 
+340 2. loads custom class type annotations with the same logic (see also
 `load_recursive`) 
-344 3. ensures the annotated types match the actual types after loading the
+341 3. ensures the annotated types match the actual types after loading the
 config file. 
-345 """ 
-346 annotations = all_annotations(cls, _except=_except) 
-347 
-348 to_load = convert_config(data) 
-349 to_load = load_recursive(cls, to_load, annotations) 
-350 to_load = ensure_types(to_load, annotations) 
-351 return to_load 
-352 
-353 
-354def load_into_recurse( 
-355 cls: typing.Type[C], 
-356 data: dict[str, typing.Any], 
-357 init: dict[str, typing.Any] = None, 
-358) -> C: 
-359 """ 
-360 Loads an instance of `cls` filled with `data`. 
-361 
-362 Uses `load_recursive` to load any fillable annotated properties (see that
+342 """ 
+343 annotations = all_annotations(cls, _except=_except) 
+344 
+345 to_load = convert_config(data) 
+346 to_load = load_recursive(cls, to_load, annotations) 
+347 to_load = ensure_types(to_load, annotations) 
+348 return to_load 
+349 
+350 
+351def load_into_recurse( 
+352 cls: typing.Type[C], 
+353 data: dict[str, typing.Any], 
+354 init: dict[str, typing.Any] = None, 
+355) -> C: 
+356 """ 
+357 Loads an instance of `cls` filled with `data`. 
+358 
+359 Uses `load_recursive` to load any fillable annotated properties (see that
 method for an example). 
-363 `init` can be used to optionally pass extra __init__ arguments. \ 
-364 NOTE: This will overwrite a config key with the same name! 
-365 """ 
-366 if init is None: 
-367 init = {} 
-368 
-369 # fixme: cls.__init__ can set other keys than the name is in kwargs!! 
-370 
-371 if dc.is_dataclass(cls): 
-372 to_load = _check_and_convert_data(cls, data, init.keys()) 
-373 to_load |= init # add extra init variables (should not happen for a
+360 `init` can be used to optionally pass extra __init__ arguments. \ 
+361 NOTE: This will overwrite a config key with the same name! 
+362 """ 
+363 if init is None: 
+364 init = {} 
+365 
+366 # fixme: cls.__init__ can set other keys than the name is in kwargs!! 
+367 
+368 if dc.is_dataclass(cls): 
+369 to_load = _check_and_convert_data(cls, data, init.keys()) 
+370 to_load |= init # add extra init variables (should not happen for a
 dataclass but whatev) 
-374 
-375 # ensure mypy inst is an instance of the cls type (and not a fictuous
+371 
+372 # ensure mypy inst is an instance of the cls type (and not a fictuous
 `DataclassInstance`) 
-376 inst = typing.cast(C, cls(**to_load)) 
-377 else: 
-378 inst = cls(**init) 
-379 to_load = _check_and_convert_data(cls, data, inst.__dict__.keys()) 
-380 inst.__dict__.update(**to_load) 
+373 inst = typing.cast(C, cls(**to_load)) 
+374 else: 
+375 inst = cls(**init) 
+376 to_load = _check_and_convert_data(cls, data, inst.__dict__.keys()) 
+377 inst.__dict__.update(**to_load) 
+378 
+379 return inst 
+380 
 381 
-382 return inst 
-383 
-384 
-385def load_into_existing( 
-386 inst: C, 
-387 cls: typing.Type[C], 
-388 data: dict[str, typing.Any], 
-389 init: dict[str, typing.Any] = None, 
-390) -> C: 
-391 """ 
-392 Similar to `load_into_recurse` but uses an existing instance of a class (so
+382def load_into_existing( 
+383 inst: C, 
+384 cls: typing.Type[C], 
+385 data: dict[str, typing.Any], 
+386 init: dict[str, typing.Any] = None, 
+387) -> C: 
+388 """ 
+389 Similar to `load_into_recurse` but uses an existing instance of a class (so
 after __init__) \ 
-393 and thus does not support init. 
-394 
-395 """ 
-396 if init is not None: 
-397 raise ValueError("Can not init an existing instance!") 
-398 
-399 existing_data = inst.__dict__ 
-400 
-401 annotations = all_annotations(cls, _except=existing_data.keys()) 
-402 to_load = convert_config(data) 
-403 to_load = load_recursive(cls, to_load, annotations) 
-404 to_load = ensure_types(to_load, annotations) 
-405 
-406 inst.__dict__.update(**to_load) 
+390 and thus does not support init. 
+391 
+392 """ 
+393 if init is not None: 
+394 raise ValueError("Can not init an existing instance!") 
+395 
+396 existing_data = inst.__dict__ 
+397 
+398 annotations = all_annotations(cls, _except=existing_data.keys()) 
+399 to_load = convert_config(data) 
+400 to_load = load_recursive(cls, to_load, annotations) 
+401 to_load = ensure_types(to_load, annotations) 
+402 
+403 inst.__dict__.update(**to_load) 
+404 
+405 return inst 
+406 
 407 
-408 return inst 
-409 
-410 
-411def load_into_class( 
-412 cls: typing.Type[C], 
-413 data: T_data, 
-414 /, 
-415 key: str = None, 
-416 init: dict[str, typing.Any] = None, 
-417) -> C: 
-418 """ 
-419 Shortcut for _load_data + load_into_recurse. 
-420 """ 
-421 to_load = _load_data(data, key, cls.__name__) 
-422 return load_into_recurse(cls, to_load, init=init) 
-423 
-424 
-425def load_into_instance( 
-426 inst: C, 
-427 data: T_data, 
-428 /, 
-429 key: str = None, 
-430 init: dict[str, typing.Any] = None, 
-431) -> C: 
-432 """ 
-433 Shortcut for _load_data + load_into_existing. 
-434 """ 
-435 cls = inst.__class__ 
-436 to_load = _load_data(data, key, cls.__name__) 
-437 return load_into_existing(inst, cls, to_load, init=init) 
-438 
-439 
-440def load_into( 
-441 cls: typing.Type[C] | C, 
-442 data: T_data, 
-443 /, 
-444 key: str = None, 
-445 init: dict[str, typing.Any] = None, 
-446) -> C: 
-447 """ 
-448 Load your config into a class (instance). 
-449 
-450 Args: 
-451 cls: either a class or an existing instance of that class. 
-452 data: can be a dictionary or a path to a file to load (as pathlib.Path or
+408def load_into_class( 
+409 cls: typing.Type[C], 
+410 data: T_data, 
+411 /, 
+412 key: str = None, 
+413 init: dict[str, typing.Any] = None, 
+414) -> C: 
+415 """ 
+416 Shortcut for _load_data + load_into_recurse. 
+417 """ 
+418 to_load = _load_data(data, key, cls.__name__) 
+419 return load_into_recurse(cls, to_load, init=init) 
+420 
+421 
+422def load_into_instance( 
+423 inst: C, 
+424 data: T_data, 
+425 /, 
+426 key: str = None, 
+427 init: dict[str, typing.Any] = None, 
+428) -> C: 
+429 """ 
+430 Shortcut for _load_data + load_into_existing. 
+431 """ 
+432 cls = inst.__class__ 
+433 to_load = _load_data(data, key, cls.__name__) 
+434 return load_into_existing(inst, cls, to_load, init=init) 
+435 
+436 
+437def load_into( 
+438 cls: typing.Type[C] | C, 
+439 data: T_data, 
+440 /, 
+441 key: str = None, 
+442 init: dict[str, typing.Any] = None, 
+443) -> C: 
+444 """ 
+445 Load your config into a class (instance). 
+446 
+447 Args: 
+448 cls: either a class or an existing instance of that class. 
+449 data: can be a dictionary or a path to a file to load (as pathlib.Path or
 str) 
-453 key: optional (nested) dictionary key to load data from (e.g.
+450 key: optional (nested) dictionary key to load data from (e.g.
 'tool.su6.specific') 
-454 init: optional data to pass to your cls' __init__ method (only if cls is
+451 init: optional data to pass to your cls' __init__ method (only if cls is
 not an instance already) 
-455 
-456 """ 
-457 if not isinstance(cls, type): 
-458 return load_into_instance(cls, data, key=key, init=init) 
-459 
-460 # make mypy and pycharm happy by telling it cls is of type C and not just
+452 
+453 """ 
+454 if not isinstance(cls, type): 
+455 return load_into_instance(cls, data, key=key, init=init) 
+456 
+457 # make mypy and pycharm happy by telling it cls is of type C and not just
 'type' 
-461 _cls = typing.cast(typing.Type[C], cls) 
-462 return load_into_class(_cls, data, key=key, init=init) 
+458 _cls = typing.cast(typing.Type[C], cls) 
+459 return load_into_class(_cls, data, key=key, init=init) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 15:57 +0200
+at 2023-06-14 16:11 +0200
```

### Comparing `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html` & `configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/helpers.py: 100%</title>
+    <title>Coverage for src/configuraptor/__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/helpers.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">2 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
+            <span class="text">3 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">3<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-14 16:09 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,34 +77,39 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Contains stand-alone helper functions.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Exposes TypedConfig and load_into for this library.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">def</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">s</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="str">    Convert CamelCase to snake_case.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    Source:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">        https://stackoverflow.com/questions/1175208/elegant-python-function-to-convert-camelcase-to-snake-case</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">return</span> <span class="str">""</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="op">[</span><span class="str">f"_{c.lower()}"</span> <span class="key">if</span> <span class="nam">c</span><span class="op">.</span><span class="nam">isupper</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">c</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">s</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">cls</span> <span class="key">import</span> <span class="nam">TypedConfig</span>  <span class="com"># noqa: F401 imported for library reasons</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="op">(</span>  <span class="com"># noqa: F401 imported for library reasons</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="nam">all_annotations</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">check_type</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">ensure_types</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="nam">load_into</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">singleton</span> <span class="key">import</span> <span class="op">(</span>  <span class="com"># noqa: F401 imported for library reasons</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="nam">Singleton</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">SingletonMeta</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-14 16:09 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,34 +1,38 @@
 
-****** Coverage for src/configuraptor/helpers.py: 100% ******
+****** Coverage for src/configuraptor/__init__.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 2 statements   2 run 0 missing 0 excluded *****
+***** 3 statements   3 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-14 16:09 +0200
 
 
 1""" 
-2Contains stand-alone helper functions. 
+2Exposes TypedConfig and load_into for this library. 
 3""" 
 4 
-5 
-6def camel_to_snake(s: str) -> str: 
-7 """ 
-8 Convert CamelCase to snake_case. 
-9 
-10 Source: 
-11 https://stackoverflow.com/questions/1175208/elegant-python-function-to-
-convert-camelcase-to-snake-case 
-12 """ 
-13 return "".join([f"_{c.lower()}" if c.isupper() else c for c in s]).lstrip
-("_") 
+5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
+<robinvandernoord@gmail.com> 
+6# 
+7# SPDX-License-Identifier: MIT 
+8from .cls import TypedConfig # noqa: F401 imported for library reasons 
+9from .core import ( # noqa: F401 imported for library reasons 
+10 all_annotations, 
+11 check_type, 
+12 ensure_types, 
+13 load_into, 
+14) 
+15from .singleton import ( # noqa: F401 imported for library reasons 
+16 Singleton, 
+17 SingletonMeta, 
+18) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-14 16:09 +0200
```

### Comparing `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.2.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/favicon_32.png` & `configuraptor-1.2.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/index.html` & `configuraptor-1.2.0/htmlcov/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 15:57 +0200
+            created at 2023-06-14 16:11 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -80,18 +80,18 @@
                 <td>7</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="7 7">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_core_py.html">src/configuraptor/core.py</a></td>
-                <td>150</td>
+                <td>152</td>
                 <td>0</td>
                 <td>3</td>
-                <td class="right" data-ratio="150 150">100%</td>
+                <td class="right" data-ratio="152 152">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_errors_py.html">src/configuraptor/errors.py</a></td>
                 <td>26</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="26 26">100%</td>
@@ -145,30 +145,30 @@
                 <td>0</td>
                 <td class="right" data-ratio="13 13">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>241</td>
+                <td>243</td>
                 <td>0</td>
                 <td>13</td>
-                <td class="right" data-ratio="241 241">100%</td>
+                <td class="right" data-ratio="243 243">100%</td>
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
-            created at 2023-06-14 15:57 +0200
+            created at 2023-06-14 16:11 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html"/>
         <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -2,28 +2,28 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-06-14 15:57 +0200
+coverage.py_v7.2.7, created at 2023-06-14 16:11 +0200
 
 Module                                   statements missing excluded coverage
 src/configuraptor/__about__.py           1          0       0        100%
 src/configuraptor/__init__.py            3          0       0        100%
 src/configuraptor/cls.py                 7          0       0        100%
-src/configuraptor/core.py                150        0       3        100%
+src/configuraptor/core.py                152        0       3        100%
 src/configuraptor/errors.py              26         0       0        100%
 src/configuraptor/helpers.py             2          0       0        100%
 src/configuraptor/loaders/__init__.py    14         0       2        100%
 src/configuraptor/loaders/_types.py      4          0       0        100%
 src/configuraptor/loaders/loaders_310.py 5          0       6        100%
 src/configuraptor/loaders/loaders_311.py 6          0       2        100%
 src/configuraptor/loaders/               10         0       0        100%
 loaders_shared.py
 src/configuraptor/singleton.py           13         0       0        100%
-Total                                    241        0       13       100%
+Total                                    243        0       13       100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-06-14 15:57 +0200
+coverage.py_v7.2.7, created at 2023-06-14 16:11 +0200
  ____
```

### Comparing `configuraptor-1.1.2/htmlcov/keybd_closed.png` & `configuraptor-1.2.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/keybd_open.png` & `configuraptor-1.2.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/htmlcov/status.json` & `configuraptor-1.2.0/htmlcov/status.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979367954911433%*

 * *Differences: {"'files'": "{'d_eb75b6cf8f5eab40___about___py': {'hash': '79b97372de56f3e7302236281ed024f9'}, "*

 * *            "'d_eb75b6cf8f5eab40___init___py': {'hash': 'e217e576066a3efb5823f1082f379d0d'}, "*

 * *            "'d_eb75b6cf8f5eab40_core_py': {'hash': 'da08476d01eb49f1f9506cb11bac6824', 'index': "*

 * *            "{'nums': {insert: [(2, 152)], delete: [2]}}}}"}*

```diff
@@ -269,15 +269,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_shared.py"
             }
         },
         "d_eb75b6cf8f5eab40___about___py": {
-            "hash": "23bbd4e516061a9ed7bf681e3c283590",
+            "hash": "79b97372de56f3e7302236281ed024f9",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -286,15 +286,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/__about__.py"
             }
         },
         "d_eb75b6cf8f5eab40___init___py": {
-            "hash": "b2a5175e7119f8f9720b25617f19316d",
+            "hash": "e217e576066a3efb5823f1082f379d0d",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___init___py.html",
                 "nums": [
                     0,
                     1,
                     3,
                     0,
@@ -320,21 +320,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/cls.py"
             }
         },
         "d_eb75b6cf8f5eab40_core_py": {
-            "hash": "2511d6fe7b8b9e00a64b4de9962ffb78",
+            "hash": "da08476d01eb49f1f9506cb11bac6824",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_core_py.html",
                 "nums": [
                     0,
                     1,
-                    150,
+                    152,
                     3,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/core.py"
```

### Comparing `configuraptor-1.1.2/htmlcov/style.css` & `configuraptor-1.2.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/pytest_examples/some.toml` & `configuraptor-1.2.0/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/src/configuraptor/cls.py` & `configuraptor-1.2.0/src/configuraptor/cls.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/src/configuraptor/core.py` & `configuraptor-1.2.0/src/configuraptor/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,20 +311,23 @@
     """
     Returns a dictionary-like ChainMap that includes annotations for all \
     attributes defined in cls or inherited from superclasses.
     """
     return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if "__annotations__" in c.__dict__))
 
 
-def all_annotations(cls: Type, _except: typing.Iterable[str]) -> dict[str, Type]:
+def all_annotations(cls: Type, _except: typing.Iterable[str] = None) -> dict[str, Type]:
     """
     Wrapper around `_all_annotations` that filters away any keys in _except.
 
     It also flattens the ChainMap to a regular dict.
     """
+    if _except is None:
+        _except = set()
+
     _all = _all_annotations(cls)
     return {k: v for k, v in _all.items() if k not in _except}
 
 
 def _check_and_convert_data(
     cls: typing.Type[C],
     data: dict[str, typing.Any],
```

### Comparing `configuraptor-1.1.2/src/configuraptor/errors.py` & `configuraptor-1.2.0/src/configuraptor/errors.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/src/configuraptor/singleton.py` & `configuraptor-1.2.0/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/src/configuraptor/loaders/__init__.py` & `configuraptor-1.2.0/src/configuraptor/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/tests/test_json_yaml.py` & `configuraptor-1.2.0/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/tests/test_singleton.py` & `configuraptor-1.2.0/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/tests/test_toml_basic.py` & `configuraptor-1.2.0/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/tests/test_toml_dataclass.py` & `configuraptor-1.2.0/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/tests/test_toml_existing.py` & `configuraptor-1.2.0/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/tests/test_toml_typedconfig_class.py` & `configuraptor-1.2.0/tests/test_toml_typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/LICENSE.txt` & `configuraptor-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/README.md` & `configuraptor-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/pyproject.toml` & `configuraptor-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.2/PKG-INFO` & `configuraptor-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.1.2
+Version: 1.2.0
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

