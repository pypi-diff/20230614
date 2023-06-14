# Comparing `tmp/robotcode_runner-0.41.0.tar.gz` & `tmp/robotcode_runner-0.43.0.tar.gz`

## Comparing `robotcode_runner-0.41.0.tar` & `robotcode_runner-0.43.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    20419 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    23700 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.43.0/PKG-INFO
```

### Comparing `robotcode_runner-0.41.0/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.43.0/src/robotcode/runner/cli/libdoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     },
     add_help_option=True,
     epilog='Use "-- --help" to see the `libdoc` help.',
 )
 @click.version_option(
     version=__version__,
     package_name="robotcode.runner.libdoc",
-    prog_name="RobotCode LibDoc",
+    prog_name="RobotCode libdoc",
     message=f"%(prog)s %(version)s\n{USAGE.splitlines()[0].split(' -- ')[0].strip()} {get_full_version()}",
 )
 @click.argument("robot_options_and_args", nargs=-1, type=click.Path())
 @pass_application
 def libdoc(
     app: Application,
     robot_options_and_args: Tuple[str, ...],
```

### Comparing `robotcode_runner-0.41.0/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.43.0/src/robotcode/runner/cli/rebot.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `rebot` help.',
 )
 @click.version_option(
     version=__version__,
-    package_name="robotcode.runner.libdoc",
-    prog_name="RobotCode LibDoc",
+    package_name="robotcode.runner.rebot",
+    prog_name="RobotCode rebot",
     message=f"%(prog)s %(version)s\n{USAGE.splitlines()[0].split(' -- ')[0].strip()} {get_full_version()}",
 )
 @click.argument("robot_options_and_args", nargs=-1, type=click.Path())
 @pass_application
 def rebot(
     app: Application,
     robot_options_and_args: Tuple[str, ...],
```

### Comparing `robotcode_runner-0.41.0/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.43.0/src/robotcode/runner/cli/robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,16 @@
     robot_options_and_args: Tuple[str, ...],
 ) -> None:
     """Runs `robot` with the selected configuration, profiles, options and arguments.
 
     The options and arguments are passed to `robot` as is.
 
     Examples:
+
+    \b
     ```
     robotcode run
     ```
     """
 
     root_folder, profile, cmd_options = handle_robot_options(
         app, by_longname, exclude_by_longname, robot_options_and_args
```

### Comparing `robotcode_runner-0.41.0/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.43.0/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.41.0/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.43.0/src/robotcode/runner/cli/discover/discover.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import platform
 import re
 import sys
 from collections import defaultdict
 from dataclasses import dataclass
 from io import IOBase
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
@@ -40,16 +41,16 @@
 
 def _patch() -> None:
     global __patched
     if __patched:
         return
     __patched = True
 
-    if get_robot_version() <= (6, 1, 0, "a", 1, None):
-        if get_robot_version() > (5, 0) and get_robot_version() < (6, 0, 0) or get_robot_version() < (5, 0):
+    if get_robot_version() <= (6, 1):
+        if get_robot_version() > (5, 0) and get_robot_version() < (6, 0) or get_robot_version() < (5, 0):
             from robot.running.builder.testsettings import TestDefaults  # pyright: ignore[reportMissingImports]
         else:
             from robot.running.builder.settings import Defaults as TestDefaults  # pyright: ignore[reportMissingImports]
 
         old_validate_test_counts = TestSuiteBuilder._validate_test_counts
 
         def _validate_test_counts(self: Any, suite: TestSuite, multisource: bool = False) -> None:
@@ -65,28 +66,38 @@
 
         def build_suite(self: SuiteStructureParser, structure: Any) -> Tuple[TestSuite, TestDefaults]:
             try:
                 return old_build_suite_file(self, structure)  # type: ignore
             except DataError as e:
                 LOGGER.error(str(e))
                 parent_defaults = self._stack[-1][-1] if self._stack else None
-                if get_robot_version() < (6, 1, 0, "a", 1, None):
+                if get_robot_version() < (6, 1):
                     from robot.running.builder.parsers import format_name
 
                     return ErroneousTestSuite(
                         error_message=str(e), name=format_name(structure.source), source=structure.source
                     ), TestDefaults(parent_defaults)
 
                 return ErroneousTestSuite(
                     error_message=str(e), name=TestSuite.name_from_source(structure.source), source=structure.source
                 ), TestDefaults(parent_defaults)
 
         SuiteStructureParser._build_suite = build_suite
 
-    elif get_robot_version() >= (6, 1, 0, "a", 1, None):
+        old_validate_execution_mode = SuiteStructureParser._validate_execution_mode
+
+        def _validate_execution_mode(self: SuiteStructureParser, suite: TestSuite) -> None:
+            try:
+                old_validate_execution_mode(self, suite)
+            except DataError as e:
+                LOGGER.error(f"Parsing '{suite.source}' failed: {e.message}")
+
+        SuiteStructureParser._validate_execution_mode = _validate_execution_mode
+
+    elif get_robot_version() >= (6, 1):
         from robot.parsing.suitestructure import SuiteDirectory, SuiteFile
         from robot.running.builder.settings import TestDefaults  # pyright: ignore[reportMissingImports]
 
         old_validate_not_empty = TestSuiteBuilder._validate_not_empty
 
         def _validate_not_empty(self: Any, suite: TestSuite, multi_source: bool = False) -> None:
             try:
@@ -120,14 +131,24 @@
                 LOGGER.error(str(e))
                 return ErroneousTestSuite(
                     error_message=str(e), name=TestSuite.name_from_source(structure.source), source=structure.source
                 ), TestDefaults(self.parent_defaults)
 
         SuiteStructureParser._build_suite_directory = build_suite_directory
 
+        old_validate_execution_mode = SuiteStructureParser._validate_execution_mode
+
+        def _validate_execution_mode(self: SuiteStructureParser, suite: TestSuite) -> None:
+            try:
+                old_validate_execution_mode(self, suite)
+            except DataError as e:
+                LOGGER.error(f"Parsing '{suite.source}' failed: {e.message}")
+
+        SuiteStructureParser._validate_execution_mode = _validate_execution_mode
+
     old_get_file = FileReader._get_file
 
     def get_file(self: FileReader, source: Union[str, Path, IOBase], accept_text: bool) -> Any:
         path = self._get_path(source, accept_text)
         if path:
             if _stdin_data is not None and (data := _stdin_data.get(str(path))) is not None:
                 if data is not None:
@@ -141,14 +162,16 @@
 @dataclass
 class TestItem:
     type: str
     id: str
     name: str
     longname: str
     uri: Optional[DocumentUri] = None
+    rel_source: Optional[str] = None
+    needs_parse_include: bool = False
     children: Optional[List["TestItem"]] = None
     description: Optional[str] = None
     range: Optional[Range] = None
     tags: Optional[List[str]] = None
     error: Optional[str] = None
 
 
@@ -161,46 +184,60 @@
 @dataclass
 class Statistics:
     suites: int = 0
     suites_with_tests: int = 0
     tests: int = 0
 
 
+def get_rel_source(source: Optional[str]) -> Optional[str]:
+    if source is None:
+        return None
+    try:
+        return str(Path(source).relative_to(Path.cwd()).as_posix())
+    except ValueError:
+        return str(source)
+
+
 class Collector(SuiteVisitor):
     def __init__(self) -> None:
         super().__init__()
         self.all: TestItem = TestItem(
             type="workspace",
             id=str(Path.cwd().resolve()),
             name=Path.cwd().name,
             longname=Path.cwd().name,
             uri=str(Uri.from_path(Path.cwd())),
+            needs_parse_include=get_robot_version() >= (6, 1),
         )
         self._current = self.all
         self.suites: List[TestItem] = []
         self.tests: List[TestItem] = []
         self.tags: Dict[str, List[TestItem]] = defaultdict(list)
         self.statistics = Statistics()
 
     def visit_suite(self, suite: TestSuite) -> None:
-        item = TestItem(
-            type="suite",
-            id=f"{Path(suite.source).resolve() if suite.source is not None else ''};{suite.longname}",
-            name=suite.name,
-            longname=suite.longname,
-            uri=str(Uri.from_path(suite.source)) if suite.source else None,
-            range=Range(
-                start=Position(line=0, character=0),
-                end=Position(line=0, character=0),
+        try:
+            item = TestItem(
+                type="suite",
+                id=f"{Path(suite.source).resolve() if suite.source is not None else ''};{suite.longname}",
+                name=suite.name,
+                longname=suite.longname,
+                uri=str(Uri.from_path(Path(suite.source).resolve())) if suite.source else None,
+                rel_source=get_rel_source(suite.source),
+                range=Range(
+                    start=Position(line=0, character=0),
+                    end=Position(line=0, character=0),
+                )
+                if suite.source and Path(suite.source).is_file()
+                else None,
+                children=[],
+                error=suite.error_message if isinstance(suite, ErroneousTestSuite) else None,
             )
-            if suite.source and Path(suite.source).is_file()
-            else None,
-            children=[],
-            error=suite.error_message if isinstance(suite, ErroneousTestSuite) else None,
-        )
+        except ValueError as e:
+            raise ValueError(f"Error while parsing suite {suite.source}: {e}") from e
 
         self.suites.append(item)
 
         if self._current.children is None:
             self._current.children = []
         self._current.children.append(item)
 
@@ -214,26 +251,31 @@
         self.statistics.suites += 1
         if suite.tests:
             self.statistics.suites_with_tests += 1
 
     def visit_test(self, test: TestCase) -> None:
         if self._current.children is None:
             self._current.children = []
-        item = TestItem(
-            type="test",
-            id=f"{Path(test.source).resolve() if test.source is not None else ''};{test.longname};{test.lineno}",
-            name=test.name,
-            longname=test.longname,
-            uri=str(Uri.from_path(test.source)) if test.source else None,
-            range=Range(
-                start=Position(line=test.lineno - 1, character=0),
-                end=Position(line=test.lineno - 1, character=0),
-            ),
-            tags=list(test.tags) if test.tags else None,
-        )
+        try:
+            item = TestItem(
+                type="test",
+                id=f"{Path(test.source).resolve() if test.source is not None else ''};{test.longname};{test.lineno}",
+                name=test.name,
+                longname=test.longname,
+                uri=str(Uri.from_path(Path(test.source).resolve())) if test.source else None,
+                rel_source=get_rel_source(test.source),
+                range=Range(
+                    start=Position(line=test.lineno - 1, character=0),
+                    end=Position(line=test.lineno - 1, character=0),
+                ),
+                tags=list(test.tags) if test.tags else None,
+            )
+        except ValueError as e:
+            raise ValueError(f"Error while parsing suite {test.source}: {e}") from e
+
         for tag in test.tags:
             self.tags[str(tag)].append(item)
 
         self.tests.append(item)
         self._current.children.append(item)
 
         self.statistics.tests += 1
@@ -276,15 +318,15 @@
 
 def build_diagnostics(messages: List[Message]) -> Dict[str, List[Diagnostic]]:
     result: Dict[str, List[Diagnostic]] = {}
 
     def add_diagnostic(
         message: Message, source_uri: Optional[str] = None, line: Optional[int] = None, text: Optional[str] = None
     ) -> None:
-        source_uri = str(Uri.from_path(Path(source_uri).absolute() if source_uri else Path.cwd()))
+        source_uri = str(Uri.from_path(Path(source_uri).resolve() if source_uri else Path.cwd()))
 
         if source_uri not in result:
             result[source_uri] = []
 
         result[source_uri].append(
             Diagnostic(
                 range=Range(
@@ -340,24 +382,24 @@
         diagnostics_logger = DiagnosticsLogger()
         LOGGER.register_logger(diagnostics_logger)
 
         if get_robot_version() >= (5, 0):
             if settings.pythonpath:
                 sys.path = settings.pythonpath + sys.path
 
-        if get_robot_version() > (6, 1, 0, "a", 1, None):
+        if get_robot_version() > (6, 1):
             builder = TestSuiteBuilder(
-                settings["SuiteNames"],
-                custom_parsers=settings.parsers,
                 included_extensions=settings.extension,
+                included_files=settings.parse_include,
+                custom_parsers=settings.parsers,
                 rpa=settings.rpa,
                 lang=settings.languages,
                 allow_empty_suite=settings.run_empty_suite,
             )
-        elif get_robot_version() >= (6, 0, 0):
+        elif get_robot_version() >= (6, 0):
             builder = TestSuiteBuilder(
                 settings["SuiteNames"],
                 included_extensions=settings.extension,
                 rpa=settings.rpa,
                 lang=settings.languages,
                 allow_empty_suite=settings.run_empty_suite,
             )
@@ -572,31 +614,104 @@
     robotcode discover tags
     robotcode --profile regression discover tags
 
     robotcode --profile regression discover tags -i wip
     ```
     """
 
-    suite, diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
+    suite, _diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
 
     collector = Collector()
     suite.visit(collector)
 
     if collector.all.children:
         if app.config.output_format is None or app.config.output_format == OutputFormat.TEXT:
 
             def print(tags: Dict[str, List[TestItem]]) -> Iterable[str]:
                 for tag, items in tags.items():
                     yield f"{tag}{os.linesep}"
-                    # for item in items:
-                    #     yield f"  {item.longname}{os.linesep}"
-                    #     if item.uri:
-                    #         yield (
-                    #             f" ({Uri(item.uri).to_path()}{f':{item.range.start.line+1}' if item.range else ''})"
-                    #             f"{os.linesep}"
-                    #         )
 
             if collector.suites:
                 app.echo_via_pager(print(collector.tags))
 
         else:
             app.print_data(TagsResult(collector.tags), remove_defaults=True)
+
+
+@dataclass
+class RobotVersion:
+    major: int
+    minor: int
+    patch: Optional[int] = None
+    pre_id: Optional[str] = None
+    pre_number: Optional[int] = None
+    dev: Optional[int] = None
+
+
+@dataclass
+class PythonVersion:
+    major: int
+    minor: int
+    micro: int
+    releaselevel: str
+    serial: int
+
+
+@dataclass
+class Info:
+    robot_version: RobotVersion
+    robot_version_string: str
+    robot_env: Dict[str, str]
+    python_version: PythonVersion
+    python_version_string: str
+    machine: str
+    processor: str
+    platform: str
+    system: str
+    system_version: str
+
+
+@discover.command(
+    add_help_option=True,
+)
+@pass_application
+def info(
+    app: Application,
+) -> None:
+    """\
+    Shows some informations about the current *robot* environment.
+
+    \b
+    Examples:
+    ```
+    robotcode discover info
+    ```
+    """
+    from robot.version import get_version as get_version
+
+    robot_env: Dict[str, str] = {}
+    if "ROBOT_OPTIONS" in os.environ:
+        robot_env["ROBOT_OPTIONS"] = os.environ["ROBOT_OPTIONS"]
+    if "ROBOT_SYSLOG_FILE" in os.environ:
+        robot_env["ROBOT_SYSLOG_FILE"] = os.environ["ROBOT_SYSLOG_FILE"]
+    if "ROBOT_SYSLOG_LEVEL" in os.environ:
+        robot_env["ROBOT_SYSLOG_LEVEL"] = os.environ["ROBOT_SYSLOG_LEVEL"]
+    if "ROBOT_INTERNAL_TRACES" in os.environ:
+        robot_env["ROBOT_INTERNAL_TRACES"] = os.environ["ROBOT_INTERNAL_TRACES"]
+
+    info = Info(
+        RobotVersion(*get_robot_version()),
+        get_version(),
+        robot_env,
+        PythonVersion(*sys.version_info),
+        platform.python_version(),
+        platform.machine(),
+        platform.processor(),
+        sys.platform,
+        platform.system(),
+        platform.version(),
+    )
+
+    if app.config.output_format is None or app.config.output_format == OutputFormat.TEXT:
+        app.print_data(info, remove_defaults=True)
+    else:
+        app.print_data(info, remove_defaults=True)
```

### Comparing `robotcode_runner-0.41.0/.gitignore` & `robotcode_runner-0.43.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.41.0/LICENSE.txt` & `robotcode_runner-0.43.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.41.0/README.md` & `robotcode_runner-0.43.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.41.0/pyproject.toml` & `robotcode_runner-0.43.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.41.0",
-  "robotcode-modifiers==0.41.0",
-  "robotcode==0.41.0",
+  "robotcode-robot==0.43.0",
+  "robotcode-modifiers==0.43.0",
+  "robotcode==0.43.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.41.0/PKG-INFO` & `robotcode_runner-0.43.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.41.0
+Version: 0.43.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.41.0
-Requires-Dist: robotcode-robot==0.41.0
-Requires-Dist: robotcode==0.41.0
+Requires-Dist: robotcode-modifiers==0.43.0
+Requires-Dist: robotcode-robot==0.43.0
+Requires-Dist: robotcode==0.43.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

