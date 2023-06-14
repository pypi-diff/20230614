# Comparing `tmp/configuraptor-1.0.3.tar.gz` & `tmp/configuraptor-1.1.0.tar.gz`

## Comparing `configuraptor-1.0.3.tar` & `configuraptor-1.1.0.tar`

### file list

```diff
@@ -1,71 +1,81 @@
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 configuraptor-1.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.0.3/coverage.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 configuraptor-1.0.3/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.0.3/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.0.3/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.0.3/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.0.3/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/dataclass.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/example_from_docs.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/example_from_docs.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/main.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.0.3/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   119587 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.0.3/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.0.3/pytest_examples/empty.toml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.0.3/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.0.3/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.0.3/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/cls.py
--rw-r--r--   0        0        0    13973 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/core.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 configuraptor-1.0.3/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_about.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_core.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.0.3/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.0.3/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 configuraptor-1.0.3/README.md
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 configuraptor-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 configuraptor-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 configuraptor-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.1.0/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.1.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.1.0/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.1.0/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.1.0/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.1.0/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 configuraptor-1.1.0/examples/dataclass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.1.0/examples/example_from_docs.json
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.1.0/examples/example_from_docs.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.1.0/examples/example_from_docs.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.1.0/examples/example_from_docs.yaml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 configuraptor-1.1.0/examples/main.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.1.0/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.1.0/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   119767 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.1.0/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.1.0/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.1.0/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.1.0/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.1.0/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.1.0/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.1.0/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.1.0/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    13982 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.1.0/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.1.0/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.1.0/tests/test_about.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.1.0/tests/test_core.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.1.0/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.1.0/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.1.0/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 configuraptor-1.1.0/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.1.0/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.1.0/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 configuraptor-1.1.0/README.md
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 configuraptor-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 configuraptor-1.1.0/PKG-INFO
```

### Comparing `configuraptor-1.0.3/CHANGELOG.md` & `configuraptor-1.1.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.1.0 (2023-06-14)
+### Feature
+* Added JSON and YAML file loading. ([`e4f920f`](https://github.com/trialandsuccess/configuraptor/commit/e4f920f0ab1ffaebea2b7b5ad64e33f54f034a33))
+
 ## v1.0.3 (2023-06-14)
 ### Fix
 * **core:** Checking for a required parameterized type (e.g. list[str]) crashed for a missing key (with the wrong error) ([`68ccc1c`](https://github.com/trialandsuccess/configuraptor/commit/68ccc1c44e29c940d14acd6ce6b49e9885eaa03a))
 
 ### Documentation
 * **readme:** Added first example code ([`da0b13d`](https://github.com/trialandsuccess/configuraptor/commit/da0b13d6e90fb0d26b1f33d804657a21304be745))
 * **changelog:** Manually added changes ([`c1c40ef`](https://github.com/trialandsuccess/configuraptor/commit/c1c40efb568abec30578d38a0a92d97f398fc23b))
```

### Comparing `configuraptor-1.0.3/coverage.svg` & `configuraptor-1.1.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/_static/configuraptor_circle.png` & `configuraptor-1.1.0/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/_static/configuraptor_original.jpeg` & `configuraptor-1.1.0/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/_static/configuraptor_round.png` & `configuraptor-1.1.0/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/_static/configuraptor_transparent.png` & `configuraptor-1.1.0/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/examples/dataclass.py` & `configuraptor-1.1.0/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/examples/example_from_docs.py` & `configuraptor-1.1.0/examples/example_from_docs.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class Config:
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = load_into(Config, "example_from_docs.toml")
+    my_config = load_into(Config, "example_from_docs.json")
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 
 
@@ -36,13 +36,13 @@
 
 class OtherConfig(TypedConfig):
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = OtherConfig.load("example_from_docs.toml")
+    my_config = OtherConfig.load("example_from_docs.json")
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
```

### Comparing `configuraptor-1.0.3/examples/main.py` & `configuraptor-1.1.0/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/examples/typedconfig_class.py` & `configuraptor-1.1.0/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/coverage_html.js` & `configuraptor-1.1.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.1.0/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.1.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.1.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.1.0/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.1.0/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.1.0/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/loaders/__init__.py: 100%</title>
+    <title>Coverage for src/configuraptor/helpers.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/loaders/__init__.py</b>:
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
-            <span class="text">4 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">4<span class="text"> run</span></button>
+            <span class="text">2 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_310_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
             created at 2023-06-14 11:42 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
@@ -77,32 +77,33 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Loads loaders based on Python version.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Contains stand-alone helper functions.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">if</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">version_info</span> <span class="op">></span> <span class="op">(</span><span class="num">3</span><span class="op">,</span> <span class="num">11</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">    <span class="key">from</span> <span class="op">.</span><span class="nam">loaders_311</span> <span class="key">import</span> <span class="nam">toml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">else</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="key">from</span> <span class="op">.</span><span class="nam">loaders_310</span> <span class="key">import</span> <span class="nam">toml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span><span class="str">"toml"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
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
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_310_py.html">&#xbb; next</a>
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
@@ -1,31 +1,34 @@
 
-****** Coverage for src/configuraptor/loaders/__init__.py: 100% ******
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
-***** 4 statements   4 run 0 missing 2 excluded *****
+***** 2 statements   2 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
 at 2023-06-14 11:42 +0200
 
 
 1""" 
-2Loads loaders based on Python version. 
+2Contains stand-alone helper functions. 
 3""" 
 4 
-5import sys 
-6 
-7if sys.version_info > (3, 11): 
-8 from .loaders_311 import toml 
-9else: # pragma: no cover 
-10 from .loaders_310 import toml 
-11 
-12__all__ = ["toml"] 
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

### Comparing `configuraptor-1.0.3/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.1.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">5 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">5<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">6<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97__types_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-14 12:24 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -81,37 +81,37 @@
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Loaders for Python 3.10.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">if</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">version_info</span> <span class="op">></span> <span class="op">(</span><span class="num">3</span><span class="op">,</span> <span class="num">11</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"Wrong Python version!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">else</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="nam">T_toml</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="key">def</span> <span class="nam">toml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_toml</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">        Load a toml file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">T_toml</span><span class="op">,</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span><span class="op">,</span> <span class="nam">as_tconfig</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">if</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">version_info</span> <span class="op">></span> <span class="op">(</span><span class="num">3</span><span class="op">,</span> <span class="num">11</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"Wrong Python version!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">else</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="key">def</span> <span class="nam">toml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">        Load a toml file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="nam">data</span> <span class="op">=</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="key">return</span> <span class="nam">as_tconfig</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97__types_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-14 12:24 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,33 +7,33 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 5 statements   5 run 0 missing 6 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-14 12:24 +0200
 
 
 1""" 
 2Loaders for Python 3.10. 
 3""" 
 4 
 5import sys 
-6import typing 
-7from typing import BinaryIO 
-8 
-9if sys.version_info > (3, 11): 
-10 raise EnvironmentError("Wrong Python version!") 
-11else: # pragma: no cover 
-12 import tomlkit 
-13 
-14 T_toml = dict[str, typing.Any] 
-15 
-16 def toml(f: BinaryIO) -> T_toml: 
-17 """ 
-18 Load a toml file. 
-19 """ 
-20 return typing.cast(T_toml, tomlkit.load(f)) 
+6from typing import BinaryIO 
+7 
+8from ._types import T_config, as_tconfig 
+9 
+10if sys.version_info > (3, 11): 
+11 raise EnvironmentError("Wrong Python version!") 
+12else: # pragma: no cover 
+13 import tomlkit 
+14 
+15 def toml(f: BinaryIO) -> T_config: 
+16 """ 
+17 Load a toml file. 
+18 """ 
+19 data = tomlkit.load(f) 
+20 return as_tconfig(data) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-14 12:24 +0200
```

### Comparing `configuraptor-1.0.3/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.1.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -58,18 +58,18 @@
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">6<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_310_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_shared_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-14 12:24 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,35 +80,36 @@
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Loaders for Python 3.11+.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">if</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">version_info</span> <span class="op">&lt;</span> <span class="op">(</span><span class="num">3</span><span class="op">,</span> <span class="num">11</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"Wrong Python version!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">import</span> <span class="nam">tomllib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">def</span> <span class="nam">toml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">        Load a toml file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="key">return</span> <span class="nam">tomllib</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">if</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">version_info</span> <span class="op">&lt;</span> <span class="op">(</span><span class="num">3</span><span class="op">,</span> <span class="num">11</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"Wrong Python version!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">import</span> <span class="nam">tomllib</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="key">def</span> <span class="nam">toml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">        Load a toml file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="key">return</span> <span class="nam">tomllib</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_310_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_shared_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-14 12:24 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,30 +7,31 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 6 statements   6 run 0 missing 2 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-14 12:24 +0200
 
 
 1""" 
 2Loaders for Python 3.11+. 
 3""" 
 4import sys 
-5import typing 
-6from typing import BinaryIO 
-7 
-8if sys.version_info < (3, 11): # pragma: no cover 
-9 raise EnvironmentError("Wrong Python version!") 
-10else: 
-11 import tomllib 
-12 
-13 def toml(f: BinaryIO) -> dict[str, typing.Any]: 
-14 """ 
-15 Load a toml file. 
-16 """ 
-17 return tomllib.load(f) 
+5from typing import BinaryIO 
+6 
+7from ._types import T_config 
+8 
+9if sys.version_info < (3, 11): # pragma: no cover 
+10 raise EnvironmentError("Wrong Python version!") 
+11else: 
+12 import tomllib 
+13 
+14 def toml(f: BinaryIO) -> T_config: 
+15 """ 
+16 Load a toml file. 
+17 """ 
+18 return tomllib.load(f) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-14 12:24 +0200
```

### Comparing `configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

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
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-14 12:24 +0200
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
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.0.2"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.0.3"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-14 12:24 +0200
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
-at 2023-06-14 11:42 +0200
+at 2023-06-14 12:24 +0200
 
 
 1""" 
 2This file contains the module version. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "1.0.2" 
+8__version__ = "1.0.3" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-14 12:24 +0200
```

### Comparing `configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

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
-            <span class="text">144 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">144<span class="text"> run</span></button>
+            <span class="text">145 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">145<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">3<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:44 +0200
+            created at 2023-06-14 12:24 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -140,17 +140,17 @@
     <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    E.g. class Tool will be mapped to key tool.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">    It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="nam">data</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">Path</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="com"># todo: more than toml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="key">with</span> <span class="nam">data</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"rb"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">f</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">            <span class="nam">data</span> <span class="op">=</span> <span class="nam">loaders</span><span class="op">.</span><span class="nam">toml</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="key">with</span> <span class="nam">data</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"rb"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">f</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="nam">loader</span> <span class="op">=</span> <span class="nam">loaders</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">suffix</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">            <span class="nam">data</span> <span class="op">=</span> <span class="nam">loader</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="key">if</span> <span class="nam">key</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="com"># try to guess key by grabbing the first one or using the class name</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
@@ -529,13 +529,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:44 +0200
+            created at 2023-06-14 12:24 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,17 +5,17 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 144 statements   144 run 0 missing 3 excluded *****
+***** 145 statements   145 run 0 missing 3 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:44 +0200
+at 2023-06-14 12:24 +0200
 
 
 1""" 
 2Contains most of the loading logic. 
 3""" 
 4 
 5import types 
@@ -78,17 +78,17 @@
 58 
 59 E.g. class Tool will be mapped to key tool. 
 60 It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}} 
 61 """ 
 62 if isinstance(data, str): 
 63 data = Path(data) 
 64 if isinstance(data, Path): 
-65 # todo: more than toml 
-66 with data.open("rb") as f: 
-67 data = loaders.toml(f) 
+65 with data.open("rb") as f: 
+66 loader = loaders.get(data.suffix) 
+67 data = loader(f) 
 68 
 69 if not data: 
 70 return {} 
 71 
 72 if key is None: 
 73 # try to guess key by grabbing the first one or using the class name 
 74 if len(data) == 1: 
@@ -487,8 +487,8 @@
 441 
 442 # make mypy and pycharm happy by telling it cls is of type C and not just
 'type' 
 443 _cls = typing.cast(typing.Type[C], cls) 
 444 return load_into_class(_cls, data, key=key, init=init) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:44 +0200
+at 2023-06-14 12:24 +0200
```

### Comparing `configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_errors_py.html` & `configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.1.0/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/helpers.py: 100%</title>
+    <title>Coverage for src/configuraptor/loaders/_types.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/helpers.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/loaders/_types.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,61 +50,59 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">2 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
+            <span class="text">4 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">4<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_310_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-14 12:24 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Contains stand-alone helper functions.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="nam">T_config</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">def</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">s</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">def</span> <span class="nam">as_tconfig</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="str">    Convert CamelCase to snake_case.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    Source:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">        https://stackoverflow.com/questions/1175208/elegant-python-function-to-convert-camelcase-to-snake-case</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">return</span> <span class="str">""</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="op">[</span><span class="str">f"_{c.lower()}"</span> <span class="key">if</span> <span class="nam">c</span><span class="op">.</span><span class="nam">isupper</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">c</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">s</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="str">    Does not actually do anything, but tells mypy the 'data' of type Any (json, pyyaml, tomlkit) \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="str">    is actually a dict of string keys and Any values.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">T_config</span><span class="op">,</span> <span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_310_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-14 12:24 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,34 +1,31 @@
 
-****** Coverage for src/configuraptor/helpers.py: 100% ******
+****** Coverage for src/configuraptor/loaders/_types.py: 100% ******
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
+***** 4 statements   4 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-14 12:24 +0200
 
 
-1""" 
-2Contains stand-alone helper functions. 
-3""" 
+1import typing 
+2 
+3T_config = dict[str, typing.Any] 
 4 
 5 
-6def camel_to_snake(s: str) -> str: 
+6def as_tconfig(data: typing.Any) -> T_config: 
 7 """ 
-8 Convert CamelCase to snake_case. 
-9 
-10 Source: 
-11 https://stackoverflow.com/questions/1175208/elegant-python-function-to-
-convert-camelcase-to-snake-case 
-12 """ 
-13 return "".join([f"_{c.lower()}" if c.isupper() else c for c in s]).lstrip
-("_") 
+8 Does not actually do anything, but tells mypy the 'data' of type Any (json,
+pyyaml, tomlkit) \ 
+9 is actually a dict of string keys and Any values. 
+10 """ 
+11 return typing.cast(T_config, data) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-14 12:24 +0200
```

### Comparing `configuraptor-1.0.3/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.1.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/favicon_32.png` & `configuraptor-1.1.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/index.html` & `configuraptor-1.1.0/htmlcov/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:44 +0200
+            created at 2023-06-14 12:25 +0200
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
-                <td>144</td>
+                <td>145</td>
                 <td>0</td>
                 <td>3</td>
-                <td class="right" data-ratio="144 144">100%</td>
+                <td class="right" data-ratio="145 145">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_errors_py.html">src/configuraptor/errors.py</a></td>
                 <td>26</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="26 26">100%</td>
@@ -101,17 +101,24 @@
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_6c7dc8b73849fb97___init___py.html">src/configuraptor/loaders/__init__.py</a></td>
-                <td>4</td>
+                <td>14</td>
                 <td>0</td>
                 <td>2</td>
+                <td class="right" data-ratio="14 14">100%</td>
+            </tr>
+            <tr class="file">
+                <td class="name left"><a href="d_6c7dc8b73849fb97__types_py.html">src/configuraptor/loaders/_types.py</a></td>
+                <td>4</td>
+                <td>0</td>
+                <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_6c7dc8b73849fb97_loaders_310_py.html">src/configuraptor/loaders/loaders_310.py</a></td>
                 <td>5</td>
                 <td>0</td>
                 <td>6</td>
@@ -121,40 +128,47 @@
                 <td class="name left"><a href="d_6c7dc8b73849fb97_loaders_311_py.html">src/configuraptor/loaders/loaders_311.py</a></td>
                 <td>6</td>
                 <td>0</td>
                 <td>2</td>
                 <td class="right" data-ratio="6 6">100%</td>
             </tr>
             <tr class="file">
+                <td class="name left"><a href="d_6c7dc8b73849fb97_loaders_shared_py.html">src/configuraptor/loaders/loaders_shared.py</a></td>
+                <td>10</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="10 10">100%</td>
+            </tr>
+            <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_singleton_py.html">src/configuraptor/singleton.py</a></td>
                 <td>13</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="13 13">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>211</td>
+                <td>236</td>
                 <td>0</td>
                 <td>13</td>
-                <td class="right" data-ratio="211 211">100%</td>
+                <td class="right" data-ratio="236 236">100%</td>
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
-            created at 2023-06-14 11:44 +0200
+            created at 2023-06-14 12:25 +0200
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
@@ -2,25 +2,28 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-06-14 11:44 +0200
+coverage.py_v7.2.7, created at 2023-06-14 12:25 +0200
 
 Module                                   statements missing excluded coverage
 src/configuraptor/__about__.py           1          0       0        100%
 src/configuraptor/__init__.py            3          0       0        100%
 src/configuraptor/cls.py                 7          0       0        100%
-src/configuraptor/core.py                144        0       3        100%
+src/configuraptor/core.py                145        0       3        100%
 src/configuraptor/errors.py              26         0       0        100%
 src/configuraptor/helpers.py             2          0       0        100%
-src/configuraptor/loaders/__init__.py    4          0       2        100%
+src/configuraptor/loaders/__init__.py    14         0       2        100%
+src/configuraptor/loaders/_types.py      4          0       0        100%
 src/configuraptor/loaders/loaders_310.py 5          0       6        100%
 src/configuraptor/loaders/loaders_311.py 6          0       2        100%
+src/configuraptor/loaders/               10         0       0        100%
+loaders_shared.py
 src/configuraptor/singleton.py           13         0       0        100%
-Total                                    211        0       13       100%
+Total                                    236        0       13       100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-06-14 11:44 +0200
+coverage.py_v7.2.7, created at 2023-06-14 12:25 +0200
  ____
```

### Comparing `configuraptor-1.0.3/htmlcov/keybd_closed.png` & `configuraptor-1.1.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/keybd_open.png` & `configuraptor-1.1.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/htmlcov/status.json` & `configuraptor-1.1.0/htmlcov/status.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9856833735909822%*

 * *Differences: {"'files'": "{'d_eb75b6cf8f5eab40___about___py': {'hash': '592ad5b31e242df1a606d56d42dd873e'}, "*

 * *            "'d_eb75b6cf8f5eab40_core_py': {'hash': '63af632a38c5bd948c1e8996eb4ee94c', 'index': "*

 * *            "{'nums': {insert: [(2, 145)], delete: [2]}}}, 'd_6c7dc8b73849fb97___init___py': "*

 * *            "{'hash': '387fed3bd7e9638e77a3769fe2de3836', 'index': {'nums': {insert: [(2, 14)], "*

 * *            "delete: [2]}}}, 'd_6c7dc8b73849fb97_loaders_310_py': {'hash': "*

 * *            "'1afd90c369f649538d18695e2737585d […]*

```diff
@@ -184,32 +184,49 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/typedconfig/singleton.py"
             }
         },
         "d_6c7dc8b73849fb97___init___py": {
-            "hash": "31acd8370bf54e4b53a47e4f8088db0d",
+            "hash": "387fed3bd7e9638e77a3769fe2de3836",
             "index": {
                 "html_filename": "d_6c7dc8b73849fb97___init___py.html",
                 "nums": [
                     0,
                     1,
-                    4,
+                    14,
                     2,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/__init__.py"
             }
         },
+        "d_6c7dc8b73849fb97__types_py": {
+            "hash": "1a491a5575599b4c1c0e95472348d26b",
+            "index": {
+                "html_filename": "d_6c7dc8b73849fb97__types_py.html",
+                "nums": [
+                    0,
+                    1,
+                    4,
+                    0,
+                    0,
+                    0,
+                    0,
+                    0
+                ],
+                "relative_filename": "src/configuraptor/loaders/_types.py"
+            }
+        },
         "d_6c7dc8b73849fb97_loaders_310_py": {
-            "hash": "aa0dd3427c86a2e1b719bdc13eefeaa8",
+            "hash": "1afd90c369f649538d18695e2737585d",
             "index": {
                 "html_filename": "d_6c7dc8b73849fb97_loaders_310_py.html",
                 "nums": [
                     0,
                     1,
                     5,
                     6,
@@ -218,15 +235,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_310.py"
             }
         },
         "d_6c7dc8b73849fb97_loaders_311_py": {
-            "hash": "0138f8f658302cb92e8857fb25a0d5c6",
+            "hash": "74469c8e02e9fa066fcf5c98bf9ca8a8",
             "index": {
                 "html_filename": "d_6c7dc8b73849fb97_loaders_311_py.html",
                 "nums": [
                     0,
                     1,
                     6,
                     2,
@@ -234,16 +251,33 @@
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_311.py"
             }
         },
+        "d_6c7dc8b73849fb97_loaders_shared_py": {
+            "hash": "29bbd19f2094f5964490560a65a5aead",
+            "index": {
+                "html_filename": "d_6c7dc8b73849fb97_loaders_shared_py.html",
+                "nums": [
+                    0,
+                    1,
+                    10,
+                    0,
+                    0,
+                    0,
+                    0,
+                    0
+                ],
+                "relative_filename": "src/configuraptor/loaders/loaders_shared.py"
+            }
+        },
         "d_eb75b6cf8f5eab40___about___py": {
-            "hash": "b080702da1e189e343abce2366f2346f",
+            "hash": "592ad5b31e242df1a606d56d42dd873e",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -286,21 +320,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/cls.py"
             }
         },
         "d_eb75b6cf8f5eab40_core_py": {
-            "hash": "702e02c3a7e5ab4f5468f661da19f29b",
+            "hash": "63af632a38c5bd948c1e8996eb4ee94c",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_core_py.html",
                 "nums": [
                     0,
                     1,
-                    144,
+                    145,
                     3,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/core.py"
```

### Comparing `configuraptor-1.0.3/htmlcov/style.css` & `configuraptor-1.1.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/pytest_examples/some.toml` & `configuraptor-1.1.0/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/src/configuraptor/cls.py` & `configuraptor-1.1.0/src/configuraptor/cls.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/src/configuraptor/core.py` & `configuraptor-1.1.0/src/configuraptor/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,17 @@
 
     E.g. class Tool will be mapped to key tool.
     It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}}
     """
     if isinstance(data, str):
         data = Path(data)
     if isinstance(data, Path):
-        # todo: more than toml
         with data.open("rb") as f:
-            data = loaders.toml(f)
+            loader = loaders.get(data.suffix)
+            data = loader(f)
 
     if not data:
         return {}
 
     if key is None:
         # try to guess key by grabbing the first one or using the class name
         if len(data) == 1:
```

### Comparing `configuraptor-1.0.3/src/configuraptor/errors.py` & `configuraptor-1.1.0/src/configuraptor/errors.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/src/configuraptor/singleton.py` & `configuraptor-1.1.0/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/tests/test_singleton.py` & `configuraptor-1.1.0/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/tests/test_toml_basic.py` & `configuraptor-1.1.0/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/tests/test_toml_dataclass.py` & `configuraptor-1.1.0/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/tests/test_toml_existing.py` & `configuraptor-1.1.0/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/tests/test_toml_typedconfig_class.py` & `configuraptor-1.1.0/tests/test_toml_typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/LICENSE.txt` & `configuraptor-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.0.3/README.md` & `configuraptor-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 class Config:
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = load_into(Config, "example_from_docs.toml")
+    my_config = load_into(Config, "example_from_docs.toml")  # or .json, .yaml
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 
 
@@ -96,15 +96,15 @@
 
 class OtherConfig(TypedConfig):
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = OtherConfig.load("example_from_docs.toml")
+    my_config = OtherConfig.load("example_from_docs.toml")  # or .json, .yaml
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 ```
```

### Comparing `configuraptor-1.0.3/pyproject.toml` & `configuraptor-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,25 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "typeguard",
     "tomlkit; python_version < '3.11'",
+    "PyYAML",
 ]
 
 [template.plugins.default]
 src-layout = true
 
 [project.optional-dependencies]
 dev = [
     "su6[all]",
     "hatch",
+    "types-PyYAML",
 ]
 
 [project.urls]
 Documentation = "https://github.com/trialandsuccess/configuraptor#readme"
 Issues = "https://github.com/trialandsuccess/configuraptor/issues"
 Source = "https://github.com/trialandsuccess/configuraptor"
```

### Comparing `configuraptor-1.0.3/PKG-INFO` & `configuraptor-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.0.3
+Version: 1.1.0
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -12,19 +12,21 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
+Requires-Dist: pyyaml
 Requires-Dist: tomlkit; python_version < '3.11'
 Requires-Dist: typeguard
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: su6[all]; extra == 'dev'
+Requires-Dist: types-pyyaml; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img 
         align="center" 
         src="https://raw.githubusercontent.com/trialandsuccess/configuraptor/master/_static/configuraptor_circle.png" 
         alt="Classy Configuraptor"
@@ -97,15 +99,15 @@
 
 class Config:
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = load_into(Config, "example_from_docs.toml")
+    my_config = load_into(Config, "example_from_docs.toml")  # or .json, .yaml
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 
 
@@ -121,15 +123,15 @@
 
 class OtherConfig(TypedConfig):
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = OtherConfig.load("example_from_docs.toml")
+    my_config = OtherConfig.load("example_from_docs.toml")  # or .json, .yaml
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 ```
```

