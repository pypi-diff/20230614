# Comparing `tmp/mypy_baseline-0.5.1.tar.gz` & `tmp/mypy_baseline-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_baseline-0.5.1.tar", last modified: Thu May 11 07:59:28 2023, max compression
+gzip compressed data, was "mypy_baseline-0.5.2.tar", last modified: Wed Jun 14 09:12:20 2023, max compression
```

## Comparing `mypy_baseline-0.5.1.tar` & `mypy_baseline-0.5.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      654 2023-02-24 08:10:15.428694 mypy_baseline-0.5.1/.github/workflows/main.yml
--rw-r--r--   0        0        0      108 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/.gitignore
--rw-r--r--   0        0        0      325 2023-02-24 08:10:15.428694 mypy_baseline-0.5.1/.markdownlint.yaml
--rw-r--r--   0        0        0     1048 2022-09-01 10:06:03.899566 mypy_baseline-0.5.1/LICENSE
--rw-r--r--   0        0        0     1946 2023-04-14 07:02:53.049087 mypy_baseline-0.5.1/README.md
--rw-r--r--   0        0        0     3448 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/Taskfile.yml
--rw-r--r--   0        0        0   127812 2022-09-28 08:10:05.956227 mypy_baseline-0.5.1/assets/example.png
--rw-r--r--   0        0        0   180974 2022-10-01 08:47:06.040486 mypy_baseline-0.5.1/assets/history.png
--rw-r--r--   0        0        0      326 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/docs/conf.py
--rw-r--r--   0        0        0      811 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/docs/config.md
--rw-r--r--   0        0        0      512 2023-04-14 07:08:04.277478 mypy_baseline-0.5.1/docs/filter.md
--rw-r--r--   0        0        0     4410 2023-02-27 13:02:41.839663 mypy_baseline-0.5.1/docs/follower.md
--rw-r--r--   0        0        0      852 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/docs/history.md
--rw-r--r--   0        0        0      486 2023-02-24 08:04:06.077059 mypy_baseline-0.5.1/docs/index.md
--rw-r--r--   0        0        0     4341 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/docs/leader.md
--rw-r--r--   0        0        0      377 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/docs/plot.md
--rw-r--r--   0        0        0     1297 2023-02-27 12:49:23.969584 mypy_baseline-0.5.1/docs/suggest.md
--rw-r--r--   0        0        0     1202 2023-04-14 07:15:00.364969 mypy_baseline-0.5.1/docs/sync.md
--rw-r--r--   0        0        0      540 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/docs/top-files.md
--rw-r--r--   0        0        0       74 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/docs/usage.md
--rw-r--r--   0        0        0      139 2023-05-11 07:59:13.339635 mypy_baseline-0.5.1/mypy_baseline/__init__.py
--rw-r--r--   0        0        0       44 2022-09-28 08:10:05.956227 mypy_baseline-0.5.1/mypy_baseline/__main__.py
--rw-r--r--   0        0        0      912 2022-09-28 08:10:05.956227 mypy_baseline-0.5.1/mypy_baseline/_cli.py
--rw-r--r--   0        0        0     2200 2022-10-08 07:27:10.462038 mypy_baseline-0.5.1/mypy_baseline/_colors.py
--rw-r--r--   0        0        0     4042 2023-02-24 08:04:06.077059 mypy_baseline-0.5.1/mypy_baseline/_config.py
--rw-r--r--   0        0        0     2315 2023-05-11 07:59:17.535586 mypy_baseline-0.5.1/mypy_baseline/_error.py
--rw-r--r--   0        0        0     2370 2022-10-08 07:27:10.462038 mypy_baseline-0.5.1/mypy_baseline/_git.py
--rw-r--r--   0        0        0      583 2023-02-24 08:04:06.077059 mypy_baseline-0.5.1/mypy_baseline/commands/__init__.py
--rw-r--r--   0        0        0      870 2022-10-26 09:21:57.066380 mypy_baseline-0.5.1/mypy_baseline/commands/_base.py
--rw-r--r--   0        0        0     3532 2022-11-05 08:39:22.834206 mypy_baseline-0.5.1/mypy_baseline/commands/_filter.py
--rw-r--r--   0        0        0     1219 2022-10-08 07:27:10.462038 mypy_baseline-0.5.1/mypy_baseline/commands/_history.py
--rw-r--r--   0        0        0     1514 2023-02-20 10:17:46.003690 mypy_baseline-0.5.1/mypy_baseline/commands/_plot.py
--rw-r--r--   0        0        0     7674 2023-03-10 09:22:19.906984 mypy_baseline-0.5.1/mypy_baseline/commands/_suggest.py
--rw-r--r--   0        0        0     2167 2022-11-05 08:39:22.834206 mypy_baseline-0.5.1/mypy_baseline/commands/_sync.py
--rw-r--r--   0        0        0     1508 2023-02-20 10:21:07.493456 mypy_baseline-0.5.1/mypy_baseline/commands/_top_files.py
--rw-r--r--   0        0        0      384 2022-09-28 08:10:05.960227 mypy_baseline-0.5.1/mypy_baseline/commands/_version.py
--rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.5.1/mypy_baseline/py.typed
--rwxr-xr-x   0        0        0      147 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/netlify.sh
--rw-r--r--   0        0        0       95 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/netlify.toml
--rw-r--r--   0        0        0     1690 2023-02-27 12:49:23.969584 mypy_baseline-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       66 2023-02-21 08:54:27.062504 mypy_baseline-0.5.1/setup.cfg
--rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-24 08:04:06.077059 mypy_baseline-0.5.1/tests/test_commands/__init__.py
--rw-r--r--   0        0        0      786 2023-05-11 07:59:17.539586 mypy_baseline-0.5.1/tests/test_commands/helpers.py
--rw-r--r--   0        0        0     1168 2023-05-11 07:59:17.539586 mypy_baseline-0.5.1/tests/test_commands/test_filter.py
--rw-r--r--   0        0        0      416 2023-02-24 08:04:06.081059 mypy_baseline-0.5.1/tests/test_commands/test_history.py
--rw-r--r--   0        0        0     3453 2023-03-10 09:22:19.906984 mypy_baseline-0.5.1/tests/test_commands/test_suggest.py
--rw-r--r--   0        0        0     1235 2023-05-11 07:59:17.539586 mypy_baseline-0.5.1/tests/test_commands/test_sync.py
--rw-r--r--   0        0        0      637 2023-04-14 07:15:00.368969 mypy_baseline-0.5.1/tests/test_commands/test_top_files.py
--rw-r--r--   0        0        0      147 2023-02-24 08:04:06.081059 mypy_baseline-0.5.1/tests/test_commands/test_version.py
--rw-r--r--   0        0        0     1574 2022-09-28 08:10:05.960227 mypy_baseline-0.5.1/tests/test_error.py
--rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 mypy_baseline-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      710 2023-06-14 09:11:46.439051 mypy_baseline-0.5.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0      108 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/.gitignore
+-rw-r--r--   0        0        0      325 2023-02-24 08:10:15.428694 mypy_baseline-0.5.2/.markdownlint.yaml
+-rw-r--r--   0        0        0     1048 2022-09-01 10:06:03.899566 mypy_baseline-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1946 2023-04-14 07:02:53.049087 mypy_baseline-0.5.2/README.md
+-rw-r--r--   0        0        0     3448 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/Taskfile.yml
+-rw-r--r--   0        0        0   127812 2022-09-28 08:10:05.956227 mypy_baseline-0.5.2/assets/example.png
+-rw-r--r--   0        0        0   180974 2022-10-01 08:47:06.040486 mypy_baseline-0.5.2/assets/history.png
+-rw-r--r--   0        0        0      326 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/docs/conf.py
+-rw-r--r--   0        0        0      811 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/docs/config.md
+-rw-r--r--   0        0        0      512 2023-04-14 07:08:04.277478 mypy_baseline-0.5.2/docs/filter.md
+-rw-r--r--   0        0        0     4410 2023-02-27 13:02:41.839663 mypy_baseline-0.5.2/docs/follower.md
+-rw-r--r--   0        0        0      852 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/docs/history.md
+-rw-r--r--   0        0        0      486 2023-02-24 08:04:06.077059 mypy_baseline-0.5.2/docs/index.md
+-rw-r--r--   0        0        0     4341 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/docs/leader.md
+-rw-r--r--   0        0        0      377 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/docs/plot.md
+-rw-r--r--   0        0        0     1297 2023-02-27 12:49:23.969584 mypy_baseline-0.5.2/docs/suggest.md
+-rw-r--r--   0        0        0     1202 2023-04-14 07:15:00.364969 mypy_baseline-0.5.2/docs/sync.md
+-rw-r--r--   0        0        0      540 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/docs/top-files.md
+-rw-r--r--   0        0        0       74 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/docs/usage.md
+-rw-r--r--   0        0        0      139 2023-06-14 09:11:53.006829 mypy_baseline-0.5.2/mypy_baseline/__init__.py
+-rw-r--r--   0        0        0       44 2022-09-28 08:10:05.956227 mypy_baseline-0.5.2/mypy_baseline/__main__.py
+-rw-r--r--   0        0        0      912 2022-09-28 08:10:05.956227 mypy_baseline-0.5.2/mypy_baseline/_cli.py
+-rw-r--r--   0        0        0     2200 2022-10-08 07:27:10.462038 mypy_baseline-0.5.2/mypy_baseline/_colors.py
+-rw-r--r--   0        0        0     4042 2023-02-24 08:04:06.077059 mypy_baseline-0.5.2/mypy_baseline/_config.py
+-rw-r--r--   0        0        0     2317 2023-06-14 09:11:56.154725 mypy_baseline-0.5.2/mypy_baseline/_error.py
+-rw-r--r--   0        0        0     2370 2022-10-08 07:27:10.462038 mypy_baseline-0.5.2/mypy_baseline/_git.py
+-rw-r--r--   0        0        0      583 2023-02-24 08:04:06.077059 mypy_baseline-0.5.2/mypy_baseline/commands/__init__.py
+-rw-r--r--   0        0        0      870 2022-10-26 09:21:57.066380 mypy_baseline-0.5.2/mypy_baseline/commands/_base.py
+-rw-r--r--   0        0        0     3532 2022-11-05 08:39:22.834206 mypy_baseline-0.5.2/mypy_baseline/commands/_filter.py
+-rw-r--r--   0        0        0     1219 2022-10-08 07:27:10.462038 mypy_baseline-0.5.2/mypy_baseline/commands/_history.py
+-rw-r--r--   0        0        0     1514 2023-02-20 10:17:46.003690 mypy_baseline-0.5.2/mypy_baseline/commands/_plot.py
+-rw-r--r--   0        0        0     7674 2023-03-10 09:22:19.906984 mypy_baseline-0.5.2/mypy_baseline/commands/_suggest.py
+-rw-r--r--   0        0        0     2167 2022-11-05 08:39:22.834206 mypy_baseline-0.5.2/mypy_baseline/commands/_sync.py
+-rw-r--r--   0        0        0     1508 2023-02-20 10:21:07.493456 mypy_baseline-0.5.2/mypy_baseline/commands/_top_files.py
+-rw-r--r--   0        0        0      384 2022-09-28 08:10:05.960227 mypy_baseline-0.5.2/mypy_baseline/commands/_version.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.5.2/mypy_baseline/py.typed
+-rwxr-xr-x   0        0        0      147 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/netlify.sh
+-rw-r--r--   0        0        0       95 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/netlify.toml
+-rw-r--r--   0        0        0     1690 2023-02-27 12:49:23.969584 mypy_baseline-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-02-21 08:54:27.062504 mypy_baseline-0.5.2/setup.cfg
+-rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-24 08:04:06.077059 mypy_baseline-0.5.2/tests/test_commands/__init__.py
+-rw-r--r--   0        0        0      786 2023-05-11 07:59:17.539586 mypy_baseline-0.5.2/tests/test_commands/helpers.py
+-rw-r--r--   0        0        0     1168 2023-05-11 07:59:17.539586 mypy_baseline-0.5.2/tests/test_commands/test_filter.py
+-rw-r--r--   0        0        0      416 2023-02-24 08:04:06.081059 mypy_baseline-0.5.2/tests/test_commands/test_history.py
+-rw-r--r--   0        0        0     3453 2023-03-10 09:22:19.906984 mypy_baseline-0.5.2/tests/test_commands/test_suggest.py
+-rw-r--r--   0        0        0     1235 2023-05-11 07:59:17.539586 mypy_baseline-0.5.2/tests/test_commands/test_sync.py
+-rw-r--r--   0        0        0      637 2023-04-14 07:15:00.368969 mypy_baseline-0.5.2/tests/test_commands/test_top_files.py
+-rw-r--r--   0        0        0      147 2023-02-24 08:04:06.081059 mypy_baseline-0.5.2/tests/test_commands/test_version.py
+-rw-r--r--   0        0        0     2151 2023-06-14 09:11:56.154725 mypy_baseline-0.5.2/tests/test_error.py
+-rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 mypy_baseline-0.5.2/PKG-INFO
```

### Comparing `mypy_baseline-0.5.1/.github/workflows/main.yml` & `mypy_baseline-0.5.2/.github/workflows/main.yml`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: "3.8"
       - uses: arduino/setup-task@v1
+        with:
+          repo-token: ${{ github.token }}
       - run: task lint
 
   markdownlint-cli:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: nosborn/github-action-markdown-cli@v3.2.0
```

### Comparing `mypy_baseline-0.5.1/LICENSE` & `mypy_baseline-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/README.md` & `mypy_baseline-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/Taskfile.yml` & `mypy_baseline-0.5.2/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/assets/example.png` & `mypy_baseline-0.5.2/assets/example.png`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/assets/history.png` & `mypy_baseline-0.5.2/assets/history.png`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/docs/config.md` & `mypy_baseline-0.5.2/docs/config.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/docs/filter.md` & `mypy_baseline-0.5.2/docs/filter.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/docs/follower.md` & `mypy_baseline-0.5.2/docs/follower.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/docs/history.md` & `mypy_baseline-0.5.2/docs/history.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/docs/leader.md` & `mypy_baseline-0.5.2/docs/leader.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/docs/suggest.md` & `mypy_baseline-0.5.2/docs/suggest.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/docs/sync.md` & `mypy_baseline-0.5.2/docs/sync.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/docs/top-files.md` & `mypy_baseline-0.5.2/docs/top-files.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/_cli.py` & `mypy_baseline-0.5.2/mypy_baseline/_cli.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/_colors.py` & `mypy_baseline-0.5.2/mypy_baseline/_colors.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/_config.py` & `mypy_baseline-0.5.2/mypy_baseline/_config.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/_error.py` & `mypy_baseline-0.5.2/mypy_baseline/_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 if TYPE_CHECKING:
     from ._config import Config
 
 REX_COLOR = re.compile('(\x1b\\[\\d*m?|\x0f)*')
 REX_COLOR_NBQA = re.compile(r'\[\d*\x1bm|\x1b|\(B')
 REX_LINE = re.compile(r"""
-    (?P<path>.+\.py):
+    (?P<path>.+\.pyi?):
     (?P<lineno>[0-9]+):\s
     (?P<severity>[a-z]+):\s
     (?P<message>.+?)
     (?:\s\s\[(?P<category>[a-z-]+)\])?
     \s*
 """, re.VERBOSE | re.MULTILINE)
 REX_LINE_NBQA = re.compile(r"""
```

### Comparing `mypy_baseline-0.5.1/mypy_baseline/_git.py` & `mypy_baseline-0.5.2/mypy_baseline/_git.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/commands/__init__.py` & `mypy_baseline-0.5.2/mypy_baseline/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/commands/_base.py` & `mypy_baseline-0.5.2/mypy_baseline/commands/_base.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/commands/_filter.py` & `mypy_baseline-0.5.2/mypy_baseline/commands/_filter.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/commands/_history.py` & `mypy_baseline-0.5.2/mypy_baseline/commands/_history.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/commands/_plot.py` & `mypy_baseline-0.5.2/mypy_baseline/commands/_plot.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/commands/_suggest.py` & `mypy_baseline-0.5.2/mypy_baseline/commands/_suggest.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/commands/_sync.py` & `mypy_baseline-0.5.2/mypy_baseline/commands/_sync.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/mypy_baseline/commands/_top_files.py` & `mypy_baseline-0.5.2/mypy_baseline/commands/_top_files.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/pyproject.toml` & `mypy_baseline-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/tests/test_commands/helpers.py` & `mypy_baseline-0.5.2/tests/test_commands/helpers.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/tests/test_commands/test_filter.py` & `mypy_baseline-0.5.2/tests/test_commands/test_filter.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/tests/test_commands/test_suggest.py` & `mypy_baseline-0.5.2/tests/test_commands/test_suggest.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/tests/test_commands/test_sync.py` & `mypy_baseline-0.5.2/tests/test_commands/test_sync.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/tests/test_commands/test_top_files.py` & `mypy_baseline-0.5.2/tests/test_commands/test_top_files.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.5.1/tests/test_error.py` & `mypy_baseline-0.5.2/tests/test_error.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,7 +26,23 @@
     assert e is not None
     assert e.path.parts == ('my_project', 'api', 'views.py')
     assert e.line_number == 0
     assert e.severity == 'note'
     assert e.message == 'This violates the Liskov substitution principle'
     assert e.category == 'note'
     assert e.get_clean_line(Config()) == LINE2EXP
+
+
+# pyi files
+LINE3 = 'my_project/api/views.pyi:0: note: This violates the Liskov substitution principle\r\n'  # noqa
+LINE3EXP = 'my_project/api/views.pyi:0: note: This violates the Liskov substitution principle'  # noqa
+
+
+def test_line3_parse():
+    e = Error.new(LINE3)
+    assert e is not None
+    assert e.path.parts == ('my_project', 'api', 'views.pyi')
+    assert e.line_number == 0
+    assert e.severity == 'note'
+    assert e.message == 'This violates the Liskov substitution principle'
+    assert e.category == 'note'
+    assert e.get_clean_line(Config()) == LINE3EXP
```

### Comparing `mypy_baseline-0.5.1/PKG-INFO` & `mypy_baseline-0.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy_baseline
-Version: 0.5.1
+Version: 0.5.2
 Summary: Integrate mypy with existing codebase.
 Keywords: mypy,typing,annotations,type annotations
 Author-email: Gram <git@orsinium.dev>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

