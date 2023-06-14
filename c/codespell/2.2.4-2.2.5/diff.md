# Comparing `tmp/codespell-2.2.4.tar.gz` & `tmp/codespell-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codespell-2.2.4.tar", last modified: Wed Mar  8 19:00:10 2023, max compression
+gzip compressed data, was "codespell-2.2.5.tar", last modified: Wed Jun 14 17:59:23 2023, max compression
```

## Comparing `codespell-2.2.4.tar` & `codespell-2.2.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:10.866082 codespell-2.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:10.862082 codespell-2.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-08 18:59:52.000000 codespell-2.2.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-08 18:59:52.000000 codespell-2.2.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:10.862082 codespell-2.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-08 18:59:52.000000 codespell-2.2.4/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-03-08 18:59:52.000000 codespell-2.2.4/.github/workflows/codespell-private.yml
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-08 18:59:52.000000 codespell-2.2.4/.github/workflows/codespell-windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-08 18:59:52.000000 codespell-2.2.4/.github/workflows/codespell.yml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-08 18:59:52.000000 codespell-2.2.4/.github/workflows/isort.yml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-08 18:59:52.000000 codespell-2.2.4/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-08 18:59:52.000000 codespell-2.2.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-08 18:59:52.000000 codespell-2.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-03-08 18:59:52.000000 codespell-2.2.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-08 18:59:52.000000 codespell-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-03-08 19:00:10.866082 codespell-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-03-08 18:59:52.000000 codespell-2.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:10.862082 codespell-2.2.4/codespell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-03-08 19:00:10.000000 codespell-2.2.4/codespell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-08 19:00:10.000000 codespell-2.2.4/codespell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 19:00:10.000000 codespell-2.2.4/codespell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-08 19:00:10.000000 codespell-2.2.4/codespell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-08 19:00:10.000000 codespell-2.2.4/codespell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-08 19:00:10.000000 codespell-2.2.4/codespell.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:10.862082 codespell-2.2.4/codespell_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38799 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/_codespell.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-08 19:00:10.000000 codespell-2.2.4/codespell_lib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:10.866082 codespell-2.2.4/codespell_lib/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   933843 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/data/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/data/dictionary_code.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/data/dictionary_en-GB_to_en-US.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/data/dictionary_informal.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/data/dictionary_names.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/data/dictionary_rare.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/data/dictionary_usage.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/data/linux-kernel.exclude
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:10.866082 codespell-2.2.4/codespell_lib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35824 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-03-08 18:59:52.000000 codespell-2.2.4/codespell_lib/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-08 18:59:52.000000 codespell-2.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 19:00:10.866082 codespell-2.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:59:23.986128 codespell-2.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:59:23.974128 codespell-2.2.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-14 17:58:55.000000 codespell-2.2.5/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-14 17:58:55.000000 codespell-2.2.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:59:23.978128 codespell-2.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-14 17:58:55.000000 codespell-2.2.5/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-14 17:58:55.000000 codespell-2.2.5/.github/workflows/codespell-private.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-14 17:58:55.000000 codespell-2.2.5/.github/workflows/codespell-windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-14 17:58:55.000000 codespell-2.2.5/.github/workflows/codespell.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-14 17:58:55.000000 codespell-2.2.5/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-14 17:58:55.000000 codespell-2.2.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-14 17:58:55.000000 codespell-2.2.5/.github/workflows/ruff.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 17:58:55.000000 codespell-2.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 17:58:55.000000 codespell-2.2.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-14 17:58:55.000000 codespell-2.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-06-14 17:59:23.986128 codespell-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-06-14 17:58:55.000000 codespell-2.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:59:23.978128 codespell-2.2.5/codespell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-06-14 17:59:23.000000 codespell-2.2.5/codespell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-14 17:59:23.000000 codespell-2.2.5/codespell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:59:23.000000 codespell-2.2.5/codespell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-14 17:59:23.000000 codespell-2.2.5/codespell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-14 17:59:23.000000 codespell-2.2.5/codespell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 17:59:23.000000 codespell-2.2.5/codespell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:59:23.982128 codespell-2.2.5/codespell_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39558 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/_codespell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 17:59:23.000000 codespell-2.2.5/codespell_lib/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:59:23.986128 codespell-2.2.5/codespell_lib/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   938540 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/data/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/data/dictionary_code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/data/dictionary_en-GB_to_en-US.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/data/dictionary_informal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/data/dictionary_names.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/data/dictionary_rare.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/data/dictionary_usage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/data/linux-kernel.exclude
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:59:23.986128 codespell-2.2.5/codespell_lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37009 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-14 17:58:55.000000 codespell-2.2.5/codespell_lib/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-14 17:58:55.000000 codespell-2.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:59:23.986128 codespell-2.2.5/setup.cfg
```

### Comparing `codespell-2.2.4/.github/CODEOWNERS` & `codespell-2.2.5/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `codespell-2.2.4/.github/dependabot.yml` & `codespell-2.2.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `codespell-2.2.4/.github/workflows/codespell-private.yml` & `codespell-2.2.5/.github/workflows/codespell-private.yml`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - run: sudo apt-get install libaspell-dev aspell-en
       - name: Install dependencies
         run: |
           python --version  # just to check
-          pip install -U pip wheel # upgrade to latest pip find 3.5 wheels; wheel to avoid errors
+          pip install --upgrade pip wheel # upgrade to latest pip find 3.5 wheels; wheel to avoid errors
           pip install --upgrade "setuptools!=47.2.0" docutils setuptools_scm[toml] twine
           pip install aspell-python-py3
           pip install -e ".[dev]" # install the codespell dev packages
       - run: codespell --help
       - run: codespell --version
       - run: make check
       - uses: codecov/codecov-action@v3
@@ -64,27 +64,27 @@
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - uses: actions/checkout@v3
         with:
           persist-credentials: false
       - name: Install general dependencies
-        run: pip install -U pip wheel # upgrade to latest pip find 3.5 wheels; wheel to avoid errors
+        run: pip install --upgrade pip wheel # upgrade to latest pip find 3.5 wheels; wheel to avoid errors
       - name: Install codespell dependencies
         run: pip install -e ".[dev]"
       - uses: codespell-project/sort-problem-matcher@v1
       - run: make check-dictionaries
 
-  flake8-annotation:
+  ruff-annotation:
     runs-on: ubuntu-latest
     steps:
       - name: Setup python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - uses: actions/checkout@v3
         with:
           persist-credentials: false
       - name: Install codespell dependencies
         run: pip install -e ".[dev]"
-      - name: Flake8 with annotations
-        uses: TrueBrain/actions-flake8@v2
+      - name: Ruff with annotations
+        run: ruff --select=ANN --ignore=ANN101,ANN401 .
```

### Comparing `codespell-2.2.4/.github/workflows/codespell-windows.yml` & `codespell-2.2.5/.github/workflows/codespell-windows.yml`

 * *Files identical despite different names*

### Comparing `codespell-2.2.4/.github/workflows/codespell.yml` & `codespell-2.2.5/.github/workflows/codespell.yml`

 * *Files identical despite different names*

### Comparing `codespell-2.2.4/.github/workflows/release.yml` & `codespell-2.2.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `codespell-2.2.4/COPYING` & `codespell-2.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `codespell-2.2.4/PKG-INFO` & `codespell-2.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codespell
-Version: 2.2.4
+Version: 2.2.5
 Summary: Codespell
 Author-email: Lucas De Marchi <lucas.de.marchi@gmail.com>
 License: GPL v2
 Project-URL: homepage, https://github.com/codespell-project/codespell
 Project-URL: repository, https://github.com/codespell-project/codespell
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: hard-encoding-detection
 Provides-Extra: toml
 Provides-Extra: types
+License-File: COPYING
 
 codespell
 =========
 
 Fix common misspellings in text files. It's designed primarily for checking
 misspelled words in source code, but it can be used with other files as well.
 It does not check for word membership in a complete dictionary, but instead
@@ -82,27 +83,27 @@
 
 Some noteworthy flags:
 
 .. code-block:: sh
 
     codespell -w, --write-changes
 
-The ``-w`` flag will actually implement the changes recommended by codespell. Running without the ``-w`` flag is the same as with doing a dry run. It is recommended to run this with the ``-i`` or ``--interactive`` flag.
+The ``-w`` flag will actually implement the changes recommended by codespell. Running without the ``-w`` flag is the same as doing a dry run. It is recommended to run this with the ``-i`` or ``--interactive`` flag.
 
 .. code-block:: sh
 
     codespell -I FILE, --ignore-words=FILE
 
-The ``-I`` flag can be used for a list of certain words to allow that are in the codespell dictionaries. The format of the file is one word per line. Invoke using: ``codespell -I path/to/file.txt`` to execute codespell referencing said list of allowed words. **Important note:** The list passed to ``-I`` is case-sensitive based on how it is listed in the codespell dictionaries.
+The ``-I`` flag can be used for a list of certain words to allow that are in the codespell dictionaries. The format of the file is one word per line. Invoke using: ``codespell -I path/to/file.txt`` to execute codespell referencing said list of allowed words. See `Ignoring Words`_ for more details.
 
 .. code-block:: sh
 
     codespell -L word1,word2,word3,word4
 
-The ``-L`` flag can be used to allow certain words that are comma-separated placed immediately after it.  **Important note:** The list passed to ``-L`` is case-sensitive based on how it is listed in the codespell dictionaries.
+The ``-L`` flag can be used to allow certain words that are comma-separated placed immediately after it.  See `Ignoring Words`_ for more details.
 
 .. code-block:: sh
 
     codespell -x FILE, --exclude-file=FILE
 
 Ignore whole lines that match those in ``FILE``.  The lines in ``FILE`` should match the to-be-excluded lines exactly.
 
@@ -143,14 +144,33 @@
 .. code-block:: sh
 
     echo "word" | codespell -
     echo "1stword,2ndword" | codespell -
 
 You can select the optional dictionaries with the ``--builtin`` option.
 
+Ignoring Words
+--------------
+
+When ignoring false positives, note that spelling errors are *case-insensitive* but words to ignore are *case-sensitive*. For example, the dictionary entry ``wrod`` will also match the typo ``Wrod``, but to ignore it you must pass ``wrod``.
+
+The words to ignore can be passed in two ways:
+
+1. ``-I``: A file with a word per line to ignore:
+
+   .. code-block:: sh
+
+       codespell -I FILE, --ignore-words=FILE
+
+2. ``-L``: A comma separated list of words to ignore on the command line:
+
+   .. code-block:: sh
+
+       codespell -L word1,word2,word3,word4
+
 Using a config file
 -------------------
 
 Command line options can also be specified in a config file.
 
 When running ``codespell``, it will check in the current directory for a file
 named ``setup.cfg`` or ``.codespellrc`` (or a file specified via ``--config``),
@@ -202,24 +222,24 @@
 --------------------------------------------
 
 codespell also works with `pre-commit`, using
 
 .. code-block:: yaml
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
     - id: codespell
 
 If one configures codespell using the `pyproject.toml` file instead use:
 
 .. code-block:: yaml
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
     - id: codespell
       additional_dependencies:
         - tomli
 
 Dictionary format
 -----------------
```

### Comparing `codespell-2.2.4/README.rst` & `codespell-2.2.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -51,27 +51,27 @@
 
 Some noteworthy flags:
 
 .. code-block:: sh
 
     codespell -w, --write-changes
 
-The ``-w`` flag will actually implement the changes recommended by codespell. Running without the ``-w`` flag is the same as with doing a dry run. It is recommended to run this with the ``-i`` or ``--interactive`` flag.
+The ``-w`` flag will actually implement the changes recommended by codespell. Running without the ``-w`` flag is the same as doing a dry run. It is recommended to run this with the ``-i`` or ``--interactive`` flag.
 
 .. code-block:: sh
 
     codespell -I FILE, --ignore-words=FILE
 
-The ``-I`` flag can be used for a list of certain words to allow that are in the codespell dictionaries. The format of the file is one word per line. Invoke using: ``codespell -I path/to/file.txt`` to execute codespell referencing said list of allowed words. **Important note:** The list passed to ``-I`` is case-sensitive based on how it is listed in the codespell dictionaries.
+The ``-I`` flag can be used for a list of certain words to allow that are in the codespell dictionaries. The format of the file is one word per line. Invoke using: ``codespell -I path/to/file.txt`` to execute codespell referencing said list of allowed words. See `Ignoring Words`_ for more details.
 
 .. code-block:: sh
 
     codespell -L word1,word2,word3,word4
 
-The ``-L`` flag can be used to allow certain words that are comma-separated placed immediately after it.  **Important note:** The list passed to ``-L`` is case-sensitive based on how it is listed in the codespell dictionaries.
+The ``-L`` flag can be used to allow certain words that are comma-separated placed immediately after it.  See `Ignoring Words`_ for more details.
 
 .. code-block:: sh
 
     codespell -x FILE, --exclude-file=FILE
 
 Ignore whole lines that match those in ``FILE``.  The lines in ``FILE`` should match the to-be-excluded lines exactly.
 
@@ -112,14 +112,33 @@
 .. code-block:: sh
 
     echo "word" | codespell -
     echo "1stword,2ndword" | codespell -
 
 You can select the optional dictionaries with the ``--builtin`` option.
 
+Ignoring Words
+--------------
+
+When ignoring false positives, note that spelling errors are *case-insensitive* but words to ignore are *case-sensitive*. For example, the dictionary entry ``wrod`` will also match the typo ``Wrod``, but to ignore it you must pass ``wrod``.
+
+The words to ignore can be passed in two ways:
+
+1. ``-I``: A file with a word per line to ignore:
+
+   .. code-block:: sh
+
+       codespell -I FILE, --ignore-words=FILE
+
+2. ``-L``: A comma separated list of words to ignore on the command line:
+
+   .. code-block:: sh
+
+       codespell -L word1,word2,word3,word4
+
 Using a config file
 -------------------
 
 Command line options can also be specified in a config file.
 
 When running ``codespell``, it will check in the current directory for a file
 named ``setup.cfg`` or ``.codespellrc`` (or a file specified via ``--config``),
@@ -171,24 +190,24 @@
 --------------------------------------------
 
 codespell also works with `pre-commit`, using
 
 .. code-block:: yaml
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
     - id: codespell
 
 If one configures codespell using the `pyproject.toml` file instead use:
 
 .. code-block:: yaml
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
     - id: codespell
       additional_dependencies:
         - tomli
 
 Dictionary format
 -----------------
```

### Comparing `codespell-2.2.4/codespell.egg-info/PKG-INFO` & `codespell-2.2.5/codespell.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codespell
-Version: 2.2.4
+Version: 2.2.5
 Summary: Codespell
 Author-email: Lucas De Marchi <lucas.de.marchi@gmail.com>
 License: GPL v2
 Project-URL: homepage, https://github.com/codespell-project/codespell
 Project-URL: repository, https://github.com/codespell-project/codespell
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: hard-encoding-detection
 Provides-Extra: toml
 Provides-Extra: types
+License-File: COPYING
 
 codespell
 =========
 
 Fix common misspellings in text files. It's designed primarily for checking
 misspelled words in source code, but it can be used with other files as well.
 It does not check for word membership in a complete dictionary, but instead
@@ -82,27 +83,27 @@
 
 Some noteworthy flags:
 
 .. code-block:: sh
 
     codespell -w, --write-changes
 
-The ``-w`` flag will actually implement the changes recommended by codespell. Running without the ``-w`` flag is the same as with doing a dry run. It is recommended to run this with the ``-i`` or ``--interactive`` flag.
+The ``-w`` flag will actually implement the changes recommended by codespell. Running without the ``-w`` flag is the same as doing a dry run. It is recommended to run this with the ``-i`` or ``--interactive`` flag.
 
 .. code-block:: sh
 
     codespell -I FILE, --ignore-words=FILE
 
-The ``-I`` flag can be used for a list of certain words to allow that are in the codespell dictionaries. The format of the file is one word per line. Invoke using: ``codespell -I path/to/file.txt`` to execute codespell referencing said list of allowed words. **Important note:** The list passed to ``-I`` is case-sensitive based on how it is listed in the codespell dictionaries.
+The ``-I`` flag can be used for a list of certain words to allow that are in the codespell dictionaries. The format of the file is one word per line. Invoke using: ``codespell -I path/to/file.txt`` to execute codespell referencing said list of allowed words. See `Ignoring Words`_ for more details.
 
 .. code-block:: sh
 
     codespell -L word1,word2,word3,word4
 
-The ``-L`` flag can be used to allow certain words that are comma-separated placed immediately after it.  **Important note:** The list passed to ``-L`` is case-sensitive based on how it is listed in the codespell dictionaries.
+The ``-L`` flag can be used to allow certain words that are comma-separated placed immediately after it.  See `Ignoring Words`_ for more details.
 
 .. code-block:: sh
 
     codespell -x FILE, --exclude-file=FILE
 
 Ignore whole lines that match those in ``FILE``.  The lines in ``FILE`` should match the to-be-excluded lines exactly.
 
@@ -143,14 +144,33 @@
 .. code-block:: sh
 
     echo "word" | codespell -
     echo "1stword,2ndword" | codespell -
 
 You can select the optional dictionaries with the ``--builtin`` option.
 
+Ignoring Words
+--------------
+
+When ignoring false positives, note that spelling errors are *case-insensitive* but words to ignore are *case-sensitive*. For example, the dictionary entry ``wrod`` will also match the typo ``Wrod``, but to ignore it you must pass ``wrod``.
+
+The words to ignore can be passed in two ways:
+
+1. ``-I``: A file with a word per line to ignore:
+
+   .. code-block:: sh
+
+       codespell -I FILE, --ignore-words=FILE
+
+2. ``-L``: A comma separated list of words to ignore on the command line:
+
+   .. code-block:: sh
+
+       codespell -L word1,word2,word3,word4
+
 Using a config file
 -------------------
 
 Command line options can also be specified in a config file.
 
 When running ``codespell``, it will check in the current directory for a file
 named ``setup.cfg`` or ``.codespellrc`` (or a file specified via ``--config``),
@@ -202,24 +222,24 @@
 --------------------------------------------
 
 codespell also works with `pre-commit`, using
 
 .. code-block:: yaml
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
     - id: codespell
 
 If one configures codespell using the `pyproject.toml` file instead use:
 
 .. code-block:: yaml
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
     - id: codespell
       additional_dependencies:
         - tomli
 
 Dictionary format
 -----------------
```

### Comparing `codespell-2.2.4/codespell.egg-info/SOURCES.txt` & `codespell-2.2.5/codespell.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 pyproject.toml
 .github/CODEOWNERS
 .github/dependabot.yml
 .github/workflows/black.yml
 .github/workflows/codespell-private.yml
 .github/workflows/codespell-windows.yml
 .github/workflows/codespell.yml
-.github/workflows/isort.yml
 .github/workflows/mypy.yml
 .github/workflows/release.yml
+.github/workflows/ruff.yml
 codespell.egg-info/PKG-INFO
 codespell.egg-info/SOURCES.txt
 codespell.egg-info/dependency_links.txt
 codespell.egg-info/entry_points.txt
 codespell.egg-info/requires.txt
 codespell.egg-info/top_level.txt
 codespell_lib/__init__.py
```

### Comparing `codespell-2.2.4/codespell_lib/_codespell.py` & `codespell-2.2.5/codespell_lib/_codespell.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import os
 import re
 import sys
 import textwrap
 from typing import Dict, List, Match, Optional, Pattern, Sequence, Set, Tuple
 
 # autogenerated by setuptools_scm
-from ._version import __version__ as VERSION
+from ._version import __version__ as VERSION  # noqa: N812
 
 word_regex_def = "[\\w\\-'’`]+"
 # While we want to treat characters like ( or " as okay for a starting break,
 # these may occur unescaped in URIs, and so we are more restrictive on the
 # endpoint.  Emails are more restrictive, so the endpoint remains flexible.
 uri_regex_def = (
     "(\\b(?:https?|[ts]?ftp|file|git|smb)://[^\\s]+(?=$|\\s)|"
@@ -212,27 +212,25 @@
             )
 
         self.encdetector = UniversalDetector()
 
     def open(self, filename: str) -> Tuple[List[str], str]:
         if self.use_chardet:
             return self.open_with_chardet(filename)
-        else:
-            return self.open_with_internal(filename)
+        return self.open_with_internal(filename)
 
     def open_with_chardet(self, filename: str) -> Tuple[List[str], str]:
         self.encdetector.reset()
         with open(filename, "rb") as fb:
             for line in fb:
                 self.encdetector.feed(line)
                 if self.encdetector.done:
                     break
         self.encdetector.close()
         encoding = self.encdetector.result["encoding"]
-        assert encoding is not None
 
         try:
             f = open(filename, encoding=encoding, newline="")
         except UnicodeDecodeError:
             print(f"ERROR: Could not detect encoding: {filename}", file=sys.stderr)
             raise
         except LookupError:
@@ -241,15 +239,15 @@
                 file=sys.stderr,
             )
             raise
         else:
             lines = f.readlines()
             f.close()
 
-        return lines, encoding
+        return lines, f.encoding
 
     def open_with_internal(self, filename: str) -> Tuple[List[str], str]:
         encoding = None
         first_try = True
         for encoding in encodings:
             if first_try:
                 first_try = False
@@ -584,15 +582,15 @@
         # Build a "fake" argv list using option name and value.
         cfg_args = []
         for key in config["codespell"]:
             # Add option as arg.
             cfg_args.append(f"--{key}")
             # If value is blank, skip.
             val = config["codespell"][key]
-            if val != "":
+            if val:
                 cfg_args.append(val)
 
         # Parse config file options.
         options = parser.parse_args(cfg_args)
 
         # Re-parse command line options to override config.
         options = parser.parse_args(list(args), namespace=options)
@@ -669,15 +667,15 @@
         s = f.read(1024)
     return b"\x00" not in s
 
 
 def fix_case(word: str, fixword: str) -> str:
     if word == word.capitalize():
         return ", ".join(w.strip().capitalize() for w in fixword.split(","))
-    elif word == word.upper():
+    if word == word.upper():
         return fixword.upper()
     # they are both lower case
     # or we don't have any idea
     return fixword
 
 
 def ask_for_word_fix(
@@ -746,15 +744,15 @@
     lines: List[str],
     index: int,
     context: Tuple[int, int],
 ) -> None:
     # context = (context_before, context_after)
     for i in range(index - context[0], index + context[1] + 1):
         if 0 <= i < len(lines):
-            print("{} {}".format(">" if i == index else ":", lines[i].rstrip()))
+            print(f"{'>' if i == index else ':'} {lines[i].rstrip()}")
 
 
 def _ignore_word_sub(
     text: str,
     ignore_word_regex: Optional[Pattern[str]],
 ) -> str:
     if ignore_word_regex:
@@ -895,14 +893,27 @@
                 uri_regex,
                 uri_ignore_words,
             )
         for match in check_matches:
             word = match.group()
             lword = word.lower()
             if lword in misspellings:
+                # Sometimes we find a 'misspelling' which is actually a valid word
+                # preceded by a string escape sequence.  Ignore such cases as
+                # they're usually false alarms; see issue #17 among others.
+                char_before_idx = match.start() - 1
+                if (
+                    char_before_idx >= 0
+                    and line[char_before_idx] == "\\"
+                    # bell, backspace, formfeed, newline, carriage-return, tab, vtab.
+                    and word.startswith(("a", "b", "f", "n", "r", "t", "v"))
+                    and lword[1:] not in misspellings
+                ):
+                    continue
+
                 context_shown = False
                 fix = misspellings[lword].fix
                 fixword = fix_case(word, misspellings[lword].data)
 
                 if options.interactive and lword not in asked_for:
                     if context is not None:
                         context_shown = True
@@ -1168,15 +1179,20 @@
                         uri_regex,
                         uri_ignore_words,
                         context,
                         options,
                     )
 
                 # skip (relative) directories
-                dirs[:] = [dir_ for dir_ in dirs if not glob_match.match(dir_)]
+                dirs[:] = [
+                    dir_
+                    for dir_ in dirs
+                    if not glob_match.match(dir_)
+                    and not is_hidden(dir_, options.check_hidden)
+                ]
 
         elif not glob_match.match(filename):  # skip files
             bad_count += parse_file(
                 filename,
                 colors,
                 summary,
                 misspellings,
```

### Comparing `codespell-2.2.4/codespell_lib/data/dictionary.txt` & `codespell-2.2.5/codespell_lib/data/dictionary.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 aaccessibility->accessibility
 aaccession->accession
 aache->cache, ache,
 aack->ack
 aactual->actual
 aactually->actually
 aadd->add
+aadded->added
+aadding->adding
 aagain->again
 aaggregation->aggregation
 aanother->another
 aapply->apply
 aaproximate->approximate
 aaproximated->approximated
 aaproximately->approximately
 aaproximates->approximates
 aaproximating->approximating
 aare->are
+aas->ass, as,
 aassign->assign
 aassignment->assignment
 aassignments->assignments
 aassociated->associated
 aassumed->assumed
 aautomatic->automatic
 aautomatically->automatically
@@ -452,14 +455,18 @@
 accompagnies->accompanies
 accompagniment->accompaniment
 accompagning->accompanying
 accompagny->accompany
 accompagnying->accompanying
 accompained->accompanied
 accompanyed->accompanied
+accomponied->accompanied
+accomponies->accompanies
+accompony->accompany
+accomponying->accompanying
 accompt->account
 acconding->according
 accont->account
 accontant->accountant
 acconted->accounted
 acconting->accounting
 accoording->according
@@ -1158,14 +1165,15 @@
 affitnity->affinity
 afforementioned->aforementioned
 affort->afford, effort,
 affortable->affordable
 afforts->affords
 affraid->afraid
 affter->after
+afile->a file, agile,
 afinity->affinity
 afor->for
 aforememtioned->aforementioned
 aforementiond->aforementioned
 aforementionned->aforementioned
 aformentioned->aforementioned
 afrer->after
@@ -1722,14 +1730,18 @@
 allocateng->allocating
 allocationg->allocating, allocation,
 allocaton->allocation
 allocatoor->allocator
 allocatote->allocate
 allocatrd->allocated
 allocattion->allocation
+alloccate->allocate
+alloccated->allocated
+alloccates->allocates
+alloccating->allocating
 alloco->alloc
 allocos->allocs
 allocte->allocate
 allocted->allocated
 allocting->allocating
 alloction->allocation
 alloctions->allocations
@@ -3360,14 +3372,16 @@
 assemly->assembly
 assemnly->assembly
 assemple->assemble
 assending->ascending
 asser->assert
 assersion->assertion
 assertation->assertion
+assertino->assertion
+assertinos->assertions
 assertio->assertion
 assertting->asserting
 assesmenet->assessment
 assesment->assessment
 assesments->assessments
 assessmant->assessment
 assessmants->assessments
@@ -3695,14 +3709,15 @@
 atach->attach
 atached->attached
 ataching->attaching
 atachment->attachment
 atachments->attachments
 atack->attack
 atain->attain
+atalog->catalog
 atatch->attach
 atatchable->attachable
 atatched->attached
 atatches->attaches
 atatching->attaching
 atatchment->attachment
 atatchments->attachments
@@ -4143,14 +4158,16 @@
 auto-destrcut->auto-destruct
 auto-detet->auto-detect, auto-delete,
 auto-deteted->auto-detected, auto-deleted,
 auto-detetes->auto-deletes, auto-detects,
 auto-deteting->auto-detecting, auto-deleting,
 auto-detetion->auto-detection, auto-deletion,
 auto-detets->auto-detects, auto-deletes,
+auto-ganerated->auto-generated
+auto-generaged->auto-generated
 auto-genrated->auto-generated
 auto-genratet->auto-generated
 auto-genration->auto-generation
 auto-identation->auto-indentation
 auto-negatiotiation->auto-negotiation
 auto-negatiotiations->auto-negotiations
 auto-negoatiation->auto-negotiation
@@ -4926,14 +4943,15 @@
 beteeen->between
 beteen->between
 beter->better
 beteween->between
 betrween->between
 bettern->better
 bettery->better, battery,
+bettr->better, bettor,
 bettween->between
 betwean->between
 betwee->between
 betweed->between
 betweeen->between
 betweem->between
 betweend->between
@@ -5995,14 +6013,15 @@
 canoical->canonical
 canonalize->canonicalize
 canonalized->canonicalized
 canonalizes->canonicalizes
 canonalizing->canonicalizing
 canoncal->canonical
 canoncial->canonical
+canoncical->canonical
 canonicalizations->canonicalization
 canonival->canonical
 canot->cannot
 cant'->can't
 cant't->can't
 cant;->can't
 cantact->contact
@@ -6551,14 +6570,15 @@
 chaing->chain
 chalenging->challenging
 challanage->challenge
 challange->challenge
 challanged->challenged
 challanges->challenges
 challege->challenge
+challening->challenging
 chambre->chamber
 chambres->chambers
 champain->Champagne
 champane->Champagne
 Champange->Champagne
 chanage->change
 chanaged->changed
@@ -8398,14 +8418,15 @@
 comsumers->consumers
 comsumes->consumes
 comsuming->consuming
 comsumption->consumption
 comtain->contain
 comtained->contained
 comtainer->container
+comtaining->containing
 comtains->contains
 comunicate->communicate
 comunication->communication
 comunism->communism
 comunist->communist
 comunists->communists
 comunity->community
@@ -8987,14 +9008,15 @@
 conrrupts->corrupts
 conrtib->contrib
 conrtibs->contribs
 consants->constants
 conscent->consent
 consciencious->conscientious
 consciouness->consciousness
+consciousely->consciously
 consctruct->construct
 consctructed->constructed
 consctructing->constructing
 consctruction->construction
 consctructions->constructions
 consctructive->constructive
 consctructor->constructor
@@ -9282,14 +9304,15 @@
 containe->contain, contained, container, contains,
 containees->containers
 containerr->container
 containes->contains, container, contained,
 containg->containing
 containging->containing
 containig->containing
+containin->containing
 containined->contained
 containings->containing
 containining->containing
 containinng->containing
 containint->containing
 containn->contain
 containner->container
@@ -10297,14 +10320,16 @@
 creatin->creation, creating, creatine, cretin,
 creationg->creation, creating,
 creatning->creating
 creatre->create
 creatred->created
 creats->creates
 credate->created
+credentail->credential
+credentails->credentials
 credetial->credential
 credetials->credentials
 credidential->credential
 credidentials->credentials
 credintial->credential
 credintials->credentials
 credis->credits
@@ -10534,14 +10559,15 @@
 curresponding->corresponding
 curretly->currently
 curretn->current
 curretnly->currently
 curriculem->curriculum
 currious->curious
 currnet->current
+currnetly->currently
 currnt->current
 currntly->currently
 curros->cursor
 currrency->currency
 currrent->current
 currrently->currently
 curruent->current
@@ -11420,16 +11446,21 @@
 defualts->defaults
 defult->default
 defulted->defaulted
 defulting->defaulting
 defults->defaults
 degenarate->degenerate
 degenarated->degenerated
+degenarates->degenerates
 degenarating->degenerating
 degenaration->degeneration
+degenerage->degenerate
+degeneraged->degenerated
+degenerages->degenerates
+degeneraging->degenerating
 degenracy->degeneracy
 degenrate->degenerate
 degenrated->degenerated
 degenrates->degenerates
 degenratet->degenerated
 degenrating->degenerating
 degenration->degeneration
@@ -11586,14 +11617,15 @@
 deliverate->deliberate
 delivermode->deliverymode
 deliverying->delivering
 deliverys->deliveries, delivers,
 delpoy->deploy
 delpoyed->deployed
 delpoying->deploying
+delpoys->deploys
 delt->dealt
 delte->delete
 delted->deleted
 deltes->deletes
 delting->deleting
 deltion->deletion
 delusionally->delusively
@@ -12672,16 +12704,20 @@
 differntiated->differentiated
 differntiates->differentiates
 differntiating->differentiating
 differntly->differently
 differnty->different, differently,
 differred->differed
 differrence->difference
+differrences->differences
 differrent->different
+differrently->differently
 difffered->differed
+diffference->difference
+diffferences->differences
 diffferent->different
 diffferently->differently
 difffers->differs
 difficault->difficult
 difficaulties->difficulties
 difficaulty->difficulty
 difficulity->difficulty
@@ -12745,14 +12781,16 @@
 dilligently->diligently
 dillimport->dllimport
 dimand->demand, diamond,
 dimands->demands, diamonds,
 dimansion->dimension
 dimansional->dimensional
 dimansions->dimensions
+dimaond->diamond
+dimaonds->diamonds
 dimemsions->dimensions
 dimenion->dimension, dominion,
 dimenional->dimensional
 dimenionalities->dimensionalities
 dimenionality->dimensionality
 dimenions->dimensions
 dimenionsal->dimensional
@@ -12809,14 +12847,15 @@
 diplayed->displayed
 diplaying->displaying
 diplays->displays
 diplomancy->diplomacy
 dipose->dispose, depose,
 diposed->disposed, deposed,
 diposing->disposing, deposing,
+diposition->disposition
 diptheria->diphtheria
 dipthong->diphthong
 dipthongs->diphthongs
 dircet->direct
 dircetories->directories
 dircetory->directory
 dirctly->directly
@@ -13212,14 +13251,15 @@
 dispicable->despicable
 dispite->despite
 displa->display
 displacemnt->displacement
 displacemnts->displacements
 displacment->displacement
 displacments->displacements
+displaing->displaying
 displayd->displayed
 displayes->displays, displayed,
 displayied->displayed
 displayig->displaying
 disply->display
 displyed->displayed
 displying->displaying
@@ -14687,34 +14727,48 @@
 endien->endian, indian,
 endiens->endians, indians,
 endig->ending
 endiif->endif
 endiness->endianness
 endnoden->endnode
 endoint->endpoint
+endoints->endpoints
 endolithes->endoliths
+endpdoint->endpoint
+endpdoints->endpoints
+endpint->endpoint
 endpints->endpoints
 endpiont->endpoint
 endpionts->endpoints
 endpont->endpoint
 endponts->endpoints
 endsup->ends up
 enduce->induce
+enduced->induced
+enduces->induces
+enducing->inducing
 endur->endure
+eneable->enable
+eneabled->enabled
 eneables->enables
+eneabling->enabling
 enebale->enable
 enebaled->enabled
+enebales->enables
+enebaling->enabling
 eneble->enable
 ened->need
 enegeries->energies
 enegery->energy
 enehanced->enhanced
 enery->energy
 eneter->enter
 enetered->entered
+enetering->entering
+eneters->enters
 enetities->entities
 enetity->entity
 eneumeration->enumeration
 eneumerations->enumerations
 eneumretaion->enumeration
 eneumretaions->enumerations
 enew->new
@@ -14722,35 +14776,46 @@
 enforcable->enforceable
 enforceing->enforcing
 enforcmement->enforcement
 enforcment->enforcement
 enfore->enforce
 enfored->enforced
 enfores->enforces
+enforing->enforcing
 enforncing->enforcing
 engagment->engagement
 engeneer->engineer
 engeneering->engineering
+engeneers->engineers
 engery->energy
 engieer->engineer
+engieering->engineering
+engieers->engineers
 engieneer->engineer
 engieneers->engineers
-enginee->engine
+enginee->engine, engineer,
+enginees->engines, engineers,
 enginge->engine
+enginges->engines
 enginin->engine
 enginineer->engineer
+enginineering->engineering
+enginineers->engineers
 engoug->enough
+engouh->enough
 enhabce->enhance
 enhabced->enhanced
 enhabces->enhances
 enhabcing->enhancing
 enhace->enhance
 enhaced->enhanced
 enhacement->enhancement
 enhacements->enhancements
+enhaces->enhances
+enhacing->enhancing
 enhancd->enhanced
 enhancment->enhancement
 enhancments->enhancements
 enhaned->enhanced
 enhence->enhance
 enhenced->enhanced
 enhencement->enhancement
@@ -15073,14 +15138,17 @@
 equiptment->equipment
 equire->require, enquire, equine, esquire,
 equitorial->equatorial
 equivalance->equivalence
 equivalant->equivalent
 equivalenet->equivalent, equivalents,
 equivalentsly->equivalently, equivalency,
+equivallent->equivalent
+equivallently->equivalently
+equivallents->equivalents
 equivelant->equivalent
 equivelent->equivalent
 equivelents->equivalents
 equivilant->equivalent
 equivilent->equivalent
 equivivalent->equivalent
 equivlalent->equivalent
@@ -15722,14 +15790,18 @@
 exclamantion->exclamation
 excliude->exclude
 excliuded->excluded
 excliudes->excludes
 excliuding->excluding
 excludde->exclude
 excludind->excluding
+excludle->exclude
+excludled->excluded
+excludles->excludes
+excludling->excluding
 exclue->exclude
 excluse->exclude, excuse, exclusive,
 exclusiv->exclusive
 exclusivelly->exclusively
 exclusivly->exclusively
 exclusivs->exclusives
 excluslvely->exclusively
@@ -16787,14 +16859,16 @@
 exproted->exported
 exproting->exporting
 exprots->exports
 exprted->exported
 exptected->expected
 exra->extra
 exract->extract
+exrension->extension
+exrensions->extensions
 exressed->expressed
 exression->expression
 exsist->exists, exist,
 exsistence->existence
 exsistent->existent
 exsisting->existing
 exsists->exists
@@ -16994,14 +17068,16 @@
 facour->favour, favor,
 facourite->favourite
 facourites->favourites
 facours->favours
 factization->factorization
 factorizaiton->factorization
 factorys->factories
+facttories->factories
+facttory->factory
 fadind->fading
 faeture->feature
 faetures->features
 Fahrenheight->Fahrenheit
 faied->failed, fade,
 faield->failed
 faild->failed
@@ -17461,16 +17537,21 @@
 fo->of, for, to, do, go,
 focu->focus
 focued->focused
 focument->document
 focuse->focus
 focusf->focus
 focuss->focus
+foded->folded, coded, faded, forded, boded,
+foder->folder, coder,
+foders->folders, coders,
+foding->folding, coding, fading, fording, boding,
 fof->for
 foget->forget
+fogets->forgets
 fogot->forgot
 fogotten->forgotten
 fointers->pointers
 folde->folder, fold,
 foler->folder
 folers->folders
 folfer->folder
@@ -17698,14 +17779,15 @@
 fontier->frontier
 fontisizing->fontifying
 fontonfig->fontconfig
 fontrier->frontier
 fonud->found
 foontnotes->footnotes
 foootball->football
+foor->foot, for,
 foorter->footer
 footnoes->footnotes
 footprinst->footprints
 foound->found
 foppy->floppy
 foppys->floppies
 foramatting->formatting
@@ -18180,14 +18262,15 @@
 furutre->future
 furzzer->fuzzer
 fuschia->fuchsia
 fusha->fuchsia
 fushas->fuchsias
 fushed->flushed
 fushing->flushing
+fusipn->fusion
 futal->futile
 futer->further, future,
 futher->further
 futherize->further
 futhermore->furthermore
 futhroc->futhark, futhorc,
 futrue->future
@@ -18213,14 +18296,17 @@
 gallleries->galleries
 galllery->gallery
 galllerys->galleries
 galvinized->galvanized
 Gameboy->Game Boy
 ganbia->gambia
 ganerate->generate
+ganerated->generated
+ganerates->generates
+ganerating->generating
 ganes->games
 ganster->gangster
 garabge->garbage
 garantee->guarantee
 garanteed->guaranteed
 garanteeed->guaranteed
 garantees->guarantees
@@ -18281,14 +18367,15 @@
 geeral->general
 gemetrical->geometrical
 gemetry->geometry
 gemoetry->geometry
 gemometric->geometric
 genarate->generate
 genarated->generated
+genarates->generates
 genarating->generating
 genaration->generation
 genearal->general
 genearally->generally
 genearted->generated
 geneate->generate
 geneated->generated
@@ -18296,14 +18383,18 @@
 geneating->generating
 geneation->generation
 geneic->generic, genetic,
 geneological->genealogical
 geneologies->genealogies
 geneology->genealogy
 generaates->generates
+generage->generate
+generaged->generated
+generages->generates
+generaging->generating
 generaing->generating
 generall->generally, general,
 generaly->generally
 generalyl->generally
 generalyse->generalise
 generat->generate, general,
 generater->generator
@@ -19395,14 +19486,15 @@
 htis->this
 htmp->html
 htose->those, these,
 htpt->http
 htpts->https
 htting->hitting
 hueristic->heuristic
+huld->held, hold,
 humber->number
 humer->humor, humour,
 humerous->humorous, humerus,
 huminoid->humanoid
 humoural->humoral
 humurous->humorous
 hunderd->hundred
@@ -19505,14 +19597,15 @@
 idenfied->identified
 idenfifier->identifier
 idenfifiers->identifiers
 idenfitifer->identifier
 idenfitifers->identifiers
 idenfitify->identify
 idenitfy->identify
+idenities->identities
 idenitify->identify
 identation->indentation
 identcial->identical
 identfied->identified
 identfier->identifier
 identfiers->identifiers
 identiable->identifiable
@@ -19529,17 +19622,21 @@
 identifers->identifiers
 identificable->identifiable
 identifictaion->identification
 identifieer->identifier
 identifiler->identifier
 identifilers->identifiers
 identifing->identifying
+identifiter->identifier
+identifiters->identifier
 identifiy->identify
 identifyable->identifiable
 identifyed->identified
+identiies->identities
+identites->identities
 identitiy->identity
 identiviert->identifiers
 identiy->identify, identity,
 identtation->indentation
 identties->identities
 identtifier->identifier
 identty->identity
@@ -19993,14 +20090,15 @@
 imporvements->improvements
 imporves->improves
 imporving->improving
 imporvment->improvement
 imposible->impossible
 impossiblble->impossible
 impot->import
+impotant->impotent, important,
 impotr->import, importer,
 impotrt->import, imported, importer,
 impove->improve
 impoved->improved
 impovement->improvement
 impovements->improvements
 impoves->improves
@@ -20514,14 +20612,16 @@
 individally->individually
 individals->individuals
 individaul->individual
 individaully->individually
 individauls->individuals
 individauly->individually
 individial->individual
+individiual->individual
+individiually->individually
 individuall->individually, individual,
 individualy->individually
 individuel->individual
 individuelly->individually
 individuely->individually
 individul->individual
 individule->individual
@@ -20731,14 +20831,19 @@
 inidicated->indicated
 inidicates->indicates
 inidicating->indicating
 inidication->indication
 inidications->indications
 inidividual->individual
 inidvidual->individual
+iniect->inject
+iniected->injected
+iniecting->injecting
+iniection->injection
+iniects->injects
 inifinite->infinite
 inifinity->infinity
 inifinte->infinite
 inifite->infinite
 iniitalize->initialize
 iniitial->initial
 iniitialization->initialization
@@ -21862,14 +21967,16 @@
 inveting->inverting
 invetory->inventory
 inviation->invitation
 invididual->individual
 invidivual->individual
 invidual->individual
 invidually->individually
+invirant->invariant
+invirants->invariants
 invisble->invisible
 invisblity->invisibility
 invisiable->invisible
 invisibile->invisible
 invisivble->invisible
 invlaid->invalid
 invlid->invalid
@@ -22337,15 +22444,14 @@
 kuberentes->Kubernetes
 kuberetes->Kubernetes
 kubermetes->Kubernetes
 kubernates->Kubernetes
 kubernests->Kubernetes
 kubernete->Kubernetes
 kuberntes->Kubernetes
-Kwanza->Kwanzaa
 kwno->know
 kwoledgebase->knowledge base
 kwuzine->cuisine
 kwuzines->cuisines
 kyebosh->kibosh
 kyeboshed->kiboshed
 kyeboshes->kiboshes
@@ -23209,14 +23315,15 @@
 mananger->manager
 manangers->managers
 manaul->manual
 manaully->manually
 manauls->manuals
 manaze->mayonnaise
 mandatatory->mandatory
+mandess->madness
 mandetory->mandatory
 manement->management
 maneouvre->manoeuvre
 maneouvred->manoeuvred
 maneouvres->manoeuvres
 maneouvring->manoeuvring
 manetain->maintain
@@ -23876,14 +23983,15 @@
 microoseconds->microseconds
 micropone->microphone
 micropones->microphones
 microprocesspr->microprocessor
 microprocessprs->microprocessors
 microseond->microsecond
 microseonds->microseconds
+Microsfoft->Microsoft
 Microsft->Microsoft
 microship->microchip
 microships->microchips
 Microsof->Microsoft
 Microsofot->Microsoft
 Micrsft->Microsoft
 Micrsoft->Microsoft
@@ -24083,14 +24191,15 @@
 mirorring->mirroring
 mirorrs->mirrors
 mirors->mirrors, minors,
 mirro->mirror
 mirroed->mirrored
 mirrorn->mirror
 mirrorred->mirrored
+mis->miss, mist,
 mis-alignement->misalignment
 mis-alignment->misalignment
 mis-intepret->mis-interpret
 mis-intepreted->mis-interpreted
 mis-match->mismatch
 misake->mistake
 misaken->mistaken
@@ -24559,29 +24668,43 @@
 muder->murder
 mudering->murdering
 mudule->module
 mudules->modules
 muext->mutex
 muiltiple->multiple
 muiltiples->multiples
+muiltiplied->multiplied
+muiltiplies->multiplies
+muiltiply->multiply
+muiltiplying->multiplying
 muliple->multiple
 muliples->multiples
+muliplied->multiplied
+muliplies->multiplies
+muliply->multiply
+muliplying->multiplying
 mulithread->multithread
 mulitiple->multiple
+mulitiplied->multiplied
 mulitiplier->multiplier
 mulitipliers->multipliers
+mulitiplies->multiplies
+mulitiply->multiply
+mulitiplying->multiplying
 mulitpart->multipart
 mulitpath->multipath
 mulitple->multiple
 mulitplication->multiplication
 mulitplicative->multiplicative
 mulitplied->multiplied
 mulitplier->multiplier
 mulitpliers->multipliers
+mulitplies->multiplies
 mulitply->multiply
+mulitplying->multiplying
 multi-dimenional->multi-dimensional
 multi-dimenionsal->multi-dimensional
 multi-langual->multi-lingual
 multi-presistion->multi-precision
 multi-threded->multi-threaded
 multible->multiple
 multibye->multibyte
@@ -24593,17 +24716,28 @@
 multidimension->multidimensional
 multidimensionnal->multidimensional
 multidimentionnal->multidimensional
 multiecast->multicast
 multifuction->multifunction
 multilangual->multilingual
 multile->multiple
+multilied->multiplied
+multilies->multiplies
 multilpe->multiple
+multilpies->multiplies
+multilplied->multiplied
+multilplies->multiplies
+multilpy->multiply
+multilpying->multiplying
+multily->multiply
+multilying->multiplying
 multipe->multiple
 multipes->multiples
+multipied->multiplied
+multipies->multiplies
 multipiler->multiplier
 multipilers->multipliers
 multipl->multiple, multiply,
 multipled->multiplied
 multipler->multiplier, multiple,
 multiplers->multipliers
 multipliciaton->multiplication
@@ -24612,14 +24746,15 @@
 multiplikation->multiplication
 multipling->multiplying
 multipllication->multiplication
 multiplyed->multiplied
 multipresistion->multiprecision
 multipul->multiple
 multipy->multiply
+multipying->multiplying
 multipyling->multiplying
 multithreded->multithreaded
 multitute->multitude
 multivriate->multivariate
 multixsite->multisite
 multline->multiline
 multliple->multiple
@@ -24664,14 +24799,15 @@
 mussil->muscle, mussel,
 mussils->muscles, mussels,
 must't->mustn't
 mustash->mustache, moustache,
 mustator->mutator
 muste->must
 mutablity->mutability
+mutbal->mutable
 mutbale->mutable
 mutch->much
 mutches->matches
 mutecies->mutexes
 mutexs->mutexes
 muti->multi
 muti-statement->multi-statement
@@ -24680,26 +24816,32 @@
 mutiindex->multi index, multi-index, multiindex,
 mutilcast->multicast
 mutiliated->mutilated
 mutimarked->multimarked
 mutipath->multipath
 mutipl->multiple, multiply,
 mutiple->multiple
+mutiplied->multiplied
+mutiplies->multiplies
 mutiply->multiply
+mutiplying->multiplying
 mutli->multi
 mutli-threaded->multi-threaded
 mutlipart->multipart
 mutliple->multiple
 mutlipler->multiplier, multiple,
 mutliples->multiples
 mutliplication->multiplication
 mutliplicites->multiplicities
+mutliplied->multiplied
 mutliplier->multiplier
 mutlipliers->multipliers
+mutliplies->multiplies
 mutliply->multiply
+mutliplying->multiplying
 mutully->mutually
 mutux->mutex
 mutuxes->mutexes
 mutuxs->mutexes
 muyst->must
 myabe->maybe
 mybe->maybe
@@ -25630,14 +25772,15 @@
 non-negotiote->non-negotiated
 non-negotitable->non-negotiable
 non-negotitaed->non-negotiated
 non-negotitated->non-negotiated
 non-negotited->non-negotiated
 non-negoziable->non-negotiable
 non-negoziated->non-negotiated
+non-persistant->non-persistent
 non-priviliged->non-privileged
 non-referenced-counted->non-reference-counted
 non-replacable->non-replaceable
 non-replacalbe->non-replaceable
 non-reproducable->non-reproducible
 non-seperable->non-separable
 non-trasparent->non-transparent
@@ -25782,14 +25925,15 @@
 notmutch->notmuch
 notning->nothing
 notod->noted
 notofocation->notification
 notofocations->notifications
 notoreous->notorious
 notoreously->notoriously
+notority->notoriety
 notse->notes, note,
 nott->not
 nottaion->notation
 nottaions->notations
 notwhithstanding->notwithstanding
 noveau->nouveau
 novemeber->November
@@ -26072,14 +26216,15 @@
 occurence->occurrence
 occurences->occurrences
 occures->occurs
 occuring->occurring
 occurr->occur
 occurrance->occurrence
 occurrances->occurrences
+occurrencies->occurrences
 occurrencs->occurrences
 occurrs->occurs
 oce->once, one, ore,
 ocilate->oscillate
 ocilated->oscillated
 ocilater->oscillator
 ocilaters->oscillators
@@ -26566,14 +26711,15 @@
 optinally->optionally
 optins->options
 optio->option
 optioanl->optional
 optioin->option
 optioinal->optional
 optioins->options
+optiona->optional
 optionall->optional, optionally,
 optionalliy->optionally
 optionallly->optionally
 optionaly->optionally
 optionel->optional
 optiones->options
 optionial->optional
@@ -27700,14 +27846,16 @@
 peotry->poetry
 pepare->prepare
 peported->reported, purported,
 peprocessor->preprocessor
 per-interpeter->per-interpreter
 perade->parade
 peraphs->perhaps
+percenatge->percentage
+percenatges->percentages
 percentange->percentage
 percentanges->percentages
 percentil->percentile
 percepted->perceived
 percetage->percentage
 percetages->percentages
 percievable->perceivable
@@ -28234,14 +28382,16 @@
 placeemnt->placement
 placeemnts->placements
 placehoder->placeholder
 placeholde->placeholder
 placeholdes->placeholders
 placeholer->placeholder
 placeholers->placeholders
+placehoulder->placeholder
+placehoulders->placeholders
 placematt->placemat, placement,
 placemenet->placement
 placemenets->placements
 placemet->placement, placemat, place mat,
 placemets->placements, placemats, place mats,
 placholder->placeholder
 placholders->placeholders
@@ -28687,14 +28837,15 @@
 possiblec->possible
 possiblely->possibly
 possiblility->possibility
 possiblilty->possibility
 possiblities->possibilities
 possiblity->possibility
 possiblly->possibly
+possiibly->possibly
 possilbe->possible
 possily->possibly
 possition->position
 possitive->positive
 possitives->positives
 possobily->possibly
 possoble->possible
@@ -28834,14 +28985,18 @@
 pre-confured->pre-configured
 pre-congifure->pre-configure
 pre-congifured->pre-configured
 pre-defiend->pre-defined
 pre-defiened->pre-defined
 pre-empt->preempt
 pre-pended->prepended
+pre-poulate->pre-populate
+pre-poulated->pre-populated
+pre-poulates->pre-populates
+pre-poulating->pre-populating
 pre-pre-realease->pre-pre-release
 pre-proces->pre-process
 pre-procesing->pre-processing
 pre-realease->pre-release
 pre-registeres->pre-registers
 preallocationg->preallocating, preallocation,
 prealocate->preallocate
@@ -29672,14 +29827,18 @@
 promprted->prompted
 promps->prompts
 promt->prompt
 promted->prompted, promoted,
 promter->prompter, promoter,
 promters->prompters, promoters,
 promting->prompting, promoting,
+promtp->prompt
+promtped->prompted
+promtping->prompting
+promtps->prompts
 promts->prompts
 pronnounced->pronounced
 pronomial->pronominal
 prononciation->pronunciation
 pronouce->pronounce
 pronouced->pronounced
 pronounched->pronounced
@@ -30343,14 +30502,16 @@
 rapsadies->rhapsodies
 rapsady->rhapsody
 rapsadys->rhapsodies
 rapsberry->raspberry
 rarelly->rarely
 rarified->rarefied
 rasberry->raspberry
+rasbperries->raspberries
+rasbperry->raspberry
 rasie->raise
 rasied->raised
 rasies->raises
 rasiing->raising
 rasing->raising
 rasons->reasons
 raspbery->raspberry
@@ -30623,15 +30784,15 @@
 readble->readable
 readby->read, read by,
 readdrss->readdress
 readdrssed->readdressed
 readdrsses->readdresses
 readdrssing->readdressing
 readeable->readable
-readed->read, readd, readded,
+readed->read, re-add, re-added,
 reademe->README
 readiable->readable
 readibility->readability
 readible->readable
 readig->reading
 readigs->readings
 readius->radius
@@ -31567,14 +31728,18 @@
 relaeses->releases
 relaesing->releasing
 relaged->related
 relaimed->reclaimed
 relaion->relation
 relaive->relative
 relaly->really
+relaod->reload
+relaoded->reloaded
+relaoding->reloading
+relaods->reloads
 relase->release
 relased->released
 relaser->releaser
 relases->releases
 relashionship->relationship
 relashionships->relationships
 relasing->releasing
@@ -32435,14 +32600,16 @@
 requesr->request
 requestd->requested
 requestes->requests, requested,
 requestesd->requested
 requestested->requested
 requestests->requests, requested,
 requestied->requested
+requestor->requester
+requestors->requesters
 requestying->requesting
 requet->request
 requeted->requested
 requeting->requesting
 requets->requests
 requeum->requiem
 requied->required
@@ -32460,14 +32627,15 @@
 requiests->requests
 requird->required
 requireing->requiring
 requiremenet->requirement
 requiremenets->requirements
 requiremnt->requirement
 requirment->requirement
+requirmentes->requirements
 requirments->requirements
 requisit->requisite
 requisits->requisites
 requre->require
 requred->required
 requrement->requirement
 requrements->requirements
@@ -32696,14 +32864,16 @@
 resposiblity->responsibility
 respositories->repositories
 respository->repository
 resposive->responsive
 resposiveness->responsiveness
 resposne->response
 resposnes->responses
+respponse->response
+respponses->responses
 respresent->represent
 respresentation->representation
 respresentational->representational
 respresentations->representations
 respresented->represented
 respresenting->representing
 respresents->represents
@@ -34320,14 +34490,16 @@
 sertificate->certificate
 sertificated->certificated
 sertificates->certificates
 sertification->certification
 servce->service, serve,
 servced->serviced, served,
 servces->services, serves,
+servcie->service
+servcies->services
 servcing->servicing, serving,
 servece->service
 serveced->serviced
 serveces->services
 servecing->servicing
 serveice->service
 serveiced->serviced
@@ -34444,15 +34616,20 @@
 shadoloo->shadaloo
 shal->shall
 shamen->shaman, shamans,
 shandeleer->chandelier
 shandeleers->chandeliers
 shandow->shadow
 shaneal->chenille
+shange->change
+shanged->changed, shanked,
+shanger->changer
+shanges->changes
 shanghi->Shanghai
+shanging->changing, shanking,
 shapshot->snapshot
 shapshots->snapshots
 shapsnot->snapshot
 shapsnots->snapshots
 shapt->shaped, shape,
 shareed->shared
 shareing->sharing
@@ -34641,14 +34818,16 @@
 siffixes->suffixes
 siffixing->suffixing
 sigal->signal, sigil,
 sigaled->signaled
 sigals->signals, sigils,
 siganture->signature
 sigantures->signatures
+sigature->signature
+sigatures->signatures
 sigen->sign
 sighrynge->syringe
 sighrynges->syringes
 sighth->scythe, sight,
 sighths->scythes, sights,
 sigificance->significance
 sigificant->significant
@@ -34913,14 +35092,17 @@
 sinnagog->synagogue
 sinnagogs->synagogues
 sinnic->cynic
 sinnical->cynical
 sinnically->cynically
 sinnicaly->cynically
 sinnics->cynics
+sinoid->sinusoid
+sinoidal->sinusoidal
+sinoids->sinusoids
 sinply->simply
 sinse->sines, since,
 sintac->syntax
 sintacks->syntax
 sintacs->syntax
 sintact->syntax
 sintacts->syntax
@@ -35021,14 +35203,15 @@
 situtaions->situations
 situtation->situation
 situtations->situations
 siutable->suitable
 siute->suite
 sive->sieve, save,
 sived->sieved, saved,
+siver->silver, sliver, diver,
 sives->sieves, saves,
 sivible->visible
 siving->sieving, saving,
 siwtch->switch
 siwtched->switched
 siwtching->switching
 Sixtin->Sistine, Sixteen,
@@ -36112,15 +36295,15 @@
 statemanet->statement
 statememts->statements
 statemen->statement
 statemenet->statement
 statemenets->statements
 statemet->statement
 statemnts->statements
-stati->statuses
+stati->statuses, state,
 staticly->statically
 statictic->statistic
 statictics->statistics
 statisfied->satisfied
 statisfies->satisfies
 statisfy->satisfy
 statisfying->satisfying
@@ -36302,14 +36485,15 @@
 strictist->strictest
 strig->string
 strigification->stringification
 strigifying->stringifying
 striing->string
 striings->strings
 strikely->strikingly
+strin->string, strine, stein,
 stringifed->stringified
 strinsg->strings
 strippen->stripped
 stript->stripped, script,
 stripted->scripted, stripped,
 stripting->scripting, stripping,
 stripts->scripts, strips,
@@ -36431,14 +36615,16 @@
 subcommnad->subcommand
 subconchus->subconscious
 subconsiously->subconsciously
 subcribe->subscribe
 subcribed->subscribed
 subcribes->subscribes
 subcribing->subscribing
+subcription->subscription
+subcriptions->subscriptions
 subdirectoires->subdirectories
 subdirectorys->subdirectories
 subdirecty->subdirectory
 subdivisio->subdivision
 subdivisiond->subdivisioned
 subdoamin->subdomain
 subdoamins->subdomains
@@ -36655,15 +36841,20 @@
 subsysytem->subsystem
 subsysytems->subsystems
 subsytem->subsystem
 subsytems->subsystems
 subtabels->subtables
 subtak->subtask
 subtaks->subtask, subtasks,
+subtance->substance
 subtances->substances
+subtarct->subtract
+subtarcted->subtracted
+subtarcting->subtracting
+subtarcts->subtracts
 subtarger->subtarget, sub-target,
 subtargers->subtargets, sub-targets,
 subterranian->subterranean
 subtile->subtle, subtitle, subfile,
 subtiles->subtitles, subfiles,
 subtitute->substitute
 subtituted->substituted
@@ -36893,14 +37084,18 @@
 summersalt->somersault
 summmaries->summaries
 summmarisation->summarisation
 summmarised->summarised
 summmarization->summarization
 summmarized->summarized
 summmary->summary
+summurize->summarize
+summurized->summarized
+summurizes->summarizes
+summurizing->summarizing
 sumodules->submodules
 sumulate->simulate
 sumulated->simulated
 sumulates->simulates
 sumulation->simulation
 sumulations->simulations
 sundey->Sunday
@@ -36939,14 +37134,18 @@
 suplanted->supplanted
 suplanting->supplanting
 suplants->supplants
 suplementary->supplementary
 suplied->supplied
 suplimented->supplemented
 supllies->supplies
+supoort->support
+supoorted->supported
+supoorting->supporting
+supoorts->supports
 suport->support
 suported->supported
 suporting->supporting
 suports->supports
 suportted->supported
 suposable->supposable
 supose->suppose
@@ -37223,14 +37422,17 @@
 swticher->switcher
 swtichers->switchers
 swtiches->switches
 swtiching->switching
 swtichover->switchover
 swtichs->switches
 sxl->xsl
+sxmbol->symbol
+sxmbolic->symbolic
+sxmbols->symbols
 syantax->syntax
 syas->says
 syatem->system
 syatems->systems
 sybsystem->subsystem
 sybsystems->subsystems
 sychronisation->synchronisation
@@ -38312,14 +38514,15 @@
 toghether->together
 togle->toggle
 togled->toggled
 togling->toggling
 toglle->toggle
 toglled->toggled
 togther->together
+togueter->together
 toi->to, toy,
 tolarable->tolerable
 tolelerance->tolerance
 tolen->token
 tolens->tokens
 toleranz->tolerance
 tolerence->tolerance
@@ -38352,14 +38555,17 @@
 toom->tomb
 tooo->todo, too, tool, took,
 toos->tools
 Toosday->Tuesday
 tootonic->teutonic
 topicaizer->topicalizer
 topologie->topology
+topoplogical->topological
+topoplogies->topologies
+topoplogy->topology
 torerable->tolerable
 toriodal->toroidal
 tork->torque
 torlence->tolerance
 tormenters->tormentors
 tornadoe->tornado
 torpeados->torpedoes
@@ -39127,14 +39333,18 @@
 Tuscon->Tucson
 tusday->Tuesday
 tuseday->Tuesday
 tust->trust
 tution->tuition
 tutoriel->tutorial
 tutoriels->tutorials
+tweek->tweak
+tweeked->tweaked
+tweeking->tweaking
+tweeks->tweaks
 tweleve->twelve
 twelth->twelfth
 two-dimenional->two-dimensional
 two-dimenionsal->two-dimensional
 twodimenional->two-dimensional
 twodimenionsal->two-dimensional
 twon->town
@@ -40454,14 +40664,15 @@
 vacumme->vacuum
 vacummes->vacuums
 vacums->vacuums
 vacuosly->vacuously
 vaelue->value, valued,
 vaelues->values
 vaguaries->vagaries
+vai->via, vie,
 vaiable->variable
 vaiables->variables
 vaiant->variant
 vaiants->variants
 vaid->valid, void,
 vaidate->validate
 vaieties->varieties
@@ -41341,14 +41552,16 @@
 weilded->wielded
 weill->will
 weired->weird
 weitght->weight
 wel->well
 well-reknown->well-renowned, well renown,
 well-reknowned->well-renowned, well renowned,
+wellplate->well plate
+wellplates->well plates
 welp->whelp
 wendesday->Wednesday
 wendsay->Wednesday
 wendsday->Wednesday
 wensday->Wednesday
 wepon->weapon
 wepons->weapons
```

### Comparing `codespell-2.2.4/codespell_lib/data/dictionary_code.txt` & `codespell-2.2.5/codespell_lib/data/dictionary_code.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 dosclose->disclose
 dur->due
 endcode->encode
 errorstring->error string
 exitst->exits, exists,
 falsy->falsely, false,
 files'->file's
+gadjet->gadget
+gadjets->gadgets
 gae->game, Gael, gale,
 hist->heist, his,
 iam->I am, aim,
 iff->if
 ifset->if set
 isenough->is enough
 ith->with
```

### Comparing `codespell-2.2.4/codespell_lib/data/dictionary_en-GB_to_en-US.txt` & `codespell-2.2.5/codespell_lib/data/dictionary_en-GB_to_en-US.txt`

 * *Files identical despite different names*

### Comparing `codespell-2.2.4/codespell_lib/data/dictionary_rare.txt` & `codespell-2.2.5/codespell_lib/data/dictionary_rare.txt`

 * *Files 3% similar despite different names*

```diff
@@ -157,23 +157,26 @@
 predicable->predictable
 preform->perform
 preformed->performed
 preforming->performing
 preforms->performs
 pres->press
 prioritary->priority
+processus->processes, process,
 programed->programmed
 programing->programming
 prosses->process, processes, possess,
 provence->province
 purportive->supportive
 purvue->purview
 ques->quest
 readd->re-add, read,
-readded->read
+readded->re-added, read,
+readding->re-adding, reading,
+readds->re-adds, reads,
 ream->stream
 recuse->recurse
 remainer->remainder
 remainers->remainders
 retuned->returned
 retying->retrying
 revered->reversed
```

### Comparing `codespell-2.2.4/codespell_lib/data/dictionary_usage.txt` & `codespell-2.2.5/codespell_lib/data/dictionary_usage.txt`

 * *Files identical despite different names*

### Comparing `codespell-2.2.4/codespell_lib/data/linux-kernel.exclude` & `codespell-2.2.5/codespell_lib/data/linux-kernel.exclude`

 * *Files identical despite different names*

### Comparing `codespell-2.2.4/codespell_lib/tests/test_basic.py` & `codespell-2.2.5/codespell_lib/tests/test_basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,29 +46,31 @@
         if code == EX_DATAERR:  # have some misspellings
             code = int(stderr.split("\n")[-2])
         elif code == EX_OK and count:
             code = int(stderr.split("\n")[-2])
             assert code == 0
         if std:
             return (code, stdout, stderr)
-        else:
-            return code
+        return code
 
 
 cs = MainWrapper()
 
 
 def run_codespell(
     args: Tuple[Any, ...] = (),
     cwd: Optional[Path] = None,
 ) -> int:
     """Run codespell."""
     args = tuple(str(arg) for arg in args)
     proc = subprocess.run(
-        ["codespell", "--count", *args], cwd=cwd, capture_output=True, encoding="utf-8"
+        ["codespell", "--count", *args],  # noqa: S603, S607
+        cwd=cwd,
+        capture_output=True,
+        encoding="utf-8",
     )
     count = int(proc.stderr.split("\n")[-2])
     return count
 
 
 def test_command(tmp_path: Path) -> None:
     """Test running the codespell executable."""
@@ -92,14 +94,17 @@
     assert code == EX_USAGE, "missing dictionary"
     assert "cannot find dictionary" in stderr
     assert cs.main(fname) == 0, "empty file"
     with fname.open("a") as f:
         f.write("this is a test file\n")
     assert cs.main(fname) == 0, "good"
     with fname.open("a") as f:
+        f.write("var = '\\nDoes not error on newline'\n")
+    assert cs.main(fname) == 0, "with string escape"
+    with fname.open("a") as f:
         f.write("abandonned\n")
     assert cs.main(fname) == 1, "bad"
     with fname.open("a") as f:
         f.write("abandonned\n")
     assert cs.main(fname) == 2, "worse"
     with fname.open("a") as f:
         f.write("tim\ngonna\n")
@@ -137,15 +142,15 @@
 
     (tmp_path / "bad.txt").write_text("abandonned abandonned\n")
     assert cs.main(tmp_path) == 2
     result = cs.main("-q", "16", "-w", tmp_path, count=False, std=True)
     assert isinstance(result, tuple)
     code, stdout, stderr = result
     assert code == 0
-    assert stdout == stderr == ""
+    assert not stdout and not stderr
     assert cs.main(tmp_path) == 0
 
     # empty directory
     (tmp_path / "empty").mkdir()
     assert cs.main(tmp_path) == 0
 
 
@@ -168,15 +173,15 @@
         assert "invalid glob" in stderr
     else:  # Python >= 3.10.5 does not match
         assert code == 1
     # properly escaped glob is valid, and matches glob-like file name
     assert cs.main("--skip", "[[]b-a[]].txt", g) == 0
 
 
-@pytest.mark.skipif(not sys.platform == "linux", reason="Only supported on Linux")
+@pytest.mark.skipif(sys.platform != "linux", reason="Only supported on Linux")
 def test_permission_error(
     tmp_path: Path,
     capsys: pytest.CaptureFixture[str],
 ) -> None:
     """Test permission error handling."""
     fname = tmp_path / "unreadable.txt"
     fname.write_text("abandonned\n")
@@ -262,15 +267,15 @@
     """Test summary functionality."""
     fname = tmp_path / "tmp"
     fname.touch()
     result = cs.main(fname, std=True, count=False)
     assert isinstance(result, tuple)
     code, stdout, stderr = result
     assert code == 0
-    assert stdout == stderr == "", "no output"
+    assert not stdout and not stderr, "no output"
     result = cs.main(fname, "--summary", std=True)
     assert isinstance(result, tuple)
     code, stdout, stderr = result
     assert code == 0
     assert stderr == "0\n"
     assert "SUMMARY" in stdout
     assert len(stdout.split("\n")) == 5
@@ -371,23 +376,33 @@
     assert "iso-8859-1" not in stderr
     # Binary file warning
     fname.write_bytes(b"\x00\x00naiive\x00\x00")
     result = cs.main(fname, std=True, count=False)
     assert isinstance(result, tuple)
     code, stdout, stderr = result
     assert code == 0
-    assert stdout == stderr == ""
+    assert not stdout and not stderr
     result = cs.main("-q", "0", fname, std=True, count=False)
     assert isinstance(result, tuple)
     code, stdout, stderr = result
     assert code == 0
-    assert stdout == ""
+    assert not stdout
     assert "WARNING: Binary file" in stderr
 
 
+def test_unknown_encoding_chardet(
+    tmp_path: Path,
+    capsys: pytest.CaptureFixture[str],
+) -> None:
+    """Test opening a file with unknown encoding using chardet"""
+    fname = tmp_path / "tmp"
+    fname.touch()
+    assert cs.main("--hard-encoding-detection", fname) == 0
+
+
 def test_ignore(
     tmp_path: Path,
     capsys: pytest.CaptureFixture[str],
 ) -> None:
     """Test ignoring of files and directories."""
     goodtxt = tmp_path / "good.txt"
     goodtxt.write_text("this file is okay")
@@ -441,67 +456,101 @@
 
 
 def test_check_hidden(
     tmp_path: Path,
     capsys: pytest.CaptureFixture[str],
 ) -> None:
     """Test ignoring of hidden files."""
-    fname = tmp_path / "test.txt"
     # visible file
-    fname.write_text("abandonned\n")
+    #
+    #         tmp_path
+    #         └── test.txt
+    #
+    fname = tmp_path / "test.txt"
+    fname.write_text("erorr\n")
     assert cs.main(fname) == 1
     assert cs.main(tmp_path) == 1
+
     # hidden file
+    #
+    #         tmp_path
+    #         └── .test.txt
+    #
     hidden_file = tmp_path / ".test.txt"
     fname.rename(hidden_file)
     assert cs.main(hidden_file) == 0
     assert cs.main(tmp_path) == 0
     assert cs.main("--check-hidden", hidden_file) == 1
     assert cs.main("--check-hidden", tmp_path) == 1
+
     # hidden file with typo in name
+    #
+    #         tmp_path
+    #         └── .abandonned.txt
+    #
     typo_file = tmp_path / ".abandonned.txt"
     hidden_file.rename(typo_file)
     assert cs.main(typo_file) == 0
     assert cs.main(tmp_path) == 0
     assert cs.main("--check-hidden", typo_file) == 1
     assert cs.main("--check-hidden", tmp_path) == 1
     assert cs.main("--check-hidden", "--check-filenames", typo_file) == 2
     assert cs.main("--check-hidden", "--check-filenames", tmp_path) == 2
+
     # hidden directory
+    #
+    #         tmp_path
+    #         ├── .abandonned
+    #         │   ├── .abandonned.txt
+    #         │   └── subdir
+    #         │       └── .abandonned.txt
+    #         └── .abandonned.txt
+    #
     assert cs.main(tmp_path) == 0
     assert cs.main("--check-hidden", tmp_path) == 1
     assert cs.main("--check-hidden", "--check-filenames", tmp_path) == 2
-    hidden_dir = tmp_path / ".abandonned"
-    hidden_dir.mkdir()
-    copyfile(typo_file, hidden_dir / typo_file.name)
+    hidden = tmp_path / ".abandonned"
+    hidden.mkdir()
+    copyfile(typo_file, hidden / typo_file.name)
+    subdir = hidden / "subdir"
+    subdir.mkdir()
+    copyfile(typo_file, subdir / typo_file.name)
     assert cs.main(tmp_path) == 0
-    assert cs.main("--check-hidden", tmp_path) == 2
-    assert cs.main("--check-hidden", "--check-filenames", tmp_path) == 5
+    assert cs.main("--check-hidden", tmp_path) == 3
+    assert cs.main("--check-hidden", "--check-filenames", tmp_path) == 8
     # check again with a relative path
     try:
         rel = op.relpath(tmp_path)
     except ValueError:
         # Windows: path is on mount 'C:', start on mount 'D:'
         pass
     else:
         assert cs.main(rel) == 0
-        assert cs.main("--check-hidden", rel) == 2
-        assert cs.main("--check-hidden", "--check-filenames", rel) == 5
+        assert cs.main("--check-hidden", rel) == 3
+        assert cs.main("--check-hidden", "--check-filenames", rel) == 8
+
     # hidden subdirectory
-    assert cs.main(tmp_path) == 0
-    assert cs.main("--check-hidden", tmp_path) == 2
-    assert cs.main("--check-hidden", "--check-filenames", tmp_path) == 5
+    #
+    #         tmp_path
+    #         ├── .abandonned
+    #         │   ├── .abandonned.txt
+    #         │   └── subdir
+    #         │       └── .abandonned.txt
+    #         ├── .abandonned.txt
+    #         └── subdir
+    #             └── .abandonned
+    #                 └── .abandonned.txt
     subdir = tmp_path / "subdir"
     subdir.mkdir()
-    hidden_subdir = subdir / ".abandonned"
-    hidden_subdir.mkdir()
-    copyfile(typo_file, hidden_subdir / typo_file.name)
+    hidden = subdir / ".abandonned"
+    hidden.mkdir()
+    copyfile(typo_file, hidden / typo_file.name)
     assert cs.main(tmp_path) == 0
-    assert cs.main("--check-hidden", tmp_path) == 3
-    assert cs.main("--check-hidden", "--check-filenames", tmp_path) == 8
+    assert cs.main("--check-hidden", tmp_path) == 4
+    assert cs.main("--check-hidden", "--check-filenames", tmp_path) == 11
 
 
 def test_case_handling(
     tmp_path: Path,
     capsys: pytest.CaptureFixture[str],
 ) -> None:
     """Test that capitalized entries get detected properly."""
```

### Comparing `codespell-2.2.4/codespell_lib/tests/test_dictionary.py` & `codespell-2.2.5/codespell_lib/tests/test_dictionary.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 
     for lang in supported_languages:
         spellers[lang] = aspell.Speller("lang", lang)
 except Exception as exp:  # probably ImportError, but maybe also language
     if os.getenv("REQUIRE_ASPELL", "false").lower() == "true":
         raise RuntimeError(
             "Cannot run complete tests without aspell when "
-            "REQUIRE_ASPELL=true. Got error during import:\n%s" % (exp,)
-        )
-    else:
-        warnings.warn(
-            "aspell not found, but not required, skipping aspell tests. Got "
-            "error during import:\n%s" % (exp,)
+            f"REQUIRE_ASPELL=true. Got error during import:\n{exp}"
         )
+    warnings.warn(
+        "aspell not found, but not required, skipping aspell tests. Got "
+        f"error during import:\n{exp}",
+        stacklevel=2,
+    )
 
 global_err_dicts: Dict[str, Dict[str, Any]] = {}
 global_pairs: Set[Tuple[str, str]] = set()
 
 # Filename, should be seen as errors in aspell or not
 _data_dir = op.join(op.dirname(__file__), "..", "data")
 _fnames_in_aspell = [
-    (op.join(_data_dir, "dictionary%s.txt" % d[2]), d[3:5], d[5:7])
+    (op.join(_data_dir, f"dictionary{d[2]}.txt"), d[3:5], d[5:7])
     for d in _builtin_dictionaries
 ]
 fname_params = pytest.mark.parametrize(
     "fname, in_aspell, in_dictionary", _fnames_in_aspell
 )  # noqa: E501
 
 
@@ -61,15 +61,15 @@
         for line in fid:
             err, rep = line.split("->")
             err = err.lower()
             rep = rep.rstrip("\n")
             try:
                 _check_err_rep(err, rep, in_aspell, fname, in_dictionary)
             except AssertionError as exp:
-                errors.append(str(exp).split("\n")[0])
+                errors.append(str(exp).split("\n", maxsplit=1)[0])
     if errors:
         raise AssertionError("\n" + "\n".join(errors))
 
 
 def _check_aspell(
     phrase: str,
     msg: str,
@@ -85,18 +85,15 @@
         for word in phrase.split():
             _check_aspell(word, msg, in_aspell, fname, languages)
         return  # stop normal checking as we've done each word above
     this_in_aspell = any(
         spellers[lang].check(phrase.encode(spellers[lang].ConfigKeys()["encoding"][1]))
         for lang in languages
     )
-    end = "be in aspell dictionaries ({}) for dictionary {}".format(
-        ", ".join(languages),
-        fname,
-    )
+    end = f"be in aspell dictionaries ({', '.join(languages)}) for dictionary {fname}"
     if in_aspell:  # should be an error in aspell
         assert this_in_aspell, f"{msg} should {end}"
     else:  # shouldn't be
         assert not this_in_aspell, f"{msg} should not {end}"
 
 
 whitespace = re.compile(r"\s")
@@ -112,16 +109,16 @@
 def _check_err_rep(
     err: str,
     rep: str,
     in_aspell: Tuple[Optional[bool], Optional[bool]],
     fname: str,
     languages: Tuple[Iterable[str], Iterable[str]],
 ) -> None:
-    assert whitespace.search(err) is None, "error %r has whitespace" % err
-    assert "," not in err, "error %r has a comma" % err
+    assert whitespace.search(err) is None, f"error {err!r} has whitespace"
+    assert "," not in err, f"error {err!r} has a comma"
     assert len(rep) > 0, f"error {err}: correction {rep!r} must be non-empty"
     assert not start_whitespace.match(
         rep
     ), f"error {err}: correction {rep!r} cannot start with whitespace"
     _check_aspell(err, f"error {err!r}", in_aspell[0], fname, languages[0])
     prefix = f"error {err}: correction {rep!r}"
     for regex, msg in [
@@ -139,15 +136,15 @@
         (single_comma, "%s has a single entry but contains a trailing comma"),
     ]:
         assert not regex.search(rep), msg % (prefix,)
     del msg
     if rep.count(","):
         assert rep.endswith(
             ","
-        ), "error %s: multiple corrections must end " 'with trailing ","' % (err,)
+        ), f'error {err}: multiple corrections must end with trailing ","'
     reps = [r.strip() for r in rep.split(",")]
     reps = [r for r in reps if len(r)]
     for r in reps:
         assert err != r.lower(), f"error {err!r} corrects to itself amongst others"
         _check_aspell(
             r,
             f"error {err}: correction {r!r}",
@@ -158,15 +155,15 @@
 
     # aspell dictionary is case sensitive, so pass the original case into there
     # we could ignore the case, but that would miss things like days of the
     # week which we want to be correct
     reps = [r.lower() for r in reps]
     assert len(set(reps)) == len(
         reps
-    ), 'error %s: corrections "%s" are not ' "(lower-case) unique" % (err, rep)
+    ), f'error {err}: corrections "{rep}" are not (lower-case) unique'
 
 
 @pytest.mark.parametrize(
     "err, rep, match",
     [
         ("a a", "bar", "has whitespace"),
         ("a,a", "bar", "has a comma"),
@@ -276,70 +273,61 @@
     """Test that all dictionary entries are valid."""
     this_err_dict = {}
     short_fname = op.basename(fname)
     with open(fname, encoding="utf-8") as fid:
         for line in fid:
             err, rep = line.split("->")
             err = err.lower()
-            assert err not in this_err_dict, "error {!r} already exists in {}".format(
-                err,
-                short_fname,
-            )
+            assert (
+                err not in this_err_dict
+            ), f"error {err!r} already exists in {short_fname}"
             rep = rep.rstrip("\n")
             reps = [r.strip() for r in rep.lower().split(",")]
             reps = [r for r in reps if len(r)]
             this_err_dict[err] = reps
     # 1. check the dict against itself (diagonal)
     for err in this_err_dict:
         for r in this_err_dict[err]:
             assert r not in this_err_dict, (
-                "error %s: correction %s is an error itself in the same "
-                "dictionary file %s" % (err, r, short_fname)
+                f"error {err}: correction {r} is an error itself "
+                f"in the same dictionary file {short_fname}"
             )
     pair = (short_fname, short_fname)
     assert pair not in global_pairs
     global_pairs.add(pair)
     for other_fname, other_err_dict in global_err_dicts.items():
         # error duplication (eventually maybe we should just merge?)
         for err in this_err_dict:
-            assert (
-                err not in other_err_dict
-            ), "error {!r} in dictionary {} already exists in dictionary {}".format(
-                err,
-                short_fname,
-                other_fname,
+            assert err not in other_err_dict, (
+                f"error {err!r} in dictionary {short_fname} "
+                f"already exists in dictionary {other_fname}"
             )
         # 2. check corrections in this dict against other dicts (upper)
         pair = (short_fname, other_fname)
         if pair not in allowed_dups:
             for err in this_err_dict:
-                assert (
-                    err not in other_err_dict
-                ), "error {!r} in dictionary {} already exists in dictionary {}".format(
-                    err,
-                    short_fname,
-                    other_fname,
+                assert err not in other_err_dict, (
+                    f"error {err!r} in dictionary {short_fname} "
+                    f"already exists in dictionary {other_fname}"
                 )
                 for r in this_err_dict[err]:
                     assert r not in other_err_dict, (
-                        "error %s: correction %s from dictionary %s is an "
-                        "error itself in dictionary %s"
-                        % (err, r, short_fname, other_fname)
+                        f"error {err}: correction {r} from dictionary {short_fname} "
+                        f"is an error itself in dictionary {other_fname}"
                     )
         assert pair not in global_pairs
         global_pairs.add(pair)
         # 3. check corrections in other dicts against this dict (lower)
         pair = (other_fname, short_fname)
         if pair not in allowed_dups:
             for err in other_err_dict:
                 for r in other_err_dict[err]:
                     assert r not in this_err_dict, (
-                        "error %s: correction %s from dictionary %s is an "
-                        "error itself in dictionary %s"
-                        % (err, r, other_fname, short_fname)
+                        f"error {err}: correction {r} from dictionary {other_fname} "
+                        f"is an error itself in dictionary {short_fname}"
                     )
         assert pair not in global_pairs
         global_pairs.add(pair)
     global_err_dicts[short_fname] = this_err_dict
 
 
 @pytest.mark.dependency(depends=["dictionary loop"])
```

