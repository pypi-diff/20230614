# Comparing `tmp/repo_review-0.7.0b8.tar.gz` & `tmp/repo_review-0.7.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jun  7 21:09:14 2023, max compression
+gzip compressed data, last modified: Mon Jun 12 21:33:23 2023, max compression
```

## Comparing `repo_review-0.7.0b8.tar` & `repo_review-0.7.0b9.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0      125 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.gitattributes
--rw-r--r--   0        0        0     2061 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      187 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      399 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.readthedocs.yml
--rw-r--r--   0        0        0     1216 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/action.yml
--rw-r--r--   0        0        0     2291 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/noxfile.py
--rw-r--r--   0        0        0      359 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2544 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.github/matchers/pylint.json
--rw-r--r--   0        0        0      669 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1856 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/.nojekyll
--rw-r--r--   0        0        0     4826 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/checks.md
--rw-r--r--   0        0        0      990 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/cli.md
--rw-r--r--   0        0        0      590 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/conf.py
--rw-r--r--   0        0        0     1236 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/families.md
--rw-r--r--   0        0        0     2023 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/fixtures.md
--rw-r--r--   0        0        0     1917 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/index.html
--rw-r--r--   0        0        0      172 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/index.md
--rw-r--r--   0        0        0     2239 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/intro.md
--rw-r--r--   0        0        0     2731 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/plugins.md
--rw-r--r--   0        0        0    10238 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/webapp.js
--rw-r--r--   0        0        0     1770 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/webapp.md
--rw-r--r--   0        0        0      243 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/__init__.py
--rw-r--r--   0        0        0     7283 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/__main__.py
--rw-r--r--   0        0        0      162 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_version.pyi
--rw-r--r--   0        0        0     1311 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/checks.py
--rw-r--r--   0        0        0      494 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/families.py
--rw-r--r--   0        0        0     2004 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     4767 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     2176 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/html.py
--rw-r--r--   0        0        0     5156 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0      246 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/typing.py
--rw-r--r--   0        0        0        0 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     4393 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_checks.py
--rw-r--r--   0        0        0      904 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_cmd.py
--rw-r--r--   0        0        0     2460 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_package.py
--rw-r--r--   0        0        0     2185 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_self.py
--rw-r--r--   0        0        0     3981 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0      333 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2086 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/LICENSE
--rw-r--r--   0        0        0     5552 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/README.md
--rw-r--r--   0        0        0     5108 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/pyproject.toml
--rw-r--r--   0        0        0     7717 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.gitattributes
+-rw-r--r--   0        0        0     2061 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      187 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      399 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.readthedocs.yml
+-rw-r--r--   0        0        0     1216 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/action.yml
+-rw-r--r--   0        0        0     3197 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/noxfile.py
+-rw-r--r--   0        0        0      359 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2544 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      669 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2356 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/.nojekyll
+-rw-r--r--   0        0        0     4836 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/checks.md
+-rw-r--r--   0        0        0      990 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/cli.md
+-rw-r--r--   0        0        0      925 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/conf.py
+-rw-r--r--   0        0        0     1236 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/families.md
+-rw-r--r--   0        0        0     2023 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/fixtures.md
+-rw-r--r--   0        0        0     1917 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/index.html
+-rw-r--r--   0        0        0      243 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/index.md
+-rw-r--r--   0        0        0     2244 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/intro.md
+-rw-r--r--   0        0        0     2746 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/plugins.md
+-rw-r--r--   0        0        0    10216 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/webapp.js
+-rw-r--r--   0        0        0     1770 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/webapp.md
+-rw-r--r--   0        0        0     1033 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/api/repo_review.rst
+-rw-r--r--   0        0        0      230 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     7353 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/__main__.py
+-rw-r--r--   0        0        0      162 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_version.pyi
+-rw-r--r--   0        0        0     2741 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/checks.py
+-rw-r--r--   0        0        0     1055 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/families.py
+-rw-r--r--   0        0        0     3156 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     6010 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     2301 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/html.py
+-rw-r--r--   0        0        0     6278 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0      246 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/typing.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     4393 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_checks.py
+-rw-r--r--   0        0        0      904 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_cmd.py
+-rw-r--r--   0        0        0     2460 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_package.py
+-rw-r--r--   0        0        0     2185 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_self.py
+-rw-r--r--   0        0        0     3981 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      333 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2086 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/LICENSE
+-rw-r--r--   0        0        0     6104 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/README.md
+-rw-r--r--   0        0        0     5190 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/pyproject.toml
+-rw-r--r--   0        0        0     8326 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/PKG-INFO
```

### Comparing `repo_review-0.7.0b8/.pre-commit-config.yaml` & `repo_review-0.7.0b9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/action.yml` & `repo_review-0.7.0b9/action.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/noxfile.py` & `repo_review-0.7.0b9/noxfile.py`

 * *Files 19% similar despite different names*

```diff
@@ -80,16 +80,56 @@
 def docs(session: nox.Session) -> None:
     """
     Build the docs. Pass "--serve" to serve.
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--serve", action="store_true", help="Serve after building")
-    args = parser.parse_args(session.posargs)
+    parser.add_argument(
+        "-b", dest="builder", default="html", help="Build target (default: html)"
+    )
+    args, posargs = parser.parse_known_args(session.posargs)
+
+    if args.builder != "html" and args.serve:
+        session.error("Must not specify non-HTML builder with --serve")
 
     session.install(".[docs]")
     session.chdir("docs")
-    session.run("sphinx-build", "-M", "html", ".", "_build")
+
+    if args.builder == "linkcheck":
+        session.run(
+            "sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs
+        )
+        return
+
+    session.run(
+        "sphinx-build",
+        "-n",  # nitpicky mode
+        "-T",  # full tracebacks
+        "-b",
+        args.builder,
+        ".",
+        f"_build/{args.builder}",
+        *posargs,
+    )
 
     if args.serve:
         session.log("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
         session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
+
+
+@nox.session
+def build_api_docs(session: nox.Session) -> None:
+    """
+    Build (regenerate) API docs.
+    """
+    session.install("sphinx")
+    session.chdir("docs")
+    session.run(
+        "sphinx-apidoc",
+        "-o",
+        "api/",
+        "--module-first",
+        "--no-toc",
+        "--force",
+        "../src/repo_review",
+    )
```

### Comparing `repo_review-0.7.0b8/.github/CONTRIBUTING.md` & `repo_review-0.7.0b9/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/.github/matchers/pylint.json` & `repo_review-0.7.0b9/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/.github/workflows/cd.yml` & `repo_review-0.7.0b9/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/.github/workflows/ci.yml` & `repo_review-0.7.0b9/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -68,14 +68,37 @@
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - uses: hynek/build-and-inspect-python-package@v1
 
+  docs:
+    name: Docs
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+
+      - uses: wntrblm/nox@2023.04.22
+        with:
+          python-versions: "3.11"
+
+      - name: Linkcheck
+        run: nox -s docs -- -b linkcheck
+
+      - name: Build docs with warnings as errors
+        run: nox -s docs -- -W
+
+      - name: Verify no changes required to API docs
+        run: |
+          nox -s build_api_docs
+          git diff --exit-code
+
   action:
     name: Action
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
```

### Comparing `repo_review-0.7.0b8/docs/checks.md` & `repo_review-0.7.0b9/docs/checks.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         """
         Error message if returns False.
         """
         ...
 ```
 
 You need to implement `family`, which is a string indicating which family it is
-grouped under, and `check()`, which can take [](fixtures), and returns `True` if
+grouped under, and `check()`, which can take [](./fixtures.md), and returns `True` if
 the check passes, or `False` if the check fails. If you want a dynamic error
 explanation instead of the `check()` docstring, you can return a non-empty
 string from the check instead of `False`. Returning `None` makes a check
 "skipped". Docstrings/error messages can access their own object with `{self}`
 and check name with `{name}` (these are processed with `.format`, so escape `{}`
 as `{{}}`). The error message is in markdown format.
 
@@ -85,15 +85,15 @@
 - Likewise, all attributes are set on the class (`family`, `requires`, `url`) since there is no state.
 - `requries` is used so that the pyproject checks are skipped if the pyproject file is missing.
 
 ## Registering checks
 
 You register checks with a function that returns a dict of checks, with the code
 of the check (letters + number) as the key, and check instances as the values.
-This function can take [](fixtures), as well, allowing customization of checks
+This function can take [](./fixtures.md), as well, allowing customization of checks
 based on repo properties.
 
 Here is the suggested function for the above example:
 
 ```python
 def repo_review_checks() -> dict[str, General | PyProject]:
     general = {p.__name__: p() for p in General.__subclasses__()}
```

### Comparing `repo_review-0.7.0b8/docs/cli.md` & `repo_review-0.7.0b9/docs/cli.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/docs/families.md` & `repo_review-0.7.0b9/docs/families.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/docs/fixtures.md` & `repo_review-0.7.0b9/docs/fixtures.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/docs/index.html` & `repo_review-0.7.0b9/docs/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -59,13 +59,13 @@
   <body>
     <div id="root">Loading...</div>
     <script type="text/babel">
       const root = ReactDOM.createRoot(document.getElementById("root"));
       root.render(
         <App
           header={true}
-          deps={["sp_repo_review==2023.06.01", "repo-review==0.7.0b7"]}
+          deps={["sp_repo_review==2023.06.07", "repo-review==0.7.0b8"]}
         />,
       );
     </script>
   </body>
 </html>
```

### Comparing `repo_review-0.7.0b8/docs/intro.md` & `repo_review-0.7.0b9/docs/intro.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 and `pip install`.
 
 Plugins are also encouraged to support pre-commit and GitHub Actions.
 
 ## Running checks
 
 You can run checks with (`pipx run`) `repo-review <path>` or `python -m
-repo_review <path>`. See [](cli) for command-line options.
+repo_review <path>`. See [](./cli.md) for command-line options.
 
 ## Configuring
 
 You can explicitly list checks to select or skip in your `pyproject.toml`:
 
 ```toml
 [tool.repo-review]
```

### Comparing `repo_review-0.7.0b8/docs/plugins.md` & `repo_review-0.7.0b9/docs/plugins.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Writing a plugin
 
-To write a plugin for repo-review, you should provide one or more [](checks).
-You can also add new [](fixtures), and customize [](families) with sorting and
+To write a plugin for repo-review, you should provide one or more [](./checks.md).
+You can also add new [](./fixtures.md), and customize [](./families.md) with sorting and
 nicer display names. When writing a plugin, you should also do a few things
 when setting up the package. These suggestions assume you are using a
 standardized backend, such as `hatchling`, `flit-core`, `pdm-backend`, or
 `setuptools>=61`. If you are using some other build backend, please adjust
 accordingly.
 
 ## Avoiding CLI requirements on WebAssembly usage
```

### Comparing `repo_review-0.7.0b8/docs/webapp.js` & `repo_review-0.7.0b9/docs/webapp.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -272,15 +272,15 @@
         /MaterialUI.ThemeProvider>
     );
 }
 
 class App extends React.Component {
     constructor(props) {
         super(props);
-        const deps_str = props.deps.map((i) => `"${i}"`).join(", ");
+        const deps_str = props.deps.join(" ");
         this.state = {
             results: [],
             repo: urlParams.get("repo") || "",
             branch: urlParams.get("branch") || "",
             msg: `${DEFAULT_MSG} Packages: ${deps_str}`,
             progress: false,
             err_msg: "",
```

### Comparing `repo_review-0.7.0b8/docs/webapp.md` & `repo_review-0.7.0b9/docs/webapp.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/src/repo_review/__main__.py` & `repo_review-0.7.0b9/src/repo_review/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import json
 import sys
 import typing
 from collections.abc import Mapping
 from pathlib import Path
 from typing import Literal
 
+import click as orig_click
+
 if typing.TYPE_CHECKING:
-    import click
+    import click  # pylint: disable=reimported
 else:
     import rich_click as click
 
 import rich.console
 import rich.markdown
 import rich.syntax
 import rich.terminal_theme
@@ -32,15 +34,15 @@
 __all__ = ["main"]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
-rich.traceback.install(suppress=[click, rich], show_locals=True, width=None)
+rich.traceback.install(suppress=[click, rich, orig_click], show_locals=True, width=None)
 
 
 def list_all(ctx: click.Context, _param: click.Parameter, value: bool) -> None:
     if not value or ctx.resilient_parsing:
         return
 
     _, checks, families = _collect_all(EmptyTraversable())
```

### Comparing `repo_review-0.7.0b8/src/repo_review/fixtures.py` & `repo_review-0.7.0b9/src/repo_review/fixtures.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,53 +20,82 @@
 
 def __dir__() -> list[str]:
     return __all__
 
 
 def pyproject(package: Traversable) -> dict[str, Any]:
     """
-    The pyproject.toml structure from the package.
+    Fixture: The ``pyproject.toml`` structure from the package. Returned an
+    empty dict if no pyproject.toml found.
+
+    :param package: The package fixture.
     """
     pyproject_path = package.joinpath("pyproject.toml")
     if pyproject_path.is_file():
         with pyproject_path.open("rb") as f:
             return tomllib.load(f)
     return {}
 
 
 def compute_fixtures(
-    root: Traversable, package: Traversable, fixtures: Mapping[str, Callable[..., Any]]
+    root: Traversable,
+    package: Traversable,
+    unevaluated_fixtures: Mapping[str, Callable[..., Any]],
 ) -> dict[str, Any]:
-    results: dict[str, Any] = {"root": root, "package": package}
+    """
+    Given the repo ``root`` Traversable, the ``package`` Traversable, and the dict
+    of all fixture callables, compute the dict of fixture results.
+
+    :param root: The root of the repository
+    :param package: The path to the package (``root / subdir``)
+    :param unevaluated_fixtures: The unevaluated mapping of fixture names to
+                                 callables.
+
+    :return: The fully evaluated dict of fixtures.
+    """
+    fixtures: dict[str, Any] = {"root": root, "package": package}
     graph: dict[str, Set[str]] = {"root": set(), "package": set()}
     graph |= {
-        name: inspect.signature(fix).parameters.keys() for name, fix in fixtures.items()
+        name: inspect.signature(fix).parameters.keys()
+        for name, fix in unevaluated_fixtures.items()
     }
     ts = graphlib.TopologicalSorter(graph)
     for fixture_name in ts.static_order():
         if fixture_name in {"package", "root"}:
             continue
-        func = fixtures[fixture_name]
+        func = unevaluated_fixtures[fixture_name]
         signature = inspect.signature(func)
-        kwargs = {name: results[name] for name in signature.parameters}
-        results[fixture_name] = fixtures[fixture_name](**kwargs)
-    return results
+        kwargs = {name: fixtures[name] for name in signature.parameters}
+        fixtures[fixture_name] = unevaluated_fixtures[fixture_name](**kwargs)
+    return fixtures
 
 
 T = typing.TypeVar("T")
 
 
-def apply_fixtures(computed_fixtures: Mapping[str, Any], func: Callable[..., T]) -> T:
+def apply_fixtures(fixtures: Mapping[str, Any], func: Callable[..., T]) -> T:
+    """
+    Given the pre-computed dict of fixtures and a function, fill in any
+    fixtures from that dict that it requests and return the result.
+
+    :param fixtures: Fully evaluated dict of fixtures.
+    :param func: Some callable that can take fixtures.
+    """
     signature = inspect.signature(func)
     kwargs = {
-        name: value
-        for name, value in computed_fixtures.items()
-        if name in signature.parameters
+        name: value for name, value in fixtures.items() if name in signature.parameters
     }
     return func(**kwargs)
 
 
 def collect_fixtures() -> dict[str, Callable[[Traversable], Any]]:
+    """
+    Produces a dict of fixture callables based on installed entry points. You
+    should call :func:`compute_fixtures` on the result to get the standard dict of
+    fixture results that most other functions in repo-review expect.
+
+    :return: A dict of unevaluated fixtures.
+    """
     return {
         ep.name: ep.load()
         for ep in importlib.metadata.entry_points(group="repo_review.fixtures")
     }
```

### Comparing `repo_review-0.7.0b8/src/repo_review/html.py` & `repo_review-0.7.0b9/src/repo_review/html.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 
 def __dir__() -> list[str]:
     return __all__
 
 
 def to_html(families: Mapping[str, Family], processed: list[Result]) -> str:
     """
-    Convert the results of a repo review to HTML.
+    Convert the results of a repo review (``families``, ``processed``) to HTML.
+
+    :param families: The family mapping.
+    :param processed: The list of processed results.
     """
     out = io.StringIO()
     print = functools.partial(builtins.print, file=out)
     md = markdown_it.MarkdownIt()
 
     for family, results_list in itertools.groupby(processed, lambda r: r.family):
         family_name = families[family].get("name", family)
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations import builtins import functools import io
 import itertools from collections.abc import Mapping import markdown_it from
 .families import Family from .processor import Result __all__ = ["to_html"] def
 __dir__() -> list[str]: return __all__ def to_html(families: Mapping[str,
 Family], processed: list[Result]) -> str: """ Convert the results of a repo
-review to HTML. """ out = io.StringIO() print = functools.partial
-(builtins.print, file=out) md = markdown_it.MarkdownIt() for family,
-results_list in itertools.groupby(processed, lambda r: r.family): family_name =
-families[family].get("name", family) print(f"
+review (``families``, ``processed``) to HTML. :param families: The family
+mapping. :param processed: The list of processed results. """ out = io.StringIO
+() print = functools.partial(builtins.print, file=out) md =
+markdown_it.MarkdownIt() for family, results_list in itertools.groupby
+(processed, lambda r: r.family): family_name = families[family].get("name",
+family) print(f"
 ***** {family_name} *****
 ") print("
 ?      Name          Description
 {icon} {result.name} {description} ") print(description) print("
                                    ") print(md.render(result.err_msg)) print("
 ") if len(processed) == 0: print('No checks ran.') return out.getvalue()
```

### Comparing `repo_review-0.7.0b8/src/repo_review/processor.py` & `repo_review-0.7.0b9/src/repo_review/processor.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,43 +27,62 @@
 def __dir__() -> list[str]:
     return __all__
 
 
 md = markdown_it.MarkdownIt()
 
 
-# Helper to get the type in the JSON style returns
 class ResultDict(typing.TypedDict):
-    family: str
-    description: str
-    result: bool | None
-    err_msg: str
-    url: str
+    """
+    Helper to get the type in the JSON style returns. Basically identical to
+    :class:`Result` but in dict form and without the name.
+    """
+
+    family: str  #: The family string
+    description: str  #: The short description of what the check looks for
+    result: bool | None  #: The result, None means skip
+    err_msg: str  #: The error message if the result is false, in markdown format
+    url: str  #: An optional URL (empty string if missing)
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
 class Result:
-    family: str
-    name: str
-    description: str
-    result: bool | None
-    err_msg: str = ""
-    url: str = ""
+    """
+    This is the returned value from a processed check.
+    """
+
+    family: str  #: The family string
+    name: str  #: The name of the check
+    description: str  #: The short description of what the check looks for
+    result: bool | None  #: The result, None means skip
+    err_msg: str = ""  #: The error message if the result is false, in markdown format
+    url: str = ""  #: An optional URL (empty string if missing)
 
     def err_markdown(self) -> str:
+        """
+        Produces HTML from the error message, assuming it is in markdown.
+        """
         result: str = md.render(self.err_msg).strip()
         return result.removeprefix("<p>").removesuffix("</p>").strip()
 
 
 class ProcessReturn(typing.NamedTuple):
-    families: dict[str, Family]
-    results: list[Result]
+    """
+    Return type for :func:`process`.
+    """
+
+    families: dict[str, Family]  #: A mapping of family strings to Family info dicts
+    results: list[Result]  #: The results list
 
 
 class HasFamily(typing.Protocol):
+    """
+    Simple Protocol to see if family property is present.
+    """
+
     @property
     def family(self) -> str:
         ...
 
 
 T = TypeVar("T", bound=HasFamily)
 
@@ -111,24 +130,22 @@
     select: Set[str] = frozenset(),
     ignore: Set[str] = frozenset(),
     subdir: str = "",
 ) -> ProcessReturn:
     """
     Process the package and return a dictionary of results.
 
-    Parameters
-    ----------
-    root: Traversable | Path
-        The Path(like) to the repository to process
+    :param root: The Path(like) to the repository to process
 
-    ignore: Sequence[str]
-        A list of checks to ignore
+    :param ignore: A list of checks to ignore
 
-    subidr: str
-        The path to the package in the subdirectory, if not at the root of the repository.
+    :param subdir: The path to the package in the subdirectory, if not at the
+                   root of the repository.
+
+    :return: A dictionary of check results.
     """
     package = root.joinpath(subdir) if subdir else root
 
     fixtures, tasks, families = _collect_all(root, subdir)
 
     # Collect our own config
     config = pyproject(package).get("tool", {}).get("repo-review", {})
@@ -175,14 +192,20 @@
             )
         )
 
     return ProcessReturn(families, result_list)
 
 
 def as_simple_dict(results: list[Result]) -> dict[str, ResultDict]:
+    """
+    Convert a results list into a simple dict of dicts structure. The name of
+    the result turns into the key of the outer dict.
+
+    :param results: The list of results.
+    """
     return {
         result.name: typing.cast(
             ResultDict,
             {k: v for k, v in dataclasses.asdict(result).items() if k != "name"},
         )
         for result in results
     }
```

### Comparing `repo_review-0.7.0b8/tests/test_checks.py` & `repo_review-0.7.0b9/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/tests/test_cmd.py` & `repo_review-0.7.0b9/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/tests/test_fixtures.py` & `repo_review-0.7.0b9/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/tests/test_package.py` & `repo_review-0.7.0b9/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/tests/test_self.py` & `repo_review-0.7.0b9/tests/test_self.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/tests/test_utilities/pyproject.py` & `repo_review-0.7.0b9/tests/test_utilities/pyproject.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/.gitignore` & `repo_review-0.7.0b9/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/LICENSE` & `repo_review-0.7.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b8/README.md` & `repo_review-0.7.0b9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 mean this rule is followed, red x’s mean the rule is not. A yellow warning sign
 means that the check was skipped because a previous required check failed. Four
 output formats are supported; `rich`, `svg`, `html`, and `json`.
 
 `sp-repo-review` provides checks based on the
 [Scientific-Python Development Guide][] at [scientific-python/cookie][]. A live
 WebAssembly demo using `sp-repo-review` is
-[here](https://scientific-python.github.io/repo-review).
+[here][repo-review-demo].
 
 ## Running repo-review
 
 Repo-review supports running multiple ways:
 
 - From the command line on a local folder
 - From the command line on a remote repository on GitHub (`gh:org/repo@branch`)
-- From WebAssembly in Pyodide (example in `docs/index.html`)
+- From WebAssembly in [Pyodide][] (example in `docs/index.html`)
 
 If the root of a package is not the repository root, pass `--package-dir a/b/c`.
 
 ## Configuration
 
 Repo-review supports configuration via `pyproject.toml`:
 
@@ -43,37 +43,42 @@
 ```
 
 If `--select` or `--ignore` are given on the command line, they will override
 the `pyproject.toml` config.
 
 ## Comparison to other frameworks
 
-Repo-review was inspired by frameworks like flake8 and Ruff. It is primarily
-different in two ways: It was designed to look at configuration files rather
-than Python files; which means it also only needs a subset of the repository
-(since most files are not configuration files). And it was designed to be
-runnable on external repositories, rather than pre-configured and run from
-inside the repository (which it can be). These differences also power the
+Repo-review was inspired by frameworks like [Flake8][] and [Ruff][]. It is
+primarily different in two ways: It was designed to look at configuration files
+rather than Python files; which means it also only needs a subset of the
+repository (since most files are not configuration files). And it was designed
+to be runnable on external repositories, rather than pre-configured and run
+from inside the repository (which it can be). These differences also power the
 WebAssembly/remote version, which only needs to make a few API calls to look at
 the files that interest the plugin in question.
 
+So if you want to lint Python code, use Flake8 or Ruff. But if you want to
+check Flake8 or Ruff's configuration, use repo-review! Generally, repo-review
+plugins are more about requiring things to be present, like making use all your
+repos have some [pre-commit][] check.
+
 ## Development of repo-review and plugins
 
 This repository is intended to be fun and easy to develop - it requires and uses
 Python 3.10, and uses a lot of the new features in 3.9 and 3.10. It's maybe not
 entirely conventional, but it enables very simple plugin development. It works
-locally, remotely, and in WebAssembly (using Pyodide).
+locally, remotely, and in WebAssembly (using [Pyodide][]).
 
 There are a few key designs that are very useful and make this possible. First,
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
 
-Checks can request fixtures (like pytest) as arguments. Check files can add new
+Checks can request fixtures (like [pytest][]) as arguments. Check files can add new
 fixtures as needed. Fixtures are are specified with entry points, and take any
 other fixture as arguments as well - the `root` and `package` fixtures
 represents the root of the repository and of the package you are checking,
 respectively, and are the basis for all other fixtures. `pyproject` is provided
 as well. Checks are specified via an entrypoint that returns a dict of checks;
 this also can accept fixtures, allowing dynamic check listings.
 
@@ -102,17 +107,27 @@
 interface for a High Energy Physics package in Scikit-HEP.
 
 This project inspired [abSENSE](https://princetonuniversity.github.io/abSENSE/), an
 web interface to abSENSE.
 
 This was developed for [Scikit-HEP][] before moving to Scientific-Python.
 
+<!-- prettier-ignore-start -->
+
 [actions-badge]: https://github.com/scientific-python/repo-review/workflows/CI/badge.svg
 [actions-link]: https://github.com/scientific-python/repo-review/actions
+[docs-badge]: https://readthedocs.org/projects/repo-review/badge/?version=latest
+[docs-link]: https://repo-review.readthedocs.io/en/latest/?badge=latest
+[flake8]: https://flake8.pycqa.org
+[pre-commit]: https://pre-commit.com
+[pyodide]: https://pyodide.org
 [pypi-link]: https://pypi.org/project/repo-review/
 [pypi-platforms]: https://img.shields.io/pypi/pyversions/repo-review
 [pypi-version]: https://badge.fury.io/py/repo-review.svg
-[docs-badge]: https://readthedocs.org/projects/repo-review/badge/?version=latest
-[docs-link]: https://repo-review.readthedocs.io/en/latest/?badge=latest
+[pytest]: https://pytest.org
+[repo-review-demo]: https://scientific-python.github.io/repo-review
+[ruff]: https://beta.ruff.rs
 [scientific-python development guide]: https://learn.scientific-python.org/development
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
 [scikit-hep]: https://scikit-hep.org
+
+<!-- prettier-ignore-end -->
```

### Comparing `repo_review-0.7.0b8/pyproject.toml` & `repo_review-0.7.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
   "repo-review[test,cli]",
 ]
 docs = [
   "furo",
   "myst_parser >=0.13",
   "repo-review[cli]",
   "sphinx >=4.0",
+  "sphinx-autodoc-typehints",
   "sphinx-copybutton",
   "sphinxcontrib-programoutput",
   "sphinxext-opengraph",
 ]
 
 [project.urls]
 Changelog = "https://github.com/scientific-python/repo-review/releases"
@@ -121,14 +122,15 @@
   "missing-module-docstring",
   "missing-class-docstring",
   "missing-function-docstring",
   "invalid-name",
   "redefined-outer-name",
   "no-member",  # better handled by mypy, etc.
   "used-before-assignment",  # False positive on conditional import
+  "unnecessary-ellipsis",  # Not correct for typing
 ]
 
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
   "B", "B904",   # flake8-bugbear
```

### Comparing `repo_review-0.7.0b8/PKG-INFO` & `repo_review-0.7.0b9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.7.0b8
+Version: 0.7.0b9
 Summary: Framework that can run checks on repos
 Project-URL: Changelog, https://github.com/scientific-python/repo-review/releases
 Project-URL: Demo, https://scientific-python.github.io/repo-review
 Project-URL: Documentation, https://repo-review.readthedocs.io/
 Project-URL: Homepage, https://repo-review.readthedocs.io/
 Project-URL: Source, https://github.com/scientific-python/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
@@ -35,14 +35,15 @@
 Requires-Dist: rich>=12.2; extra == 'cli'
 Provides-Extra: dev
 Requires-Dist: repo-review[cli,test]; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: repo-review[cli]; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx>=4.0; extra == 'docs'
 Requires-Dist: sphinxcontrib-programoutput; extra == 'docs'
 Requires-Dist: sphinxext-opengraph; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == 'test'
 Requires-Dist: sp-repo-review; extra == 'test'
@@ -66,23 +67,23 @@
 mean this rule is followed, red x’s mean the rule is not. A yellow warning sign
 means that the check was skipped because a previous required check failed. Four
 output formats are supported; `rich`, `svg`, `html`, and `json`.
 
 `sp-repo-review` provides checks based on the
 [Scientific-Python Development Guide][] at [scientific-python/cookie][]. A live
 WebAssembly demo using `sp-repo-review` is
-[here](https://scientific-python.github.io/repo-review).
+[here][repo-review-demo].
 
 ## Running repo-review
 
 Repo-review supports running multiple ways:
 
 - From the command line on a local folder
 - From the command line on a remote repository on GitHub (`gh:org/repo@branch`)
-- From WebAssembly in Pyodide (example in `docs/index.html`)
+- From WebAssembly in [Pyodide][] (example in `docs/index.html`)
 
 If the root of a package is not the repository root, pass `--package-dir a/b/c`.
 
 ## Configuration
 
 Repo-review supports configuration via `pyproject.toml`:
 
@@ -93,37 +94,42 @@
 ```
 
 If `--select` or `--ignore` are given on the command line, they will override
 the `pyproject.toml` config.
 
 ## Comparison to other frameworks
 
-Repo-review was inspired by frameworks like flake8 and Ruff. It is primarily
-different in two ways: It was designed to look at configuration files rather
-than Python files; which means it also only needs a subset of the repository
-(since most files are not configuration files). And it was designed to be
-runnable on external repositories, rather than pre-configured and run from
-inside the repository (which it can be). These differences also power the
+Repo-review was inspired by frameworks like [Flake8][] and [Ruff][]. It is
+primarily different in two ways: It was designed to look at configuration files
+rather than Python files; which means it also only needs a subset of the
+repository (since most files are not configuration files). And it was designed
+to be runnable on external repositories, rather than pre-configured and run
+from inside the repository (which it can be). These differences also power the
 WebAssembly/remote version, which only needs to make a few API calls to look at
 the files that interest the plugin in question.
 
+So if you want to lint Python code, use Flake8 or Ruff. But if you want to
+check Flake8 or Ruff's configuration, use repo-review! Generally, repo-review
+plugins are more about requiring things to be present, like making use all your
+repos have some [pre-commit][] check.
+
 ## Development of repo-review and plugins
 
 This repository is intended to be fun and easy to develop - it requires and uses
 Python 3.10, and uses a lot of the new features in 3.9 and 3.10. It's maybe not
 entirely conventional, but it enables very simple plugin development. It works
-locally, remotely, and in WebAssembly (using Pyodide).
+locally, remotely, and in WebAssembly (using [Pyodide][]).
 
 There are a few key designs that are very useful and make this possible. First,
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
 
-Checks can request fixtures (like pytest) as arguments. Check files can add new
+Checks can request fixtures (like [pytest][]) as arguments. Check files can add new
 fixtures as needed. Fixtures are are specified with entry points, and take any
 other fixture as arguments as well - the `root` and `package` fixtures
 represents the root of the repository and of the package you are checking,
 respectively, and are the basis for all other fixtures. `pyproject` is provided
 as well. Checks are specified via an entrypoint that returns a dict of checks;
 this also can accept fixtures, allowing dynamic check listings.
 
@@ -152,17 +158,27 @@
 interface for a High Energy Physics package in Scikit-HEP.
 
 This project inspired [abSENSE](https://princetonuniversity.github.io/abSENSE/), an
 web interface to abSENSE.
 
 This was developed for [Scikit-HEP][] before moving to Scientific-Python.
 
+<!-- prettier-ignore-start -->
+
 [actions-badge]: https://github.com/scientific-python/repo-review/workflows/CI/badge.svg
 [actions-link]: https://github.com/scientific-python/repo-review/actions
+[docs-badge]: https://readthedocs.org/projects/repo-review/badge/?version=latest
+[docs-link]: https://repo-review.readthedocs.io/en/latest/?badge=latest
+[flake8]: https://flake8.pycqa.org
+[pre-commit]: https://pre-commit.com
+[pyodide]: https://pyodide.org
 [pypi-link]: https://pypi.org/project/repo-review/
 [pypi-platforms]: https://img.shields.io/pypi/pyversions/repo-review
 [pypi-version]: https://badge.fury.io/py/repo-review.svg
-[docs-badge]: https://readthedocs.org/projects/repo-review/badge/?version=latest
-[docs-link]: https://repo-review.readthedocs.io/en/latest/?badge=latest
+[pytest]: https://pytest.org
+[repo-review-demo]: https://scientific-python.github.io/repo-review
+[ruff]: https://beta.ruff.rs
 [scientific-python development guide]: https://learn.scientific-python.org/development
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
 [scikit-hep]: https://scikit-hep.org
+
+<!-- prettier-ignore-end -->
```

