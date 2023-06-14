# Comparing `tmp/eparse-0.2.1.tar.gz` & `tmp/eparse-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eparse-0.2.1.tar", last modified: Tue Jun 13 21:00:45 2023, max compression
+gzip compressed data, was "eparse-0.3.0.tar", last modified: Wed Jun 14 15:56:47 2023, max compression
```

## Comparing `eparse-0.2.1.tar` & `eparse-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-13 21:00:45.487618 eparse-0.2.1/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.2.1/AUTHORS.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      323 2023-06-13 20:47:22.000000 eparse-0.2.1/HISTORY.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.2.1/LICENSE
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.2.1/MANIFEST.in
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9649 2023-06-13 21:00:45.487618 eparse-0.2.1/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     8636 2023-06-13 20:56:47.000000 eparse-0.2.1/README.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-13 21:00:45.487618 eparse-0.2.1/docs/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.2.1/docs/Makefile
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.2.1/docs/authors.rst
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.2.1/docs/conf.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.2.1/docs/contributing.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.2.1/docs/history.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.2.1/docs/index.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.2.1/docs/installation.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.2.1/docs/make.bat
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.2.1/docs/readme.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.2.1/docs/usage.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-13 21:00:45.487618 eparse-0.2.1/eparse/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-13 20:59:37.000000 eparse-0.2.1/eparse/__init__.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    11329 2023-06-13 20:47:22.000000 eparse-0.2.1/eparse/cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     4115 2023-06-08 00:46:57.000000 eparse-0.2.1/eparse/core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3241 2023-06-13 20:47:22.000000 eparse-0.2.1/eparse/interfaces.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.2.1/eparse/migrations.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-13 21:00:45.487618 eparse-0.2.1/eparse.egg-info/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9649 2023-06-13 21:00:45.000000 eparse-0.2.1/eparse.egg-info/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      669 2023-06-13 21:00:45.000000 eparse-0.2.1/eparse.egg-info/SOURCES.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-13 21:00:45.000000 eparse-0.2.1/eparse.egg-info/dependency_links.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-13 21:00:45.000000 eparse-0.2.1/eparse.egg-info/entry_points.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-13 21:00:45.000000 eparse-0.2.1/eparse.egg-info/not-zip-safe
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-13 21:00:45.000000 eparse-0.2.1/eparse.egg-info/requires.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-13 21:00:45.000000 eparse-0.2.1/eparse.egg-info/top_level.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      427 2023-06-13 21:00:45.487618 eparse-0.2.1/setup.cfg
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1513 2023-06-13 20:59:47.000000 eparse-0.2.1/setup.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-13 21:00:45.487618 eparse-0.2.1/tests/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.2.1/tests/__init__.py
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.2.1/tests/eparse_unit_test_data.xlsx
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      800 2023-06-13 20:47:22.000000 eparse-0.2.1/tests/test_cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.2.1/tests/test_core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2750 2023-06-13 20:47:22.000000 eparse-0.2.1/tests/test_interfaces.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 15:56:47.130245 eparse-0.3.0/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.3.0/AUTHORS.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      323 2023-06-13 20:47:22.000000 eparse-0.3.0/HISTORY.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.3.0/LICENSE
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.3.0/MANIFEST.in
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10455 2023-06-14 15:56:47.130245 eparse-0.3.0/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9442 2023-06-14 15:19:41.000000 eparse-0.3.0/README.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 15:56:47.130245 eparse-0.3.0/docs/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/Makefile
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/authors.rst
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/conf.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/contributing.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/history.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/index.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/installation.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/make.bat
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/readme.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/usage.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 15:56:47.130245 eparse-0.3.0/eparse/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-14 00:08:57.000000 eparse-0.3.0/eparse/__init__.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10172 2023-06-14 15:53:36.000000 eparse-0.3.0/eparse/cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     4736 2023-06-14 15:27:35.000000 eparse-0.3.0/eparse/core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5572 2023-06-14 15:53:50.000000 eparse-0.3.0/eparse/interfaces.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.3.0/eparse/migrations.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 15:56:47.130245 eparse-0.3.0/eparse.egg-info/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10455 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/SOURCES.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/dependency_links.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/entry_points.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/not-zip-safe
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/requires.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/top_level.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      427 2023-06-14 15:56:47.130245 eparse-0.3.0/setup.cfg
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1513 2023-06-14 00:08:48.000000 eparse-0.3.0/setup.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 15:56:47.130245 eparse-0.3.0/tests/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.3.0/tests/__init__.py
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.3.0/tests/eparse_unit_test_data.xlsx
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      893 2023-06-14 14:09:23.000000 eparse-0.3.0/tests/fixtures.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.3.0/tests/test.db
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1950 2023-06-14 15:53:16.000000 eparse-0.3.0/tests/test_cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.3.0/tests/test_core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.3.0/tests/test_interfaces.py
```

### Comparing `eparse-0.2.1/CONTRIBUTING.rst` & `eparse-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.2.1/LICENSE` & `eparse-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eparse-0.2.1/PKG-INFO` & `eparse-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.2.1
+Version: 0.3.0
 Summary: Excel spreadsheet crawler and table parser for data extraction and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -66,55 +66,57 @@
 Usage
 =====
 eparse is intended to be used from the command-line.  You can view
 supported commands and usage with ``--help`` as follows:
 
 .. code-block:: bash
 
-   $ eparse --help
-   Usage: eparse [OPTIONS] COMMAND [ARGS]...
+    $ eparse --help
+    Usage: eparse [OPTIONS] COMMAND [ARGS]...
 
-   excel parser
+    excel parser
 
-   Options:
-     -i, --input TEXT   input dir(s) or file(s)
-     -o, --output TEXT  output destination
-     -d, --debug        use debug mode
-     -l, --loose        find tables loosely
-     -r, --recursive    find files recursively
-     -t, --truncate     truncate dataframe output
-     -v, --verbose      increase output verbosity
-     --help             Show this message and exit.
-
-   Commands:
-     parse  parse table(s) found in sheet for target(s)
-     query  query eparse output
-     scan   scan for excel files in target
+    Options:
+    -i, --input TEXT   input source
+    -o, --output TEXT  output destination
+    -f, --file TEXT    file(s) or dir(s) to target
+    -d, --debug        use debug mode
+    -l, --loose        find tables loosely
+    -r, --recursive    find files recursively
+    -t, --truncate     truncate dataframe output
+    -v, --verbose      increase output verbosity
+    --help             Show this message and exit.
+
+    Commands:
+    migrate  migrate eparse table
+    parse    parse table(s) found in sheet for target(s)
+    query    query eparse output
+    scan     scan for excel files in target
 
 
 Scan
 ----
 To scan one or more directories for Excel files with descriptive
 information, you can use the ``scan`` command like so:
 
 .. code-block:: bash
 
-    $ eparse -v -i <path_to_files> scan
+    $ eparse -v -f <path_to_files> scan
 
 Increase the verbosity with additional flags, such as ``-vvv``, for
 more descriptive information about the file(s), including sheet names.
 
 
 Parse
 -----
 Excel files can be parsed as follows:
 
 .. code-block:: bash
 
-    $ eparse -v -i <path_to_files> parse
+    $ eparse -v -f <path_to_files> parse
 
 This mode will list each table found in each Excel file to the command-line.
 This mode is useful for initial discovery for parseable data.
 
 eparse uses a simple algorithm for identifying tables.  Table "corners"
 are identified as cells that contain empty cells above and to the right
 (or sheet boundaries).  A densely or sparsely populated 2x2 table must
@@ -136,31 +138,31 @@
 ^^^^^^
 This mode is good for viewing data extracted from Excel files in the
 console.  For example, you could view all tables found in `Sheet1`
 with the following command:
 
 .. code-block:: bash
 
-    $ eparse -i <path_to_files> -o stdout:/// parse -s "Sheet1"
+    $ eparse -f <path_to_files> -o stdout:/// parse -s "Sheet1"
 
 eparse uses `pandas <https://github.com/pandas-dev/pandas>`_
 to handle table data.  You can view larger tables without truncation
 using the ``-t`` flag as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -i <path_to_files> -o stdout:/// parse -s "Sheet1"
+    $ eparse -t -f <path_to_files> -o stdout:/// parse -s "Sheet1"
 
 Data in table format is useful for human viewing, but a serialized
 form is better for data interfacing.  Serialize your output with
 the ``-z`` flag as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -i <path_to_files> -o stdout:/// parse -z
+    $ eparse -t -f <path_to_files> -o stdout:/// parse -z
 
 Each cell of extracted table data is serialized as follows:
 
 * `row` - 0-indexed table row number
 * `column` - 0-indexed table column number
 * `value` - the value of the cell as a ``str``
 * `type` - the implied python ``type`` of the data found
@@ -180,56 +182,62 @@
 
 To create a `SQLite3 <https://github.com/sqlite/sqlite>`_ database
 with your parsed Excel data, use the following command:
 
 .. code-block:: bash
 
     $ mkdir .files
-    $ eparse -i <path_to_files> -o sqlite3:/// parse
+    $ eparse -f <path_to_files> -o sqlite3:/// parse -z
 
 This command will automatically generate a unique database filename
 using the ``uuid`` python package in the ``.files/`` sub-directory
 of the working directory.  You may need to create this directory
 before running this command, as shown.
 
+You can also specify a path and filename of your choosing, like so:
+
+.. code-block:: bash
+
+    $ mkdir .files
+    $ eparse -f <path_to_files> -o sqlite3:///path/filename.db parse -z
+
 
 Query
 -----
 Once you have stored parsed data, you can begin to query it using the
 ``peewee`` ORM.  This can be done with the tool or directly with
 the database.
 
 For example, query distinct column header names from a generated
 ``SQLite3`` database as follows:
 
 .. code-block:: bash
 
-    $ eparse -o stdout:/// query -i from_sqlite3 .files/<db_file> -m get_c_header
+    $ eparse -i sqlite3:///.files/<db_file> -o stdout:/// query -m get_c_header
                    c_header  Total Rows  Data Types  Distinct Values
       0             ABC-col         150           2               76
       1             DEF-col        3981           3               15
       2             GHI-col          20           1                2
       ..                ...         ...         ...              ...
 
 This command will give descriptive information of each distinct c_header
 found, including total rows, unique data types, and distinct values.
 
-You can also get raw un-truncated data as follows, which is the default
-behavior:
+You can also get raw un-truncated data as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -o stdout:/// query -i from_sqlite3 .files/<db_file>
+    $ eparse -t -i sqlite3:///.files/<db_file> -o stdout:/// query
 
 Filtering data on content is easy.  Use the ``--filter`` option as
 follows:
 
 .. code-block:: bash
 
-    $ eparse -t -o stdout:/// query -i from_sqlite3 .files/<db_file> --filter f_name "somefile.xlsx"
+    $ eparse -i sqlite3:///.files/<db_file> -o stdout:/// query --filter f_name "somefile.xlsx"
 
 The above command will filter all rows from an Excel file named
 `somefile.xlsx`. You can use any of the following ``django``-style
 filters:
 
 * ``__eq`` equals X
 * ``__lt`` less than X
@@ -250,15 +258,17 @@
 * ``--filter value__ne 100`` all data with values other than `100`
 
 Queried data can even be stored into a new database for creating
 curated data subsets, as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -o sqlite3:/// query -i from_sqlite3 .files/<db_file>
+    $ eparse -i sqlite3:///.files/<db_file> \
+             -o sqlite3:///.files/<subq_db_file> \
+             query --filter f_name "somefile.xlsx"
 
 Since database files the tool generates when using `sqlite3:///` are
 ``SQLite`` native, you can also use `SQLite` database client tools
 and execute raw SQL like so:
 
 .. code-block:: bash
 
@@ -270,14 +280,30 @@
     CREATE TABLE IF NOT EXISTS "excelparse" ("id" INTEGER NOT NULL PRIMARY KEY, "row" INTEGER NOT NULL, "column" INTEGER NOT NULL, "value" VARCHAR(255) NOT NULL, "type" VARCHAR(255) NOT NULL, "c_header" VARCHAR(255) NOT NULL, "r_header" VARCHAR(255) NOT NULL, "excel_RC" VARCHAR(255) NOT NULL, "name" VARCHAR(255) NOT NULL, "sheet" VARCHAR(255) NOT NULL, "f_name" VARCHAR(255) NOT NULL);
     sqlite> .header on
     sqlite> SELECT * FROM excelparse limit 1;
     id|row|column|value|type|c_header|r_header|excel_RC|name|sheet|f_name
     1|0|0|ABC|<class 'str'>|SomeCol|SomeRow|B2|MyTable|Sheet1|myfile.xlsm
 
 
+Migrate
+-------
+eparse wouldn't be a solid tool without the ability to migrate your
+eparse databases for future code changes.  You can apply migrations
+that ship with future versions of eparse as follows:
+
+.. code-block:: bash
+
+    $ eparse -i sqlite3:///.files/<db_file> migrate -m <migration>
+    applied <migration>
+
+It is up to you to determine the migrations you need based on the
+eparse version you are upgrading from and to. Migrations can be
+found in `eparse/migrations.py <eparse/migrations.py>`_
+
+
 Contributing
 ============
 As an open-source project, contributions are always welcome. Please see `Contributing <CONTRIBUTING.rst>`_ for more information.
 
 
 License
 =======
```

### Comparing `eparse-0.2.1/README.rst` & `eparse-0.3.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -46,55 +46,57 @@
 Usage
 =====
 eparse is intended to be used from the command-line.  You can view
 supported commands and usage with ``--help`` as follows:
 
 .. code-block:: bash
 
-   $ eparse --help
-   Usage: eparse [OPTIONS] COMMAND [ARGS]...
+    $ eparse --help
+    Usage: eparse [OPTIONS] COMMAND [ARGS]...
 
-   excel parser
+    excel parser
 
-   Options:
-     -i, --input TEXT   input dir(s) or file(s)
-     -o, --output TEXT  output destination
-     -d, --debug        use debug mode
-     -l, --loose        find tables loosely
-     -r, --recursive    find files recursively
-     -t, --truncate     truncate dataframe output
-     -v, --verbose      increase output verbosity
-     --help             Show this message and exit.
-
-   Commands:
-     parse  parse table(s) found in sheet for target(s)
-     query  query eparse output
-     scan   scan for excel files in target
+    Options:
+    -i, --input TEXT   input source
+    -o, --output TEXT  output destination
+    -f, --file TEXT    file(s) or dir(s) to target
+    -d, --debug        use debug mode
+    -l, --loose        find tables loosely
+    -r, --recursive    find files recursively
+    -t, --truncate     truncate dataframe output
+    -v, --verbose      increase output verbosity
+    --help             Show this message and exit.
+
+    Commands:
+    migrate  migrate eparse table
+    parse    parse table(s) found in sheet for target(s)
+    query    query eparse output
+    scan     scan for excel files in target
 
 
 Scan
 ----
 To scan one or more directories for Excel files with descriptive
 information, you can use the ``scan`` command like so:
 
 .. code-block:: bash
 
-    $ eparse -v -i <path_to_files> scan
+    $ eparse -v -f <path_to_files> scan
 
 Increase the verbosity with additional flags, such as ``-vvv``, for
 more descriptive information about the file(s), including sheet names.
 
 
 Parse
 -----
 Excel files can be parsed as follows:
 
 .. code-block:: bash
 
-    $ eparse -v -i <path_to_files> parse
+    $ eparse -v -f <path_to_files> parse
 
 This mode will list each table found in each Excel file to the command-line.
 This mode is useful for initial discovery for parseable data.
 
 eparse uses a simple algorithm for identifying tables.  Table "corners"
 are identified as cells that contain empty cells above and to the right
 (or sheet boundaries).  A densely or sparsely populated 2x2 table must
@@ -116,31 +118,31 @@
 ^^^^^^
 This mode is good for viewing data extracted from Excel files in the
 console.  For example, you could view all tables found in `Sheet1`
 with the following command:
 
 .. code-block:: bash
 
-    $ eparse -i <path_to_files> -o stdout:/// parse -s "Sheet1"
+    $ eparse -f <path_to_files> -o stdout:/// parse -s "Sheet1"
 
 eparse uses `pandas <https://github.com/pandas-dev/pandas>`_
 to handle table data.  You can view larger tables without truncation
 using the ``-t`` flag as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -i <path_to_files> -o stdout:/// parse -s "Sheet1"
+    $ eparse -t -f <path_to_files> -o stdout:/// parse -s "Sheet1"
 
 Data in table format is useful for human viewing, but a serialized
 form is better for data interfacing.  Serialize your output with
 the ``-z`` flag as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -i <path_to_files> -o stdout:/// parse -z
+    $ eparse -t -f <path_to_files> -o stdout:/// parse -z
 
 Each cell of extracted table data is serialized as follows:
 
 * `row` - 0-indexed table row number
 * `column` - 0-indexed table column number
 * `value` - the value of the cell as a ``str``
 * `type` - the implied python ``type`` of the data found
@@ -160,56 +162,62 @@
 
 To create a `SQLite3 <https://github.com/sqlite/sqlite>`_ database
 with your parsed Excel data, use the following command:
 
 .. code-block:: bash
 
     $ mkdir .files
-    $ eparse -i <path_to_files> -o sqlite3:/// parse
+    $ eparse -f <path_to_files> -o sqlite3:/// parse -z
 
 This command will automatically generate a unique database filename
 using the ``uuid`` python package in the ``.files/`` sub-directory
 of the working directory.  You may need to create this directory
 before running this command, as shown.
 
+You can also specify a path and filename of your choosing, like so:
+
+.. code-block:: bash
+
+    $ mkdir .files
+    $ eparse -f <path_to_files> -o sqlite3:///path/filename.db parse -z
+
 
 Query
 -----
 Once you have stored parsed data, you can begin to query it using the
 ``peewee`` ORM.  This can be done with the tool or directly with
 the database.
 
 For example, query distinct column header names from a generated
 ``SQLite3`` database as follows:
 
 .. code-block:: bash
 
-    $ eparse -o stdout:/// query -i from_sqlite3 .files/<db_file> -m get_c_header
+    $ eparse -i sqlite3:///.files/<db_file> -o stdout:/// query -m get_c_header
                    c_header  Total Rows  Data Types  Distinct Values
       0             ABC-col         150           2               76
       1             DEF-col        3981           3               15
       2             GHI-col          20           1                2
       ..                ...         ...         ...              ...
 
 This command will give descriptive information of each distinct c_header
 found, including total rows, unique data types, and distinct values.
 
-You can also get raw un-truncated data as follows, which is the default
-behavior:
+You can also get raw un-truncated data as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -o stdout:/// query -i from_sqlite3 .files/<db_file>
+    $ eparse -t -i sqlite3:///.files/<db_file> -o stdout:/// query
 
 Filtering data on content is easy.  Use the ``--filter`` option as
 follows:
 
 .. code-block:: bash
 
-    $ eparse -t -o stdout:/// query -i from_sqlite3 .files/<db_file> --filter f_name "somefile.xlsx"
+    $ eparse -i sqlite3:///.files/<db_file> -o stdout:/// query --filter f_name "somefile.xlsx"
 
 The above command will filter all rows from an Excel file named
 `somefile.xlsx`. You can use any of the following ``django``-style
 filters:
 
 * ``__eq`` equals X
 * ``__lt`` less than X
@@ -230,15 +238,17 @@
 * ``--filter value__ne 100`` all data with values other than `100`
 
 Queried data can even be stored into a new database for creating
 curated data subsets, as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -o sqlite3:/// query -i from_sqlite3 .files/<db_file>
+    $ eparse -i sqlite3:///.files/<db_file> \
+             -o sqlite3:///.files/<subq_db_file> \
+             query --filter f_name "somefile.xlsx"
 
 Since database files the tool generates when using `sqlite3:///` are
 ``SQLite`` native, you can also use `SQLite` database client tools
 and execute raw SQL like so:
 
 .. code-block:: bash
 
@@ -250,14 +260,30 @@
     CREATE TABLE IF NOT EXISTS "excelparse" ("id" INTEGER NOT NULL PRIMARY KEY, "row" INTEGER NOT NULL, "column" INTEGER NOT NULL, "value" VARCHAR(255) NOT NULL, "type" VARCHAR(255) NOT NULL, "c_header" VARCHAR(255) NOT NULL, "r_header" VARCHAR(255) NOT NULL, "excel_RC" VARCHAR(255) NOT NULL, "name" VARCHAR(255) NOT NULL, "sheet" VARCHAR(255) NOT NULL, "f_name" VARCHAR(255) NOT NULL);
     sqlite> .header on
     sqlite> SELECT * FROM excelparse limit 1;
     id|row|column|value|type|c_header|r_header|excel_RC|name|sheet|f_name
     1|0|0|ABC|<class 'str'>|SomeCol|SomeRow|B2|MyTable|Sheet1|myfile.xlsm
 
 
+Migrate
+-------
+eparse wouldn't be a solid tool without the ability to migrate your
+eparse databases for future code changes.  You can apply migrations
+that ship with future versions of eparse as follows:
+
+.. code-block:: bash
+
+    $ eparse -i sqlite3:///.files/<db_file> migrate -m <migration>
+    applied <migration>
+
+It is up to you to determine the migrations you need based on the
+eparse version you are upgrading from and to. Migrations can be
+found in `eparse/migrations.py <eparse/migrations.py>`_
+
+
 Contributing
 ============
 As an open-source project, contributions are always welcome. Please see `Contributing <CONTRIBUTING.rst>`_ for more information.
 
 
 License
 =======
```

### Comparing `eparse-0.2.1/docs/Makefile` & `eparse-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eparse-0.2.1/docs/conf.py` & `eparse-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eparse-0.2.1/docs/installation.rst` & `eparse-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.2.1/docs/make.bat` & `eparse-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eparse-0.2.1/eparse/cli.py` & `eparse-0.3.0/eparse/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 
 '''
 excel parser cli module
 '''
 
 import click
 from collections.abc import Iterable
-import importlib
 from pathlib import Path
 from pprint import PrettyPrinter
-import re
 import sys
 
 import pandas as pd
 
-from .core import df_find_tables, df_parse_table, df_serialize_table
-from .interfaces import parse_uri
+from .core import (
+    df_find_tables,
+    df_parse_table,
+    df_normalize_data,
+    df_serialize_table,
+)
+from .interfaces import ExcelParse, i_factory
 
 
 def handle(e, exceptions=None, msg=None, debug=False, exit=True):
     '''
     handle exceptions based on settings
     '''
 
@@ -39,24 +42,30 @@
 
 
 @click.group()
 @click.pass_context
 @click.option(
     '--input', '-i',
     type=str,
-    multiple=True,
-    help='input dir(s) or file(s)',
+    default='null:///',
+    help='input source',
 )
 @click.option(
     '--output', '-o',
     type=str,
     default='null:///',
     help='output destination',
 )
 @click.option(
+    '--file', '-f',
+    type=str,
+    multiple=True,
+    help='file(s) or dir(s) to target',
+)
+@click.option(
     '--debug', '-d',
     is_flag=True,
     default=False,
     help='use debug mode',
 )
 @click.option(
     '--loose', '-l',
@@ -81,56 +90,55 @@
     count=True,
     help='increase output verbosity',
 )
 def main(
     ctx,
     input,
     output,
+    file,
     debug,
     loose,
     recursive,
     truncate,
     verbose,
 ):
     '''
     excel parser
     '''
 
     ctx.obj['input'] = input
     ctx.obj['output'] = output
+    ctx.obj['file'] = file
     ctx.obj['debug'] = debug
     ctx.obj['loose'] = loose
     ctx.obj['recursive'] = recursive
     ctx.obj['truncate'] = truncate
     ctx.obj['verbose'] = verbose
 
     files = []
 
     # get target file(s)
-    for i in input:
+    for i in file:
         if Path(i).is_dir():
             g = '**/*' if recursive else '*'
             files += Path(i).glob(g)
         elif Path(i).is_file():
             files.append(Path(i))
 
     ctx.obj['files'] = files
 
     if ctx.obj['verbose']:
         print(f'found {len(files)} files')
 
-    # set output function
-    try:
-        m = importlib.import_module('eparse.interfaces')
-        ctx.obj['output_kwargs'] = parse_uri(output)
-        ctx.obj['output_fcn'] = getattr(
-            m, f'to_{ctx.obj["output_kwargs"]["endpoint"]}'
-        )
-    except Exception as e:
-        handle(e, AttributeError, f'there is no {output}', debug)
+    # get input and output objects
+    for t in ('input', 'output'):
+        try:
+            ctx.obj[f'{t}_obj'] = i_factory(ctx.obj[t], ExcelParse)
+        except ValueError as e:
+            handle(e, msg=f'{t} error - {e}', debug=debug)
 
     # set truncate option
     if not truncate:
         # pd.set_option('display.max_colwidth', None)
         pd.set_option('display.max_rows', None)
 
 
@@ -301,145 +309,105 @@
                         )
 
                     if ctx.obj['debug']:
                         PrettyPrinter().pprint(output)
 
                     # output table
                     try:
-                        ctx.obj['output_fcn'](output, ctx)
+                        ctx.obj['output_obj'].output(output, ctx)
                     except Exception as e:
-                        msg = f'output {ctx.obj["output"]} failed - {e}'
+                        msg = f'output to {ctx.obj["output"]} failed - {e}'
                         handle(e, msg=msg, debug=ctx.obj['debug'], exit=False)
                         continue
 
 
 @main.command()
 @click.pass_context
 @click.option(
-    '--input', '-i',
-    required=True,
-    type=str,
-    nargs=2,
-    help='eparse data source',
-)
-@click.option(
     '--filter', '-f',
     type=str,
     nargs=2,
     multiple=True,
     help='django-style filter(s) to apply to base queryset',
 )
 @click.option(
     '--method', '-m',
     type=str,
     default='get_queryset',
     help='method to call on eparse model',
 )
-def query(ctx, input, filter, method):
+@click.option(
+    '--serialize', '-z',
+    is_flag=True,
+    default=False,
+    help='serialize query output',
+)
+def query(ctx, filter, method, serialize):
     '''
     query eparse output
     '''
 
-    ctx.obj['input_fcn'], ctx.obj['input_src'] = input
     ctx.obj['filters'] = {k: v for k, v in filter}
     ctx.obj['method'] = method
 
-    # set input function
-    try:
-        m = importlib.import_module('eparse.interfaces')
-        ctx.obj['input_fcn'] = getattr(m, ctx.obj['input_fcn'])
-    except AttributeError as e:
-        msg = f'input error - there is no {ctx.obj["input_fcn"]}'
-        handle(e, AttributeError, msg, ctx.obj['debug'])
-
     if ctx.obj['debug']:
         PrettyPrinter().pprint(ctx.obj)
 
-    # get model from input factory
-    model = ctx.obj['input_fcn'](ctx.obj['input_src'])
-
-    # call model method and output results
-    m = getattr(model, method, None)
-    kwargs = ctx.obj['filters']
-
-    # if no explicit method is available, try get_column
-    if m is None:
-        patt = r'^(?:get_)?(.*)$'
-        m = model.get_column
-        kwargs['column'] = re.match(patt, method)[1]
-
-    # call query method
+    # input data
     try:
-        data = m(**kwargs)
+        data = ctx.obj['input_obj'].input(method, **ctx.obj['filters'])
     except Exception as e:
-        handle(e, msg=f'an error occurred: {e}', debug=ctx.obj['debug'])
+        msg = f'input from {ctx.obj["input"]} failed with {e}'
+        handle(e, msg=msg, debug=ctx.obj['debug'])
+
+    if serialize:
+        try:
+            data = [
+                df_normalize_data(d)
+                for d in data.to_dict('records')
+            ]
+        except Exception as e:
+            msg = 'serialization error (some methods can\'t be serialized)'
+            handle(e, msg=f'{msg} - {e}', debug=ctx.obj['debug'])
 
     # output data
     try:
-        ctx.obj['output_fcn'](data, ctx)
+        ctx.obj['output_obj'].output(data, ctx)
     except Exception as e:
-        msg = f'output {ctx.obj["output"]} failed with {e}'
+        msg = f'output to {ctx.obj["output"]} failed with {e}'
         handle(e, msg=msg, debug=ctx.obj['debug'])
 
 
 @main.command()
 @click.pass_context
 @click.option(
-    '--input', '-i',
-    required=True,
-    type=str,
-    nargs=2,
-    help='eparse data source',
-)
-@click.option(
     '--migration', '-m',
     required=True,
     type=str,
     multiple=True,
     help='database migration(s) to apply',
 )
-def migrate(ctx, input, migration):
+def migrate(ctx, migration):
     '''
     migrate eparse table
     '''
 
-    ctx.obj['input_fcn'], ctx.obj['input_src'] = input
     ctx.obj['migration'] = migration
 
-    # set input function
-    try:
-        m = importlib.import_module('eparse.interfaces')
-        ctx.obj['input_fcn'] = getattr(m, ctx.obj['input_fcn'])
-    except AttributeError as e:
-        msg = f'input error - there is no {ctx.obj["input_fcn"]}'
-        handle(e, msg=msg, debug=ctx.obj['debug'])
-
     if ctx.obj['debug']:
         PrettyPrinter().pprint(ctx.obj)
 
-    # get model from input factory
-    model = ctx.obj['input_fcn'](ctx.obj['input_src'])
-
     # apply migrations
     for _migration in ctx.obj['migration']:
         try:
-            m = importlib.import_module('eparse.migrations')
-            migration_fcn = getattr(m, _migration)
-        except AttributeError as e:
-            msg = f'migration error - there is no {_migration}'
-            handle(e, AttributeError, msg, ctx.obj['debug'])
-
-        # call migration function on model
-        try:
-            migration_fcn(model)
+            ctx.obj['input_obj'].migrate(_migration)
+            print(f'applied {_migration}')
         except Exception as e:
             handle(e, msg=f'migration error - {e}', debug=ctx.obj['debug'])
 
-        print(f'Applied {_migration}')
-
 
 def entry_point():
     '''
     required to make setuptools and click play nicely (context object)
     '''
 
     return sys.exit(main(obj={}))
```

### Comparing `eparse-0.2.1/eparse/core.py` & `eparse-0.3.0/eparse/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -129,14 +129,39 @@
         if pd.isna(df.at[r, col]):
             break
         _c += 1
 
     return df.iloc[r:_r, c:_c]
 
 
+def df_normalize_data(data: Dict) -> Dict:
+    '''
+    normalize table data
+    '''
+
+    result = {}
+    ints = ('row', 'column')
+    strs = ('value', 'type', 'c_header', 'r_header', 'excel_RC',
+            'name', 'sheet', 'f_name')
+
+    for k in ints:
+        if k in data:
+            result[k] = int(data[k])
+
+    for k in strs:
+        if k in data:
+            result[k] = str(data[k])
+
+    if 'timestamp' in data:
+        if isinstance(data['timestamp'], pd.Timestamp):
+            result['timestamp'] = data['timestamp'].to_pydatetime()
+
+    return result
+
+
 def df_serialize_table(
         df: pd.DataFrame,
         **other_data,
         ) -> List[Dict]:
     '''
     serialize table into a list of dicts with meta data
     '''
@@ -146,19 +171,21 @@
 
     result = []
 
     for r in range(df.shape[0]):
         for c in range(df.shape[1]):
             _r = df.index[r]  # excel df row
             _c = df.columns[c]  # excel df col
-            result.append({
-                'row': int(r),
-                'column': int(c),
-                'value': str(df.iloc[r, c]),
-                'type': str(type(df.iloc[r, c])),
-                'c_header': str(column_header.iloc[c]),
-                'r_header': str(row_header.iloc[r]),
-                'excel_RC': f'{get_column_letter(_c+1)}{_r+1}',
-                **other_data,
-            })
+            result.append(
+                df_normalize_data({
+                    'row': r,
+                    'column': c,
+                    'value': df.iloc[r, c],
+                    'type': type(df.iloc[r, c]),
+                    'c_header': column_header.iloc[c],
+                    'r_header': row_header.iloc[r],
+                    'excel_RC': f'{get_column_letter(_c+1)}{_r+1}',
+                    **other_data,
+                })
+            )
 
     return result
```

### Comparing `eparse-0.2.1/eparse/migrations.py` & `eparse-0.3.0/eparse/migrations.py`

 * *Files identical despite different names*

### Comparing `eparse-0.2.1/eparse.egg-info/PKG-INFO` & `eparse-0.3.0/eparse.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.2.1
+Version: 0.3.0
 Summary: Excel spreadsheet crawler and table parser for data extraction and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -66,55 +66,57 @@
 Usage
 =====
 eparse is intended to be used from the command-line.  You can view
 supported commands and usage with ``--help`` as follows:
 
 .. code-block:: bash
 
-   $ eparse --help
-   Usage: eparse [OPTIONS] COMMAND [ARGS]...
+    $ eparse --help
+    Usage: eparse [OPTIONS] COMMAND [ARGS]...
 
-   excel parser
+    excel parser
 
-   Options:
-     -i, --input TEXT   input dir(s) or file(s)
-     -o, --output TEXT  output destination
-     -d, --debug        use debug mode
-     -l, --loose        find tables loosely
-     -r, --recursive    find files recursively
-     -t, --truncate     truncate dataframe output
-     -v, --verbose      increase output verbosity
-     --help             Show this message and exit.
-
-   Commands:
-     parse  parse table(s) found in sheet for target(s)
-     query  query eparse output
-     scan   scan for excel files in target
+    Options:
+    -i, --input TEXT   input source
+    -o, --output TEXT  output destination
+    -f, --file TEXT    file(s) or dir(s) to target
+    -d, --debug        use debug mode
+    -l, --loose        find tables loosely
+    -r, --recursive    find files recursively
+    -t, --truncate     truncate dataframe output
+    -v, --verbose      increase output verbosity
+    --help             Show this message and exit.
+
+    Commands:
+    migrate  migrate eparse table
+    parse    parse table(s) found in sheet for target(s)
+    query    query eparse output
+    scan     scan for excel files in target
 
 
 Scan
 ----
 To scan one or more directories for Excel files with descriptive
 information, you can use the ``scan`` command like so:
 
 .. code-block:: bash
 
-    $ eparse -v -i <path_to_files> scan
+    $ eparse -v -f <path_to_files> scan
 
 Increase the verbosity with additional flags, such as ``-vvv``, for
 more descriptive information about the file(s), including sheet names.
 
 
 Parse
 -----
 Excel files can be parsed as follows:
 
 .. code-block:: bash
 
-    $ eparse -v -i <path_to_files> parse
+    $ eparse -v -f <path_to_files> parse
 
 This mode will list each table found in each Excel file to the command-line.
 This mode is useful for initial discovery for parseable data.
 
 eparse uses a simple algorithm for identifying tables.  Table "corners"
 are identified as cells that contain empty cells above and to the right
 (or sheet boundaries).  A densely or sparsely populated 2x2 table must
@@ -136,31 +138,31 @@
 ^^^^^^
 This mode is good for viewing data extracted from Excel files in the
 console.  For example, you could view all tables found in `Sheet1`
 with the following command:
 
 .. code-block:: bash
 
-    $ eparse -i <path_to_files> -o stdout:/// parse -s "Sheet1"
+    $ eparse -f <path_to_files> -o stdout:/// parse -s "Sheet1"
 
 eparse uses `pandas <https://github.com/pandas-dev/pandas>`_
 to handle table data.  You can view larger tables without truncation
 using the ``-t`` flag as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -i <path_to_files> -o stdout:/// parse -s "Sheet1"
+    $ eparse -t -f <path_to_files> -o stdout:/// parse -s "Sheet1"
 
 Data in table format is useful for human viewing, but a serialized
 form is better for data interfacing.  Serialize your output with
 the ``-z`` flag as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -i <path_to_files> -o stdout:/// parse -z
+    $ eparse -t -f <path_to_files> -o stdout:/// parse -z
 
 Each cell of extracted table data is serialized as follows:
 
 * `row` - 0-indexed table row number
 * `column` - 0-indexed table column number
 * `value` - the value of the cell as a ``str``
 * `type` - the implied python ``type`` of the data found
@@ -180,56 +182,62 @@
 
 To create a `SQLite3 <https://github.com/sqlite/sqlite>`_ database
 with your parsed Excel data, use the following command:
 
 .. code-block:: bash
 
     $ mkdir .files
-    $ eparse -i <path_to_files> -o sqlite3:/// parse
+    $ eparse -f <path_to_files> -o sqlite3:/// parse -z
 
 This command will automatically generate a unique database filename
 using the ``uuid`` python package in the ``.files/`` sub-directory
 of the working directory.  You may need to create this directory
 before running this command, as shown.
 
+You can also specify a path and filename of your choosing, like so:
+
+.. code-block:: bash
+
+    $ mkdir .files
+    $ eparse -f <path_to_files> -o sqlite3:///path/filename.db parse -z
+
 
 Query
 -----
 Once you have stored parsed data, you can begin to query it using the
 ``peewee`` ORM.  This can be done with the tool or directly with
 the database.
 
 For example, query distinct column header names from a generated
 ``SQLite3`` database as follows:
 
 .. code-block:: bash
 
-    $ eparse -o stdout:/// query -i from_sqlite3 .files/<db_file> -m get_c_header
+    $ eparse -i sqlite3:///.files/<db_file> -o stdout:/// query -m get_c_header
                    c_header  Total Rows  Data Types  Distinct Values
       0             ABC-col         150           2               76
       1             DEF-col        3981           3               15
       2             GHI-col          20           1                2
       ..                ...         ...         ...              ...
 
 This command will give descriptive information of each distinct c_header
 found, including total rows, unique data types, and distinct values.
 
-You can also get raw un-truncated data as follows, which is the default
-behavior:
+You can also get raw un-truncated data as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -o stdout:/// query -i from_sqlite3 .files/<db_file>
+    $ eparse -t -i sqlite3:///.files/<db_file> -o stdout:/// query
 
 Filtering data on content is easy.  Use the ``--filter`` option as
 follows:
 
 .. code-block:: bash
 
-    $ eparse -t -o stdout:/// query -i from_sqlite3 .files/<db_file> --filter f_name "somefile.xlsx"
+    $ eparse -i sqlite3:///.files/<db_file> -o stdout:/// query --filter f_name "somefile.xlsx"
 
 The above command will filter all rows from an Excel file named
 `somefile.xlsx`. You can use any of the following ``django``-style
 filters:
 
 * ``__eq`` equals X
 * ``__lt`` less than X
@@ -250,15 +258,17 @@
 * ``--filter value__ne 100`` all data with values other than `100`
 
 Queried data can even be stored into a new database for creating
 curated data subsets, as follows:
 
 .. code-block:: bash
 
-    $ eparse -t -o sqlite3:/// query -i from_sqlite3 .files/<db_file>
+    $ eparse -i sqlite3:///.files/<db_file> \
+             -o sqlite3:///.files/<subq_db_file> \
+             query --filter f_name "somefile.xlsx"
 
 Since database files the tool generates when using `sqlite3:///` are
 ``SQLite`` native, you can also use `SQLite` database client tools
 and execute raw SQL like so:
 
 .. code-block:: bash
 
@@ -270,14 +280,30 @@
     CREATE TABLE IF NOT EXISTS "excelparse" ("id" INTEGER NOT NULL PRIMARY KEY, "row" INTEGER NOT NULL, "column" INTEGER NOT NULL, "value" VARCHAR(255) NOT NULL, "type" VARCHAR(255) NOT NULL, "c_header" VARCHAR(255) NOT NULL, "r_header" VARCHAR(255) NOT NULL, "excel_RC" VARCHAR(255) NOT NULL, "name" VARCHAR(255) NOT NULL, "sheet" VARCHAR(255) NOT NULL, "f_name" VARCHAR(255) NOT NULL);
     sqlite> .header on
     sqlite> SELECT * FROM excelparse limit 1;
     id|row|column|value|type|c_header|r_header|excel_RC|name|sheet|f_name
     1|0|0|ABC|<class 'str'>|SomeCol|SomeRow|B2|MyTable|Sheet1|myfile.xlsm
 
 
+Migrate
+-------
+eparse wouldn't be a solid tool without the ability to migrate your
+eparse databases for future code changes.  You can apply migrations
+that ship with future versions of eparse as follows:
+
+.. code-block:: bash
+
+    $ eparse -i sqlite3:///.files/<db_file> migrate -m <migration>
+    applied <migration>
+
+It is up to you to determine the migrations you need based on the
+eparse version you are upgrading from and to. Migrations can be
+found in `eparse/migrations.py <eparse/migrations.py>`_
+
+
 Contributing
 ============
 As an open-source project, contributions are always welcome. Please see `Contributing <CONTRIBUTING.rst>`_ for more information.
 
 
 License
 =======
```

### Comparing `eparse-0.2.1/eparse.egg-info/SOURCES.txt` & `eparse-0.3.0/eparse.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -26,10 +26,12 @@
 eparse.egg-info/dependency_links.txt
 eparse.egg-info/entry_points.txt
 eparse.egg-info/not-zip-safe
 eparse.egg-info/requires.txt
 eparse.egg-info/top_level.txt
 tests/__init__.py
 tests/eparse_unit_test_data.xlsx
+tests/fixtures.py
+tests/test.db
 tests/test_cli.py
 tests/test_core.py
 tests/test_interfaces.py
```

### Comparing `eparse-0.2.1/setup.py` & `eparse-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,10 +54,10 @@
     include_package_data=True,
     keywords='eparse',
     name='eparse',
     packages=find_packages(include=['eparse', 'eparse.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChrisPappalardo/eparse',
-    version='0.2.1',
+    version='0.3.0',
     zip_safe=False,
 )
```

### Comparing `eparse-0.2.1/tests/eparse_unit_test_data.xlsx` & `eparse-0.3.0/tests/eparse_unit_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `eparse-0.2.1/tests/test_core.py` & `eparse-0.3.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.2.1/tests/test_interfaces.py` & `eparse-0.3.0/tests/test_interfaces.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,118 +1,86 @@
-#!/usr/bin/env python
+# -*- coding: utf-8 -*-
 
 '''
 unit tests for eparse interfaces
 '''
 
-from peewee import SqliteDatabase
 import pytest
 
+import pandas as pd
+from peewee import ModelBase, SqliteDatabase
+
+from .fixtures import ctx, data, sqlite3_db
 from eparse.interfaces import (
     DATABASE,
-    SQLITE3_DATABASE,
     ExcelParse,
-    parse_uri,
-    to_null,
-    to_stdout,
+    BaseInterface,
+    NullInterface,
+    StdoutInterface,
+    Sqlite3Interface,
+    i_factory,
 )
 
 
-@pytest.fixture
-def ctx():
-    '''
-    click style ctx object fixture
-    '''
-
-    class Obj():
-        obj = {}
-
-    return Obj()
-
-
-@pytest.fixture
-def data():
-    '''
-    serialized data fixture
-    '''
-
-    return dict(
-        row=0,
-        column=0,
-        value='test',
-        type='test',
-        c_header='test',
-        r_header='test',
-        excel_RC='A1',
-        name='test',
-        sheet='test',
-        f_name='test',
-    )
-
-
-@pytest.fixture
-def sqlite3_db(data):
-    '''
-    sqlite3 in-memory database fixture
-    '''
-
-    global DATABASE
-    global SQLITE3_DATABASE
-
-    SQLITE3_DATABASE = ':memory:'
-    DATABASE.initialize(SqliteDatabase(SQLITE3_DATABASE))
-    DATABASE.connect()
-    DATABASE.create_tables([ExcelParse])
-
-    ExcelParse.create(**data)
-
-    return ExcelParse._meta.database.obj
-
-
 def test_sqlite3_db(sqlite3_db):
     assert isinstance(sqlite3_db, SqliteDatabase)
-    assert sqlite3_db.table_exists('excelparse')
+    assert DATABASE.table_exists('excelparse')
     assert len(ExcelParse.select()) == 1
 
 
 def test_ExcelParse_model(sqlite3_db):
     assert ExcelParse.get_queryset().shape == (1, 12)
     assert ExcelParse.get_column('c_header').shape == (1, 4)
 
 
-def test_to_null():
-    assert to_null() == None
-
-
-def test_to_stdout():
-    assert to_stdout({'foo'}) == None
+def test_null_interface():
+    obj = i_factory('null:///')
+    assert isinstance(obj, NullInterface)
+    assert obj.input().empty
+    assert obj.output(True) is None
+
+
+def test_stdout_interface():
+    obj = i_factory('stdout:///')
+    assert isinstance(obj, StdoutInterface)
+    assert obj.input().empty
+    assert obj.output({'foo': 1}) == None
+
+
+def test_sqlite3_interface(data, ctx):
+    obj = i_factory('sqlite3:///:memory:', ExcelParse)
+    obj.output([], ctx)
+    obj.output([data], ctx)
+    assert isinstance(obj, Sqlite3Interface)
+    assert DATABASE.table_exists('excelparse')
+    assert len(ExcelParse.select()) == 1
 
 
 def test_parse_uri():
     db = 'endpoint://user:password@host:port/name'
-    p = parse_uri(db)
+    p = BaseInterface.parse_uri(db)
     keys = ('endpoint', 'user', 'password', 'host', 'port', 'name')
     not_keys = ()
     assert all([k in p.keys() for k in (keys + not_keys)])
     assert all([k in p.values() for k in keys])
     assert all([k not in p.values() for k in not_keys])
     db = 'endpoint://user@host/name'
-    p = parse_uri(db)
+    p = BaseInterface.parse_uri(db)
     keys = ('endpoint', 'user', 'host', 'name')
     not_keys = ('password', 'port')
     assert all([k in p.keys() for k in (keys + not_keys)])
     assert all([k in p.values() for k in keys])
     assert all([k not in p.values() for k in not_keys])
     db = 'endpoint:///name'
-    p = parse_uri(db)
+    p = BaseInterface.parse_uri(db)
     keys = ('endpoint', 'name')
     not_keys = ('user', 'password', 'host', 'port')
     assert all([k in p.keys() for k in (keys + not_keys)])
     assert all([k in p.values() for k in keys])
     assert all([k not in p.values() for k in not_keys])
     db = 'endpoint:///'
-    p = parse_uri(db)
+    p = BaseInterface.parse_uri(db)
     keys = ('endpoint',)
     not_keys = ('user', 'password', 'host', 'port', 'name')
     assert all([k in p.keys() for k in (keys + not_keys)])
     assert all([k in p.values() for k in keys])
     assert all([k not in p.values() for k in not_keys])
```

