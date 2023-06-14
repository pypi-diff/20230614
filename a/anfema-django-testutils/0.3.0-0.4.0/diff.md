# Comparing `tmp/anfema-django-testutils-0.3.0.tar.gz` & `tmp/anfema_django_testutils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anfema-django-testutils-0.3.0.tar", last modified: Fri Mar  3 16:06:07 2023, max compression
+gzip compressed data, was "anfema_django_testutils-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `anfema-django-testutils-0.3.0.tar` & `anfema_django_testutils-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1912 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/.github/workflows/publish_release_packages.yaml
--rw-r--r--   0        0        0       41 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/.gitignore
--rw-r--r--   0        0        0     1067 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/LICENSE
--rw-r--r--   0        0        0     1492 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/README.md
--rw-r--r--   0        0        0      336 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/anfema_django_testutils/__init__.py
--rw-r--r--   0        0        0      317 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/anfema_django_testutils/apps.py
--rw-r--r--   0        0        0    13489 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/anfema_django_testutils/runner.py
--rw-r--r--   0        0        0      918 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/anfema_django_testutils/settings.py
--rw-r--r--   0        0        0     2335 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/anfema_django_testutils/static/css/test-results.css
--rw-r--r--   0        0        0     1636 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/anfema_django_testutils/tags.py
--rw-r--r--   0        0        0    10105 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/anfema_django_testutils/templates/test-results-template.html
--rw-r--r--   0        0        0     4965 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/anfema_django_testutils/testcases.py
--rw-r--r--   0        0        0      638 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/docs/Makefile
--rw-r--r--   0        0        0      769 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/docs/make.bat
--rw-r--r--   0        0        0      569 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/docs/source/api.rst
--rw-r--r--   0        0        0     1791 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/docs/source/conf.py
--rw-r--r--   0        0        0     2539 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/docs/source/configuration.rst
--rw-r--r--   0        0        0       93 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/docs/source/index.rst
--rw-r--r--   0        0        0       46 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/docs/source/license.rst
--rw-r--r--   0        0        0     1259 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       38 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/setup.py
--rw-r--r--   0        0        0      189 2023-03-03 16:06:00.805978 anfema-django-testutils-0.3.0/tox.ini
--rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 anfema-django-testutils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1912 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/.github/workflows/publish_release_packages.yaml
+-rw-r--r--   0        0        0       41 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1067 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1492 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/README.md
+-rw-r--r--   0        0        0      336 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/__init__.py
+-rw-r--r--   0        0        0      317 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/apps.py
+-rw-r--r--   0        0        0    16161 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/runner.py
+-rw-r--r--   0        0        0      959 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/settings.py
+-rw-r--r--   0        0        0     2335 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/static/css/test-results.css
+-rw-r--r--   0        0        0     1636 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/tags.py
+-rw-r--r--   0        0        0    10501 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/templates/test-results-template.html
+-rw-r--r--   0        0        0     4977 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/testcases.py
+-rw-r--r--   0        0        0      638 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/docs/Makefile
+-rw-r--r--   0        0        0      769 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/docs/make.bat
+-rw-r--r--   0        0        0      569 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/docs/source/api.rst
+-rw-r--r--   0        0        0     1791 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0     2829 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/docs/source/configuration.rst
+-rw-r--r--   0        0        0       93 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0       46 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/docs/source/license.rst
+-rw-r--r--   0        0        0     1259 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/setup.py
+-rw-r--r--   0        0        0      189 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/tox.ini
+-rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 anfema_django_testutils-0.4.0/PKG-INFO
```

### Comparing `anfema-django-testutils-0.3.0/.github/workflows/publish_release_packages.yaml` & `anfema_django_testutils-0.4.0/.github/workflows/publish_release_packages.yaml`

 * *Files identical despite different names*

### Comparing `anfema-django-testutils-0.3.0/LICENSE` & `anfema_django_testutils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anfema-django-testutils-0.3.0/README.md` & `anfema_django_testutils-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `anfema-django-testutils-0.3.0/anfema_django_testutils/runner.py` & `anfema_django_testutils-0.4.0/anfema_django_testutils/runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """This module provides a TestRunner."""
 from __future__ import annotations
 
 
 __all__ = ('TestRunner',)
 
+
 import argparse
 import contextlib
 import datetime
 import itertools
 import pathlib
 import re
 import sys
+import textwrap
 import unittest.runner
 from collections import defaultdict, namedtuple
 from contextlib import nullcontext
 from operator import attrgetter
 from typing import TYPE_CHECKING
 from unittest.result import TestResult
 from unittest.runner import TextTestRunner
@@ -34,14 +36,15 @@
 
 # isort: off
 if TYPE_CHECKING:
     import types
     import unittest
     from typing import Any, Dict, Tuple, Type, Union
 
+    _SubTest = unittest.case._SubTest
     _SysExcInfoType = Union[
         Tuple[Type[BaseException], BaseException, types.TracebackType],
         Tuple[None, None, None],
     ]
 # isort: on
 
 
@@ -91,25 +94,26 @@
         'passed',
         'expected_failure',
         'unexpected_success',
         'precondition_failure',
     )
 
     TestResultData = namedtuple('TestResultData', field_names=('name', 'result', 'duration', 'outcome'))
+    _subtest_result_map: defaultdict[unittest.case.TestCase, list[tuple[_SubTest, str, _SysExcInfoType]]]
 
     def __init__(self, *args, tests=None, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.dots = False
         self.showAll = False
         self.passed = []
         self.precondition_failures = []
         self.timestamp_start_testrun = None
         self.timestamp_stop_testrun = None
-
         self._test_result_data = defaultdict(list)
+        self._subtest_result_map = defaultdict(list)
         self._all_tests = tests
 
     def _add_test_result_data(self, test, result, outcome=None) -> None:
         if isinstance(test, _ErrorHolder):
             # In case an _ErrorHolder instance has been passed, which means setting up the testcase has been failed,
             # none of the testcase`s test methods have been executed, and thus they will all be set to the same result.
             parent = re.search('\((.+)\)', test.description).group(1)
@@ -131,14 +135,15 @@
         if self.options.get('html_results_enabled'):
             # Create report directory
             report_dir = pathlib.Path(self.options.get('report_dir'))
             report_dir.mkdir(exist_ok=True)
 
             # Create html test report
             html_template = get_config()['TEST_REPORT_HTML_TEMPLATE']
+            result_data['title'] = self.options.get('report_title')
             html_data = render_to_string(html_template, context=result_data)
             results_html_file = report_dir / 'test-results.html'
             results_html_file.write_text(html_data)
 
             # Copy css file into the report directory
             with contextlib.suppress(TypeError):
                 css_file = pathlib.Path(get_config()['TEST_REPORT_CSS'] or None)
@@ -206,14 +211,17 @@
         super().stopTestRun()
         self.timestamp_stop_testrun = timezone.now()
 
     def stopTest(self, test: unittest.case.TestCase) -> None:
         """Called when the given test has been run"""
         super().stopTest(test)
         test.stop_time = timezone.now()
+        if subtests_results := self._subtest_result_map.pop(test, None):
+            result, outcome = self._resolve_subtests_results(test, subtests_results)
+            self._add_test_result_data(test, result, outcome)
 
     def addSkip(self, test: unittest.case.TestCase, reason: str) -> None:
         """Called when a test is skipped."""
         super().addSkip(test, reason)
         self._add_test_result_data(test, 'skipped', reason)
 
     def addSuccess(self, test: unittest.case.TestCase) -> None:
@@ -249,14 +257,21 @@
 
     def addPreconditionFailure(self, test: unittest.case.TestCase, err: _SysExcInfoType) -> None:
         """Called when a precondition error has occurred."""
         self.precondition_failures.append((test, self._exc_info_to_string(err, test)))
         self._mirrorOutput = True
         self._add_test_result_data(test, 'precondition_failure', self._exc_info_to_string(err, test))
 
+    def addSubTest(self, test: unittest.case.TestCase, subtest, err: _SysExcInfoType) -> None:
+        """Called at the end of a subtest."""
+        if err is not None:
+            self._apply_subtest_result(test, subtest, err)
+            if getattr(self, 'failfast', False):
+                self.stop()
+
     def wasSuccessful(self) -> bool:
         """Tells whether or not this result was a success."""
         return len(self.precondition_failures) == 0 and super().wasSuccessful()
 
     def print_test_result(self, test: unittest.case.TestCase, result: str) -> None:
         result_width = max(map(len, self.supported_results)) + 10
         # ToDo: use stream instead of print
@@ -275,14 +290,48 @@
         print()
         print(
             f'{"OK" if self.wasSuccessful() else "FAILED"} (skipped={skipped}, passed={passed}, '
             f'expected failures={expected_failures}, precondition failures={precondition_failures}, '
             f'failures={failures}, unexpected successes={unexpected_successes}, errors={errors})'
         )
 
+    def _resolve_subtests_results(
+        self, test: unittest.case.TestCase, results: list[tuple[_SubTest, str, _SysExcInfoType]]
+    ) -> tuple[str, str]:
+        result_priority_map = {'error': 1, 'failure': 2, 'precondition_failure': 3}
+        reverse_result_priority_map = {v: k for k, v in result_priority_map.items()}
+        outcome = ''
+        result_priority = max(reverse_result_priority_map) + 1
+        for subtest, result, err in results:
+            assert result in result_priority_map, f'Invalid subtest result: {result!r}'
+            header = f'{result.upper()}: {subtest.id()}'
+            outcome += (
+                textwrap.dedent(
+                    f"""\
+            {len(header)*"="}
+            {header}
+            {len(header)*"-"}
+            """
+                )
+                + self._exc_info_to_string(err, test)
+                + 2 * '\n'
+            )
+            result_priority = min(result_priority_map[result], result_priority)
+        result = reverse_result_priority_map[result_priority]
+        return result, outcome.strip()
+
+    def _apply_subtest_result(self, test: unittest.case.TestCase, subtest: _SubTest, err: _SysExcInfoType) -> None:
+        if getattr(err[1], '__precondition_failure__', None):
+            result = 'precondition_failure'
+        elif issubclass(err[0], test.failureException):
+            result = 'failure'
+        else:
+            result = 'error'
+        self._subtest_result_map[test].append((subtest, result, err))
+
 
 class HtmlTestRunner(TextTestRunner):
     resultclass = HtmlTestResult
 
     def run(self, test: unittest.suite.TestSuite) -> HtmlTestResult:
         # ToDo: Consider to override the run() method to keep 'test'
         self._tests = list(test)
@@ -321,10 +370,20 @@
             dest="report_dir",
             metavar="DIR",
             default=get_config()["TEST_REPORT_DIR"],
             help="Defines the directory where to store the report artifacts. "
             "If this isn't provided, the TEST_REPORT_DIR setting will be used.",
         )
 
+        parser.add_argument(
+            "--report-title",
+            action="store",
+            dest="report_title",
+            metavar="TITLE",
+            default=get_config()["TEST_REPORT_TITLE"],
+            help="A string which defines the test-report`s title."
+            "If this isn't provided, the TEST_REPORT_TITLE setting will be used.",
+        )
+
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.test_runner.resultclass.options = kwargs
```

### Comparing `anfema-django-testutils-0.3.0/anfema_django_testutils/settings.py` & `anfema_django_testutils-0.4.0/anfema_django_testutils/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 CONFIG_DEFAULTS = {
     "TEST_REPORT_DIR": "test-report",
     "TEST_REPORT_HTML_TEMPLATE": "test-results-template.html",
     "TEST_REPORT_CSS": "test-results.css",
     "COVERAGE_REPORT_ENABLED": True,
     "HTML_RESULTS_ENABLED": True,
+    "TEST_REPORT_TITLE": "Test Results",
 }
 
 
 @lru_cache()
 def get_config() -> Dict[str, Any]:
     """Returns the current configuration"""
     return {conf: getattr(settings, conf, default) for conf, default in CONFIG_DEFAULTS.items()}
```

### Comparing `anfema-django-testutils-0.3.0/anfema_django_testutils/static/css/test-results.css` & `anfema_django_testutils-0.4.0/anfema_django_testutils/static/css/test-results.css`

 * *Files identical despite different names*

### Comparing `anfema-django-testutils-0.3.0/anfema_django_testutils/tags.py` & `anfema_django_testutils-0.4.0/anfema_django_testutils/tags.py`

 * *Files identical despite different names*

### Comparing `anfema-django-testutils-0.3.0/anfema_django_testutils/templates/test-results-template.html` & `anfema_django_testutils-0.4.0/anfema_django_testutils/templates/test-results-template.html`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         <title>Test-Report</title>
         <meta charset="UTF-8">
         <link rel="stylesheet" href="test-results.css" type="text/css" />
     </head>
     <body>
         <div>
             <div class="test-report-summary">
-                <h1>Test Results</h1>
+                <h1>{{ title }}</h1>
                 <table>
                     <tr>
                         <th>Timestamp:</th>
                         <td>{{ summary.timestamp }}</td>
                     </tr>
                     <tr>
                         <th>Duration:</th>
@@ -48,27 +48,37 @@
                         <th>Unexpected Successes:</th>
                         <td style=background-color:var(--unexpected_success);width:50%;>{{ summary.unexpected_success }}</td>
                     </tr>
                     <tr>
                         <th>Errors:</th>
                         <td style=background-color:var(--error);width:50%;>{{ summary.error }}</td>
                     </tr>
+                    <tr>
+                        <th>Coverage Report:</th>
+                        <td>
+                            <a href="coverage/index.html">click here</a>
+                        </td>
+                    </tr>
                 </table>
             </div>
             <div class="container">
                 {% for testcase, testcase_results in testcases.items %}
                     <div class="testcase">
                         <table>
                             <thead>
                                 <tr>
                                     <th>{{ testcase }}</th>
                                     <th>Duration</th>
-                                    <th>Result</th>
                                     <th>
-                                        <button class="btn-testcase-details">&ctdot;</button>
+                                        Result
+                                    </th>
+                                    <th>
+                                        <button class="btn-testcase-details">
+                                            &ctdot;
+                                        </button>
                                     </th>
                                 </tr>
                                 <tr>
                                     <td>
                                         <div class="color-bar">
                                             {% with result_width=testcase_results.summary.skipped|div:testcase_results.summary.totals|mul:100 result=testcase_results.summary.skipped %}
                                                 <div class="skipped" style="width:{{ result_width }}%;">
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
 {% load static %} {% load mathfilters %}
 
-****** Test Results ******
+****** {{ title }} ******
 Timestamp:             {{ summary.timestamp }}
 Duration:              {{ summary.duration.total_seconds }}s
 Number of tests:       {{ summary.totals }}
 Skipped:               {{ summary.skipped }}
 Passed:                {{ summary.passed }}
 Precondition Failures: {{ summary.precondition_failure }}
 Failures:              {{ summary.failure }}
 Expected Failures:     {{ summary.expected_failure }}
 Unexpected Successes:  {{ summary.unexpected_success }}
 Errors:                {{ summary.error }}
+Coverage Report:       click_here
 {% for testcase, testcase_results in testcases.items %}
-{{ testcase }}                                                  Duration                                        Result &ctdot;
+{{ testcase }}                                                  Duration                                        Result  &ctdot;
 {% with result_width=testcase_results.summary.skipped|div:
 testcase_results.summary.totals|mul:100
 result=testcase_results.summary.skipped %}
 {{ result_width }}
 {% endwith %} {% with
 result_width=testcase_results.summary.passed|div:
 testcase_results.summary.totals|mul:100
```

### Comparing `anfema-django-testutils-0.3.0/anfema_django_testutils/testcases.py` & `anfema_django_testutils-0.4.0/anfema_django_testutils/testcases.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,23 +118,23 @@
                 do_something()
 
         """
         return PreconditionContext()
 
     @contextlib.contextmanager
     def assertNotRaises(
-        self, *unexpected_exception: Exception, atomic: bool = False, msg: str = None
+        self, *unexpected_exception: type[Exception], atomic: bool = False, msg: str = None
     ) -> Iterator[None]:
         """Fail if an exception of class *unexpected_exception* is raised by the callable.
 
         Any other exception type will not be caught, and the test case will be deemed to have
         suffered an error, or, if the exception is from type :class:`AssertionError` a failure
         respectively a precondition error if its from type :class:`PreconditionError`.
 
-        :param Exception \*unexpected_exception: Exception classes expected to not be raised.
+        :param type[Exception] \*unexpected_exception: Exception classes expected to not be raised.
         :param bool atomic: If set to :code:`True`, the context will be wrapped inside
           a transaction. Default is :code:`False`.
         :param str msg: Optional message to use on failure.
         """
 
         try:
             yield transaction.atomic() if atomic else contextlib.nullcontext()
```

### Comparing `anfema-django-testutils-0.3.0/docs/Makefile` & `anfema_django_testutils-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anfema-django-testutils-0.3.0/docs/make.bat` & `anfema_django_testutils-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `anfema-django-testutils-0.3.0/docs/source/api.rst` & `anfema_django_testutils-0.4.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `anfema-django-testutils-0.3.0/docs/source/conf.py` & `anfema_django_testutils-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `anfema-django-testutils-0.3.0/docs/source/configuration.rst` & `anfema_django_testutils-0.4.0/docs/source/configuration.rst`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,20 @@
 
 .. option:: TEST_REPORT_CSS
 
     A string which defines the CSS file to be used by the test report generator.
 
     | Default is :code:`"test-results.css"`.
 
+.. option:: TEST_REPORT_TITLE
+
+    A string which defines the test-report`s title.
+
+    | Default is :code:`"Test Results"`.
+
 Coverage settings
 -----------------
 
 The coverage options can be specified in the projects :file:`pyproject.toml` file,
 for instance:
 
 .. code-block:: toml
@@ -91,8 +97,10 @@
                         True)
   --coverage, --no-coverage
                         Enables respectively disables code coverage instead of
                         using the COVERAGE_REPORT_ENABLED setting. (default:
                         True)
   --report-dir DIR      Defines the directory where to store the report
                         artifacts. If this isn't provided, the TEST_REPORT_DIR
-                        setting will be used.
+                        setting will be used.
+  --report-title TITLE  A string which defines the test-report`s title. If this
+                        isn't provided, the TEST_REPORT_TITLE setting will be used.
```

### Comparing `anfema-django-testutils-0.3.0/pyproject.toml` & `anfema_django_testutils-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anfema-django-testutils-0.3.0/PKG-INFO` & `anfema_django_testutils-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anfema-django-testutils
-Version: 0.3.0
+Version: 0.4.0
 Summary: Testrunner for django which covers html report and code coverage
 Keywords: django,tests,coverage,testrunner
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

