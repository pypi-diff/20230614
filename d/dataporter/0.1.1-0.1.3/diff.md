# Comparing `tmp/dataporter-0.1.1.tar.gz` & `tmp/dataporter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataporter-0.1.1.tar", max compression
+gzip compressed data, was "dataporter-0.1.3.tar", max compression
```

## Comparing `dataporter-0.1.1.tar` & `dataporter-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      195 2023-06-13 10:19:34.102317 dataporter-0.1.1/README.md
--rw-r--r--   0        0        0       74 2023-06-13 09:34:05.395960 dataporter-0.1.1/dataporter/__init__.py
--rw-r--r--   0        0        0     4820 2023-06-13 09:34:05.398236 dataporter-0.1.1/dataporter/csv2sql.py
--rw-r--r--   0        0        0     3436 2023-06-13 09:34:05.395591 dataporter-0.1.1/dataporter/sql2csv.py
--rw-r--r--   0        0        0      457 2023-06-13 10:22:44.014356 dataporter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 dataporter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      354 2023-06-14 10:59:50.072481 dataporter-0.1.3/README.md
+-rw-r--r--   0        0        0      177 2023-06-14 11:19:16.055673 dataporter-0.1.3/dataporter/__init__.py
+-rw-r--r--   0        0        0     6360 2023-06-14 10:55:40.759968 dataporter-0.1.3/dataporter/csv2sql.py
+-rw-r--r--   0        0        0     3532 2023-06-14 08:14:15.148442 dataporter-0.1.3/dataporter/sql2csv.py
+-rw-r--r--   0        0        0     1828 2023-06-14 11:17:06.906524 dataporter-0.1.3/dataporter/sql_schema2txt.py
+-rw-r--r--   0        0        0      502 2023-06-14 11:20:23.374180 dataporter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 dataporter-0.1.3/PKG-INFO
```

### Comparing `dataporter-0.1.1/dataporter/csv2sql.py` & `dataporter-0.1.3/dataporter/csv2sql.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Literal, Optional, Any
 from loguru import logger
 from fire import Fire
 import pandas as pd
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, text, exc
+from sqlalchemy.orm import sessionmaker
 
 
 def _exec_multi_expr(df: pd.DataFrame, exprs: List[str], debug: bool = False) -> pd.DataFrame:
     for expr in exprs:
         if debug:
             logger.info("exec expr: {}", expr)
         df = pd.eval(expr=expr, target=df)
@@ -20,62 +21,97 @@
 def csv2sql(
     sql_uri: str,
     table_name: str,
     filename: str,
     header: List[int] | Literal["infer"] | None = "infer",
     names: Optional[List[str]] = None,
     sep: str = ",",
+    index: bool = False,
     quotechar: str = '"',
     escapechar: Optional[str] = None,
     lineterminator: Optional[str] = None,
-    sql_schema: str | None = None,
+    sql_schema_file: str | None = None,
     sql_data_exists: Literal["fail", "replace", "append"] = "fail",
     read_chunk_size: Optional[int] = None,
     pandas_exprs: List[str] | None = None,
     debug: bool = False,
     ignore_error: bool = False,
     **sql_kwargs: Any
 ):
     """
     convert csv to sql table.
-    :param sql_uri: database uri, according to sqlalchemy uri.
+    :param sql_uri: database uri, according to sqlalchemy uri, according to sqlalchemy uri, e.g. "mysql+pymysql://username:pass@host:port/database.
     :param table_name: csv data insert table name.
     :param filename: source csv filename.
     :param header: default first line, also can provide by 'xxx,yyy,bbb' format.
     :param names: specify the headers of csv file, e.g. 'a,b,c,d'.
     :param sep: sep symbol, ',' default.
+    :param index: if generate index in result.
     :param quotechar: quote char, '"' default.
     :param escapechar: escape char, None default.
     :param lineterminator: line terminator, related to system ('\\n' for linux, '\\r\\n' for Windows, i.e.).
     :param sql_kwargs: other kwargs for sql, it will be pass to sqlalchemy 'create_engine' function.
     :param sql_data_exists: action on data exist in sql db, can be 'fail' or 'replace' or 'append', default 'fail'.
-    :param sql_schema: schema on create table, default None (auto generate with no index).
+    :param sql_schema_file: schema on create table, default None (auto generate with no index).
     :param read_chunk_line: if csv file is large, to reduce the memory usage, read csv to memory by trunk of lines.
     :param pandas_exprs: exec multiple pandas expr in order.
     :param debug: if debug mod on, will print every result after exec pandas exprs.
     :param ignore_error: if ignore sql insert error, it may cause loss chunks of data.
     """
     engine = create_engine(url=sql_uri, **sql_kwargs)
 
+    Session = sessionmaker(engine)
+    # handle sql schema
+    # if replace, drop table and create according to schema
+    # if append or fail, try create table if not exist according to schema
+    if sql_schema_file and sql_data_exists == "replace":
+        logger.warning("please ensure table_name matches the sql_schema_file content, or this will cause unexpected error.")
+
+        with open(sql_schema_file) as f:
+            schema = f.read()
+
+        with Session() as session:
+            session.execute(text(f"DROP TABLE IF EXISTS {table_name}"))
+            logger.info("dropping table...")
+
+            session.execute(text(schema))
+            logger.info("creating table according to schema...")
+            sql_data_exists = "append"
+    elif sql_schema_file:
+        with open(sql_schema_file) as f:
+            schema = f.read()
+
+        with Session() as session:
+            try:
+                create_res = session.execute(text(schema))
+                logger.info("creating table according to schema(if not exist)...")
+                logger.info(create_res.all())
+            except exc.OperationalError as e:
+                if e.orig.args[0] == 1050:
+                    logger.info("table already exist.")
+                else:
+                    raise e
+
     if read_chunk_size is None:
         df = pd.read_csv(
             filename,
             sep=sep,
             names=names,
             header=header,
             quotechar=quotechar,
             escapechar=escapechar,
             lineterminator=lineterminator,
         )
         if pandas_exprs:
             df = _exec_multi_expr(df, exprs=pandas_exprs, debug=debug)
         with engine.begin() as conn:
             df.to_sql(
-                name=table_name, con=conn, schema=sql_schema, if_exists=sql_data_exists
+                name=table_name, con=conn, if_exists=sql_data_exists, index=index
             )
+            logger.info(f"inserted {len(df)} rows")
     else:
         logger.info("converting csv to sql...")
         trunk_df = pd.read_csv(
             filename,
             sep=sep,
             chunksize=read_chunk_size,
             iterator=True,
@@ -110,15 +146,15 @@
                 else:
                     raise ValueError(f"cannot parse current_data_exist value:{sql_data_exists}")
 
                 with logger.catch(message="write to db error, loss chunk.", reraise=not ignore_error):
                     df.to_sql(
                         name=table_name,
                         con=conn,
-                        schema=sql_schema,
+                        index=index,
                         if_exists=current_data_exist,
                     )
 
         logger.info("done.")
 
 
 def main():
```

### Comparing `dataporter-0.1.1/dataporter/sql2csv.py` & `dataporter-0.1.3/dataporter/sql2csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,28 +30,28 @@
     lineterminator: Optional[str] = None,
     read_chunk_size: Optional[int] = None,
     pandas_exprs: List[str] | None = None,
     debug: bool = False,
     **sql_kwargs: Any
 ):
     """
-    convert sql query result to csv
-    :param sql_uri: database uri, according to sqlalchemy uri
-    :param sql: query sql
-    :param filename: result csv filename
-    :param index: if generate index in result
-    :param header: if contains header in result
-    :param sep: sep symbol, ',' default
-    :param quotechar: quote char, '"' default
-    :param escapechar: escape char, None default
-    :param lineterminator: line terminator, related to system ('\\n' for linux, '\\r\\n' for Windows, i.e.)
+    convert sql query result to csv.
+    :param sql_uri: database uri, according to sqlalchemy uri, according to sqlalchemy uri, e.g. "mysql+pymysql://username:pass@host:port/database.
+    :param sql: query sql.
+    :param filename: result csv filename.
+    :param index: if generate index in result.
+    :param header: if contains header in result.
+    :param sep: sep symbol, ',' default.
+    :param quotechar: quote char, '"' default.
+    :param escapechar: escape char, None default.
+    :param lineterminator: line terminator, related to system ('\\n' for linux, '\\r\\n' for Windows, i.e.).
     :param read_chunk_size: if sql table is large, to reduce the memory usage, read sql to memory by trunk of lines, then write to local csv.
     :param sql_kwargs: other kwargs for sql, it will be pass to sqlalchemy 'create_engine' function.
     :param pandas_exprs: exec multiple pandas expr in order.
-    :param debug: if debug mod on, will print every result after exec pandas exprs
+    :param debug: if debug mod on, will print every result after exec pandas exprs.
     """
     engine = create_engine(url=sql_uri, **sql_kwargs)
     if read_chunk_size is None:
         with engine.begin() as conn:
             df = pd.read_sql(sql, conn)
         if pandas_exprs:
             df = _exec_multi_expr(df, exprs=pandas_exprs, debug=debug)
```

### Comparing `dataporter-0.1.1/PKG-INFO` & `dataporter-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataporter
-Version: 0.1.1
+Version: 0.1.3
 Summary: 
 Author: AuthorPlaceholder
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=40.0.2,<41.0.0)
@@ -14,13 +14,20 @@
 Requires-Dist: pymysql (>=1.0.3,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.13,<3.0.0)
 Description-Content-Type: text/markdown
 
 # dataporter
 dataporter is a lightweight migration tool. It migrate data between multiple infrastructure
 ## current support
-- sql -> csv
-- csv -> sql
+### data porter
+- sql -> csv, command: `sql2csv`
+- csv -> sql, command: `csv2sql`
+
+### utils
+- sql schema -> txt, command: `sql_schema2txt`
+
+for more detail usage, please use `--help`
+
 # will support
 - kafka -> csv
 - csv -> kafka
```

