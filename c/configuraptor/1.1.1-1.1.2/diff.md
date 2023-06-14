# Comparing `tmp/configuraptor-1.1.1.tar.gz` & `tmp/configuraptor-1.1.2.tar.gz`

## Comparing `configuraptor-1.1.1.tar` & `configuraptor-1.1.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 configuraptor-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.1.1/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.1.1/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.1.1/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.1.1/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.1.1/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.1.1/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 configuraptor-1.1.1/examples/dataclass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.1.1/examples/example_from_docs.json
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.1.1/examples/example_from_docs.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.1.1/examples/example_from_docs.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.1.1/examples/example_from_docs.yaml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 configuraptor-1.1.1/examples/main.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.1.1/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.1.1/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   119767 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.1.1/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.1.1/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.1.1/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.1.1/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.1.1/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.1.1/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.1.1/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.1.1/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/cls.py
--rw-r--r--   0        0        0    13982 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/core.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.1.1/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.1.1/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.1.1/tests/test_about.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.1.1/tests/test_core.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.1.1/tests/test_json_yaml.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.1.1/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.1.1/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 configuraptor-1.1.1/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.1.1/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.1.1/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.1.1/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 configuraptor-1.1.1/README.md
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 configuraptor-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 configuraptor-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 configuraptor-1.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.1.2/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.1.2/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.1.2/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.1.2/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.1.2/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.1.2/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/dataclass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/example_from_docs.json
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/example_from_docs.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/example_from_docs.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/example_from_docs.yaml
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/main.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.1.2/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   124672 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.1.2/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.1.2/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_about.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_core.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.1.2/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 configuraptor-1.1.2/README.md
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 configuraptor-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 configuraptor-1.1.2/PKG-INFO
```

### Comparing `configuraptor-1.1.1/CHANGELOG.md` & `configuraptor-1.1.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.1.2 (2023-06-14)
+### Fix
+* **dataclass:** Support for default_factory ([`031c68d`](https://github.com/trialandsuccess/configuraptor/commit/031c68d676fd59529e41debc480235a29f206405))
+
+### Documentation
+* **readme:** Wrong package name oops ([`a9f7fad`](https://github.com/trialandsuccess/configuraptor/commit/a9f7fad7483dd55ff76655ec3a8feda9d55beef8))
+
 ## v1.1.1 (2023-06-14)
 ### Documentation
 * **readme:** Change fixed image height to width for responsiveness ([`4ea3557`](https://github.com/trialandsuccess/configuraptor/commit/4ea3557e4cbb6eb2d3128a871209920f27e033ce))
 
 ## v1.1.0 (2023-06-14)
 ### Feature
 * Added JSON and YAML file loading. ([`e4f920f`](https://github.com/trialandsuccess/configuraptor/commit/e4f920f0ab1ffaebea2b7b5ad64e33f54f034a33))
```

### Comparing `configuraptor-1.1.1/coverage.svg` & `configuraptor-1.1.2/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/_static/configuraptor_circle.png` & `configuraptor-1.1.2/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/_static/configuraptor_original.jpeg` & `configuraptor-1.1.2/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/_static/configuraptor_round.png` & `configuraptor-1.1.2/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/_static/configuraptor_transparent.png` & `configuraptor-1.1.2/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/examples/example_from_docs.py` & `configuraptor-1.1.2/examples/example_from_docs.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/examples/main.py` & `configuraptor-1.1.2/examples/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Example with basic classes
 """
 
-from typedconfig import load_into
+from configuraptor import load_into
 
 
 class AbsHasName:
     name: str
 
 
 class Two(AbsHasName):
```

### Comparing `configuraptor-1.1.1/examples/typedconfig_class.py` & `configuraptor-1.1.2/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/coverage_html.js` & `configuraptor-1.1.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.1.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.1.2/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.1.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 12:24 +0200
+            created at 2023-06-14 15:56 +0200
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
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.0.3"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.1.1"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 12:24 +0200
+            created at 2023-06-14 15:56 +0200
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
-at 2023-06-14 12:24 +0200
+at 2023-06-14 15:56 +0200
 
 
 1""" 
 2This file contains the module version. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "1.0.3" 
+8__version__ = "1.1.1" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 12:24 +0200
+at 2023-06-14 15:56 +0200
```

### Comparing `configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

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
-            <span class="text">145 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">145<span class="text"> run</span></button>
+            <span class="text">150 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">150<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">3<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 12:24 +0200
+            created at 2023-06-14 15:57 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -84,15 +84,15 @@
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Contains most of the loading logic.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">types</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">warnings</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">ChainMap</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">dataclasses</span> <span class="key">import</span> <span class="nam">is_dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">dataclasses</span> <span class="key">as</span> <span class="nam">dc</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">typeguard</span> <span class="key">import</span> <span class="nam">TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">typeguard</span> <span class="key">import</span> <span class="nam">check_type</span> <span class="key">as</span> <span class="nam">_check_type</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">loaders</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">,</span> <span class="nam">ConfigErrorMissingKey</span>&nbsp;</span><span class="r"></span></p>
@@ -292,250 +292,268 @@
     <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="nam">_type</span> <span class="key">is</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>  <span class="com"># no type  # Nonetype</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">        <span class="key">or</span> <span class="nam">type</span><span class="op">(</span><span class="key">None</span><span class="op">)</span> <span class="key">in</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>  <span class="com"># union with Nonetype</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="key">def</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="key">def</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">dc</span><span class="op">.</span><span class="nam">Field</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">    For all annotations (recursively gathered from parents with `all_annotations`), \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">    try to resolve the tree of annotations.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t"><span class="str">    Uses `load_into_recurse`, not itself directly.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">    Get Field info for a dataclass cls.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__dataclass_fields__"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">    <span class="key">return</span> <span class="nam">fields</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t"><span class="str">        class First:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="str">            key: str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t"><span class="str">        class Second:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t"><span class="str">            other: First</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t"><span class="str">        # step 1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">        cls = Second</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t"><span class="str">        data = {"second": {"other": {"key": "anything"}}}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t"><span class="key">def</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t"><span class="str">    For all annotations (recursively gathered from parents with `all_annotations`), \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t"><span class="str">    try to resolve the tree of annotations.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t"><span class="str">    Uses `load_into_recurse`, not itself directly.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t"><span class="str">        class First:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">            key: str</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="str">        # step 1.5</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">        data = {"other": {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t"><span class="str">        # step 2</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">        cls = First</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t"><span class="str">        data = {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t"><span class="str">        annotations: {"key": str}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">    <span class="nam">updated</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="key">for</span> <span class="nam">_key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="key">if</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">            <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span> <span class="op">=</span> <span class="nam">data</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>  <span class="com"># value can change so define it as any instead of T</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">            <span class="key">if</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">                <span class="nam">origin</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">                <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">                <span class="key">if</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">list</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">                    <span class="nam">subtype</span> <span class="op">=</span> <span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">subtype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">dict</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">                    <span class="com"># e.g. dict[str, Point]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">                    <span class="nam">subkeytype</span><span class="op">,</span> <span class="nam">subvaluetype</span> <span class="op">=</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">                    <span class="com"># subkey(type) is not a custom class, so don't try to convert it:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">subkey</span><span class="op">:</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">subvaluetype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subkey</span><span class="op">,</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                <span class="com"># elif origin is dict:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">                <span class="com"># keep data the same</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span> <span class="key">and</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">                    <span class="key">for</span> <span class="nam">arg</span> <span class="key">in</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">                        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">                            <span class="nam">value</span> <span class="op">=</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">arg</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">                            <span class="com"># print(_type, arg, value)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">                            <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">                <span class="com"># todo: other parameterized/unions/typing.Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">            <span class="key">elif</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">                <span class="com"># type must be C (custom class) at this point</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">                    <span class="com"># make mypy and pycharm happy by telling it _type is of type C...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">                    <span class="com"># actually just passing _type as first arg!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">                    <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">Type_C</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">                    <span class="nam">value</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">        <span class="key">elif</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">            <span class="com"># property has default, use that instead.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">            <span class="com"># type is optional and not found in __dict__ -> default is None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">            <span class="com"># todo: exception group?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="str">        class Second:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">            other: First</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t"><span class="str">        # step 1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t"><span class="str">        cls = Second</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">        data = {"second": {"other": {"key": "anything"}}}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t"><span class="str">        # step 1.5</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t"><span class="str">        data = {"other": {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="str">        # step 2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t"><span class="str">        cls = First</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">        data = {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="str">        annotations: {"key": str}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">    <span class="nam">updated</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="key">for</span> <span class="nam">_key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="key">if</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">            <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span> <span class="op">=</span> <span class="nam">data</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>  <span class="com"># value can change so define it as any instead of T</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">            <span class="key">if</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">                <span class="nam">origin</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">                <span class="key">if</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">list</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">                    <span class="nam">subtype</span> <span class="op">=</span> <span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">subtype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">dict</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">                    <span class="com"># e.g. dict[str, Point]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">                    <span class="nam">subkeytype</span><span class="op">,</span> <span class="nam">subvaluetype</span> <span class="op">=</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">                    <span class="com"># subkey(type) is not a custom class, so don't try to convert it:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">subkey</span><span class="op">:</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">subvaluetype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subkey</span><span class="op">,</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">                <span class="com"># elif origin is dict:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">                <span class="com"># keep data the same</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span> <span class="key">and</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">                    <span class="key">for</span> <span class="nam">arg</span> <span class="key">in</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">                        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">                            <span class="nam">value</span> <span class="op">=</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">arg</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">                            <span class="com"># print(_type, arg, value)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">                            <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">                <span class="com"># todo: other parameterized/unions/typing.Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">            <span class="key">elif</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">                <span class="com"># type must be C (custom class) at this point</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">                    <span class="com"># make mypy and pycharm happy by telling it _type is of type C...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">                    <span class="com"># actually just passing _type as first arg!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">                    <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">Type_C</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">                    <span class="nam">value</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">        <span class="nam">updated</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">    <span class="key">return</span> <span class="nam">updated</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">        <span class="key">elif</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">            <span class="com"># property has default, use that instead.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">            <span class="com"># type is optional and not found in __dict__ -> default is None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">        <span class="key">elif</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">            <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">            <span class="key">and</span> <span class="op">(</span><span class="nam">field</span> <span class="op">:=</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_key</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">            <span class="key">and</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span> <span class="key">is</span> <span class="key">not</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">MISSING</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">        <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">            <span class="com"># could have a default factory</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">            <span class="com"># todo: do something with field.default?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">            <span class="com"># todo: exception group?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">        <span class="nam">updated</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="key">return</span> <span class="nam">updated</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t"><span class="key">def</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">    <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t"><span class="str">    Based on class annotations, this prepares the data for `load_into_recurse`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t"><span class="str">    1. convert config-keys to python compatible config_keys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t"><span class="str">    2. loads custom class type annotations with the same logic (see also `load_recursive`)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t"><span class="str">    3. ensures the annotated types match the actual types after loading the config file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">_except</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">    <span class="key">return</span> <span class="nam">to_load</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">    Loads an instance of `cls` filled with `data`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t"><span class="str">    Uses `load_recursive` to load any fillable annotated properties (see that method for an example).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t"><span class="str">    `init` can be used to optionally pass extra __init__ arguments. \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t"><span class="str">        NOTE: This will overwrite a config key with the same name!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">        <span class="nam">init</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="com"># fixme: cls.__init__ can set other keys than the name is in kwargs!!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t"><span class="key">def</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="str">    Based on class annotations, this prepares the data for `load_into_recurse`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">    1. convert config-keys to python compatible config_keys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="str">    2. loads custom class type annotations with the same logic (see also `load_recursive`)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t"><span class="str">    3. ensures the annotated types match the actual types after loading the config file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">_except</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="key">return</span> <span class="nam">to_load</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">    <span class="key">if</span> <span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">init</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">|=</span> <span class="nam">init</span>  <span class="com"># add extra init variables (should not happen for a dataclass but whatev)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">        <span class="com"># ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">C</span><span class="op">,</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">        <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_existing</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t"><span class="str">    Similar to `load_into_recurse` but uses an existing instance of a class (so after __init__) \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t"><span class="str">    and thus does not support init.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Can not init an existing instance!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">    <span class="nam">existing_data</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">existing_data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">    <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_class</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_recurse.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t"><span class="str">    Loads an instance of `cls` filled with `data`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t"><span class="str">    Uses `load_recursive` to load any fillable annotated properties (see that method for an example).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t"><span class="str">    `init` can be used to optionally pass extra __init__ arguments. \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t"><span class="str">        NOTE: This will overwrite a config key with the same name!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">        <span class="nam">init</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">    <span class="com"># fixme: cls.__init__ can set other keys than the name is in kwargs!!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">    <span class="key">if</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">init</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">|=</span> <span class="nam">init</span>  <span class="com"># add extra init variables (should not happen for a dataclass but whatev)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">        <span class="com"># ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">C</span><span class="op">,</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">        <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_existing</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t"><span class="str">    Similar to `load_into_recurse` but uses an existing instance of a class (so after __init__) \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t"><span class="str">    and thus does not support init.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Can not init an existing instance!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">    <span class="nam">existing_data</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">existing_data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_existing.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">    <span class="nam">cls</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_existing</span><span class="op">(</span><span class="nam">inst</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span> <span class="op">|</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t"><span class="str">    Load your config into a class (instance).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t"><span class="str">        cls: either a class or an existing instance of that class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t"><span class="str">        data: can be a dictionary or a path to a file to load (as pathlib.Path or str)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t"><span class="str">        key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t"><span class="str">        init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into_instance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">    <span class="com"># make mypy and pycharm happy by telling it cls is of type C and not just 'type'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">    <span class="nam">_cls</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span> <span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_class</span><span class="op">(</span><span class="nam">_cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">    <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_class</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_recurse.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_recurse</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_existing.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">    <span class="nam">cls</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_existing</span><span class="op">(</span><span class="nam">inst</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span> <span class="op">|</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t"><span class="str">    Load your config into a class (instance).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t"><span class="str">        cls: either a class or an existing instance of that class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t"><span class="str">        data: can be a dictionary or a path to a file to load (as pathlib.Path or str)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t"><span class="str">        key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t"><span class="str">        init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into_instance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">    <span class="com"># make mypy and pycharm happy by telling it cls is of type C and not just 'type'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">    <span class="nam">_cls</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span> <span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_class</span><span class="op">(</span><span class="nam">_cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 12:24 +0200
+            created at 2023-06-14 15:57 +0200
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
-***** 145 statements   145 run 0 missing 3 excluded *****
+***** 150 statements   150 run 0 missing 3 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 12:24 +0200
+at 2023-06-14 15:57 +0200
 
 
 1""" 
 2Contains most of the loading logic. 
 3""" 
 4 
 5import types 
 6import typing 
 7import warnings 
 8from collections import ChainMap 
-9from dataclasses import is_dataclass 
+9import dataclasses as dc 
 10from pathlib import Path 
 11 
 12from typeguard import TypeCheckError 
 13from typeguard import check_type as _check_type 
 14 
 15from . import loaders 
 16from .errors import ConfigErrorInvalidType, ConfigErrorMissingKey 
@@ -240,255 +240,273 @@
 210 _type is None 
 211 or issubclass(types.NoneType, _type) 
 212 or issubclass(types.NoneType, type(_type)) # no type # Nonetype 
 213 or type(None) in typing.get_args(_type) # union with Nonetype 
 214 ) 
 215 
 216 
-217def load_recursive(cls: Type, data: dict[str, T], annotations: dict[str,
-Type]) -> dict[str, T]: 
+217def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field]: 
 218 """ 
-219 For all annotations (recursively gathered from parents with
-`all_annotations`), \ 
-220 try to resolve the tree of annotations. 
-221 
-222 Uses `load_into_recurse`, not itself directly. 
+219 Get Field info for a dataclass cls. 
+220 """ 
+221 fields = getattr(cls, "__dataclass_fields__", {}) 
+222 return fields.get(key) 
 223 
-224 Example: 
-225 class First: 
-226 key: str 
-227 
-228 class Second: 
-229 other: First 
-230 
-231 # step 1 
-232 cls = Second 
-233 data = {"second": {"other": {"key": "anything"}}} 
-234 annotations: {"other": First} 
+224 
+225def load_recursive(cls: Type, data: dict[str, T], annotations: dict[str,
+Type]) -> dict[str, T]: 
+226 """ 
+227 For all annotations (recursively gathered from parents with
+`all_annotations`), \ 
+228 try to resolve the tree of annotations. 
+229 
+230 Uses `load_into_recurse`, not itself directly. 
+231 
+232 Example: 
+233 class First: 
+234 key: str 
 235 
-236 # step 1.5 
-237 data = {"other": {"key": "anything"} 
-238 annotations: {"other": First} 
-239 
-240 # step 2 
-241 cls = First 
-242 data = {"key": "anything"} 
-243 annotations: {"key": str} 
-244 
-245 """ 
-246 updated = {} 
-247 for _key, _type in annotations.items(): 
-248 if _key in data: 
-249 value: typing.Any = data[_key] # value can change so define it as any
+236 class Second: 
+237 other: First 
+238 
+239 # step 1 
+240 cls = Second 
+241 data = {"second": {"other": {"key": "anything"}}} 
+242 annotations: {"other": First} 
+243 
+244 # step 1.5 
+245 data = {"other": {"key": "anything"} 
+246 annotations: {"other": First} 
+247 
+248 # step 2 
+249 cls = First 
+250 data = {"key": "anything"} 
+251 annotations: {"key": str} 
+252 
+253 """ 
+254 
+255 updated = {} 
+256 for _key, _type in annotations.items(): 
+257 
+258 if _key in data: 
+259 value: typing.Any = data[_key] # value can change so define it as any
 instead of T 
-250 if is_parameterized(_type): 
-251 origin = typing.get_origin(_type) 
-252 arguments = typing.get_args(_type) 
-253 if origin is list and arguments and is_custom_class(arguments[0]): 
-254 subtype = arguments[0] 
-255 value = [load_into_recurse(subtype, subvalue) for subvalue in value] 
-256 
-257 elif origin is dict and arguments and is_custom_class(arguments[1]): 
-258 # e.g. dict[str, Point] 
-259 subkeytype, subvaluetype = arguments 
-260 # subkey(type) is not a custom class, so don't try to convert it: 
-261 value = {subkey: load_into_recurse(subvaluetype, subvalue) for subkey,
+260 if is_parameterized(_type): 
+261 origin = typing.get_origin(_type) 
+262 arguments = typing.get_args(_type) 
+263 if origin is list and arguments and is_custom_class(arguments[0]): 
+264 subtype = arguments[0] 
+265 value = [load_into_recurse(subtype, subvalue) for subvalue in value] 
+266 
+267 elif origin is dict and arguments and is_custom_class(arguments[1]): 
+268 # e.g. dict[str, Point] 
+269 subkeytype, subvaluetype = arguments 
+270 # subkey(type) is not a custom class, so don't try to convert it: 
+271 value = {subkey: load_into_recurse(subvaluetype, subvalue) for subkey,
 subvalue in value.items()} 
-262 # elif origin is dict: 
-263 # keep data the same 
-264 elif origin is typing.Union and arguments: 
-265 for arg in arguments: 
-266 if is_custom_class(arg): 
-267 value = load_into_recurse(arg, value) 
-268 else: 
-269 # print(_type, arg, value) 
-270 ... 
-271 
-272 # todo: other parameterized/unions/typing.Optional 
-273 
-274 elif is_custom_class(_type): 
-275 # type must be C (custom class) at this point 
-276 value = load_into_recurse( 
-277 # make mypy and pycharm happy by telling it _type is of type C... 
-278 # actually just passing _type as first arg! 
-279 typing.cast(Type_C[typing.Any], _type), 
-280 value, 
-281 ) 
-282 
-283 elif _key in cls.__dict__: 
-284 # property has default, use that instead. 
-285 value = cls.__dict__[_key] 
-286 elif is_optional(_type): 
-287 # type is optional and not found in __dict__ -> default is None 
-288 value = None 
-289 else: 
-290 # todo: exception group? 
-291 raise ConfigErrorMissingKey(_key, cls, _type) 
+272 # elif origin is dict: 
+273 # keep data the same 
+274 elif origin is typing.Union and arguments: 
+275 for arg in arguments: 
+276 if is_custom_class(arg): 
+277 value = load_into_recurse(arg, value) 
+278 else: 
+279 # print(_type, arg, value) 
+280 ... 
+281 
+282 # todo: other parameterized/unions/typing.Optional 
+283 
+284 elif is_custom_class(_type): 
+285 # type must be C (custom class) at this point 
+286 value = load_into_recurse( 
+287 # make mypy and pycharm happy by telling it _type is of type C... 
+288 # actually just passing _type as first arg! 
+289 typing.cast(Type_C[typing.Any], _type), 
+290 value, 
+291 ) 
 292 
-293 updated[_key] = value 
-294 
-295 return updated 
-296 
-297 
-298def _all_annotations(cls: Type) -> ChainMap[str, Type]: 
-299 """ 
-300 Returns a dictionary-like ChainMap that includes annotations for all \ 
-301 attributes defined in cls or inherited from superclasses. 
-302 """ 
-303 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
-"__annotations__" in c.__dict__)) 
-304 
-305 
-306def all_annotations(cls: Type, _except: typing.Iterable[str]) -> dict[str,
-Type]: 
-307 """ 
-308 Wrapper around `_all_annotations` that filters away any keys in _except. 
-309 
-310 It also flattens the ChainMap to a regular dict. 
-311 """ 
-312 _all = _all_annotations(cls) 
-313 return {k: v for k, v in _all.items() if k not in _except} 
+293 elif _key in cls.__dict__: 
+294 # property has default, use that instead. 
+295 value = cls.__dict__[_key] 
+296 elif is_optional(_type): 
+297 # type is optional and not found in __dict__ -> default is None 
+298 value = None 
+299 elif ( 
+300 dc.is_dataclass(cls) 
+301 and (field := dataclass_field(cls, _key)) 
+302 and field.default_factory is not dc.MISSING 
+303 ): 
+304 # could have a default factory 
+305 # todo: do something with field.default? 
+306 value = field.default_factory() 
+307 else: 
+308 # todo: exception group? 
+309 raise ConfigErrorMissingKey(_key, cls, _type) 
+310 
+311 updated[_key] = value 
+312 
+313 return updated 
 314 
 315 
-316def _check_and_convert_data( 
-317 cls: typing.Type[C], 
-318 data: dict[str, typing.Any], 
-319 _except: typing.Iterable[str], 
-320) -> dict[str, typing.Any]: 
-321 """ 
-322 Based on class annotations, this prepares the data for
-`load_into_recurse`. 
+316def _all_annotations(cls: Type) -> ChainMap[str, Type]: 
+317 """ 
+318 Returns a dictionary-like ChainMap that includes annotations for all \ 
+319 attributes defined in cls or inherited from superclasses. 
+320 """ 
+321 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
+"__annotations__" in c.__dict__)) 
+322 
 323 
-324 1. convert config-keys to python compatible config_keys 
-325 2. loads custom class type annotations with the same logic (see also
+324def all_annotations(cls: Type, _except: typing.Iterable[str]) -> dict[str,
+Type]: 
+325 """ 
+326 Wrapper around `_all_annotations` that filters away any keys in _except. 
+327 
+328 It also flattens the ChainMap to a regular dict. 
+329 """ 
+330 _all = _all_annotations(cls) 
+331 return {k: v for k, v in _all.items() if k not in _except} 
+332 
+333 
+334def _check_and_convert_data( 
+335 cls: typing.Type[C], 
+336 data: dict[str, typing.Any], 
+337 _except: typing.Iterable[str], 
+338) -> dict[str, typing.Any]: 
+339 """ 
+340 Based on class annotations, this prepares the data for
+`load_into_recurse`. 
+341 
+342 1. convert config-keys to python compatible config_keys 
+343 2. loads custom class type annotations with the same logic (see also
 `load_recursive`) 
-326 3. ensures the annotated types match the actual types after loading the
+344 3. ensures the annotated types match the actual types after loading the
 config file. 
-327 """ 
-328 annotations = all_annotations(cls, _except=_except) 
-329 
-330 to_load = convert_config(data) 
-331 to_load = load_recursive(cls, to_load, annotations) 
-332 to_load = ensure_types(to_load, annotations) 
-333 return to_load 
-334 
-335 
-336def load_into_recurse( 
-337 cls: typing.Type[C], 
-338 data: dict[str, typing.Any], 
-339 init: dict[str, typing.Any] = None, 
-340) -> C: 
-341 """ 
-342 Loads an instance of `cls` filled with `data`. 
-343 
-344 Uses `load_recursive` to load any fillable annotated properties (see that
-method for an example). 
-345 `init` can be used to optionally pass extra __init__ arguments. \ 
-346 NOTE: This will overwrite a config key with the same name! 
-347 """ 
-348 if init is None: 
-349 init = {} 
-350 
-351 # fixme: cls.__init__ can set other keys than the name is in kwargs!! 
+345 """ 
+346 annotations = all_annotations(cls, _except=_except) 
+347 
+348 to_load = convert_config(data) 
+349 to_load = load_recursive(cls, to_load, annotations) 
+350 to_load = ensure_types(to_load, annotations) 
+351 return to_load 
 352 
-353 if is_dataclass(cls): 
-354 to_load = _check_and_convert_data(cls, data, init.keys()) 
-355 to_load |= init # add extra init variables (should not happen for a
+353 
+354def load_into_recurse( 
+355 cls: typing.Type[C], 
+356 data: dict[str, typing.Any], 
+357 init: dict[str, typing.Any] = None, 
+358) -> C: 
+359 """ 
+360 Loads an instance of `cls` filled with `data`. 
+361 
+362 Uses `load_recursive` to load any fillable annotated properties (see that
+method for an example). 
+363 `init` can be used to optionally pass extra __init__ arguments. \ 
+364 NOTE: This will overwrite a config key with the same name! 
+365 """ 
+366 if init is None: 
+367 init = {} 
+368 
+369 # fixme: cls.__init__ can set other keys than the name is in kwargs!! 
+370 
+371 if dc.is_dataclass(cls): 
+372 to_load = _check_and_convert_data(cls, data, init.keys()) 
+373 to_load |= init # add extra init variables (should not happen for a
 dataclass but whatev) 
-356 
-357 # ensure mypy inst is an instance of the cls type (and not a fictuous
+374 
+375 # ensure mypy inst is an instance of the cls type (and not a fictuous
 `DataclassInstance`) 
-358 inst = typing.cast(C, cls(**to_load)) 
-359 else: 
-360 inst = cls(**init) 
-361 to_load = _check_and_convert_data(cls, data, inst.__dict__.keys()) 
-362 inst.__dict__.update(**to_load) 
-363 
-364 return inst 
-365 
-366 
-367def load_into_existing( 
-368 inst: C, 
-369 cls: typing.Type[C], 
-370 data: dict[str, typing.Any], 
-371 init: dict[str, typing.Any] = None, 
-372) -> C: 
-373 """ 
-374 Similar to `load_into_recurse` but uses an existing instance of a class (so
+376 inst = typing.cast(C, cls(**to_load)) 
+377 else: 
+378 inst = cls(**init) 
+379 to_load = _check_and_convert_data(cls, data, inst.__dict__.keys()) 
+380 inst.__dict__.update(**to_load) 
+381 
+382 return inst 
+383 
+384 
+385def load_into_existing( 
+386 inst: C, 
+387 cls: typing.Type[C], 
+388 data: dict[str, typing.Any], 
+389 init: dict[str, typing.Any] = None, 
+390) -> C: 
+391 """ 
+392 Similar to `load_into_recurse` but uses an existing instance of a class (so
 after __init__) \ 
-375 and thus does not support init. 
-376 
-377 """ 
-378 if init is not None: 
-379 raise ValueError("Can not init an existing instance!") 
-380 
-381 existing_data = inst.__dict__ 
-382 
-383 annotations = all_annotations(cls, _except=existing_data.keys()) 
-384 to_load = convert_config(data) 
-385 to_load = load_recursive(cls, to_load, annotations) 
-386 to_load = ensure_types(to_load, annotations) 
-387 
-388 inst.__dict__.update(**to_load) 
-389 
-390 return inst 
-391 
-392 
-393def load_into_class( 
-394 cls: typing.Type[C], 
-395 data: T_data, 
-396 /, 
-397 key: str = None, 
-398 init: dict[str, typing.Any] = None, 
-399) -> C: 
-400 """ 
-401 Shortcut for _load_data + load_into_recurse. 
-402 """ 
-403 to_load = _load_data(data, key, cls.__name__) 
-404 return load_into_recurse(cls, to_load, init=init) 
+393 and thus does not support init. 
+394 
+395 """ 
+396 if init is not None: 
+397 raise ValueError("Can not init an existing instance!") 
+398 
+399 existing_data = inst.__dict__ 
+400 
+401 annotations = all_annotations(cls, _except=existing_data.keys()) 
+402 to_load = convert_config(data) 
+403 to_load = load_recursive(cls, to_load, annotations) 
+404 to_load = ensure_types(to_load, annotations) 
 405 
-406 
-407def load_into_instance( 
-408 inst: C, 
-409 data: T_data, 
-410 /, 
-411 key: str = None, 
-412 init: dict[str, typing.Any] = None, 
-413) -> C: 
-414 """ 
-415 Shortcut for _load_data + load_into_existing. 
-416 """ 
-417 cls = inst.__class__ 
-418 to_load = _load_data(data, key, cls.__name__) 
-419 return load_into_existing(inst, cls, to_load, init=init) 
-420 
-421 
-422def load_into( 
-423 cls: typing.Type[C] | C, 
-424 data: T_data, 
-425 /, 
-426 key: str = None, 
-427 init: dict[str, typing.Any] = None, 
-428) -> C: 
-429 """ 
-430 Load your config into a class (instance). 
-431 
-432 Args: 
-433 cls: either a class or an existing instance of that class. 
-434 data: can be a dictionary or a path to a file to load (as pathlib.Path or
+406 inst.__dict__.update(**to_load) 
+407 
+408 return inst 
+409 
+410 
+411def load_into_class( 
+412 cls: typing.Type[C], 
+413 data: T_data, 
+414 /, 
+415 key: str = None, 
+416 init: dict[str, typing.Any] = None, 
+417) -> C: 
+418 """ 
+419 Shortcut for _load_data + load_into_recurse. 
+420 """ 
+421 to_load = _load_data(data, key, cls.__name__) 
+422 return load_into_recurse(cls, to_load, init=init) 
+423 
+424 
+425def load_into_instance( 
+426 inst: C, 
+427 data: T_data, 
+428 /, 
+429 key: str = None, 
+430 init: dict[str, typing.Any] = None, 
+431) -> C: 
+432 """ 
+433 Shortcut for _load_data + load_into_existing. 
+434 """ 
+435 cls = inst.__class__ 
+436 to_load = _load_data(data, key, cls.__name__) 
+437 return load_into_existing(inst, cls, to_load, init=init) 
+438 
+439 
+440def load_into( 
+441 cls: typing.Type[C] | C, 
+442 data: T_data, 
+443 /, 
+444 key: str = None, 
+445 init: dict[str, typing.Any] = None, 
+446) -> C: 
+447 """ 
+448 Load your config into a class (instance). 
+449 
+450 Args: 
+451 cls: either a class or an existing instance of that class. 
+452 data: can be a dictionary or a path to a file to load (as pathlib.Path or
 str) 
-435 key: optional (nested) dictionary key to load data from (e.g.
+453 key: optional (nested) dictionary key to load data from (e.g.
 'tool.su6.specific') 
-436 init: optional data to pass to your cls' __init__ method (only if cls is
+454 init: optional data to pass to your cls' __init__ method (only if cls is
 not an instance already) 
-437 
-438 """ 
-439 if not isinstance(cls, type): 
-440 return load_into_instance(cls, data, key=key, init=init) 
-441 
-442 # make mypy and pycharm happy by telling it cls is of type C and not just
+455 
+456 """ 
+457 if not isinstance(cls, type): 
+458 return load_into_instance(cls, data, key=key, init=init) 
+459 
+460 # make mypy and pycharm happy by telling it cls is of type C and not just
 'type' 
-443 _cls = typing.cast(typing.Type[C], cls) 
-444 return load_into_class(_cls, data, key=key, init=init) 
+461 _cls = typing.cast(typing.Type[C], cls) 
+462 return load_into_class(_cls, data, key=key, init=init) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 12:24 +0200
+at 2023-06-14 15:57 +0200
```

### Comparing `configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html` & `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.1.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/favicon_32.png` & `configuraptor-1.1.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/index.html` & `configuraptor-1.1.2/htmlcov/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 12:25 +0200
+            created at 2023-06-14 15:57 +0200
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
-                <td>145</td>
+                <td>150</td>
                 <td>0</td>
                 <td>3</td>
-                <td class="right" data-ratio="145 145">100%</td>
+                <td class="right" data-ratio="150 150">100%</td>
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
-                <td>236</td>
+                <td>241</td>
                 <td>0</td>
                 <td>13</td>
-                <td class="right" data-ratio="236 236">100%</td>
+                <td class="right" data-ratio="241 241">100%</td>
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
-            created at 2023-06-14 12:25 +0200
+            created at 2023-06-14 15:57 +0200
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
-coverage.py_v7.2.7, created at 2023-06-14 12:25 +0200
+coverage.py_v7.2.7, created at 2023-06-14 15:57 +0200
 
 Module                                   statements missing excluded coverage
 src/configuraptor/__about__.py           1          0       0        100%
 src/configuraptor/__init__.py            3          0       0        100%
 src/configuraptor/cls.py                 7          0       0        100%
-src/configuraptor/core.py                145        0       3        100%
+src/configuraptor/core.py                150        0       3        100%
 src/configuraptor/errors.py              26         0       0        100%
 src/configuraptor/helpers.py             2          0       0        100%
 src/configuraptor/loaders/__init__.py    14         0       2        100%
 src/configuraptor/loaders/_types.py      4          0       0        100%
 src/configuraptor/loaders/loaders_310.py 5          0       6        100%
 src/configuraptor/loaders/loaders_311.py 6          0       2        100%
 src/configuraptor/loaders/               10         0       0        100%
 loaders_shared.py
 src/configuraptor/singleton.py           13         0       0        100%
-Total                                    236        0       13       100%
+Total                                    241        0       13       100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-06-14 12:25 +0200
+coverage.py_v7.2.7, created at 2023-06-14 15:57 +0200
  ____
```

### Comparing `configuraptor-1.1.1/htmlcov/keybd_closed.png` & `configuraptor-1.1.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/keybd_open.png` & `configuraptor-1.1.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/htmlcov/status.json` & `configuraptor-1.1.2/htmlcov/status.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986161433172303%*

 * *Differences: {"'files'": "{'d_eb75b6cf8f5eab40___about___py': {'hash': '23bbd4e516061a9ed7bf681e3c283590'}, "*

 * *            "'d_eb75b6cf8f5eab40_core_py': {'hash': '2511d6fe7b8b9e00a64b4de9962ffb78', 'index': "*

 * *            "{'nums': {insert: [(2, 150)], delete: [2]}}}}"}*

```diff
@@ -269,15 +269,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_shared.py"
             }
         },
         "d_eb75b6cf8f5eab40___about___py": {
-            "hash": "592ad5b31e242df1a606d56d42dd873e",
+            "hash": "23bbd4e516061a9ed7bf681e3c283590",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -320,21 +320,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/cls.py"
             }
         },
         "d_eb75b6cf8f5eab40_core_py": {
-            "hash": "63af632a38c5bd948c1e8996eb4ee94c",
+            "hash": "2511d6fe7b8b9e00a64b4de9962ffb78",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_core_py.html",
                 "nums": [
                     0,
                     1,
-                    145,
+                    150,
                     3,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/core.py"
```

### Comparing `configuraptor-1.1.1/htmlcov/style.css` & `configuraptor-1.1.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/pytest_examples/some.toml` & `configuraptor-1.1.2/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/src/configuraptor/cls.py` & `configuraptor-1.1.2/src/configuraptor/cls.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/src/configuraptor/core.py` & `configuraptor-1.1.2/src/configuraptor/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Contains most of the loading logic.
 """
 
+import dataclasses as dc
 import types
 import typing
 import warnings
 from collections import ChainMap
-from dataclasses import is_dataclass
 from pathlib import Path
 
 from typeguard import TypeCheckError
 from typeguard import check_type as _check_type
 
 from . import loaders
 from .errors import ConfigErrorInvalidType, ConfigErrorMissingKey
@@ -210,14 +210,22 @@
         _type is None
         or issubclass(types.NoneType, _type)
         or issubclass(types.NoneType, type(_type))  # no type  # Nonetype
         or type(None) in typing.get_args(_type)  # union with Nonetype
     )
 
 
+def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field[typing.Any]]:
+    """
+    Get Field info for a dataclass cls.
+    """
+    fields = getattr(cls, "__dataclass_fields__", {})
+    return fields.get(key)
+
+
 def load_recursive(cls: Type, data: dict[str, T], annotations: dict[str, Type]) -> dict[str, T]:
     """
     For all annotations (recursively gathered from parents with `all_annotations`), \
     try to resolve the tree of annotations.
 
     Uses `load_into_recurse`, not itself directly.
 
@@ -282,14 +290,18 @@
 
         elif _key in cls.__dict__:
             # property has default, use that instead.
             value = cls.__dict__[_key]
         elif is_optional(_type):
             # type is optional and not found in __dict__ -> default is None
             value = None
+        elif dc.is_dataclass(cls) and (field := dataclass_field(cls, _key)) and field.default_factory is not dc.MISSING:
+            # could have a default factory
+            # todo: do something with field.default?
+            value = field.default_factory()
         else:
             # todo: exception group?
             raise ConfigErrorMissingKey(_key, cls, _type)
 
         updated[_key] = value
 
     return updated
@@ -346,15 +358,15 @@
         NOTE: This will overwrite a config key with the same name!
     """
     if init is None:
         init = {}
 
     # fixme: cls.__init__ can set other keys than the name is in kwargs!!
 
-    if is_dataclass(cls):
+    if dc.is_dataclass(cls):
         to_load = _check_and_convert_data(cls, data, init.keys())
         to_load |= init  # add extra init variables (should not happen for a dataclass but whatev)
 
         # ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)
         inst = typing.cast(C, cls(**to_load))
     else:
         inst = cls(**init)
```

### Comparing `configuraptor-1.1.1/src/configuraptor/errors.py` & `configuraptor-1.1.2/src/configuraptor/errors.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/src/configuraptor/singleton.py` & `configuraptor-1.1.2/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/src/configuraptor/loaders/__init__.py` & `configuraptor-1.1.2/src/configuraptor/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/tests/test_core.py` & `configuraptor-1.1.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/tests/test_json_yaml.py` & `configuraptor-1.1.2/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/tests/test_singleton.py` & `configuraptor-1.1.2/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/tests/test_toml_basic.py` & `configuraptor-1.1.2/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/tests/test_toml_dataclass.py` & `configuraptor-1.1.2/tests/test_toml_dataclass.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime as dt
 import math
 import typing
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 import pytest
 
 from src import configuraptor
 from src.configuraptor.errors import ConfigError
 
 from .constants import EMPTY_FILE, EXAMPLE_FILE, _load_toml
@@ -91,14 +91,16 @@
     fruits: list[Fruit]
     second_extra: SecondExtra
 
 
 @dataclass
 class Empty:
     default: str = "allowed"
+    include: list[int] = field(default_factory=list)
+    # ^ not required in config file since it has a default value
 
 
 def test_empty():
     empty = configuraptor.load_into(Empty, {})
     assert empty and empty.default == "allowed"
 
     with pytest.raises(ConfigError):
```

### Comparing `configuraptor-1.1.1/tests/test_toml_existing.py` & `configuraptor-1.1.2/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/tests/test_toml_typedconfig_class.py` & `configuraptor-1.1.2/tests/test_toml_typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/LICENSE.txt` & `configuraptor-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/README.md` & `configuraptor-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -108,12 +108,12 @@
     # [41, 43]
 ```
 
 More examples will be available soon.
 
 ## License
 
-`edwh` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`configuraptor` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Changelog
 
 [See CHANGELOG.md](https://github.com/trialandsuccess/configuraptor/blob/master/CHANGELOG.md)
```

### Comparing `configuraptor-1.1.1/pyproject.toml` & `configuraptor-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.1.1/PKG-INFO` & `configuraptor-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.1.1
+Version: 1.1.2
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -135,12 +135,12 @@
     # [41, 43]
 ```
 
 More examples will be available soon.
 
 ## License
 
-`edwh` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`configuraptor` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Changelog
 
 [See CHANGELOG.md](https://github.com/trialandsuccess/configuraptor/blob/master/CHANGELOG.md)
```

