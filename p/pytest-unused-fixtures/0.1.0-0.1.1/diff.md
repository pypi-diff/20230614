# Comparing `tmp/pytest_unused_fixtures-0.1.0.tar.gz` & `tmp/pytest_unused_fixtures-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_unused_fixtures-0.1.0.tar", max compression
+gzip compressed data, was "pytest_unused_fixtures-0.1.1.tar", max compression
```

## Comparing `pytest_unused_fixtures-0.1.0.tar` & `pytest_unused_fixtures-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-06-13 20:43:22.326631 pytest_unused_fixtures-0.1.0/LICENSE
--rw-r--r--   0        0        0     1491 2023-06-14 09:39:35.790833 pytest_unused_fixtures-0.1.0/README.md
--rw-r--r--   0        0        0     2707 2023-06-14 09:40:59.583655 pytest_unused_fixtures-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-13 20:50:20.566291 pytest_unused_fixtures-0.1.0/pytest_unused_fixtures/__init__.py
--rw-r--r--   0        0        0     1196 2023-06-14 15:58:39.977422 pytest_unused_fixtures-0.1.0/pytest_unused_fixtures/options.py
--rw-r--r--   0        0        0     3848 2023-06-14 15:59:06.282051 pytest_unused_fixtures-0.1.0/pytest_unused_fixtures/plugin.py
--rw-r--r--   0        0        0     1512 2023-06-14 15:58:39.858423 pytest_unused_fixtures-0.1.0/pytest_unused_fixtures/xdist.py
--rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 pytest_unused_fixtures-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-13 20:43:22.326631 pytest_unused_fixtures-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1913 2023-06-14 21:17:40.146971 pytest_unused_fixtures-0.1.1/README.md
+-rw-r--r--   0        0        0     2702 2023-06-14 16:34:11.273375 pytest_unused_fixtures-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-06-14 21:25:33.867966 pytest_unused_fixtures-0.1.1/pytest_unused_fixtures/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-14 21:25:32.009991 pytest_unused_fixtures-0.1.1/pytest_unused_fixtures/decorators.py
+-rw-r--r--   0        0        0     1196 2023-06-14 15:58:39.977422 pytest_unused_fixtures-0.1.1/pytest_unused_fixtures/options.py
+-rw-r--r--   0        0        0     4396 2023-06-14 21:15:26.218962 pytest_unused_fixtures-0.1.1/pytest_unused_fixtures/plugin.py
+-rw-r--r--   0        0        0     1512 2023-06-14 15:58:39.858423 pytest_unused_fixtures-0.1.1/pytest_unused_fixtures/xdist.py
+-rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 pytest_unused_fixtures-0.1.1/PKG-INFO
```

### Comparing `pytest_unused_fixtures-0.1.0/LICENSE` & `pytest_unused_fixtures-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.0/README.md` & `pytest_unused_fixtures-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,28 @@
 
 ## Usage
 
 After installing the package, the plugin is enabled by adding the switch `--unused-fixtures`.
 
 Paths of fixtures can be ignored with one or multiple `--unused-fixtures-ignore-path` arguments. For example `--unused-fixtures-ignore-path=venv` will ignore all fixtures defined in the `venv` folder.
 
+### Ignoring specific fixtures from report
+
+Sometimes there will be fixture which are unused on purpose, for example when used in tests which are skipped by default. A decorator is provided for ignoring fixtures from the unused report. See the example for usage:
+
+```python
+import pytest
+from pytest_unused_fixtures import ignore_unused_fixture
+
+@pytest.fixture
+@ignore_unused_fixture
+def ignored_fixture():
+    pass
+```
+
 ## Development
 
 [Poetry](https://python-poetry.org/) (dependencies) and [pre-commit](https://pre-commit.com/) (coding standards) are required for development. Ther are some tests, obviously written in [pytest](https://pytest.org/).
 
 ```shell
 $ poetry install
 $ pre-commit install
```

### Comparing `pytest_unused_fixtures-0.1.0/pyproject.toml` & `pytest_unused_fixtures-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pytest-unused-fixtures"
-version = "0.1.0"
+version = "0.1.1"
 description = "A pytest plugin to list unused fixtures after a test run."
 authors = ["Mikuláš Poul <mikulaspoul@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_unused_fixtures"}]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Testing",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `pytest_unused_fixtures-0.1.0/pytest_unused_fixtures/options.py` & `pytest_unused_fixtures-0.1.1/pytest_unused_fixtures/options.py`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.0/pytest_unused_fixtures/plugin.py` & `pytest_unused_fixtures-0.1.1/pytest_unused_fixtures/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,100 @@
 import dataclasses
 import itertools
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, NoReturn
 
 import pytest
-from _pytest.python import _pretty_fixture_path
+from _pytest.compat import getlocation
+from _pytest.pathlib import bestrelpath
+from _pytest.python import _PYTEST_DIR
 
 if TYPE_CHECKING:
     from _pytest.config import Config, ExitCode
     from _pytest.fixtures import FixtureDef, SubRequest
     from _pytest.main import Session
     from _pytest.terminal import TerminalReporter
 
 
 @dataclasses.dataclass(frozen=True, eq=True)
 class FixtureInfo:
     module: str
-    fixture_path: str
     argname: str
     scope: str
+    location: str
 
     def __lt__(self, other):
-        return (self.module, self.fixture_path, self.argname) < (other.module, other.fixture_path, other.argname)
+        return (self.module, self.location, self.argname) < (other.module, other.location, other.argname)
+
+    @property
+    def pretty_path(self):
+        cwd = Path.cwd()
+        loc = Path(self.location)
+        prefix = Path("...", "_pytest")
+        try:
+            return str(prefix / loc.relative_to(_PYTEST_DIR))
+        except ValueError:
+            return bestrelpath(cwd, loc)
 
 
 class PytestUnusedFixturesPlugin:
     def __init__(self, ignore_paths=None):
         self.ignore_paths: list[str] | None = ignore_paths
         self.used_fixtures: set[FixtureInfo] = set()
         self.available_fixtures: None | set[FixtureInfo] = None
+        self.curdir = Path().cwd()
 
     def get_fixture_info(self, fixturedef: "FixtureDef") -> FixtureInfo:
         return FixtureInfo(
             module=fixturedef.func.__module__,
-            fixture_path=_pretty_fixture_path(fixturedef.func),
             argname=fixturedef.argname,
             scope=fixturedef.scope,
+            location=getlocation(fixturedef.func, self.curdir),
         )
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_fixture_setup(self, fixturedef: "FixtureDef", request: "SubRequest") -> Any | None:
         self.used_fixtures.add(self.get_fixture_info(fixturedef))
 
         yield
 
     def pytest_collection_finish(self, session: "Session") -> None:
         self.available_fixtures = {
-            self.get_fixture_info(x) for x in itertools.chain(*session._fixturemanager._arg2fixturedefs.values())
+            self.get_fixture_info(x)
+            for x in itertools.chain(*session._fixturemanager._arg2fixturedefs.values())
+            # if fixture is not in available fixtures, it won't be marked as unused
+            if not hasattr(x.func, "ignore_unused_fixture")
         }
 
     def _write_fixtures(self, config: "Config", terminalreporter: "TerminalReporter", fixtures: set[FixtureInfo]):
         verbose = config.getvalue("verbose")
         tw = terminalreporter
 
         available: list[FixtureInfo] = []
         seen: set[tuple[str, str]] = set()
 
         fixture: FixtureInfo
         for fixture in fixtures:
-            if (fixture.argname, fixture.fixture_path) in seen:
+            if (fixture.argname, fixture.location) in seen:
                 continue
-            seen.add((fixture.argname, fixture.fixture_path))
+            seen.add((fixture.argname, fixture.location))
             available.append(fixture)
 
         available.sort()
         current_module = None
         for fixture in available:
             if current_module != fixture.module and not fixture.module.startswith("_pytest."):
                 tw.write_sep("-", f"fixtures defined from {fixture.module}")
                 current_module = fixture.module
             if verbose <= 0 and fixture.argname.startswith("_"):
                 continue
             tw.write(f"{fixture.argname}", green=True)
             if fixture.scope != "function":
                 tw.write(" [%s scope]" % fixture.scope, cyan=True)
-            tw.write(f" -- {fixture.fixture_path}", yellow=True)
+            tw.write(f" -- {fixture.pretty_path}", yellow=True)
             tw.write("\n")
 
     def pytest_terminal_summary(
         self,
         terminalreporter: "TerminalReporter",
         exitstatus: "ExitCode",
         config: "Config",
@@ -88,15 +105,15 @@
         # do a simple set operation to get the unused fixtures
         unused_fixtures = self.available_fixtures - self.used_fixtures
 
         # ignore unused fixtures from ignored paths
         fixture: FixtureInfo
         non_ignored_unused_fixtures = []
         for fixture in unused_fixtures:
-            if any(fixture.fixture_path.startswith(x) for x in (self.ignore_paths or [])):
+            if any(fixture.pretty_path.startswith(x) for x in (self.ignore_paths or [])):
                 continue
             non_ignored_unused_fixtures.append(fixture)
         unused_fixtures = non_ignored_unused_fixtures
 
         # print fixtures
         if unused_fixtures:
             terminalreporter.write_sep(sep="=", title="UNUSED FIXTURES", fullwidth=fullwidth)
```

### Comparing `pytest_unused_fixtures-0.1.0/pytest_unused_fixtures/xdist.py` & `pytest_unused_fixtures-0.1.1/pytest_unused_fixtures/xdist.py`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.0/PKG-INFO` & `pytest_unused_fixtures-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytest-unused-fixtures
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pytest plugin to list unused fixtures after a test run.
 License: MIT
 Author: Mikuláš Poul
 Author-email: mikulaspoul@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,14 +35,28 @@
 
 ## Usage
 
 After installing the package, the plugin is enabled by adding the switch `--unused-fixtures`.
 
 Paths of fixtures can be ignored with one or multiple `--unused-fixtures-ignore-path` arguments. For example `--unused-fixtures-ignore-path=venv` will ignore all fixtures defined in the `venv` folder.
 
+### Ignoring specific fixtures from report
+
+Sometimes there will be fixture which are unused on purpose, for example when used in tests which are skipped by default. A decorator is provided for ignoring fixtures from the unused report. See the example for usage:
+
+```python
+import pytest
+from pytest_unused_fixtures import ignore_unused_fixture
+
+@pytest.fixture
+@ignore_unused_fixture
+def ignored_fixture():
+    pass
+```
+
 ## Development
 
 [Poetry](https://python-poetry.org/) (dependencies) and [pre-commit](https://pre-commit.com/) (coding standards) are required for development. Ther are some tests, obviously written in [pytest](https://pytest.org/).
 
 ```shell
 $ poetry install
 $ pre-commit install
```

