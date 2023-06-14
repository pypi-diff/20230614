# Comparing `tmp/jupyter_core-5.3.0.tar.gz` & `tmp/jupyter_core-5.3.1.tar.gz`

## Comparing `jupyter_core-5.3.0.tar` & `jupyter_core-5.3.1.tar`

### file list

```diff
@@ -1,62 +1,61 @@
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.flake8
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0    27027 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/README.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/codecov.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/docs/Makefile
--rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/docs/conf.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/docs/index.rst
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/docs/make.bat
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/docs/api/jupyter_core.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/docs/api/jupyter_core.utils.rst
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/docs/api/modules.rst
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/examples/completions-zsh
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/examples/jupyter-completion.bash
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/__main__.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/application.py
--rw-r--r--   0        0        0    15524 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/command.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/migrate.py
--rw-r--r--   0        0        0    35515 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/py.typed
--rwxr-xr-x   0        0        0     3162 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/troubleshoot.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/__init__.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/mocking.py
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/test_application.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/test_async.py
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/test_command.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/test_migrate.py
--rw-r--r--   0        0        0    18258 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/test_paths.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython/nbextensions/myext.js
--rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/ipython_config.py
--rw-r--r--   0        0        0    21668 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/ipython_console_config.py
--rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/ipython_kernel_config.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/ipython_nbconvert_config.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/ipython_notebook_config.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/static/custom/custom.css
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/static/custom/custom.js
--rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/ipython_config.py
--rw-r--r--   0        0        0    21668 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/ipython_console_config.py
--rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/ipython_kernel_config.py
--rw-r--r--   0        0        0    38737 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/ipython_nbconvert_config.py
--rw-r--r--   0        0        0    19945 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/ipython_notebook_config.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/static/custom/custom.css
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/static/custom/custom.js
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter_core/utils/__init__.py
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/scripts/jupyter
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/scripts/jupyter-migrate
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/jupyter.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/LICENSE
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/pyproject.toml
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 jupyter_core-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.flake8
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    28512 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/README.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/docs/Makefile
+-rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/docs/conf.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/docs/index.rst
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/docs/make.bat
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/docs/api/jupyter_core.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/docs/api/jupyter_core.utils.rst
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/docs/api/modules.rst
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/examples/completions-zsh
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/examples/jupyter-completion.bash
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/__main__.py
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/application.py
+-rw-r--r--   0        0        0    15540 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/command.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/migrate.py
+-rw-r--r--   0        0        0    35565 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/py.typed
+-rwxr-xr-x   0        0        0     3170 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/troubleshoot.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/__init__.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/mocking.py
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/test_application.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/test_async.py
+-rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/test_command.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/test_migrate.py
+-rw-r--r--   0        0        0    18282 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/test_paths.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython/nbextensions/myext.js
+-rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/ipython_config.py
+-rw-r--r--   0        0        0    21668 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/ipython_console_config.py
+-rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/ipython_kernel_config.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/ipython_nbconvert_config.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/ipython_notebook_config.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/static/custom/custom.css
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/static/custom/custom.js
+-rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/ipython_config.py
+-rw-r--r--   0        0        0    21668 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/ipython_console_config.py
+-rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/ipython_kernel_config.py
+-rw-r--r--   0        0        0    38737 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/ipython_nbconvert_config.py
+-rw-r--r--   0        0        0    19945 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/ipython_notebook_config.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/static/custom/custom.css
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/static/custom/custom.js
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter_core/utils/__init__.py
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/scripts/jupyter
+-rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/scripts/jupyter-migrate
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/jupyter.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/LICENSE
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 jupyter_core-5.3.1/PKG-INFO
```

### Comparing `jupyter_core-5.3.0/.pre-commit-config.yaml` & `jupyter_core-5.3.1/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -16,27 +16,27 @@
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.21.0
+    rev: 0.23.1
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.254
+    rev: v0.0.270
     hooks:
       - id: ruff
         args: ["--fix"]
         exclude: script
```

### Comparing `jupyter_core-5.3.0/CHANGELOG.md` & `jupyter_core-5.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # Changes in jupyter-core
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 5.3.1
+
+([Full Changelog](https://github.com/jupyter/jupyter_core/compare/v5.3.0...c64421919f6627f82c8899018bba0836760331f4))
+
+### Bugs fixed
+
+- Better handling of config migration [#356](https://github.com/jupyter/jupyter_core/pull/356) ([@smartass101](https://github.com/smartass101))
+
+### Maintenance and upkeep improvements
+
+- Fix write_executable test [#351](https://github.com/jupyter/jupyter_core/pull/351) ([@blink1073](https://github.com/blink1073))
+- Use local coverage [#349](https://github.com/jupyter/jupyter_core/pull/349) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/jupyter_core/graphs/contributors?from=2023-03-16&to=2023-06-14&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_core+involves%3Ablink1073+updated%3A2023-03-16..2023-06-14&type=Issues) | [@davidbrochart](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_core+involves%3Adavidbrochart+updated%3A2023-03-16..2023-06-14&type=Issues) | [@jamescooke](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_core+involves%3Ajamescooke+updated%3A2023-03-16..2023-06-14&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_core+involves%3Apre-commit-ci+updated%3A2023-03-16..2023-06-14&type=Issues) | [@smartass101](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_core+involves%3Asmartass101+updated%3A2023-03-16..2023-06-14&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 5.3.0
 
 ([Full Changelog](https://github.com/jupyter/jupyter_core/compare/v5.2.0...6cfe9fc042a0f016a0d4545bc6790b8277d80c24))
 
 ### Bugs fixed
 
 - Fix pywin32 version constraint [#347](https://github.com/jupyter/jupyter_core/pull/347) ([@blink1073](https://github.com/blink1073))
@@ -17,16 +38,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/jupyter_core/graphs/contributors?from=2023-01-30&to=2023-03-16&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_core+involves%3Ablink1073+updated%3A2023-01-30..2023-03-16&type=Issues) | [@dcsaba89](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_core+involves%3Adcsaba89+updated%3A2023-01-30..2023-03-16&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_core+involves%3Apre-commit-ci+updated%3A2023-01-30..2023-03-16&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 5.2.0
 
 ([Full Changelog](https://github.com/jupyter/jupyter_core/compare/v5.1.5...98b9a1a94e79d1137246b4c1f8c16343b72b050c))
 
 ### Enhancements made
 
 - Set up shell command-line tab-completion for jupyter and subcommands [#337](https://github.com/jupyter/jupyter_core/pull/337) ([@azjps](https://github.com/azjps))
```

### Comparing `jupyter_core-5.3.0/README.md` & `jupyter_core-5.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Jupyter Core
 
 [![Build Status](https://github.com/jupyter/jupyter_core/actions/workflows/test.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyter/jupyter_core/actions/workflows/test.yml/badge.svg?query=branch%3Amain++)
-[![codecov](https://codecov.io/gh/jupyter/jupyter_core/branch/main/graph/badge.svg?token=IRZuxPXamU)](https://codecov.io/gh/jupyter/jupyter_core)
 [![Documentation Status](https://readthedocs.org/projects/jupyter-core/badge/?version=latest)](http://jupyter-core.readthedocs.io/en/latest/?badge=latest)
 
 Core common functionality of Jupyter projects.
 
 This package contains base application classes and configuration inherited by other projects.
 It doesn't do much on its own.
```

### Comparing `jupyter_core-5.3.0/.github/workflows/codeql-analysis.yml` & `jupyter_core-5.3.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/.github/workflows/prep-release.yml` & `jupyter_core-5.3.1/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/.github/workflows/publish-release.yml` & `jupyter_core-5.3.1/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/.github/workflows/test.yml` & `jupyter_core-5.3.1/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -37,23 +37,29 @@
             python-version: "3.10"
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - name: Test
         run: |
           hatch run cov:test
-      - name: Coverage
-        run: |
-          pip install codecov coverage[toml]
-          codecov
       - name: Check CLI
         run: |
           pip install .
           cd $HOME
           jupyter troubleshoot
+      - uses: jupyterlab/maintainer-tools/.github/actions/upload-coverage@v1
+
+  coverage:
+    runs-on: ubuntu-latest
+    if: always()
+    needs:
+      - build
+    steps:
+      - uses: actions/checkout@v3
+      - uses: jupyterlab/maintainer-tools/.github/actions/report-coverage@v1
 
   test_minimum_versions:
     name: Test Minimum Versions
     timeout-minutes: 20
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
@@ -148,15 +154,15 @@
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - uses: jupyterlab/maintainer-tools/.github/actions/check-links@v1
 
   tests_check: # This job does nothing and is only used for the branch protection
     if: always()
     needs:
-      - build
+      - coverage
       - test_lint
       - test_docs
       - test_minimum_versions
       - test_prereleases
       - check_links
       - check_release
       - test_sdist
```

### Comparing `jupyter_core-5.3.0/docs/Makefile` & `jupyter_core-5.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/docs/conf.py` & `jupyter_core-5.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/docs/make.bat` & `jupyter_core-5.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/docs/api/jupyter_core.rst` & `jupyter_core-5.3.1/docs/api/jupyter_core.rst`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/examples/completions-zsh` & `jupyter_core-5.3.1/examples/completions-zsh`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/examples/jupyter-completion.bash` & `jupyter_core-5.3.1/examples/jupyter-completion.bash`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/application.py` & `jupyter_core-5.3.1/jupyter_core/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,17 +164,25 @@
         print("Writing default config to: %s" % config_file)
         ensure_dir_exists(os.path.abspath(os.path.dirname(config_file)), 0o700)
         with open(config_file, mode="w", encoding="utf-8") as f:
             f.write(config_text)
 
     def migrate_config(self):
         """Migrate config/data from IPython 3"""
-        if os.path.exists(os.path.join(self.config_dir, "migrated")):
-            # already migrated
-            return
+        try:  # let's see if we can open the marker file
+            # for reading and updating (writing)
+            f_marker = open(os.path.join(self.config_dir, "migrated"), 'r+')  # noqa
+        except PermissionError:  # not readable and/or writable
+            return  # so let's give up migration in such an environment
+        except FileNotFoundError:  # cannot find the marker file
+            pass  # that means we have not migrated yet, so continue
+        else:  # if we got here without raising anything,
+            # that means the file exists
+            f_marker.close()
+            return  # so we must have already migrated -> bail out
 
         from .migrate import get_ipython_dir, migrate
 
         # No IPython dir, nothing to migrate
         if not os.path.exists(get_ipython_dir()):
             return
 
@@ -255,15 +263,15 @@
         self.update_config(cl_config)
         if allow_insecure_writes:
             issue_insecure_write_warning()
 
     def start(self):
         """Start the whole thing"""
         if self.subcommand:
-            os.execv(self.subcommand, [self.subcommand] + self.argv[1:])
+            os.execv(self.subcommand, [self.subcommand] + self.argv[1:])  # noqa
             raise NoStart()
 
         if self.subapp:
             self.subapp.start()
             raise NoStart()
 
         if self.generate_config:
```

### Comparing `jupyter_core-5.3.0/jupyter_core/command.py` & `jupyter_core-5.3.1/jupyter_core/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,24 +115,24 @@
     """
     if sys.platform.startswith("win"):
         # PATH is ignored when shell=False,
         # so rely on shutil.which
         cmd_path = which(cmd)
         if cmd_path is None:
             raise OSError("%r not found" % cmd, errno.ENOENT)
-        p = Popen([cmd_path] + argv[1:])
+        p = Popen([cmd_path] + argv[1:])  # noqa
         # Don't raise KeyboardInterrupt in the parent process.
         # Set this after spawning, to avoid subprocess inheriting handler.
         import signal
 
         signal.signal(signal.SIGINT, signal.SIG_IGN)
         p.wait()
         sys.exit(p.returncode)
     else:
-        os.execvp(cmd, argv)
+        os.execvp(cmd, argv)  # noqa
 
 
 def _jupyter_abspath(subcommand):
     """This method get the abspath of a specified jupyter-subcommand with no
     changes on ENV.
     """
     # get env PATH with self
```

### Comparing `jupyter_core-5.3.0/jupyter_core/migrate.py` & `jupyter_core-5.3.1/jupyter_core/migrate.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/paths.py` & `jupyter_core-5.3.1/jupyter_core/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,16 @@
         if stat_res.st_file_attributes & stat.FILE_ATTRIBUTE_HIDDEN:  # type:ignore
             return True
     except AttributeError:
         # allow AttributeError on PyPy for Windows
         # 'stat_result' object has no attribute 'st_file_attributes'
         # https://foss.heptapod.net/pypy/pypy/-/issues/3469
         warnings.warn(
-            "hidden files are not detectable on this system, so no file will be marked as hidden."
+            "hidden files are not detectable on this system, so no file will be marked as hidden.",
+            stacklevel=2,
         )
         pass
 
     return False
 
 
 def is_file_hidden_posix(abs_path: str, stat_res: Optional[Any] = None) -> bool:
@@ -1006,9 +1007,10 @@
     def format_warning(msg, *args, **kwargs):
         return str(msg) + "\n"
 
     warnings.formatwarning = format_warning  # type:ignore[assignment]
     warnings.warn(
         "WARNING: Insecure writes have been enabled via environment variable "
         "'JUPYTER_ALLOW_INSECURE_WRITES'! If this is not intended, remove the "
-        "variable or set its value to 'False'."
+        "variable or set its value to 'False'.",
+        stacklevel=2,
     )
```

### Comparing `jupyter_core-5.3.0/jupyter_core/troubleshoot.py` & `jupyter_core-5.3.1/jupyter_core/troubleshoot.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def subs(cmd: Union[List[str], str]) -> Optional[str]:
     """
     get data from commands that we need to run outside of python
     """
     try:
-        stdout = subprocess.check_output(cmd)
+        stdout = subprocess.check_output(cmd)  # noqa
         return stdout.decode("utf-8", "replace").strip()
     except (OSError, subprocess.CalledProcessError):
         return None
 
 
 def get_data() -> Dict[str, Any]:
     """
```

### Comparing `jupyter_core-5.3.0/jupyter_core/version.py` & `jupyter_core-5.3.1/jupyter_core/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 store the current version info of the jupyter_core.
 """
 import re
 from typing import List
 
 # Version string must appear intact for hatch versioning
-__version__ = "5.3.0"
+__version__ = "5.3.1"
 
 # Build up version_info tuple for backwards compatibility
 pattern = r"(?P<major>\d+).(?P<minor>\d+).(?P<patch>\d+)(?P<rest>.*)"
 match = re.match(pattern, __version__)
 assert match is not None  # noqa
 parts: List[object] = [int(match[part]) for part in ["major", "minor", "patch"]]
 if match["rest"]:
```

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/mocking.py` & `jupyter_core-5.3.1/jupyter_core/tests/mocking.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/test_application.py` & `jupyter_core-5.3.1/jupyter_core/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/test_async.py` & `jupyter_core-5.3.1/jupyter_core/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/test_command.py` & `jupyter_core-5.3.1/jupyter_core/tests/test_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,19 +58,24 @@
         script = path
 
     script.write(source)
     script.chmod(0o700)
 
     if sys.platform == "win32":
         try:
-            import pkg_resources
+            import importlib.resources
 
-            w = pkg_resources.resource_string("setuptools", "cli-32.exe")
+            if not hasattr(importlib.resources, 'files'):
+                raise ImportError
+            wp = importlib.resources.files('setuptools').joinpath('cli-32.exe')
+            w = wp.read_bytes()
         except (ImportError, FileNotFoundError, SystemError):
-            pytest.skip("Need pkg_resources/setuptools to make scripts executable on Windows")
+            pytest.skip(
+                "Need importlib.resources and setuptools to make scripts executable on Windows"
+            )
         exe.write(w, "wb")
         exe.chmod(0o700)
 
 
 def assert_output(cmd, expected):
     assert get_jupyter_output(cmd) == expected
```

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/test_migrate.py` & `jupyter_core-5.3.1/jupyter_core/tests/test_migrate.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import shutil
 from tempfile import mkdtemp
 from unittest.mock import patch
 
 import pytest
 
 from jupyter_core import migrate as migrate_mod
+from jupyter_core.application import JupyterApp
 from jupyter_core.migrate import (
     migrate,
     migrate_config,
     migrate_dir,
     migrate_file,
     migrate_one,
     migrate_static_custom,
@@ -49,15 +50,15 @@
     }
     env_patch = patch.dict(os.environ, env)
     env_patch.start()
 
     def fin():
         """Cleanup test env"""
         env_patch.stop()
-        shutil.rmtree(td)
+        shutil.rmtree(td, ignore_errors=os.name == 'nt')
 
     request.addfinalizer(fin)
 
     return env
 
 
 def touch(path, content=""):
@@ -212,7 +213,35 @@
 
 
 def test_migrate(env):
     shutil.copytree(dotipython, env["IPYTHONDIR"])
     migrate()
     assert os.path.exists(env["JUPYTER_CONFIG_DIR"])
     assert os.path.exists(env["JUPYTER_DATA_DIR"])
+
+
+def test_app_migrate(env):
+    shutil.copytree(dotipython, env["IPYTHONDIR"])
+    app = JupyterApp()
+    app.initialize([])
+    assert os.path.exists(env["JUPYTER_CONFIG_DIR"])
+    assert os.path.exists(env["JUPYTER_DATA_DIR"])
+
+
+def test_app_migrate_skip_if_marker(env):
+    shutil.copytree(dotipython, env["IPYTHONDIR"])
+    touch(pjoin(env["JUPYTER_CONFIG_DIR"], "migrated"), "done")
+    app = JupyterApp()
+    app.initialize([])
+    assert os.listdir(env["JUPYTER_CONFIG_DIR"]) == ["migrated"]
+    assert not os.path.exists(env["JUPYTER_DATA_DIR"])
+
+
+def test_app_migrate_skip_unwritable_marker(env):
+    shutil.copytree(dotipython, env["IPYTHONDIR"])
+    migrated_marker = pjoin(env["JUPYTER_CONFIG_DIR"], "migrated")
+    touch(migrated_marker, "done")
+    os.chmod(migrated_marker, 0)  # make it unworkable
+    app = JupyterApp()
+    app.initialize([])
+    assert os.listdir(env["JUPYTER_CONFIG_DIR"]) == ["migrated"]
+    assert not os.path.exists(env["JUPYTER_DATA_DIR"])
```

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/test_paths.py` & `jupyter_core-5.3.1/jupyter_core/tests/test_paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -470,15 +470,15 @@
 def test_is_hidden_win32_cpython():
     import ctypes  # noqa
 
     with tempfile.TemporaryDirectory() as root:
         subdir1 = os.path.join(root, "subdir")
         os.makedirs(subdir1)
         assert not is_hidden(subdir1, root)
-        subprocess.check_call(["attrib", "+h", subdir1])
+        subprocess.check_call(["attrib", "+h", subdir1])  # noqa
         assert is_hidden(subdir1, root)
         assert is_file_hidden(subdir1)
 
 
 @pytest.mark.skipif(
     not (
         sys.platform == "win32"
@@ -490,15 +490,15 @@
 def test_is_hidden_win32_pypy():
     import ctypes  # noqa
 
     with tempfile.TemporaryDirectory() as root:
         subdir1 = os.path.join(root, "subdir")
         os.makedirs(subdir1)
         assert not is_hidden(subdir1, root)
-        subprocess.check_call(["attrib", "+h", subdir1])
+        subprocess.check_call(["attrib", "+h", subdir1])  # noqa
 
         with warnings.catch_warnings(record=True) as w:
             # Cause all warnings to always be triggered.
             warnings.simplefilter("always")
             # Trigger a warning.
             assert not is_hidden(subdir1, root)
             # Verify the warning was triggered
@@ -523,15 +523,15 @@
 
 
 @pytest.mark.skipif(sys.platform != "win32", reason="only runs on windows")
 def test_secure_write_win32():
     def fetch_win32_permissions(filename):
         """Extracts file permissions on windows using icacls"""
         role_permissions = {}
-        proc = os.popen("icacls %s" % filename)
+        proc = os.popen("icacls %s" % filename)  # noqa
         lines = proc.read().splitlines()
         proc.close()
         for index, line in enumerate(lines):
             if index == 0:
                 line = line.split(filename)[-1].strip().lower()  # noqa
             match = re.match(r"\s*([^:]+):\(([^\)]*)\)", line)
             if match:
```

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/ipython_config.py` & `jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/ipython_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/ipython_console_config.py` & `jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/ipython_console_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/ipython_kernel_config.py` & `jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/ipython_kernel_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/dotipython/profile_default/static/custom/custom.js` & `jupyter_core-5.3.1/jupyter_core/tests/dotipython/profile_default/static/custom/custom.js`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/ipython_config.py` & `jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/ipython_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/ipython_console_config.py` & `jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/ipython_console_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/ipython_kernel_config.py` & `jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/ipython_kernel_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/ipython_nbconvert_config.py` & `jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/ipython_nbconvert_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/ipython_notebook_config.py` & `jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/ipython_notebook_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/tests/dotipython_empty/profile_default/static/custom/custom.js` & `jupyter_core-5.3.1/jupyter_core/tests/dotipython_empty/profile_default/static/custom/custom.js`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/jupyter_core/utils/__init__.py` & `jupyter_core-5.3.1/jupyter_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/LICENSE` & `jupyter_core-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_core-5.3.0/pyproject.toml` & `jupyter_core-5.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 [tool.hatch.envs.typing]
 features = ["test"]
 dependencies = ["mypy>=0.990"]
 [tool.hatch.envs.typing.scripts]
 test = "mypy --install-types --non-interactive {args:.}"
 
 [tool.hatch.envs.lint]
-dependencies = ["black==23.1.0", "mdformat>0.7", "ruff==0.0.254"]
+dependencies = ["black==23.3.0", "mdformat>0.7", "ruff==0.0.270"]
 detached = true
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:*.md}"
 ]
@@ -134,14 +134,18 @@
 filterwarnings= [
   # Fail on warnings
   "error",
   # Expected internal warnings
   "module:Jupyter is migrating its paths to use standard platformdirs:DeprecationWarning",
 ]
 
+[tool.coverage.run]
+relative_files = true
+source = ["jupyter_core"]
+
 [tool.coverage.report]
 exclude_lines = [
   "pragma: no cover",
   "def __repr__",
   "if self.debug:",
   "if settings.DEBUG",
   "raise AssertionError",
@@ -189,23 +193,26 @@
 # E402 Module level import not at top of file
 # T201 `print` found
 # B007 Loop control variable `i` not used within the loop body.
 # N802 Function name `assertIn` should be lowercase
 # S101 Use of `assert` detected
 # S108 Probable insecure usage of temporary file or directory: "/tmp"
 # PLR2004 Magic value used in comparison, consider replacing b'WITNESS A' with a constant variable
-"jupyter_core/tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802", "S101", "S108", "PLR2004"]
+# S603 `subprocess` call: check for execution of untrusted input
+"jupyter_core/tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802", "S101", "S108", "PLR2004", "S603"]
 # F821 Undefined name `get_config`
 "jupyter_core/tests/**/profile_default/*_config.py" = ["F821"]
 # T201 `print` found
 "jupyter_core/application.py" = ["T201"]
 "jupyter_core/command.py" = ["T201"]
 "jupyter_core/troubleshoot.py" = ["T201"]
 # N802 Function name `SetFileSecurity` should be lowercase
 "jupyter_core/paths.py" = ["N802", "N803", "N806"]
+# C901 Function is too complex
+"jupyter_core/migrate.py" = ["C901"]  # `migrate_static_custom` is too complex (11 > 10)
 
 [tool.interrogate]
 ignore-init-module=true
 ignore-private=true
 ignore-semiprivate=true
 ignore-property-decorators=true
 ignore-nested-functions=true
```

### Comparing `jupyter_core-5.3.0/PKG-INFO` & `jupyter_core-5.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_core
-Version: 5.3.0
+Version: 5.3.1
 Summary: Jupyter core package. A base package on which Jupyter projects rely.
 Project-URL: Homepage, https://jupyter.org
 Project-URL: Documentation, https://jupyter-core.readthedocs.io/
 Project-URL: Funding, https://numfocus.org/
 Project-URL: Source, https://github.com/jupyter/jupyter_core
 Project-URL: Tracker, https://github.com/jupyter/jupyter_core/issues
 Author-email: Jupyter Development Team <jupyter@googlegroups.org>
```

