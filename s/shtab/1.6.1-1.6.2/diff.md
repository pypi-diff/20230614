# Comparing `tmp/shtab-1.6.1.tar.gz` & `tmp/shtab-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shtab-1.6.1.tar", last modified: Mon Apr  3 22:32:04 2023, max compression
+gzip compressed data, was "shtab-1.6.2.tar", last modified: Wed Jun 14 16:51:48 2023, max compression
```

## Comparing `shtab-1.6.1.tar` & `shtab-1.6.2.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:32:04.067328 shtab-1.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:32:04.063327 shtab-1.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:32:04.067328 shtab-1.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-03 22:31:47.000000 shtab-1.6.1/.github/workflows/comment-bot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-03 22:31:47.000000 shtab-1.6.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-03 22:31:47.000000 shtab-1.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-03 22:31:47.000000 shtab-1.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-03 22:31:47.000000 shtab-1.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-03 22:31:47.000000 shtab-1.6.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-03 22:32:04.067328 shtab-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-03 22:31:47.000000 shtab-1.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:32:04.067328 shtab-1.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-03 22:31:47.000000 shtab-1.6.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-03 22:31:47.000000 shtab-1.6.1/docs/pydoc-markdown.yml
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-03 22:31:47.000000 shtab-1.6.1/docs/pydoc_markdown_shtab.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-03 22:31:47.000000 shtab-1.6.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-04-03 22:31:47.000000 shtab-1.6.1/docs/use.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:32:04.067328 shtab-1.6.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-04-03 22:31:47.000000 shtab-1.6.1/examples/customcomplete.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-04-03 22:31:47.000000 shtab-1.6.1/examples/docopt-greeter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-04-03 22:31:47.000000 shtab-1.6.1/examples/pathcomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:32:04.067328 shtab-1.6.1/meta/
--rw-r--r--   0 runner    (1001) docker     (123)    16145 2023-04-03 22:31:47.000000 shtab-1.6.1/meta/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-03 22:31:47.000000 shtab-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-03 22:31:47.000000 shtab-1.6.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-03 22:32:04.071328 shtab-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-03 22:31:47.000000 shtab-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:32:04.067328 shtab-1.6.1/shtab/
--rw-r--r--   0 runner    (1001) docker     (123)    30050 2023-04-03 22:31:47.000000 shtab-1.6.1/shtab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-03 22:31:47.000000 shtab-1.6.1/shtab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 22:32:03.000000 shtab-1.6.1/shtab/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-03 22:31:47.000000 shtab-1.6.1/shtab/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-03 22:31:47.000000 shtab-1.6.1/shtab/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:32:04.067328 shtab-1.6.1/shtab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-03 22:32:03.000000 shtab-1.6.1/shtab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-03 22:32:04.000000 shtab-1.6.1/shtab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 22:32:03.000000 shtab-1.6.1/shtab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-03 22:32:03.000000 shtab-1.6.1/shtab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-03 22:32:03.000000 shtab-1.6.1/shtab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:32:04.067328 shtab-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:31:47.000000 shtab-1.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-04-03 22:31:47.000000 shtab-1.6.1/tests/test_shtab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.395580 shtab-1.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-14 16:51:26.000000 shtab-1.6.2/.github/workflows/comment-bot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-14 16:51:26.000000 shtab-1.6.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-14 16:51:26.000000 shtab-1.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-14 16:51:26.000000 shtab-1.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-14 16:51:26.000000 shtab-1.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-14 16:51:26.000000 shtab-1.6.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-14 16:51:48.395580 shtab-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-14 16:51:26.000000 shtab-1.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-14 16:51:26.000000 shtab-1.6.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-14 16:51:26.000000 shtab-1.6.2/docs/pydoc-markdown.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-14 16:51:26.000000 shtab-1.6.2/docs/pydoc_markdown_shtab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 16:51:26.000000 shtab-1.6.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-14 16:51:26.000000 shtab-1.6.2/docs/use.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-06-14 16:51:26.000000 shtab-1.6.2/examples/customcomplete.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-06-14 16:51:26.000000 shtab-1.6.2/examples/docopt-greeter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-06-14 16:51:26.000000 shtab-1.6.2/examples/pathcomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)    16145 2023-06-14 16:51:26.000000 shtab-1.6.2/meta/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-14 16:51:26.000000 shtab-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:51:48.395580 shtab-1.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/shtab/
+-rw-r--r--   0 runner    (1001) docker     (123)    30014 2023-06-14 16:51:26.000000 shtab-1.6.2/shtab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 16:51:26.000000 shtab-1.6.2/shtab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-14 16:51:26.000000 shtab-1.6.2/shtab/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-14 16:51:26.000000 shtab-1.6.2/shtab/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.395580 shtab-1.6.2/shtab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.395580 shtab-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:26.000000 shtab-1.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-06-14 16:51:26.000000 shtab-1.6.2/tests/test_shtab.py
```

### Comparing `shtab-1.6.1/.github/workflows/comment-bot.yml` & `shtab-1.6.2/.github/workflows/comment-bot.yml`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/.github/workflows/test.yml` & `shtab-1.6.2/.github/workflows/test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python }}
     - name: Install
-      run: pip install -U -r requirements-dev.txt
+      run: pip install -U -e .[dev]
     - run: pytest
     - uses: codecov/codecov-action@v3
   deploy:
     needs: [check, test]
     name: PyPI Deploy
     runs-on: ubuntu-latest
     steps:
@@ -66,15 +66,14 @@
         token: ${{ secrets.GH_TOKEN || github.token }}
     - uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - id: dist
       uses: casperdcl/deploy-pypi@v2
       with:
-        requirements: twine setuptools wheel setuptools_scm[toml]
         build: true
         password: ${{ secrets.PYPI_TOKEN }}
         upload: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags') }}
     - if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
       name: Release
       run: |
         changelog=$(git log --pretty='format:%d%n- %s%n%b---' $(git tag --sort=v:refname | tail -n2 | head -n1)..HEAD)
```

### Comparing `shtab-1.6.1/.pre-commit-config.yaml` & `shtab-1.6.2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -32,22 +32,23 @@
     args: [-j8]
     additional_dependencies:
     - flake8-broken-line
     - flake8-bugbear
     - flake8-comprehensions
     - flake8-debugger
     - flake8-isort
+    - flake8-pyproject
     - flake8-string-format
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.1.1
+  rev: v1.3.0
   hooks:
   - id: mypy
     additional_dependencies: [types-setuptools]
 - repo: https://github.com/google/yapf
-  rev: v0.32.0
+  rev: v0.33.0
   hooks:
   - id: yapf
     args: [-i]
     additional_dependencies: [toml]
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
```

### Comparing `shtab-1.6.1/CONTRIBUTING.md` & `shtab-1.6.2/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## Tests
 
 When contributing pull requests, it's a good idea to run basic checks locally:
 
 ```bash
 # install development dependencies
-shtab (main)$ pip install pre-commit -r requirements-dev.txt
+shtab (main)$ pip install pre-commit -e .[dev]
 shtab (main)$ pre-commit install  # install pre-commit checks
 shtab (main)$ pytest              # run all tests
 ```
 
 ## Layout
 
 Most of the magic lives in [`shtab/__init__.py`](./shtab/__init__.py).
```

### Comparing `shtab-1.6.1/LICENCE` & `shtab-1.6.2/LICENCE`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/PKG-INFO` & `shtab-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: shtab
-Version: 1.6.1
+Version: 1.6.2
 Summary: Automagic shell tab completion for Python CLI applications
-Home-page: https://github.com/iterative/shtab
-Author: Casper da Costa-Luis
-Author-email: casper.dcl@physics.org
-Maintainer: Iterative
-Maintainer-email: support@iterative.ai
+Author-email: Casper da Costa-Luis <casper.dcl@physics.org>
+Maintainer-email: Iterative <support@iterative.ai>
 License: Apache-2.0
-Project-URL: Changelog, https://github.com/iterative/shtab/releases
-Project-URL: Documentation, https://docs.iterative.ai/shtab
+Project-URL: documentation, https://docs.iterative.ai/shtab
+Project-URL: repository, https://github.com/iterative/shtab
+Project-URL: changelog, https://github.com/iterative/shtab/releases
 Keywords: tab,complete,completion,shell,bash,zsh,argparse
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
@@ -56,17 +53,17 @@
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: System
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
-Provides: shtab
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: LICENCE
 
 |Logo|
 
 shtab
 =====
```

### Comparing `shtab-1.6.1/README.rst` & `shtab-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/docs/index.md` & `shtab-1.6.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/docs/pydoc-markdown.yml` & `shtab-1.6.2/docs/pydoc-markdown.yml`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/docs/pydoc_markdown_shtab.py` & `shtab-1.6.2/docs/pydoc_markdown_shtab.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/docs/use.md` & `shtab-1.6.2/docs/use.md`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/examples/customcomplete.py` & `shtab-1.6.2/examples/customcomplete.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/examples/docopt-greeter.py` & `shtab-1.6.2/examples/docopt-greeter.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/examples/pathcomplete.py` & `shtab-1.6.2/examples/pathcomplete.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     parser.add_argument("--dir", default=".").complete = shtab.DIRECTORY
     return parser
 
 
 if __name__ == "__main__":
     parser = get_main_parser()
     args = parser.parse_args()
-    print("received <file>={!r} --dir={!r}".format(args.file, args.dir))
+    print(f"received <file>={args.file!r} --dir={args.dir!r}")
```

### Comparing `shtab-1.6.1/meta/logo.png` & `shtab-1.6.2/meta/logo.png`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/shtab/__init__.py` & `shtab-1.6.2/shtab/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     return wrapper
 
 
 def get_completer(shell):
     try:
         return _SUPPORTED_COMPLETERS[shell]
     except KeyError:
-        raise NotImplementedError("shell (%s) must be in {%s}" %
-                                  (shell, ",".join(SUPPORTED_SHELLS)))
+        supported = ",".join(SUPPORTED_SHELLS)
+        raise NotImplementedError(f"shell ({shell}) must be in {supported}")
 
 
 @total_ordering
 class Choice:
     """
     Placeholder to mark a special completion `<type>`.
 
@@ -182,29 +182,28 @@
         discovered_subparsers = []
         for i, positional in enumerate(parser._get_positional_actions()):
             if positional.help == SUPPRESS:
                 continue
 
             if hasattr(positional, "complete"):
                 # shtab `.complete = ...` functions
-                compgens.append("{}_pos_{}_COMPGEN={}".format(
-                    prefix, i, complete2pattern(positional.complete, "bash", choice_type2fn)))
+                comp_pattern = complete2pattern(positional.complete, "bash", choice_type2fn)
+                compgens.append(f"{prefix}_pos_{i}_COMPGEN={comp_pattern}")
 
             if positional.choices:
                 # choices (including subparsers & shtab `.complete` functions)
                 log.debug(f"choices:{prefix}:{sorted(positional.choices)}")
 
                 this_positional_choices = []
                 for choice in positional.choices:
                     if isinstance(choice, Choice):
                         # append special completion type to `compgens`
                         # NOTE: overrides `.complete` attribute
                         log.debug(f"Choice.{choice.type}:{prefix}:{positional.dest}")
-                        compgens.append("{}_pos_{}_COMPGEN={}".format(
-                            prefix, i, choice_type2fn[choice.type]))
+                        compgens.append(f"{prefix}_pos_{i}_COMPGEN={choice_type2fn[choice.type]}")
                     elif isinstance(positional.choices, dict):
                         # subparser, so append to list of subparsers & recurse
                         log.debug("subcommand:%s", choice)
                         public_cmds = get_public_subcommands(positional)
                         if choice in public_cmds:
                             discovered_subparsers.append(str(choice))
                             this_positional_choices.append(str(choice))
@@ -212,76 +211,77 @@
                                 new_subparsers,
                                 new_option_strings,
                                 new_compgens,
                                 new_choices,
                                 new_nargs,
                             ) = recurse(
                                 positional.choices[choice],
-                                prefix + "_" + wordify(choice),
+                                f"{prefix}_{wordify(choice)}",
                             )
                             sub_subparsers.extend(new_subparsers)
                             sub_option_strings.extend(new_option_strings)
                             sub_compgens.extend(new_compgens)
                             sub_choices.extend(new_choices)
                             sub_nargs.extend(new_nargs)
                         else:
                             log.debug("skip:subcommand:%s", choice)
                     else:
                         # simple choice
                         this_positional_choices.append(str(choice))
 
                 if this_positional_choices:
-                    choices.append("{}_pos_{}_choices=('{}')".format(
-                        prefix, i, "' '".join(this_positional_choices)))
+                    choices_str = "' '".join(this_positional_choices)
+                    choices.append(f"{prefix}_pos_{i}_choices=('{choices_str}')")
 
             # skip default `nargs` values
             if positional.nargs not in (None, "1", "?"):
                 nargs.append(f"{prefix}_pos_{i}_nargs={positional.nargs}")
 
         if discovered_subparsers:
-            subparsers.append("{}_subparsers=('{}')".format(prefix,
-                                                            "' '".join(discovered_subparsers)))
+            subparsers_str = "' '".join(discovered_subparsers)
+            subparsers.append(f"{prefix}_subparsers=('{subparsers_str}')")
             log.debug(f"subcommands:{prefix}:{discovered_subparsers}")
 
         # optional arguments
-        option_strings.append("{}_option_strings=('{}')".format(
-            prefix, "' '".join(get_option_strings(parser))))
+        options_strings_str = "' '".join(get_option_strings(parser))
+        option_strings.append(f"{prefix}_option_strings=('{options_strings_str}')")
         for optional in parser._get_optional_actions():
             if optional == SUPPRESS:
                 continue
 
             for option_string in optional.option_strings:
                 if hasattr(optional, "complete"):
                     # shtab `.complete = ...` functions
-                    compgens.append("{}_{}_COMPGEN={}".format(
-                        prefix, wordify(option_string),
-                        complete2pattern(optional.complete, "bash", choice_type2fn)))
+                    comp_pattern_str = complete2pattern(optional.complete, "bash", choice_type2fn)
+                    compgens.append(
+                        f"{prefix}_{wordify(option_string)}_COMPGEN={comp_pattern_str}")
 
                 if optional.choices:
                     # choices (including shtab `.complete` functions)
                     this_optional_choices = []
                     for choice in optional.choices:
                         # append special completion type to `compgens`
                         # NOTE: overrides `.complete` attribute
                         if isinstance(choice, Choice):
                             log.debug(f"Choice.{choice.type}:{prefix}:{optional.dest}")
-                            compgens.append("{}_{}_COMPGEN={}".format(
-                                prefix, wordify(option_string), choice_type2fn[choice.type]))
+                            func_str = choice_type2fn[choice.type]
+                            compgens.append(
+                                f"{prefix}_{wordify(option_string)}_COMPGEN={func_str}")
                         else:
                             # simple choice
                             this_optional_choices.append(str(choice))
 
                     if this_optional_choices:
-                        choices.append("{}_{}_choices=('{}')".format(
-                            prefix, wordify(option_string), "' '".join(this_optional_choices)))
+                        this_choices_str = "' '".join(this_optional_choices)
+                        choices.append(
+                            f"{prefix}_{wordify(option_string)}_choices=('{this_choices_str}')")
 
                 # Check for nargs.
                 if optional.nargs is not None and optional.nargs != 1:
-                    nargs.append("{}_{}_nargs={}".format(prefix, wordify(option_string),
-                                                         optional.nargs))
+                    nargs.append(f"{prefix}_{wordify(option_string)}_nargs={optional.nargs}")
 
         # append recursion results
         subparsers.extend(sub_subparsers)
         option_strings.extend(sub_option_strings)
         compgens.extend(sub_compgens)
         choices.extend(sub_choices)
         nargs.extend(sub_nargs)
@@ -294,15 +294,15 @@
 @mark_completer("bash")
 def complete_bash(parser, root_prefix=None, preamble="", choice_functions=None):
     """
     Returns bash syntax autocompletion script.
 
     See `complete` for arguments.
     """
-    root_prefix = wordify("_shtab_" + (root_prefix or parser.prog))
+    root_prefix = wordify(f"_shtab_{root_prefix or parser.prog}")
     subparsers, option_strings, compgens, choices, nargs = get_bash_commands(
         parser, root_prefix, choice_functions=choice_functions)
 
     # References:
     # - https://www.gnu.org/software/bash/manual/html_node/
     #   Programmable-Completion.html
     # - https://opensource.com/article/18/3/creating-bash-completion-script
@@ -458,15 +458,15 @@
 def complete_zsh(parser, root_prefix=None, preamble="", choice_functions=None):
     """
     Returns zsh syntax autocompletion script.
 
     See `complete` for arguments.
     """
     prog = parser.prog
-    root_prefix = wordify("_shtab_" + (root_prefix or prog))
+    root_prefix = wordify(f"_shtab_{root_prefix or prog}")
 
     choice_type2fn = {k: v["zsh"] for k, v in CHOICE_FUNCTIONS.items()}
     if choice_functions:
         choice_type2fn.update(choice_functions)
 
     def is_opt_end(opt):
         return isinstance(opt, OPTION_END) or opt.nargs == REMAINDER
@@ -474,17 +474,16 @@
     def is_opt_multiline(opt):
         return isinstance(opt, OPTION_MULTI)
 
     def format_optional(opt):
         return (('{nargs}{options}"[{help}]"' if isinstance(
             opt, FLAG_OPTION) else '{nargs}{options}"[{help}]:{dest}:{pattern}"').format(
                 nargs=('"(- : *)"' if is_opt_end(opt) else '"*"' if is_opt_multiline(opt) else ""),
-                options=("{{{}}}".format(",".join(opt.option_strings))
-                         if len(opt.option_strings) > 1 else '"{}"'.format("".join(
-                             opt.option_strings))),
+                options=("{{{}}}".format(",".join(opt.option_strings)) if len(opt.option_strings)
+                         > 1 else '"{}"'.format("".join(opt.option_strings))),
                 help=escape_zsh(opt.help or ""),
                 dest=opt.dest,
                 pattern=complete2pattern(opt.complete, "zsh", choice_type2fn) if hasattr(
                     opt, "complete") else
                 (choice_type2fn[opt.choices[0].type] if isinstance(opt.choices[0], Choice) else
                  "({})".format(" ".join(map(str, opt.choices)))) if opt.choices else "",
             ).replace('""', ""))
@@ -534,15 +533,15 @@
                         if opt.help != SUPPRESS]
 
                     # positionals
                     arguments.extend(
                         format_positional(opt) for opt in subparser._get_positional_actions()
                         if not isinstance(opt.choices, dict) if opt.help != SUPPRESS)
 
-                    new_pref = prefix + "_" + wordify(cmd)
+                    new_pref = f"{prefix}_{wordify(cmd)}"
                     options = all_commands[new_pref] = {
                         "cmd": cmd, "help": (subparser.description or "").strip().split("\n")[0],
                         "arguments": arguments, "paths": [*paths, cmd]}
                     new_subcmds = recurse(subparser, new_pref, [*paths, cmd])
                     options["commands"] = {
                         all_commands[pref]["cmd"]: all_commands[pref]
                         for pref in new_subcmds if pref in all_commands}
@@ -560,71 +559,72 @@
         for prefix, options in all_commands.items() if options.get("commands")}
     subcommands.setdefault(root_prefix, all_commands[root_prefix])
     log.debug("subcommands:%s:%s", root_prefix, sorted(all_commands))
 
     def command_case(prefix, options):
         name = options["cmd"]
         commands = options["commands"]
-        case_fmt_on_no_sub = """{name}) _arguments -C ${prefix}_{name_wordify}_options ;;"""
+        case_fmt_on_no_sub = """{name}) _arguments -C -s ${prefix}_{name_wordify}_options ;;"""
         case_fmt_on_sub = """{name}) {prefix}_{name_wordify} ;;"""
 
         cases = []
         for _, options in sorted(commands.items()):
             fmt = case_fmt_on_sub if options.get("commands") else case_fmt_on_no_sub
             cases.append(
                 fmt.format(name=options["cmd"], name_wordify=wordify(options["cmd"]),
                            prefix=prefix))
         cases = "\n\t".expandtabs(8).join(cases)
 
-        return """\
+        return f"""\
 {prefix}() {{
   local context state line curcontext="$curcontext" one_or_more='(-)*' remainder='(*)'
 
   if ((${{{prefix}_options[(I)${{(q)one_or_more}}*]}} + ${{{prefix}_options[(I)${{(q)remainder}}*]}} == 0)); then  # noqa: E501
     {prefix}_options+=(': :{prefix}_commands' '*::: :->{name}')
   fi
-  _arguments -C ${prefix}_options
+  _arguments -C -s ${prefix}_options
 
   case $state in
     {name})
       words=($line[1] "${{words[@]}}")
       (( CURRENT += 1 ))
       curcontext="${{curcontext%:*:*}}:{prefix}-$line[1]:"
       case $line[1] in
         {cases}
       esac
   esac
 }}
-""".format(prefix=prefix, name=name, cases=cases)
+"""
 
     def command_option(prefix, options):
-        return """\
+        arguments = "\n  ".join(options["arguments"])
+        return f"""\
 {prefix}_options=(
   {arguments}
 )
-""".format(prefix=prefix, arguments="\n  ".join(options["arguments"]))
+"""
 
     def command_list(prefix, options):
         name = " ".join([prog, *options["paths"]])
-        commands = "\n    ".join('"{}:{}"'.format(escape_zsh(cmd), escape_zsh(opt["help"]))
+        commands = "\n    ".join(f'"{escape_zsh(cmd)}:{escape_zsh(opt["help"])}"'
                                  for cmd, opt in sorted(options["commands"].items()))
-        return """
+        return f"""
 {prefix}_commands() {{
   local _commands=(
     {commands}
   )
   _describe '{name} commands' _commands
-}}""".format(prefix=prefix, name=name, commands=commands)
+}}"""
 
-    preamble = """\
+    preamble = (f"""\
 # Custom Preamble
-{}
+{preamble.rstrip()}
 
 # End Custom Preamble
-""".format(preamble.rstrip()) if preamble else ""
+""" if preamble else "")
     # References:
     #   - https://github.com/zsh-users/zsh-completions
     #   - http://zsh.sourceforge.net/Doc/Release/Completion-System.html
     #   - https://mads-hartmann.com/2017/08/06/
     #     writing-zsh-completion-scripts.html
     #   - http://www.linux-mag.com/id/1106/
     return Template("""\
@@ -651,108 +651,108 @@
 
 
 @mark_completer("tcsh")
 def complete_tcsh(parser, root_prefix=None, preamble="", choice_functions=None):
     """
     Return tcsh syntax autocompletion script.
 
-    See `complete` for arguments.
+    root_prefix:
+      ignored (tcsh has no support for functions)
+
+    See `complete` for other arguments.
     """
     optionals_single = set()
     optionals_double = set()
     specials = []
     index_choices = defaultdict(dict)
 
     choice_type2fn = {k: v["tcsh"] for k, v in CHOICE_FUNCTIONS.items()}
     if choice_functions:
         choice_type2fn.update(choice_functions)
 
     def get_specials(arg, arg_type, arg_sel):
         if arg.choices:
             choice_strs = ' '.join(map(str, arg.choices))
-            yield "'{}/{}/({})/'".format(
-                arg_type,
-                arg_sel,
-                choice_strs,
-            )
-        elif hasattr(arg, "complete"):
+            yield f"'{arg_type}/{arg_sel}/({choice_strs})/'"
+        elif hasattr(arg, 'complete'):
             complete_fn = complete2pattern(arg.complete, 'tcsh', choice_type2fn)
             if complete_fn:
-                yield "'{}/{}/{}/'".format(
-                    arg_type,
-                    arg_sel,
-                    complete_fn,
-                )
+                yield f"'{arg_type}/{arg_sel}/{complete_fn}/'"
 
     def recurse_parser(cparser, positional_idx, requirements=None):
-        log_prefix = '| ' * positional_idx
-        log.debug('%sParser @ %d', log_prefix, positional_idx)
+        log_prefix = "| " * positional_idx
+        log.debug("%sParser @ %d", log_prefix, positional_idx)
         if requirements:
-            log.debug('%s- Requires: %s', log_prefix, ' '.join(requirements))
+            log.debug("%s- Requires: %s", log_prefix, " ".join(requirements))
         else:
             requirements = []
 
         for optional in cparser._get_optional_actions():
-            log.debug('%s| Optional: %s', log_prefix, optional.dest)
+            log.debug("%s| Optional: %s", log_prefix, optional.dest)
             if optional.help != SUPPRESS:
                 # Mingle all optional arguments for all subparsers
                 for optional_str in optional.option_strings:
-                    log.debug('%s| | %s', log_prefix, optional_str)
+                    log.debug("%s| | %s", log_prefix, optional_str)
                     if optional_str.startswith('--'):
                         optionals_double.add(optional_str[2:])
                     elif optional_str.startswith('-'):
                         optionals_single.add(optional_str[1:])
                     specials.extend(get_specials(optional, 'n', optional_str))
 
         for positional in cparser._get_positional_actions():
             if positional.help != SUPPRESS:
                 positional_idx += 1
-                log.debug('%s| Positional #%d: %s', log_prefix, positional_idx, positional.dest)
+                log.debug("%s| Positional #%d: %s", log_prefix, positional_idx, positional.dest)
                 index_choices[positional_idx][tuple(requirements)] = positional
                 if not requirements and isinstance(positional.choices, dict):
                     for subcmd, subparser in positional.choices.items():
-                        log.debug('%s| | SubParser: %s', log_prefix, subcmd)
+                        log.debug("%s| | SubParser: %s", log_prefix, subcmd)
                         recurse_parser(subparser, positional_idx, requirements + [subcmd])
 
     recurse_parser(parser, 0)
 
     for idx, ndict in index_choices.items():
         if len(ndict) == 1:
             # Single choice, no requirements
             arg = list(ndict.values())[0]
             specials.extend(get_specials(arg, 'p', str(idx)))
         else:
             # Multiple requirements
             nlist = []
             for nn, arg in ndict.items():
-                checks = [f'[ "$cmd[{iidx}]" == "{n}" ]' for iidx, n in enumerate(nn, start=2)]
                 if arg.choices:
-                    nlist.append('( {}echo "{}" || false )'.format(
-                        ' && '.join(checks + ['']),                 # Append the separator
-                        '\\n'.join(arg.choices),
-                    ))
-
+                    checks = [f'[ "$cmd[{iidx}]" == "{n}" ]' for iidx, n in enumerate(nn, start=2)]
+                    choices_str = "' '".join(arg.choices)
+                    checks_str = ' && '.join(checks + [f"echo '{choices_str}'"])
+                    nlist.append(f"( {checks_str} || false )")
             # Ugly hack
-            specials.append("'p@{}@`set cmd=($COMMAND_LINE); {}`@'".format(
-                str(idx), ' || '.join(nlist)))
+            nlist_str = ' || '.join(nlist)
+            specials.append(f"'p@{str(idx)}@`set cmd=($COMMAND_LINE); {nlist_str}`@'")
+
+    if optionals_double:
+        if optionals_single:
+            optionals_single.add('-')
+        else:
+            # Don't add a space after completing "--" from "-"
+            optionals_single = ('-', '-')
 
     return Template("""\
 # AUTOMATICALLY GENERATED by `shtab`
 
 ${preamble}
 
 complete ${prog} \\
         'c/--/(${optionals_double_str})/' \\
-        'c/-/(${optionals_single_str} -)/' \\
+        'c/-/(${optionals_single_str})/' \\
         ${optionals_special_str} \\
         'p/*/()/'""").safe_substitute(
         preamble=("\n# Custom Preamble\n" + preamble +
                   "\n# End Custom Preamble\n" if preamble else ""), root_prefix=root_prefix,
-        prog=parser.prog, optionals_double_str=' '.join(optionals_double),
-        optionals_single_str=' '.join(optionals_single),
+        prog=parser.prog, optionals_double_str=' '.join(sorted(optionals_double)),
+        optionals_single_str=' '.join(sorted(optionals_single)),
         optionals_special_str=' \\\n        '.join(specials))
 
 
 def complete(parser: ArgumentParser, shell: str = "bash", root_prefix: Opt[str] = None,
              preamble: Union[str, Dict] = "", choice_functions: Opt[Any] = None) -> str:
     """
     shell:
```

### Comparing `shtab-1.6.1/shtab/main.py` & `shtab-1.6.2/shtab/main.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.1/shtab.egg-info/PKG-INFO` & `shtab-1.6.2/shtab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: shtab
-Version: 1.6.1
+Version: 1.6.2
 Summary: Automagic shell tab completion for Python CLI applications
-Home-page: https://github.com/iterative/shtab
-Author: Casper da Costa-Luis
-Author-email: casper.dcl@physics.org
-Maintainer: Iterative
-Maintainer-email: support@iterative.ai
+Author-email: Casper da Costa-Luis <casper.dcl@physics.org>
+Maintainer-email: Iterative <support@iterative.ai>
 License: Apache-2.0
-Project-URL: Changelog, https://github.com/iterative/shtab/releases
-Project-URL: Documentation, https://docs.iterative.ai/shtab
+Project-URL: documentation, https://docs.iterative.ai/shtab
+Project-URL: repository, https://github.com/iterative/shtab
+Project-URL: changelog, https://github.com/iterative/shtab/releases
 Keywords: tab,complete,completion,shell,bash,zsh,argparse
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
@@ -56,17 +53,17 @@
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: System
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
-Provides: shtab
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: LICENCE
 
 |Logo|
 
 shtab
 =====
```

### Comparing `shtab-1.6.1/shtab.egg-info/SOURCES.txt` & `shtab-1.6.2/shtab.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENCE
 README.rst
 pyproject.toml
-requirements-dev.txt
-setup.cfg
-setup.py
 .github/workflows/comment-bot.yml
 .github/workflows/test.yml
 docs/index.md
 docs/pydoc-markdown.yml
 docs/pydoc_markdown_shtab.py
 docs/requirements.txt
 docs/use.md
@@ -23,10 +20,11 @@
 shtab/_dist_ver.py
 shtab/main.py
 shtab/py.typed
 shtab.egg-info/PKG-INFO
 shtab.egg-info/SOURCES.txt
 shtab.egg-info/dependency_links.txt
 shtab.egg-info/entry_points.txt
+shtab.egg-info/requires.txt
 shtab.egg-info/top_level.txt
 tests/__init__.py
 tests/test_shtab.py
```

### Comparing `shtab-1.6.1/tests/test_shtab.py` & `shtab-1.6.2/tests/test_shtab.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,24 @@
         self.init = init_script
 
     def test(self, cmd="1", failure_message=""):
         """Equivalent to `bash -c '{init}; [[ {cmd} ]]'`."""
         init = self.init + "\n" if self.init else ""
         proc = subprocess.Popen(["bash", "-o", "pipefail", "-ec", f"{init}[[ {cmd} ]]"])
         stdout, stderr = proc.communicate()
-        assert (0 == proc.wait() and not stdout and not stderr), """\
-{}
-{}
+        assert (0 == proc.wait() and not stdout and not stderr), f"""\
+{failure_message}
+{cmd}
 === stdout ===
-{}=== stderr ===
-{}""".format(failure_message, cmd, stdout or "", stderr or "")
+{stdout or ""}=== stderr ===
+{stderr or ""}"""
 
     def compgen(self, compgen_cmd, word, expected_completions, failure_message=""):
         self.test(
-            '"$(echo $(compgen {} -- "{}"))" = "{}"'.format(compgen_cmd, word,
-                                                            expected_completions),
+            f'"$(echo $(compgen {compgen_cmd} -- "{word}"))" = "{expected_completions}"',
             failure_message,
         )
 
 
 @pytest.mark.parametrize("init,test", [("export FOO=1", '"$FOO" -eq 1'), ("", '-z "$FOO"')])
 def test_bash(init, test):
     shell = Bash(init)
```

