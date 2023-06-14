# Comparing `tmp/eparse-0.4.1.tar.gz` & `tmp/eparse-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eparse-0.4.1.tar", last modified: Wed Jun 14 17:30:20 2023, max compression
+gzip compressed data, was "eparse-0.5.0.tar", last modified: Wed Jun 14 18:39:02 2023, max compression
```

## Comparing `eparse-0.4.1.tar` & `eparse-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 17:30:20.804639 eparse-0.4.1/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.4.1/AUTHORS.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      323 2023-06-13 20:47:22.000000 eparse-0.4.1/HISTORY.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.4.1/LICENSE
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.4.1/MANIFEST.in
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12067 2023-06-14 17:30:20.804639 eparse-0.4.1/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10996 2023-06-14 17:19:22.000000 eparse-0.4.1/README.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 17:30:20.804639 eparse-0.4.1/docs/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/Makefile
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/authors.rst
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/conf.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/contributing.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/history.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/index.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/installation.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/make.bat
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/readme.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/usage.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 17:30:20.804639 eparse-0.4.1/eparse/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-14 17:29:53.000000 eparse-0.4.1/eparse/__init__.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10172 2023-06-14 15:53:36.000000 eparse-0.4.1/eparse/cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     4736 2023-06-14 15:27:35.000000 eparse-0.4.1/eparse/core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6280 2023-06-14 16:48:23.000000 eparse-0.4.1/eparse/interfaces.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.4.1/eparse/migrations.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 17:30:20.804639 eparse-0.4.1/eparse.egg-info/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12067 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/SOURCES.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/dependency_links.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/entry_points.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/not-zip-safe
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/requires.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/top_level.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      427 2023-06-14 17:30:20.814639 eparse-0.4.1/setup.cfg
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1570 2023-06-14 17:29:38.000000 eparse-0.4.1/setup.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 17:30:20.804639 eparse-0.4.1/tests/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.4.1/tests/__init__.py
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.4.1/tests/eparse_unit_test_data.xlsx
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      893 2023-06-14 14:09:23.000000 eparse-0.4.1/tests/fixtures.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.4.1/tests/test.db
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1950 2023-06-14 15:53:16.000000 eparse-0.4.1/tests/test_cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.4.1/tests/test_core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.4.1/tests/test_interfaces.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 18:39:02.847827 eparse-0.5.0/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.5.0/AUTHORS.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      323 2023-06-13 20:47:22.000000 eparse-0.5.0/HISTORY.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.5.0/LICENSE
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.5.0/MANIFEST.in
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12067 2023-06-14 18:39:02.847827 eparse-0.5.0/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10996 2023-06-14 17:19:22.000000 eparse-0.5.0/README.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 18:39:02.847827 eparse-0.5.0/docs/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/Makefile
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/authors.rst
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/conf.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/contributing.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/history.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/index.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/installation.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/make.bat
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/readme.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/usage.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 18:39:02.847827 eparse-0.5.0/eparse/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-14 18:26:31.000000 eparse-0.5.0/eparse/__init__.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10257 2023-06-14 18:24:15.000000 eparse-0.5.0/eparse/cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5034 2023-06-14 18:22:39.000000 eparse-0.5.0/eparse/core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6316 2023-06-14 18:30:00.000000 eparse-0.5.0/eparse/interfaces.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.5.0/eparse/migrations.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 18:39:02.847827 eparse-0.5.0/eparse.egg-info/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12067 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/SOURCES.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/dependency_links.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/entry_points.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/not-zip-safe
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/requires.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/top_level.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      427 2023-06-14 18:39:02.847827 eparse-0.5.0/setup.cfg
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1570 2023-06-14 18:26:17.000000 eparse-0.5.0/setup.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 18:39:02.847827 eparse-0.5.0/tests/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.5.0/tests/__init__.py
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.5.0/tests/eparse_unit_test_data.xlsx
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      891 2023-06-14 18:22:40.000000 eparse-0.5.0/tests/fixtures.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.5.0/tests/test.db
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1980 2023-06-14 18:22:40.000000 eparse-0.5.0/tests/test_cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.5.0/tests/test_core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.5.0/tests/test_interfaces.py
```

### Comparing `eparse-0.4.1/CONTRIBUTING.rst` & `eparse-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/LICENSE` & `eparse-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/PKG-INFO` & `eparse-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.4.1
+Version: 0.5.0
 Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 4 - Beta
```

### Comparing `eparse-0.4.1/README.rst` & `eparse-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/docs/Makefile` & `eparse-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/docs/conf.py` & `eparse-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/docs/installation.rst` & `eparse-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/docs/make.bat` & `eparse-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/eparse/cli.py` & `eparse-0.5.0/eparse/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,57 +40,65 @@
         elif exit:
             sys.exit(1)
 
 
 @click.group()
 @click.pass_context
 @click.option(
-    '--input', '-i',
+    '--input',
+    '-i',
     type=str,
     default='null:///',
     help='input source',
 )
 @click.option(
-    '--output', '-o',
+    '--output',
+    '-o',
     type=str,
     default='null:///',
     help='output destination',
 )
 @click.option(
-    '--file', '-f',
+    '--file',
+    '-f',
     type=str,
     multiple=True,
     help='file(s) or dir(s) to target',
 )
 @click.option(
-    '--debug', '-d',
+    '--debug',
+    '-d',
     is_flag=True,
     default=False,
     help='use debug mode',
 )
 @click.option(
-    '--loose', '-l',
+    '--loose',
+    '-l',
     is_flag=True,
     default=True,
     help='find tables loosely',
 )
 @click.option(
-    '--recursive', '-r',
+    '--recursive',
+    '-r',
     is_flag=True,
     default=False,
     help='find files recursively',
 )
 @click.option(
-    '--truncate', '-t',
+    '--truncate',
+    '-t',
     is_flag=True,
     default=True,
     help='truncate dataframe output',
 )
 @click.option(
-    '--verbose', '-v',
+    '--verbose',
+    '-v',
     count=True,
     help='increase output verbosity',
 )
 def main(
     ctx,
     input,
     output,
@@ -141,27 +149,30 @@
         # pd.set_option('display.max_colwidth', None)
         pd.set_option('display.max_rows', None)
 
 
 @main.command()
 @click.pass_context
 @click.option(
-    '--number', '-n',
+    '--number',
+    '-n',
     type=int,
     default=None,
     help='stop after n excel files',
 )
 @click.option(
-    '--sheet', '-s',
+    '--sheet',
+    '-s',
     type=str,
     default=None,
     help='name of sheet to scan for',
 )
 @click.option(
-    '--tables', '-t',
+    '--tables',
+    '-t',
     is_flag=True,
     default=False,
     help='count tables in scanned sheets',
 )
 def scan(ctx, number, sheet, tables):
     '''
     scan for excel files in target
@@ -173,18 +184,20 @@
 
     if ctx.obj['debug']:
         PrettyPrinter().pprint(ctx.obj)
 
     # process each Excel file in files
     for i, f in enumerate(ctx.obj['files']):
         if f.is_file() and 'xls' in f.name:
-
             try:
                 e_file = pd.read_excel(
-                    f, sheet_name=sheet, header=None, index_col=None
+                    f,
+                    sheet_name=sheet,
+                    header=None,
+                    index_col=None,
                 )
             except Exception as e:
                 msg = f'skipping {f} - {e}'
                 handle(e, msg=msg, debug=ctx.obj['debug'], exit=False)
                 continue
 
             # get basic info about Excel file
@@ -227,27 +240,30 @@
             if number is not None and i >= number:
                 break
 
 
 @main.command()
 @click.pass_context
 @click.option(
-    '--sheet', '-s',
+    '--sheet',
+    '-s',
     type=str,
     multiple=True,
     help='name of sheet(s) to parse',
 )
 @click.option(
-    '--serialize', '-z',
+    '--serialize',
+    '-z',
     is_flag=True,
     default=False,
     help='serialize table output',
 )
 @click.option(
-    '--table', '-t',
+    '--table',
+    '-t',
     type=str,
     default=None,
     help='name of table to parse',
 )
 def parse(ctx, sheet, serialize, table):
     '''
     parse table(s) found in sheet for target(s)
@@ -259,15 +275,14 @@
 
     if ctx.obj['debug']:
         PrettyPrinter().pprint(ctx.obj)
 
     # process each Excel file in files
     for i, f in enumerate(ctx.obj['files']):
         if f.is_file() and 'xls' in f.name:
-
             try:
                 e_file = pd.read_excel(
                     f,
                     sheet_name=list(sheet) or None,
                     header=None,
                     index_col=None,
                 )
@@ -319,28 +334,31 @@
                         handle(e, msg=msg, debug=ctx.obj['debug'], exit=False)
                         continue
 
 
 @main.command()
 @click.pass_context
 @click.option(
-    '--filter', '-f',
+    '--filter',
+    '-f',
     type=str,
     nargs=2,
     multiple=True,
     help='django-style filter(s) to apply to base queryset',
 )
 @click.option(
-    '--method', '-m',
+    '--method',
+    '-m',
     type=str,
     default='get_queryset',
     help='method to call on eparse model',
 )
 @click.option(
-    '--serialize', '-z',
+    '--serialize',
+    '-z',
     is_flag=True,
     default=False,
     help='serialize query output',
 )
 def query(ctx, filter, method, serialize):
     '''
     query eparse output
@@ -357,18 +375,15 @@
         data = ctx.obj['input_obj'].input(method, **ctx.obj['filters'])
     except Exception as e:
         msg = f'input from {ctx.obj["input"]} failed with {e}'
         handle(e, msg=msg, debug=ctx.obj['debug'])
 
     if serialize:
         try:
-            data = [
-                df_normalize_data(d)
-                for d in data.to_dict('records')
-            ]
+            data = [df_normalize_data(d) for d in data.to_dict('records')]
         except Exception as e:
             msg = 'serialization error (some methods can\'t be serialized)'
             handle(e, msg=f'{msg} - {e}', debug=ctx.obj['debug'])
 
     # output data
     try:
         ctx.obj['output_obj'].output(data, ctx)
@@ -376,15 +391,16 @@
         msg = f'output to {ctx.obj["output"]} failed with {e}'
         handle(e, msg=msg, debug=ctx.obj['debug'])
 
 
 @main.command()
 @click.pass_context
 @click.option(
-    '--migration', '-m',
+    '--migration',
+    '-m',
     required=True,
     type=str,
     multiple=True,
     help='database migration(s) to apply',
 )
 def migrate(ctx, migration):
     '''
```

### Comparing `eparse-0.4.1/eparse/core.py` & `eparse-0.5.0/eparse/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,137 +15,152 @@
 
 
 # NOTE: df[n] df.at[r,c] and df.iloc[r,c] are not all the same
 #       only with .iloc is it safe to assume index and column
 #       names will be ingored ; use iloc when working with
 #       sub-tables, e.g. the output from df_parse_table
 
+
 def df_find_tables(df: pd.DataFrame, loose=False) -> List[TableRef]:
     '''
     finds table corners in a dataframe
     '''
 
     result = []
 
     # for each row
     for r in range(df.shape[0]):
         # for each col
         for c in range(df.shape[1]):
-            isna_left = True if c == 0 else pd.isna(df.at[r, (c-1)])
-            isna_above = True if r == 0 else pd.isna(df.at[(r-1), c])
+            isna_left = True if c == 0 else pd.isna(df.at[r, (c - 1)])
+            isna_above = True if r == 0 else pd.isna(df.at[(r - 1), c])
             isna_value = pd.isna(df.at[r, c])
 
             try:
-                isna_right = pd.isna(df.at[r, (c+1)])
-                isna_down = pd.isna(df.at[(r+1), c])
-                isna_corner = pd.isna(df.at[(r+1), (c+1)])
+                isna_right = pd.isna(df.at[r, (c + 1)])
+                isna_down = pd.isna(df.at[(r + 1), c])
+                isna_corner = pd.isna(df.at[(r + 1), (c + 1)])
 
                 # ensure a 2x2 sparse table
-                min_size = any([
-                    not isna_right and not isna_down,
-                    not isna_right and not isna_corner,
-                    not isna_down and not isna_corner,
-                ])
+                min_size = any(
+                    [
+                        not isna_right and not isna_down,
+                        not isna_right and not isna_corner,
+                        not isna_down and not isna_corner,
+                    ]
+                )
 
                 if not loose:
                     # ensure a 2x2 dense table
-                    min_size = all([
-                        not isna_right,
-                        not isna_down,
-                        not isna_corner,
-                    ])
+                    min_size = all(
+                        [
+                            not isna_right,
+                            not isna_down,
+                            not isna_corner,
+                        ]
+                    )
 
             except Exception:
                 min_size = False
 
             if all([isna_left, isna_above, not isna_value, min_size]):
-                result.append((
-                    r,
-                    c,
-                    f'{get_column_letter(c+1)}{r+1}',
-                    str(df.at[r, c]),
-                ))
+                result.append(
+                    (
+                        r,
+                        c,
+                        f'{get_column_letter(c+1)}{r+1}',
+                        str(df.at[r, c]),
+                    )
+                )
 
     return result
 
 
 def _is_rowspan(df: pd.DataFrame, r: int, c: int) -> bool:
     '''
     detect a rowspan label
     '''
 
     try:
-        isna_right = pd.isna(df.at[r, (c+1)])
-        isna_down = pd.isna(df.at[(r+1), c])
+        isna_right = pd.isna(df.at[r, (c + 1)])
+        isna_down = pd.isna(df.at[(r + 1), c])
 
         return isna_down and not isna_right
 
     except KeyError:
         return False
 
 
 def _has_empty_corner(df: pd.DataFrame, r: int, c: int) -> bool:
     '''
     detect an empty corner
     '''
 
     try:
-        isna_above = pd.isna(df.at[(r-1), c])
-        isna_up_corner = pd.isna(df.at[(r-1), (c+1)])
+        isna_above = pd.isna(df.at[(r - 1), c])
+        isna_up_corner = pd.isna(df.at[(r - 1), (c + 1)])
 
         return isna_above and not isna_up_corner
 
     except KeyError:
         return False
 
 
 def df_parse_table(
-        df: pd.DataFrame,
-        r: int,
-        c: int,
-        ) -> pd.DataFrame:
+    df: pd.DataFrame,
+    r: int,
+    c: int,
+) -> pd.DataFrame:
     '''
     extract a table from a dataframe for a given r, c position
     '''
 
     # make reference adjustments
     if _is_rowspan(df, r, c):
         c += 1
 
     if _has_empty_corner(df, r, c):
         r -= 1
 
     _r = r + 1
 
     # get ending row
-    for row in range(r+1, df.shape[0]):
+    for row in range(r + 1, df.shape[0]):
         if pd.isna(df.at[row, c]):
             break
         _r += 1
 
     _c = c + 1
 
     # get ending col
-    for col in range(c+1, df.shape[1]):
+    for col in range(c + 1, df.shape[1]):
         if pd.isna(df.at[r, col]):
             break
         _c += 1
 
     return df.iloc[r:_r, c:_c]
 
 
 def df_normalize_data(data: Dict) -> Dict:
     '''
     normalize table data
     '''
 
     result = {}
     ints = ('row', 'column')
-    strs = ('value', 'type', 'c_header', 'r_header', 'excel_RC',
-            'name', 'sheet', 'f_name')
+    strs = (
+        'value',
+        'type',
+        'c_header',
+        'r_header',
+        'excel_RC',
+        'name',
+        'sheet',
+        'f_name',
+    )
 
     for k in ints:
         if k in data:
             result[k] = int(data[k])
 
     for k in strs:
         if k in data:
@@ -155,37 +170,39 @@
         if isinstance(data['timestamp'], pd.Timestamp):
             result['timestamp'] = data['timestamp'].to_pydatetime()
 
     return result
 
 
 def df_serialize_table(
-        df: pd.DataFrame,
-        **other_data,
-        ) -> List[Dict]:
+    df: pd.DataFrame,
+    **other_data,
+) -> List[Dict]:
     '''
     serialize table into a list of dicts with meta data
     '''
 
     column_header = df.iloc[0]
     row_header = df.iloc[:, 0]
 
     result = []
 
     for r in range(df.shape[0]):
         for c in range(df.shape[1]):
             _r = df.index[r]  # excel df row
             _c = df.columns[c]  # excel df col
             result.append(
-                df_normalize_data({
-                    'row': r,
-                    'column': c,
-                    'value': df.iloc[r, c],
-                    'type': type(df.iloc[r, c]),
-                    'c_header': column_header.iloc[c],
-                    'r_header': row_header.iloc[r],
-                    'excel_RC': f'{get_column_letter(_c+1)}{_r+1}',
-                    **other_data,
-                })
+                df_normalize_data(
+                    {
+                        'row': r,
+                        'column': c,
+                        'value': df.iloc[r, c],
+                        'type': type(df.iloc[r, c]),
+                        'c_header': column_header.iloc[c],
+                        'r_header': row_header.iloc[r],
+                        'excel_RC': f'{get_column_letter(_c+1)}{_r+1}',
+                        **other_data,
+                    }
+                )
             )
 
     return result
```

### Comparing `eparse-0.4.1/eparse/interfaces.py` & `eparse-0.5.0/eparse/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,31 +60,28 @@
     @classmethod
     def get_column(cls, column, *args, **kwargs):
         '''
         return distinct values from column with aggregations
         '''
 
         query = (
-            cls
-            .filter(**kwargs)
+            cls.filter(**kwargs)
             .select(
                 getattr(cls, column),
                 fn.COUNT(cls.id).alias('Total Rows'),
                 fn.COUNT(cls.type.distinct()).alias('Data Types'),
                 fn.COUNT(cls.value.distinct()).alias('Distinct Values'),
             )
             .group_by(getattr(cls, column))
         )
         return pd.DataFrame(query.dicts())
 
     class Meta:
         database = DATABASE
-        indexes = (
-            (('f_name', 'sheet', 'name'), False),
-        )
+        indexes = ((('f_name', 'sheet', 'name'), False),)
 
 
 class BaseInterface:
     '''
     base interface class
     '''
 
@@ -209,16 +206,16 @@
             raise ValueError('bad data - did you serialize it first?')
 
         self.initialize(DATABASE)
         DATABASE.connect()
         DATABASE.create_tables([self.Model])
 
         # insert data into Model
-        for d in data:
-            self.Model.create(**d)
+        with DATABASE.atomic():
+            self.Model.insert_many(data).execute()
 
         # DATABASE.close()
 
     def migrate(self, migration):
         try:
             m = importlib.import_module('eparse.migrations')
             migration_fcn = getattr(m, migration)
@@ -248,21 +245,23 @@
 
 class PostgresInterface(BaseDatabaseInterface):
     '''
     postgres interface
     '''
 
     def initialize(self, db):
-        db.initialize(PostgresqlDatabase(
-            self.name,
-            user=self.user,
-            password=self.password,
-            host=self.host,
-            port=self.port,
-        ))
+        db.initialize(
+            PostgresqlDatabase(
+                self.name,
+                user=self.user,
+                password=self.password,
+                host=self.host,
+                port=self.port,
+            )
+        )
 
 
 def i_factory(uri, Model=None):
     '''
     return interface object based on uri
     '''
```

### Comparing `eparse-0.4.1/eparse/migrations.py` & `eparse-0.5.0/eparse/migrations.py`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/eparse.egg-info/PKG-INFO` & `eparse-0.5.0/eparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.4.1
+Version: 0.5.0
 Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 4 - Beta
```

### Comparing `eparse-0.4.1/eparse.egg-info/SOURCES.txt` & `eparse-0.5.0/eparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/setup.py` & `eparse-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,10 +55,10 @@
     include_package_data=True,
     keywords='eparse',
     name='eparse',
     packages=find_packages(include=['eparse', 'eparse.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChrisPappalardo/eparse',
-    version='0.4.1',
+    version='0.5.0',
     zip_safe=False,
 )
```

### Comparing `eparse-0.4.1/tests/eparse_unit_test_data.xlsx` & `eparse-0.5.0/tests/eparse_unit_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/tests/fixtures.py` & `eparse-0.5.0/tests/fixtures.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 @pytest.fixture
 def ctx():
     '''
     click style ctx object fixture
     '''
 
-    class Obj():
+    class Obj:
         obj = {}
 
     return Obj()
 
 
 @pytest.fixture
 def data():
```

### Comparing `eparse-0.4.1/tests/test.db` & `eparse-0.5.0/tests/test.db`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/tests/test_cli.py` & `eparse-0.5.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,19 @@
     result = runner.invoke(main, ['-i', 'sqlite3:///tests/test.db', 'query'], **kwargs)
     assert result.exit_code == 0
     assert result.output == ''
 
 
 def test_migrate():
     runner = CliRunner()
-    result = runner.invoke(main, ['-i', 'sqlite3:///tests/test.db', 'migrate', '-m', 'migration_000102_000200'], **kwargs)
+    result = runner.invoke(
+        main,
+        ['-i', 'sqlite3:///tests/test.db', 'migrate', '-m', 'migration_000102_000200'],
+        **kwargs
+    )
     assert result.exit_code == 1
     assert 'duplicate column name: timestamp' in result.output
 
 
 def test_outputs():
     runner = CliRunner()
     result = runner.invoke(main, ['-o', 'null:///', 'scan'], **kwargs)
```

### Comparing `eparse-0.4.1/tests/test_core.py` & `eparse-0.5.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.4.1/tests/test_interfaces.py` & `eparse-0.5.0/tests/test_interfaces.py`

 * *Files identical despite different names*

