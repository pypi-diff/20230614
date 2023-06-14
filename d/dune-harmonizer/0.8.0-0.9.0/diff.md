# Comparing `tmp/dune_harmonizer-0.8.0.tar.gz` & `tmp/dune_harmonizer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_harmonizer-0.8.0.tar", max compression
+gzip compressed data, was "dune_harmonizer-0.9.0.tar", max compression
```

## Comparing `dune_harmonizer-0.8.0.tar` & `dune_harmonizer-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2023-04-26 05:55:18.460846 dune_harmonizer-0.8.0/LICENSE
--rw-r--r--   0        0        0     2378 2023-04-26 05:55:18.460846 dune_harmonizer-0.8.0/README.md
--rw-r--r--   0        0        0      440 2023-04-26 05:55:18.460846 dune_harmonizer-0.8.0/dune/harmonizer/__init__.py
--rw-r--r--   0        0        0       54 2023-04-26 05:55:18.460846 dune_harmonizer-0.8.0/dune/harmonizer/constants.py
--rw-r--r--   0        0        0    15192 2023-04-26 05:55:18.460846 dune_harmonizer-0.8.0/dune/harmonizer/custom_transforms.py
--rw-r--r--   0        0        0     4208 2023-04-26 05:55:18.460846 dune_harmonizer-0.8.0/dune/harmonizer/dialects/dunesql.py
--rw-r--r--   0        0        0      105 2023-04-26 05:55:18.464846 dune_harmonizer-0.8.0/dune/harmonizer/errors.py
--rw-r--r--   0        0        0     2018 2023-04-26 05:55:18.464846 dune_harmonizer-0.8.0/dune/harmonizer/table_replacements.py
--rw-r--r--   0        0        0     2756 2023-04-26 05:55:18.464846 dune_harmonizer-0.8.0/dune/harmonizer/translate.py
--rw-r--r--   0        0        0      570 2023-04-26 05:55:18.464846 dune_harmonizer-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 dune_harmonizer-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-26 13:31:30.025728 dune_harmonizer-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2378 2023-04-26 13:31:30.025728 dune_harmonizer-0.9.0/README.md
+-rw-r--r--   0        0        0      440 2023-04-26 13:31:30.025728 dune_harmonizer-0.9.0/dune/harmonizer/__init__.py
+-rw-r--r--   0        0        0       54 2023-04-26 13:31:30.025728 dune_harmonizer-0.9.0/dune/harmonizer/constants.py
+-rw-r--r--   0        0        0    13827 2023-04-26 13:31:30.025728 dune_harmonizer-0.9.0/dune/harmonizer/custom_transforms.py
+-rw-r--r--   0        0        0     8371 2023-04-26 13:31:30.025728 dune_harmonizer-0.9.0/dune/harmonizer/dialects/dunesql.py
+-rw-r--r--   0        0        0      105 2023-04-26 13:31:30.025728 dune_harmonizer-0.9.0/dune/harmonizer/errors.py
+-rw-r--r--   0        0        0     2018 2023-04-26 13:31:30.025728 dune_harmonizer-0.9.0/dune/harmonizer/table_replacements.py
+-rw-r--r--   0        0        0     2756 2023-04-26 13:31:30.025728 dune_harmonizer-0.9.0/dune/harmonizer/translate.py
+-rw-r--r--   0        0        0      570 2023-04-26 13:31:30.025728 dune_harmonizer-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 dune_harmonizer-0.9.0/PKG-INFO
```

### Comparing `dune_harmonizer-0.8.0/LICENSE` & `dune_harmonizer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.8.0/README.md` & `dune_harmonizer-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.8.0/dune/harmonizer/custom_transforms.py` & `dune_harmonizer-0.9.0/dune/harmonizer/custom_transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -222,39 +222,25 @@
     """if a column has amount/value in the name, cast to double"""
     if node.key == "column":
         if any(val in node.name.lower() for val in ("amount", "value")):
             return sqlglot.parse_one("cast(" + node.name + " as double)", read="trino")
     return node
 
 
-def cast_timestamp(node):
-    """Look for date-like literals and params and cast these as timestamps"""
+def cast_timestamp_parameters(node):
+    """Look for parameters with 'date' or 'time' in, and cast these as timestamps"""
     if node.key == "literal":
-        # and contains 'yyyy-mm-dd' format then cast to timestamp
-        if re.search(r"\d{4}-\d{2}-\d{2}", node.sql(dialect="trino")):
-            return sqlglot.parse_one("timestamp " + node.sql(dialect="trino"), read="trino")
-
         # or if it is a param that contains date/time
         pattern = "('" + param_left_placeholder + r".*?" + param_right_placeholder + "')"
         if any(d in node.sql(dialect="trino").lower() for d in ("date", "time")):
             q = re.sub(pattern, r"timestamp \1", node.sql(dialect="trino"))
             return sqlglot.parse_one(q, read="trino")
     return node
 
 
-def fix_boolean(node):
-    """If node.key is 'literal' and contains 'true' or 'false' then cast to boolean"""
-    if node.key == "literal":
-        if any(boolean in node.sql(dialect="trino").lower() for boolean in ("true", "false")):
-            # remove single or double quotes
-            bool_cleaned = node.sql(dialect="trino").replace('"', "").replace("'", "")
-            return sqlglot.parse_one(bool_cleaned, read="trino")
-    return node
-
-
 def warn_sequence(node):
     """Add a warning that links to docs if the query uses generate_series/sequence"""
     if node.name.lower() in ("generate_series", "sequence"):
         return sqlglot.parse_one(
             node.sql(dialect="trino")
             + (
                 "-- WARNING: Check out the docs for example of time series generation: "
@@ -266,28 +252,14 @@
 
 
 def rename_amount_column(query):
     """Rename the usd_amount column"""
     return sqlglot.parse_one(query.sql(dialect="trino").replace("usd_amount", "amount_usd"), read="trino")
 
 
-def bytea2numeric(node):
-    """Replace and warn about bytearray functions"""
-    query = node.sql(dialect="trino")
-    if "bytea2numeric" in query.lower():
-        query = re.sub("bytea2numeric", "bytearray_to_bigint", query, flags=re.IGNORECASE)
-        query = (
-            "/* !Bytea warning: We now have new bytearray functions to cover conversions and stuff like "
-            "length, concat, substring, etc. Check out the docs here: "
-            "https://dune.com/docs/reference/dune-v2/query-engine/#byte-array-to-numeric-functions */"
-            "\n\n"
-        ) + query
-    return sqlglot.parse_one(query, read="trino")
-
-
 def fix_bytearray_param(query):
     """Remove lower function call from bytearray parameters"""
     pattern = r"lower\(\s*['\"]\{\{(.*?)\}\}['\"]\s*\)"
     return re.sub(pattern, r"{{\1}}", query, flags=re.IGNORECASE)
 
 
 def chain_where(dataset):
@@ -303,40 +275,36 @@
 def postgres_transforms(query, dataset):
     """Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.
 
     Each transform takes and returns a sqlglot.Expression"""
     query_tree = sqlglot.parse_one(query, read="trino")
     transforms = (
         postgres_table_replacements(dataset),
-        fix_boolean,
         cast_numeric,
-        cast_timestamp,
+        cast_timestamp_parameters,
         warn_sequence,
         dex_trades_fixes,
         chain_where(dataset),
         bytearray_parameter_fix,
         rename_amount_column,
-        bytea2numeric,
     )
     for f in transforms:
         query_tree = query_tree.transform(f)
     return query_tree
 
 
 def spark_transforms(query):
     """Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.
 
     Each transform takes and returns a sqlglot.Expression"""
     query_tree = sqlglot.parse_one(query, read="trino")
     transforms = (
-        fix_boolean,
         cast_numeric,
-        cast_timestamp,
+        cast_timestamp_parameters,
         warn_sequence,
-        bytea2numeric,
     )
     for f in transforms:
         query_tree = query_tree.transform(f)
     return query_tree
 
 
 def add_warnings_and_banner(query):
```

### Comparing `dune_harmonizer-0.8.0/dune/harmonizer/table_replacements.py` & `dune_harmonizer-0.9.0/dune/harmonizer/table_replacements.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.8.0/dune/harmonizer/translate.py` & `dune_harmonizer-0.9.0/dune/harmonizer/translate.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.8.0/pyproject.toml` & `dune_harmonizer-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dune-harmonizer"
-version = "0.8.0"
+version = "0.9.0"
 description = ""
 authors = ["Vegard Stikbakke <vegard@dune.com>"]
 readme = "README.md"
 packages = [{include = "dune"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dune_harmonizer-0.8.0/PKG-INFO` & `dune_harmonizer-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-harmonizer
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 Author: Vegard Stikbakke
 Author-email: vegard@dune.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlglot (>=11.5.7,<12.0.0)
```

