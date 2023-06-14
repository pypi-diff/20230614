# Comparing `tmp/pyproject_api-1.5.1.tar.gz` & `tmp/pyproject_api-1.5.2.tar.gz`

## Comparing `pyproject_api-1.5.1.tar` & `pyproject_api-1.5.2.tar`

### file list

```diff
@@ -1,35 +1,33 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/.markdownlint.yaml
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/.readthedocs.yml
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tox.ini
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/whitelist.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/.github/workflows/check.yml
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/docs/changelog.rst
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/docs/conf.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/docs/index.rst
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/src/pyproject_api/__init__.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/src/pyproject_api/__main__.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/src/pyproject_api/_backend.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/src/pyproject_api/_backend.pyi
--rw-r--r--   0        0        0    20869 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/src/pyproject_api/_frontend.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/src/pyproject_api/_util.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/src/pyproject_api/_version.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/src/pyproject_api/_via_fresh_subprocess.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/src/pyproject_api/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tests/_build_sdist.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tests/test_backend.py
--rw-r--r--   0        0        0    14274 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tests/test_frontend.py
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tests/test_frontend_setuptools.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tests/test_main.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tests/test_util.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tests/test_version.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tests/demo_pkg_inline/build.pyi
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/LICENSE
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/README.md
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 pyproject_api-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.readthedocs.yml
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tox.ini
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.github/workflows/check.yml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/docs/changelog.rst
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/docs/conf.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/docs/index.rst
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/__main__.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_backend.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_backend.pyi
+-rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_frontend.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_util.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_version.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_via_fresh_subprocess.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/_build_sdist.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_backend.py
+-rw-r--r--   0        0        0    13891 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_frontend.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_frontend_setuptools.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_main.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_util.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_version.py
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/LICENSE
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/README.md
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/PKG-INFO
```

### Comparing `pyproject_api-1.5.1/CODE_OF_CONDUCT.md` & `pyproject_api-1.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.1/tox.ini` & `pyproject_api-1.5.2/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     fix
+    py312
     py311
     py310
     py39
     py38
     py37
     type
     docs
     pkg_meta
-isolated_build = true
 skip_missing_interpreters = true
-minversion = 3.22
 
 [testenv]
 description = run the tests with pytest under {envname}
-passenv =
+package = wheel
+wheel_build_env = .pkg
+extras =
+    testing
+pass_env =
     PYTEST_*
     SSL_CERT_FILE
-setenv =
+set_env =
     COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}{/}.coverage.{envname}}
-extras =
-    testing
 commands =
     pytest {tty:--color=yes} {posargs: --no-cov-on-fail --cov-context=test \
       --cov={envsitepackagesdir}{/}pyproject_api --cov={toxinidir}{/}tests --cov-config={toxinidir}{/}pyproject.toml \
       --cov-report=term-missing:skip-covered --cov-report=html:{envtmpdir}{/}htmlcov \
       --cov-report=xml:{toxworkdir}{/}coverage.{envname}.xml --junitxml={toxworkdir}{/}junit.{envname}.xml \
       tests}
 labels = test
-package = wheel
-wheel_build_env = .pkg
 
 [testenv:fix]
 description = run formatter and linters
-passenv =
-    {[testenv]passenv}
-    PROGRAMDATA
 skip_install = true
 deps =
-    pre-commit>=3.0.4
+    pre-commit>=3.3.2
+pass_env =
+    {[testenv]passenv}
+    PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure {tty:--color=always} {posargs}
 
 [testenv:type]
 description = run type check on code base
-setenv =
-    {tty:MYPY_FORCE_COLOR = 1}
 deps =
-    mypy==0.991
+    mypy==1.3
+set_env =
+    {tty:MYPY_FORCE_COLOR = 1}
 commands =
     mypy src/pyproject_api --strict
     mypy tests --strict
 
 [testenv:docs]
 description = build documentation
 extras =
@@ -71,14 +72,14 @@
 commands =
     python -m build -o {envtmpdir} -s -w .
     twine check --strict {envtmpdir}{/}*
     check-wheel-contents --no-config {envtmpdir}
 
 [testenv:dev]
 description = dev environment with all deps at {envdir}
-usedevelop = true
+package = editable
 extras =
     docs
     testing
 commands =
     python -m pip list --format=columns
     python -c "print(r'{envpython}')"
```

### Comparing `pyproject_api-1.5.1/.github/workflows/check.yml` & `pyproject_api-1.5.2/.github/workflows/check.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 name: check
 on:
   push:
+    tags-ignore: ["**"]
   pull_request:
   schedule:
     - cron: "0 8 * * *"
 
 concurrency:
   group: check-${{ github.ref }}
   cancel-in-progress: true
@@ -13,37 +14,34 @@
   test:
     name: test ${{ matrix.py }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         py:
+          - "3.12.0-beta.1"
           - "3.11"
           - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
         os:
-          - ubuntu-20.04
-          - windows-2022
-          - macos-12
+          - ubuntu-latest
+          - windows-latest
+          - macos-latest
     steps:
       - name: Setup python for tox
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Install tox
         run: python -m pip install tox
-      - name: Setup python2.7 as test dependency
-        uses: actions/setup-python@v4
-        with:
-          python-version: 2.7
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.py }}
       - name: Pick environment to run
         run: |
           import os; import platform; import sys; from pathlib import Path
@@ -69,48 +67,25 @@
       matrix:
         tox_env:
           - type
           - dev
           - docs
           - pkg_meta
         os:
-          - ubuntu-22.04
-          - windows-2022
+          - ubuntu-latest
+          - windows-latest
         exclude:
-          - { os: windows-2022, tox_env: pkg_meta }
+          - { os: windows-latest, tox_env: pkg_meta }
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup Python 3.11
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
       - name: Install tox
         run: python -m pip install tox
       - name: Run check for ${{ matrix.tox_env }}
         run: tox -e ${{ matrix.tox_env }}
         env:
           UPGRADE_ADVISORY: "yes"
-
-  publish:
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-    needs: [check, test]
-    runs-on: ubuntu-22.04
-    steps:
-      - name: Setup python to build package
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.11"
-      - name: Install build
-        run: python -m pip install build
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-      - name: Build package
-        run: pyproject-build -s -w . -o dist
-      - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.6.5
-        with:
-          skip_existing: true
-          user: __token__
-          password: ${{ secrets.pypi_password }}
```

### Comparing `pyproject_api-1.5.1/docs/changelog.rst` & `pyproject_api-1.5.2/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.1/docs/conf.py` & `pyproject_api-1.5.2/docs/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+# noqa: D100
 from __future__ import annotations
 
-from datetime import datetime
-
 from pyproject_api import __version__
 
 project = name = "pyproject_api"
 company = "tox-dev"
-copyright = f"2021-{datetime.today().year}, {company}"
+copyright = f"{company}"  # noqa: A001
 version, release = __version__, __version__.split("+")[0]
 
 extensions = [
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.extlinks",
     "sphinx.ext.autodoc",
     "sphinx_autodoc_typehints",
```

### Comparing `pyproject_api-1.5.1/docs/index.rst` & `pyproject_api-1.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.1/src/pyproject_api/__init__.py` & `pyproject_api-1.5.2/src/pyproject_api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""PyProject API interface."""
 from __future__ import annotations
 
 from ._frontend import (
     BackendFailed,
     CmdStatus,
     EditableResult,
     Frontend,
```

### Comparing `pyproject_api-1.5.1/src/pyproject_api/__main__.py` & `pyproject_api-1.5.2/src/pyproject_api/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from __future__ import annotations
+from __future__ import annotations  # noqa: D100
 
 import argparse
 import os
 import pathlib
 import sys
+from typing import TYPE_CHECKING
 
-from ._frontend import EditableResult, SdistResult, WheelResult
 from ._via_fresh_subprocess import SubprocessFrontend
 
+if TYPE_CHECKING:
+    from ._frontend import EditableResult, SdistResult, WheelResult
 
-def main_parser() -> argparse.ArgumentParser:
+
+def main_parser() -> argparse.ArgumentParser:  # noqa: D103
     parser = argparse.ArgumentParser(
         description=(
             "A pyproject.toml-based build frontend. "
             "This is mainly useful for debugging PEP-517 backends. "
             "This frontend will not do things like install required build dependencies."
         ),
     )
@@ -54,39 +57,39 @@
         "-o",
         type=pathlib.Path,
         help=f"output directory (defaults to {{srcdir}}{os.sep}dist)",
     )
     return parser
 
 
-def main(argv: list[str]) -> None:
+def main(argv: list[str]) -> None:  # noqa: D103
     parser = main_parser()
     args = parser.parse_args(argv)
 
     outdir = args.outdir or args.srcdir / "dist"
     # we intentionally do not build editable distributions by default
     distributions = args.distributions or ["sdist", "wheel"]
 
     frontend = SubprocessFrontend(*SubprocessFrontend.create_args_from_folder(args.srcdir)[:-1])
     res: SdistResult | WheelResult | EditableResult
 
     if "sdist" in distributions:
-        print("Building sdist...")
+        print("Building sdist...")  # noqa: T201
         res = frontend.build_sdist(outdir)
-        print(res.out)
-        print(res.err, file=sys.stderr)
+        print(res.out)  # noqa: T201
+        print(res.err, file=sys.stderr)  # noqa: T201
 
     if "wheel" in distributions:
-        print("Building wheel...")
+        print("Building wheel...")  # noqa: T201
         res = frontend.build_wheel(outdir)
-        print(res.out)
-        print(res.err, file=sys.stderr)
+        print(res.out)  # noqa: T201
+        print(res.err, file=sys.stderr)  # noqa: T201
 
     if "editable" in distributions:
-        print("Building editable wheel...")
+        print("Building editable wheel...")  # noqa: T201
         res = frontend.build_editable(outdir)
-        print(res.out)
-        print(res.err, file=sys.stderr)
+        print(res.out)  # noqa: T201
+        print(res.err, file=sys.stderr)  # noqa: T201
 
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `pyproject_api-1.5.1/src/pyproject_api/_backend.py` & `pyproject_api-1.5.2/src/pyproject_api/_backend.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.1/src/pyproject_api/_backend.pyi` & `pyproject_api-1.5.2/src/pyproject_api/_backend.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""Handles communication on the backend side between frontend and backend"""
-from typing import Any, Optional, Sequence
+from typing import Any, Sequence
 
-class MissingCommand(TypeError): ...
+class MissingCommand(TypeError): ...  # noqa: N818
 
 class BackendProxy:
     backend_module: str
-    backend_object: Optional[str]
+    backend_object: str | None
     backend: Any
-    def __init__(self, backend_module: str, backend_obj: Optional[str]) -> None: ...
+    def __init__(self, backend_module: str, backend_obj: str | None) -> None: ...
     def __call__(self, name: str, *args: Any, **kwargs: Any) -> Any: ...
-    def __str__(self) -> str: ...
     def _exit(self) -> None: ...
     def _optional_commands(self) -> dict[str, bool]: ...
 
 def run(argv: Sequence[str]) -> int: ...
 def read_line() -> bytearray: ...
 def flush() -> None: ...
```

### Comparing `pyproject_api-1.5.1/src/pyproject_api/_frontend.py` & `pyproject_api-1.5.2/src/pyproject_api/_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Build frontend for PEP-517"""
+"""Build frontend for PEP-517."""
 from __future__ import annotations
 
 import json
 import sys
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from pathlib import Path
@@ -26,15 +26,15 @@
     import tomli as tomllib
 
 _HERE = Path(__file__).parent
 ConfigSettings = Optional[Dict[str, Any]]
 
 
 class OptionalHooks(TypedDict, total=True):
-    """A flag indicating if the backend supports the optional hook or not"""
+    """A flag indicating if the backend supports the optional hook or not."""
 
     get_requires_for_build_sdist: bool
     prepare_metadata_for_build_wheel: bool
     get_requires_for_build_wheel: bool
     build_editable: bool
     get_requires_for_build_editable: bool
     prepare_metadata_for_build_editable: bool
@@ -50,102 +50,102 @@
     @abstractmethod
     def out_err(self) -> tuple[str, str]:
         """:return: standard output and standard error text"""
         raise NotImplementedError
 
 
 class RequiresBuildSdistResult(NamedTuple):
-    """Information collected while acquiring the source distribution build dependencies"""
+    """Information collected while acquiring the source distribution build dependencies."""
 
     #: wheel build dependencies
     requires: tuple[Requirement, ...]
     #: backend standard output while acquiring the source distribution build dependencies
     out: str
     #: backend standard output while acquiring the source distribution build dependencies
     err: str
 
 
 class RequiresBuildWheelResult(NamedTuple):
-    """Information collected while acquiring the wheel build dependencies"""
+    """Information collected while acquiring the wheel build dependencies."""
 
     #: wheel build dependencies
     requires: tuple[Requirement, ...]
     #: backend standard output while acquiring the wheel build dependencies
     out: str
     #: backend standard error while acquiring the wheel build dependencies
     err: str
 
 
 class RequiresBuildEditableResult(NamedTuple):
-    """Information collected while acquiring the wheel build dependencies"""
+    """Information collected while acquiring the wheel build dependencies."""
 
     #: editable wheel build dependencies
     requires: tuple[Requirement, ...]
     #: backend standard output while acquiring the editable wheel build dependencies
     out: str
     #: backend standard error while acquiring the editable wheel build dependencies
     err: str
 
 
 class MetadataForBuildWheelResult(NamedTuple):
-    """Information collected while acquiring the wheel metadata"""
+    """Information collected while acquiring the wheel metadata."""
 
     #: path to the wheel metadata
     metadata: Path
     #: backend standard output while generating the wheel metadata
     out: str
     #: backend standard output while generating the wheel metadata
     err: str
 
 
 class MetadataForBuildEditableResult(NamedTuple):
-    """Information collected while acquiring the editable metadata"""
+    """Information collected while acquiring the editable metadata."""
 
     #: path to the wheel metadata
     metadata: Path
     #: backend standard output while generating the editable wheel metadata
     out: str
     #: backend standard output while generating the editable wheel metadata
     err: str
 
 
 class SdistResult(NamedTuple):
-    """Information collected while building a source distribution"""
+    """Information collected while building a source distribution."""
 
     #: path to the built source distribution
     sdist: Path
     #: backend standard output while building the source distribution
     out: str
     #: backend standard output while building the source distribution
     err: str
 
 
 class WheelResult(NamedTuple):
-    """Information collected while building a wheel"""
+    """Information collected while building a wheel."""
 
     #: path to the built wheel artifact
     wheel: Path
     #: backend standard output while building the wheel
     out: str
     #: backend standard error while building the wheel
     err: str
 
 
 class EditableResult(NamedTuple):
-    """Information collected while building an editable wheel"""
+    """Information collected while building an editable wheel."""
 
     #: path to the built wheel artifact
     wheel: Path
     #: backend standard output while building the wheel
     out: str
     #: backend standard error while building the wheel
     err: str
 
 
-class BackendFailed(RuntimeError):
+class BackendFailed(RuntimeError):  # noqa: N818
     """An error of the build backend."""
 
     def __init__(self, result: dict[str, Any], out: str, err: str) -> None:
         super().__init__()
         #: standard output collected while running the command
         self.out = out
         #: standard error collected while running the command
@@ -168,31 +168,29 @@
             f"{self.__class__.__name__}("
             f"result=dict(code={self.code}, exc_type={self.exc_type!r},exc_msg={self.exc_msg!r}),"
             f" out={self.out!r}, err={self.err!r})"
         )
 
 
 class Frontend(ABC):
-    """
-    Abstract base class for a pyproject frontend.
-    """
+    """Abstract base class for a pyproject frontend."""
 
     #: backend key when the ``pyproject.toml`` does not specify it
     LEGACY_BUILD_BACKEND: str = "setuptools.build_meta:__legacy__"
     #: backend requirements when the ``pyproject.toml`` does not specify it
     LEGACY_REQUIRES: tuple[Requirement, ...] = (Requirement("setuptools >= 40.8.0"), Requirement("wheel"))
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         root: Path,
         backend_paths: tuple[Path, ...],
         backend_module: str,
         backend_obj: str | None,
         requires: tuple[Requirement, ...],
-        reuse_backend: bool = True,
+        reuse_backend: bool = True,  # noqa: FBT001, FBT002
     ) -> None:
         """
         Create a new frontend.
 
         :param root: the root path of the project
         :param backend_paths: paths to provision as available to import from for the build backend
         :param backend_module: the module where the backend lives
@@ -206,15 +204,16 @@
         self._backend_obj = backend_obj
         self.requires: tuple[Requirement, ...] = requires
         self._reuse_backend = reuse_backend
         self._optional_hooks: OptionalHooks | None = None
 
     @classmethod
     def create_args_from_folder(
-        cls, folder: Path
+        cls,
+        folder: Path,
     ) -> tuple[Path, tuple[Path, ...], str, str | None, tuple[Requirement, ...], bool]:
         """
         Frontend creation arguments from a python project folder (thould have a ``pypyproject.toml`` file per PEP-518).
 
         :param folder: the python project folder
         :return: the frontend creation args
 
@@ -295,15 +294,16 @@
         else:
             result, out, err = [], "", ""
         if not isinstance(result, list) or not all(isinstance(i, str) for i in result):
             self._unexpected_response("get_requires_for_build_wheel", result, "list of string", out, err)
         return RequiresBuildWheelResult(tuple(Requirement(r) for r in cast(List[str], result)), out, err)
 
     def get_requires_for_build_editable(
-        self, config_settings: ConfigSettings | None = None
+        self,
+        config_settings: ConfigSettings | None = None,
     ) -> RequiresBuildEditableResult:
         """
         Get build requirements for an editable wheel build (per PEP-660).
 
         :param config_settings: run arguments
         :return: outcome
         """
@@ -312,15 +312,17 @@
         else:
             result, out, err = [], "", ""
         if not isinstance(result, list) or not all(isinstance(i, str) for i in result):
             self._unexpected_response("get_requires_for_build_editable", result, "list of string", out, err)
         return RequiresBuildEditableResult(tuple(Requirement(r) for r in cast(List[str], result)), out, err)
 
     def prepare_metadata_for_build_wheel(
-        self, metadata_directory: Path, config_settings: ConfigSettings | None = None
+        self,
+        metadata_directory: Path,
+        config_settings: ConfigSettings | None = None,
     ) -> MetadataForBuildWheelResult:
         """
         Build wheel metadata (per PEP-517).
 
         :param metadata_directory: where to generate the metadata
         :param config_settings: build arguments
         :return: metadata generation result
@@ -339,21 +341,24 @@
         if not isinstance(basename, str):
             self._unexpected_response("prepare_metadata_for_build_wheel", basename, str, out, err)
         result = metadata_directory / basename
         return MetadataForBuildWheelResult(result, out, err)
 
     def _check_metadata_dir(self, metadata_directory: Path) -> None:
         if metadata_directory == self._root:
-            raise RuntimeError(f"the project root and the metadata directory can't be the same {self._root}")
+            msg = f"the project root and the metadata directory can't be the same {self._root}"
+            raise RuntimeError(msg)
         if metadata_directory.exists():  # start with fresh
             ensure_empty_dir(metadata_directory)
         metadata_directory.mkdir(parents=True, exist_ok=True)
 
     def prepare_metadata_for_build_editable(
-        self, metadata_directory: Path, config_settings: ConfigSettings | None = None
+        self,
+        metadata_directory: Path,
+        config_settings: ConfigSettings | None = None,
     ) -> MetadataForBuildEditableResult:
         """
         Build editable wheel metadata (per PEP-660).
 
         :param metadata_directory: where to generate the metadata
         :param config_settings: build arguments
         :return: metadata generation result
@@ -438,41 +443,53 @@
             config_settings=config_settings,
             metadata_directory=metadata_directory,
         )
         if not isinstance(basename, str):
             self._unexpected_response("build_editable", basename, str, out, err)
         return EditableResult(wheel_directory / basename, out, err)
 
-    def _unexpected_response(self, cmd: str, got: Any, expected_type: Any, out: str, err: str) -> NoReturn:
+    def _unexpected_response(  # noqa: PLR0913
+        self,
+        cmd: str,
+        got: Any,
+        expected_type: Any,
+        out: str,
+        err: str,
+    ) -> NoReturn:
         msg = f"{cmd!r} on {self.backend!r} returned {got!r} but expected type {expected_type!r}"
         raise BackendFailed({"code": None, "exc_type": TypeError.__name__, "exc_msg": msg}, out, err)
 
     def _metadata_from_built_wheel(
-        self, config_settings: ConfigSettings | None, metadata_directory: Path | None, cmd: str
+        self,
+        config_settings: ConfigSettings | None,
+        metadata_directory: Path | None,
+        cmd: str,
     ) -> tuple[str, str, str]:
         with self._wheel_directory() as wheel_directory:
             wheel_result = getattr(self, cmd)(
                 wheel_directory=wheel_directory,
                 config_settings=config_settings,
                 metadata_directory=None,  # let the backend populate the metadata
             )
             wheel = wheel_result.wheel
             if not wheel.exists():
-                raise RuntimeError(f"missing wheel file return by backed {wheel!r}")
+                msg = f"missing wheel file return by backed {wheel!r}"
+                raise RuntimeError(msg)
             out, err = wheel_result.out, wheel_result.err
             extract_to = str(metadata_directory)
             basename = None
             with ZipFile(str(wheel), "r") as zip_file:
                 for name in zip_file.namelist():  # pragma: no branch
                     path = Path(name)
                     if path.parts[0].endswith(".dist-info"):
                         basename = path.parts[0]
                         zip_file.extract(name, extract_to)
             if basename is None:  # pragma: no branch
-                raise RuntimeError(f"no .dist-info found inside generated wheel {wheel}")
+                msg = f"no .dist-info found inside generated wheel {wheel}"
+                raise RuntimeError(msg)
         return basename, err, out
 
     @contextmanager
     def _wheel_directory(self) -> Iterator[Path]:
         with TemporaryDirectory() as wheel_directory:
             yield Path(wheel_directory)
 
@@ -480,15 +497,15 @@
         with NamedTemporaryFile(prefix=f"pep517_{cmd}-") as result_file_marker:
             result_file = Path(result_file_marker.name).with_suffix(".json")
             msg = json.dumps(
                 {
                     "cmd": cmd,
                     "kwargs": {k: (str(v) if isinstance(v, Path) else v) for k, v in kwargs.items()},
                     "result": str(result_file),
-                }
+                },
             )
             with self._send_msg(cmd, result_file, msg) as status:
                 while not status.done:  # pragma: no branch
                     sleep(0.001)  # wait a bit for things to happen
             if result_file.exists():
                 try:
                     with result_file.open("rt") as result_handler:
```

### Comparing `pyproject_api-1.5.1/src/pyproject_api/_via_fresh_subprocess.py` & `pyproject_api-1.5.2/src/pyproject_api/_via_fresh_subprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import os
 import sys
 from contextlib import contextmanager
-from pathlib import Path
 from subprocess import PIPE, Popen
 from threading import Thread
-from typing import IO, Any, Iterator, Tuple, cast
-
-from packaging.requirements import Requirement
+from typing import IO, TYPE_CHECKING, Any, Iterator, Tuple, cast
 
 from ._frontend import CmdStatus, Frontend
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from packaging.requirements import Requirement
+
 
 class SubprocessCmdStatus(CmdStatus, Thread):
     def __init__(self, process: Popen[str]) -> None:
         super().__init__()
         self.process = process
         self._out_err: tuple[str, str] | None = None
         self.start()
@@ -30,40 +32,42 @@
     def out_err(self) -> tuple[str, str]:
         return cast(Tuple[str, str], self._out_err)
 
 
 class SubprocessFrontend(Frontend):
     """A frontend that creates fresh subprocess at every call to communicate with the backend."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         root: Path,
         backend_paths: tuple[Path, ...],
         backend_module: str,
         backend_obj: str | None,
         requires: tuple[Requirement, ...],
-    ):
+    ) -> None:
         """
+        Create a subprocess frontend.
+
         :param root: the root path to the built project
         :param backend_paths: paths that are available on the python path for the backend
         :param backend_module: module where the backend is located
         :param backend_obj: object within the backend module identifying the backend
         :param requires: seed requirements for the backend
         """
         super().__init__(root, backend_paths, backend_module, backend_obj, requires, reuse_backend=False)
         self.executable = sys.executable
 
     @contextmanager
-    def _send_msg(self, cmd: str, result_file: Path, msg: str) -> Iterator[SubprocessCmdStatus]:  # noqa: U100
+    def _send_msg(self, cmd: str, result_file: Path, msg: str) -> Iterator[SubprocessCmdStatus]:  # noqa: ARG002
         env = os.environ.copy()
         backend = os.pathsep.join(str(i) for i in self._backend_paths).strip()
         if backend:
             env["PYTHONPATH"] = backend
         process = Popen(
-            args=[self.executable] + self.backend_args,
+            args=[self.executable, *self.backend_args],
             stdout=PIPE,
             stderr=PIPE,
             stdin=PIPE,
             universal_newlines=True,
             cwd=self._root,
             env=env,
         )
```

### Comparing `pyproject_api-1.5.1/tests/test_backend.py` & `pyproject_api-1.5.2/tests/test_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import json
-from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import pytest
-import pytest_mock
 
 from pyproject_api._backend import BackendProxy, run
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    import pytest_mock
+
 
 def test_invalid_module(capsys: pytest.CaptureFixture[str]) -> None:
     with pytest.raises(ImportError):
         run([str(False), "an.invalid.module"])
 
     captured = capsys.readouterr()
     assert "failed to start backend" in captured.err
@@ -72,15 +75,15 @@
     ret = run([str(False), "a.dummy.module"])
 
     assert ret == 0
     captured = capsys.readouterr()
     assert "started backend FakeBackendProxy" in captured.out
     assert "Backend: run command dummy_command with args {'foo': 'bar'}" in captured.out
     assert "Backend: Wrote response " in captured.out
-    assert "" == captured.err
+    assert not captured.err
 
 
 def test_reuse_process(mocker: pytest_mock.MockerFixture, capsys: pytest.CaptureFixture[str], tmp_path: Path) -> None:
     """Validate behavior when reusing the backend proxy process.
 
     There are a couple of things we'd like to check here:
 
@@ -97,15 +100,15 @@
     commands = [
         json.dumps({"cmd": "dummy_command_a", "kwargs": {"foo": "bar"}, "result": results[0]}),
         json.dumps({"cmd": "dummy_command_b", "kwargs": {"baz": "qux"}, "result": results[1]}),
         json.dumps({"cmd": "dummy_command_c", "kwargs": {"win": "wow"}, "result": results[2]}),
         json.dumps({"cmd": "_exit", "kwargs": {}, "result": results[3]}),
     ]
 
-    def fake_backend(name: str, *args: Any, **kwargs: Any) -> Any:  # noqa: U100
+    def fake_backend(name: str, *args: Any, **kwargs: Any) -> Any:  # noqa: ARG001
         if name == "dummy_command_b":
             raise SystemExit(2)
 
         return "dummy-result"
 
     backend_proxy = mocker.MagicMock(spec=BackendProxy)
     backend_proxy.side_effect = fake_backend
```

### Comparing `pyproject_api-1.5.1/tests/test_frontend.py` & `pyproject_api-1.5.2/tests/test_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from pathlib import Path
 from textwrap import dedent
 from typing import Callable
 
 import pytest
 from packaging.requirements import Requirement
-from virtualenv import session_via_cli
 
 from pyproject_api._frontend import BackendFailed
 from pyproject_api._via_fresh_subprocess import SubprocessFrontend
 
 
 @pytest.fixture()
 def local_builder(tmp_path: Path) -> Callable[[str], Path]:
@@ -303,16 +302,7 @@
     exc = context.value
     assert exc.code is None
     assert not exc.err
     assert " build_editable " in exc.out
     assert not exc.args
     assert exc.exc_type == "TypeError"
     assert exc.exc_msg == "'build_editable' on 'build' returned 1 but expected type <class 'str'>"
-
-
-def test_can_build_on_python_2(demo_pkg_inline: Path, tmp_path: Path) -> None:
-    frontend = SubprocessFrontend(*SubprocessFrontend.create_args_from_folder(demo_pkg_inline)[:-1])
-    env = session_via_cli(["-p", "2.7", str(tmp_path / "venv")])
-    env.run()
-    frontend.executable = str(env.creator.exe)
-
-    frontend.build_sdist(tmp_path)
```

### Comparing `pyproject_api-1.5.1/tests/test_frontend_setuptools.py` & `pyproject_api-1.5.2/tests/test_frontend_setuptools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from __future__ import annotations
 
 import sys
 from contextlib import contextmanager
-from pathlib import Path
 from stat import S_IWGRP, S_IWOTH, S_IWUSR
-from typing import Iterator, NamedTuple
+from typing import TYPE_CHECKING, Iterator, NamedTuple
 
 import pytest
-from _pytest.tmpdir import TempPathFactory
 from packaging.requirements import Requirement
-from pytest_mock import MockerFixture
 
 from pyproject_api._frontend import BackendFailed
 from pyproject_api._via_fresh_subprocess import SubprocessFrontend
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from _pytest.tmpdir import TempPathFactory
+    from pytest_mock import MockerFixture
+
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from importlib.metadata import Distribution, EntryPoint
 else:  # pragma: no cover (<py38)
     from importlib_metadata import Distribution, EntryPoint
 
 
 @pytest.fixture(scope="session")
 def frontend_setuptools(tmp_path_factory: TempPathFactory) -> SubprocessFrontend:
     prj = tmp_path_factory.mktemp("proj")
     (prj / "pyproject.toml").write_text(
-        '[build-system]\nrequires=["setuptools","wheel"]\nbuild-backend = "setuptools.build_meta"'
+        '[build-system]\nrequires=["setuptools","wheel"]\nbuild-backend = "setuptools.build_meta"',
     )
     cfg = """
         [metadata]
         name = demo
         version = 1.0
 
         [options]
@@ -69,15 +72,15 @@
 def test_setuptools_prepare_metadata_for_build_wheel(frontend_setuptools: SubprocessFrontend, tmp_path: Path) -> None:
     meta = tmp_path / "meta"
     result = frontend_setuptools.prepare_metadata_for_build_wheel(metadata_directory=meta)
     dist = Distribution.at(str(result.metadata))
     assert list(dist.entry_points) == [EntryPoint(name="demo_exe", value="demo:a", group="console_scripts")]
     assert dist.version == "1.0"
     assert dist.metadata["Name"] == "demo"
-    values = [v for k, v in dist.metadata.items() if k == "Requires-Dist"]  # type: ignore
+    values = [v for k, v in dist.metadata.items() if k == "Requires-Dist"]  # type: ignore[attr-defined]
     # ignore because "PackageMetadata" has no attribute "items"
     assert values == ["requests (>2)", "magic (>3)"]
     assert isinstance(result.out, str)
     assert isinstance(result.err, str)
 
     # call it again regenerates it because frontend always deletes earlier content
     before = result.metadata.stat().st_mtime
@@ -131,15 +134,15 @@
     assert context.value.args == ()
     assert repr(context.value)
     assert str(context.value)
     assert repr(context.value) != str(context.value)
 
 
 def test_bad_message(frontend_setuptools: SubprocessFrontend, tmp_path: Path) -> None:
-    with frontend_setuptools._send_msg("bad_cmd", tmp_path / "a", "{{") as status:
+    with frontend_setuptools._send_msg("bad_cmd", tmp_path / "a", "{{") as status:  # noqa: SLF001
         while not status.done:  # pragma: no branch
             pass
     out, err = status.out_err()
     assert out
     assert "Backend: incorrect request to backend: bytearray(b'{{')" in err
```

### Comparing `pyproject_api-1.5.1/tests/test_main.py` & `pyproject_api-1.5.2/tests/test_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
-import pytest_mock
 
 import pyproject_api.__main__
 from pyproject_api._frontend import EditableResult, SdistResult, WheelResult
 
+if TYPE_CHECKING:
+    import pytest_mock
+
 
 @pytest.mark.parametrize(
     ("cli_args", "srcdir", "outdir", "hooks"),
     [
         (
             [],
             Path.cwd(),
@@ -52,15 +55,15 @@
             ["-s", "-w"],
             Path.cwd(),
             Path.cwd() / "dist",
             ["build_sdist", "build_wheel"],
         ),
     ],
 )
-def test_parse_args(
+def test_parse_args(  # noqa: PLR0913
     mocker: pytest_mock.MockerFixture,
     capsys: pytest.CaptureFixture[str],
     cli_args: list[str],
     srcdir: Path,
     outdir: Path,
     hooks: list[str],
 ) -> None:
@@ -68,15 +71,17 @@
     subprocess_frontend.create_args_from_folder.return_value = (srcdir, (), "foo.bar", "baz", (), True)
     subprocess_frontend.return_value.build_sdist.return_value = SdistResult(
         sdist=outdir / "foo.whl",
         out="sdist out",
         err="sdist err",
     )
     subprocess_frontend.return_value.build_wheel.return_value = WheelResult(
-        wheel=outdir / "foo.whl", out="wheel out", err="wheel err"
+        wheel=outdir / "foo.whl",
+        out="wheel out",
+        err="wheel err",
     )
     subprocess_frontend.return_value.build_editable.return_value = EditableResult(
         wheel=outdir / "foo.whl",
         out="editable wheel out",
         err="editable wheel err",
     )
```

### Comparing `pyproject_api-1.5.1/tests/test_util.py` & `pyproject_api-1.5.2/tests/test_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 from pyproject_api._util import ensure_empty_dir
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 def test_ensure_empty_dir_on_empty(tmp_path: Path) -> None:
     ensure_empty_dir(tmp_path)
     assert list(tmp_path.iterdir()) == []
 
 
 def test_ensure_empty_dir_on_path_missing(tmp_path: Path) -> None:
```

### Comparing `pyproject_api-1.5.1/tests/demo_pkg_inline/build.py` & `pyproject_api-1.5.2/tests/demo_pkg_inline/build.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,138 @@
 """
 Please keep this file Python 2.7 compatible.
 See https://tox.readthedocs.io/en/rewrite/development.html#code-style-guide
 """
+from __future__ import annotations
 
 import os
 import sys
 import tarfile
+from pathlib import Path
 from textwrap import dedent
 from zipfile import ZipFile
 
 name = "demo_pkg_inline"
 pkg_name = name.replace("_", "-")
 
 version = "1.0.0"
-dist_info = "{}-{}.dist-info".format(name, version)
-logic = "{}/__init__.py".format(name)
-metadata = "{}/METADATA".format(dist_info)
-wheel = "{}/WHEEL".format(dist_info)
-record = "{}/RECORD".format(dist_info)
+dist_info = f"{name}-{version}.dist-info"
+logic = f"{name}/__init__.py"
+metadata_file = f"{dist_info}/METADATA"
+wheel = f"{dist_info}/WHEEL"
+record = f"{dist_info}/RECORD"
 content = {
-    logic: "def do():\n    print('greetings from {}')".format(name),
+    logic: f"def do():\n    print('greetings from {name}')",
 }
 metadata = {
-    metadata: """
+    metadata_file: """
         Metadata-Version: 2.1
         Name: {}
         Version: {}
         Summary: UNKNOWN
         Home-page: UNKNOWN
         Author: UNKNOWN
         Author-email: UNKNOWN
         License: UNKNOWN
         Platform: UNKNOWN
 
         UNKNOWN
        """.format(
-        pkg_name, version
+        pkg_name,
+        version,
     ),
     wheel: """
         Wheel-Version: 1.0
         Generator: {}-{}
         Root-Is-Purelib: true
         Tag: py{}-none-any
        """.format(
-        name, version, sys.version_info[0]
+        name,
+        version,
+        sys.version_info[0],
     ),
-    "{}/top_level.txt".format(dist_info): name,
+    f"{dist_info}/top_level.txt": name,
     record: """
         {0}/__init__.py,,
         {1}/METADATA,,
         {1}/WHEEL,,
         {1}/top_level.txt,,
         {1}/RECORD,,
        """.format(
-        name, dist_info
+        name,
+        dist_info,
     ),
 }
 
 
-def build_wheel(wheel_directory, metadata_directory=None, config_settings=None):  # noqa: U100
-    base_name = "{}-{}-py{}-none-any.whl".format(name, version, sys.version_info[0])
-    path = os.path.join(wheel_directory, base_name)
-    with ZipFile(path, "w") as zip_file_handler:
+def build_wheel(
+    wheel_directory: str,
+    metadata_directory: str | None = None,
+    config_settings: dict[str, str] | None = None,  # noqa: ARG001
+) -> str:
+    base_name = f"{name}-{version}-py{sys.version_info[0]}-none-any.whl"
+    path = Path(wheel_directory) / base_name
+    with ZipFile(str(path), "w") as zip_file_handler:
         for arc_name, data in content.items():  # pragma: no branch
             zip_file_handler.writestr(arc_name, dedent(data).strip())
         if metadata_directory is not None:
             for sub_directory, _, filenames in os.walk(metadata_directory):
                 for filename in filenames:
                     zip_file_handler.write(
-                        os.path.join(metadata_directory, sub_directory, filename),
-                        os.path.join(sub_directory, filename),
+                        str(Path(metadata_directory) / sub_directory / filename),
+                        str(Path(sub_directory) / filename),
                     )
         else:
             for arc_name, data in metadata.items():  # pragma: no branch
                 zip_file_handler.writestr(arc_name, dedent(data).strip())
-    print("created wheel {}".format(path))
+    print(f"created wheel {path}")  # noqa: T201
     return base_name
 
 
-def get_requires_for_build_wheel(config_settings=None):  # noqa: U100
+def get_requires_for_build_wheel(config_settings: dict[str, str] | None = None) -> list[str]:  # noqa: ARG001
     return []  # pragma: no cover # only executed in non-host pythons
 
 
-def build_sdist(sdist_directory, config_settings=None):  # noqa: U100
-    result = "{}-{}.tar.gz".format(name, version)
-    with tarfile.open(os.path.join(sdist_directory, result), "w:gz") as tar:
-        root = os.path.dirname(os.path.abspath(__file__))
-        tar.add(os.path.join(root, "build.py"), "build.py")
-        tar.add(os.path.join(root, "pyproject.toml"), "pyproject.toml")
+def build_sdist(sdist_directory: str, config_settings: dict[str, str] | None = None) -> str:  # noqa: ARG001
+    result = f"{name}-{version}.tar.gz"
+    with tarfile.open(str(Path(sdist_directory) / result), "w:gz") as tar:
+        root = Path(__file__).parent
+        tar.add(str(root / "build.py"), "build.py")
+        tar.add(str(root / "pyproject.toml"), "pyproject.toml")
     return result
 
 
-def get_requires_for_build_sdist(config_settings=None):  # noqa: U100
+def get_requires_for_build_sdist(config_settings: dict[str, str] | None = None) -> list[str]:  # noqa: ARG001
     return []  # pragma: no cover # only executed in non-host pythons
 
 
 if "HAS_REQUIRES_EDITABLE" in os.environ:
 
-    def get_requires_for_build_editable(config_settings=None):  # noqa: U100
-        return [1] if "REQUIRES_EDITABLE_BAD_RETURN" in os.environ else ["editables"]
+    def get_requires_for_build_editable(config_settings: dict[str, str] | None = None) -> list[str]:  # noqa: ARG001
+        return [1] if "REQUIRES_EDITABLE_BAD_RETURN" in os.environ else ["editables"]  # type: ignore[list-item]
 
 
 if "HAS_PREPARE_EDITABLE" in os.environ:
 
-    def prepare_metadata_for_build_editable(metadata_directory, config_settings=None):  # noqa: U100
-        dest = os.path.join(metadata_directory, dist_info)
-        os.mkdir(dest)
+    def prepare_metadata_for_build_editable(
+        metadata_directory: str,
+        config_settings: dict[str, str] | None = None,  # noqa: ARG001
+    ) -> str:
+        dest = Path(metadata_directory) / dist_info
+        dest.mkdir(parents=True)
         for arc_name, data in content.items():
             if arc_name.startswith(dist_info):
-                with open(os.path.join(metadata_directory, arc_name), "w") as file_handler:
-                    file_handler.write(dedent(data).strip())
-        print("created metadata {}".format(dest))
+                (dest.parent / arc_name).write_text(dedent(data).strip())
+        print(f"created metadata {dest}")  # noqa: T201
         if "PREPARE_EDITABLE_BAD" in os.environ:
-            return 1  # type: ignore # checking bad type on purpose
+            return 1  # type: ignore[return-value] # checking bad type on purpose
         return dist_info
 
 
-def build_editable(wheel_directory, metadata_directory=None, config_settings=None):
+def build_editable(
+    wheel_directory: str,
+    metadata_directory: str | None = None,
+    config_settings: dict[str, str] | None = None,
+) -> str:
     if "BUILD_EDITABLE_BAD" in os.environ:
-        return 1  # type: ignore # checking bad type on purpose
+        return 1  # type: ignore[return-value] # checking bad type on purpose
     return build_wheel(wheel_directory, metadata_directory, config_settings)
```

### Comparing `pyproject_api-1.5.1/LICENSE` & `pyproject_api-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.1/README.md` & `pyproject_api-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.1/pyproject.toml` & `pyproject_api-1.5.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.3",
-  "hatchling>=1.12.2",
+  "hatchling>=1.17.1",
 ]
 
 [project]
-name = "pyproject_api"
+name = "pyproject-api"
 description = "API to interact with the python pyproject.toml based projects"
 readme.content-type = "text/markdown"
 readme.file = "README.md"
 keywords = [
   "environments",
   "isolated",
   "testing",
@@ -24,38 +24,45 @@
   "Development Status :: 5 - Production/Stable",
   "Framework :: tox",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Testing",
   "Topic :: Utilities",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "packaging>=23",
+  "packaging>=23.1",
   'tomli>=2.0.1; python_version < "3.11"',
 ]
 optional-dependencies.docs = [
-  "furo>=2022.12.7",
-  "sphinx>=6.1.3",
-  "sphinx-autodoc-typehints!=1.23.4,>=1.22",
+  "furo>=2023.5.20",
+  "sphinx>=7.0.1",
+  "sphinx-autodoc-typehints!=1.23.4,>=1.23",
 ]
 optional-dependencies.testing = [
-  "covdefaults>=2.2.2",
-  'importlib-metadata>=6; python_version < "3.8"',
-  "pytest>=7.2.1",
-  "pytest-cov>=4",
+  "covdefaults>=2.3",
+  'importlib-metadata>=6.6; python_version < "3.8"',
+  "pytest>=7.3.1",
+  "pytest-cov>=4.1",
   "pytest-mock>=3.10",
-  "virtualenv>=20.17.1",
-  "wheel>=0.38.4",
+  "setuptools>=67.8",
+  "wheel>=0.40",
 ]
 urls.Homepage = "http://pyproject_api.readthedocs.org"
 urls.Source = "https://github.com/tox-dev/pyproject-api"
 urls.Tracker = "https://github.com/tox-dev/pyproject-api/issues"
 
 [tool.hatch]
 build.hooks.vcs.version-file = "src/pyproject_api/_version.py"
@@ -71,32 +78,41 @@
   "src",
   ".tox*/*/lib/python*/site-packages",
   ".tox*/pypy*/site-packages",
   ".tox*\\*\\Lib\\site-packages",
   "*/src",
   "*\\src",
 ]
-report.fail_under = 88
+report.fail_under = 98
 report.omit = []
 run.parallel = true
 run.plugins = ["covdefaults"]
 
-[tool.isort]
-known_first_party = ["pyproject_api"]
-profile = "black"
-line_length = 120
-
 [tool.mypy]
 python_version = "3.11"
 show_error_codes = true
 strict = true
 overrides = [{ module = ["virtualenv.*"], ignore_missing_imports = true }]
 
-[tool.pep8]
-max-line-length = "120"
-
-[tool.flake8]
-max-complexity = 22
-max-line-length = 120
-unused-arguments-ignore-abstract-functions = true
-noqa-require-code = true
-dictionaries = ["en_US", "python", "technical", "django"]
+[tool.ruff]
+select = ["ALL"]
+line-length = 120
+target-version = "py37"
+isort = {known-first-party = ["pyproject_api"], required-imports = ["from __future__ import annotations"]}
+ignore = [
+  "INP001",  # no implicit namespaces here
+  "ANN101",  # Missing type annotation for `self` in method
+  "ANN102",  # Missing type annotation for `cls` in classmethod"
+  "ANN401",  # Dynamically typed expressions
+  "D203",  # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
+  "D212",  # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
+  "S104",  # Possible binding to all interface
+]
+[tool.ruff.per-file-ignores]
+"tests/**/*.py" = [
+  "S101",  # asserts allowed in tests...
+  "FBT",  # don"t care about booleans as positional arguments in tests
+  "INP001", # no implicit namespace
+  "D",  # don"t care about documentation in tests
+  "S603",  # `subprocess` call: check for execution of untrusted input
+  "PLR2004",  # Magic value used in comparison, consider replacing with a constant variable
+]
```

### Comparing `pyproject_api-1.5.1/PKG-INFO` & `pyproject_api-1.5.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyproject_api
-Version: 1.5.1
+Name: pyproject-api
+Version: 1.5.2
 Summary: API to interact with the python pyproject.toml based projects
 Project-URL: Homepage, http://pyproject_api.readthedocs.org
 Project-URL: Source, https://github.com/tox-dev/pyproject-api
 Project-URL: Tracker, https://github.com/tox-dev/pyproject-api/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
 License-Expression: MIT
@@ -13,32 +13,39 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Requires-Dist: packaging>=23
+Requires-Dist: packaging>=23.1
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Provides-Extra: docs
-Requires-Dist: furo>=2022.12.7; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.22; extra == 'docs'
-Requires-Dist: sphinx>=6.1.3; extra == 'docs'
+Requires-Dist: furo>=2023.5.20; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23; extra == 'docs'
+Requires-Dist: sphinx>=7.0.1; extra == 'docs'
 Provides-Extra: testing
-Requires-Dist: covdefaults>=2.2.2; extra == 'testing'
-Requires-Dist: importlib-metadata>=6; python_version < '3.8' and extra == 'testing'
-Requires-Dist: pytest-cov>=4; extra == 'testing'
+Requires-Dist: covdefaults>=2.3; extra == 'testing'
+Requires-Dist: importlib-metadata>=6.6; python_version < '3.8' and extra == 'testing'
+Requires-Dist: pytest-cov>=4.1; extra == 'testing'
 Requires-Dist: pytest-mock>=3.10; extra == 'testing'
-Requires-Dist: pytest>=7.2.1; extra == 'testing'
-Requires-Dist: virtualenv>=20.17.1; extra == 'testing'
-Requires-Dist: wheel>=0.38.4; extra == 'testing'
+Requires-Dist: pytest>=7.3.1; extra == 'testing'
+Requires-Dist: setuptools>=67.8; extra == 'testing'
+Requires-Dist: wheel>=0.40; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # [`pyproject-api`](https://pyproject-api.readthedocs.io/en/latest/)
 
 [![PyPI](https://img.shields.io/pypi/v/pyproject-api?style=flat-square)](https://pypi.org/project/pyproject-api/)
 [![Supported Python
 versions](https://img.shields.io/pypi/pyversions/pyproject-api.svg)](https://pypi.org/project/pyproject-api/)
```

