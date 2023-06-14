# Comparing `tmp/configuraptor-1.2.1.tar.gz` & `tmp/configuraptor-1.3.0.tar.gz`

## Comparing `configuraptor-1.2.1.tar` & `configuraptor-1.3.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 configuraptor-1.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.2.1/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.2.1/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.2.1/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.2.1/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.2.1/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.2.1/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 configuraptor-1.2.1/examples/dataclass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.2.1/examples/example_from_docs.json
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.2.1/examples/example_from_docs.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.2.1/examples/example_from_docs.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.2.1/examples/example_from_docs.yaml
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.2.1/examples/main.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.2.1/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.2.1/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   124666 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.2.1/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.2.1/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.2.1/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.2.1/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.2.1/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.2.1/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.2.1/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.2.1/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/cls.py
--rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/core.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.2.1/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.2.1/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.2.1/tests/test_about.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 configuraptor-1.2.1/tests/test_core.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.2.1/tests/test_json_yaml.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.2.1/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.2.1/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.2.1/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.2.1/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.2.1/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.2.1/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.2.1/LICENSE.txt
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 configuraptor-1.2.1/README.md
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 configuraptor-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 configuraptor-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 configuraptor-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.3.0/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.3.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.3.0/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.3.0/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.3.0/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.3.0/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/dataclass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/example_from_docs.json
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/example_from_docs.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/example_from_docs.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/example_from_docs.yaml
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/main.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   124666 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_about.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_core.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 configuraptor-1.3.0/README.md
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 configuraptor-1.3.0/PKG-INFO
```

### Comparing `configuraptor-1.2.1/CHANGELOG.md` & `configuraptor-1.3.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.0 (2023-06-14)
+### Feature
+* **strict:** Allow strict=False for load_into to ignore types (not recommended) ([`16853bb`](https://github.com/trialandsuccess/configuraptor/commit/16853bb62b88c229ca0d9487692f9688b504bcf2))
+
 ## v1.2.1 (2023-06-14)
 ### Fix
 * **lib:** Exposed wrong method ([`d57b6df`](https://github.com/trialandsuccess/configuraptor/commit/d57b6df10e85693729ffb87f4ec36a7a932e1a3e))
 
 ## v1.2.0 (2023-06-14)
 ### Feature
 * **lib:** Expose more methods externally + make second arg of all_annotations optional ([`63605ba`](https://github.com/trialandsuccess/configuraptor/commit/63605babb48ac2313e063def86608f82628688b7))
```

### Comparing `configuraptor-1.2.1/coverage.svg` & `configuraptor-1.3.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/_static/configuraptor_circle.png` & `configuraptor-1.3.0/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/_static/configuraptor_original.jpeg` & `configuraptor-1.3.0/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/_static/configuraptor_round.png` & `configuraptor-1.3.0/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/_static/configuraptor_transparent.png` & `configuraptor-1.3.0/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/examples/dataclass.py` & `configuraptor-1.3.0/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/examples/example_from_docs.py` & `configuraptor-1.3.0/examples/example_from_docs.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/examples/main.py` & `configuraptor-1.3.0/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/examples/typedconfig_class.py` & `configuraptor-1.3.0/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/coverage_html.js` & `configuraptor-1.3.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html` & `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/favicon_32.png` & `configuraptor-1.3.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/index.html` & `configuraptor-1.3.0/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/keybd_closed.png` & `configuraptor-1.3.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/keybd_open.png` & `configuraptor-1.3.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/status.json` & `configuraptor-1.3.0/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/htmlcov/style.css` & `configuraptor-1.3.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/pytest_examples/some.toml` & `configuraptor-1.3.0/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/src/configuraptor/__init__.py` & `configuraptor-1.3.0/src/configuraptor/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/src/configuraptor/cls.py` & `configuraptor-1.3.0/src/configuraptor/cls.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/src/configuraptor/core.py` & `configuraptor-1.3.0/src/configuraptor/core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/src/configuraptor/errors.py` & `configuraptor-1.3.0/src/configuraptor/errors.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/src/configuraptor/singleton.py` & `configuraptor-1.3.0/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/src/configuraptor/loaders/__init__.py` & `configuraptor-1.3.0/src/configuraptor/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/tests/test_core.py` & `configuraptor-1.3.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/tests/test_json_yaml.py` & `configuraptor-1.3.0/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/tests/test_singleton.py` & `configuraptor-1.3.0/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/tests/test_toml_basic.py` & `configuraptor-1.3.0/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/tests/test_toml_dataclass.py` & `configuraptor-1.3.0/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/tests/test_toml_existing.py` & `configuraptor-1.3.0/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/tests/test_toml_typedconfig_class.py` & `configuraptor-1.3.0/tests/test_toml_typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/LICENSE.txt` & `configuraptor-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/README.md` & `configuraptor-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.2.1/pyproject.toml` & `configuraptor-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     "tomlkit; python_version < '3.11'",
     "PyYAML",
 ]
 
 [template.plugins.default]
 src-layout = true
 
+[tool.setuptools.package-data]
+"configuraptor" = ["py.typed"]
+
 [project.optional-dependencies]
 dev = [
     "su6[all]",
     "hatch",
     "types-PyYAML",
 ]
```

### Comparing `configuraptor-1.2.1/PKG-INFO` & `configuraptor-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.2.1
+Version: 1.3.0
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

