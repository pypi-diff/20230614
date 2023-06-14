# Comparing `tmp/pg_bulk_ingest-0.0.8.tar.gz` & `tmp/pg_bulk_ingest-0.0.9.tar.gz`

## Comparing `pg_bulk_ingest-0.0.8.tar` & `pg_bulk_ingest-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    13856 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/pg_bulk_ingest.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/LICENSE
--rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/README.md
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    13768 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.9/pg_bulk_ingest.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.9/README.md
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.9/PKG-INFO
```

### Comparing `pg_bulk_ingest-0.0.8/pg_bulk_ingest.py` & `pg_bulk_ingest-0.0.9/pg_bulk_ingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,22 +271,18 @@
     except (TypeError, ValueError):
         comment_parsed = {}
 
     high_watermark_value = \
         comment_parsed.get('pg-bulk-ingest', {}).get('high-watermark') if high_watermark is HighWatermark.LATEST else\
         high_watermark
 
+    table_to_ingest_into = migrate_and_delete_if_necessary(conn, target_table, delete)
     at_least_one_batch = False
-    for high_watermark_value, batch in batches(high_watermark_value):
-        if not at_least_one_batch:
-            table_to_ingest_into = migrate_and_delete_if_necessary(conn, target_table, delete)
-        else:
-            table_to_ingest_into = target_table
-        at_least_one_batch = True
 
+    for high_watermark_value, batch in batches(high_watermark_value):
         if not is_upsert:
             csv_copy(sql, copy_from_stdin, conn, target_table, table_to_ingest_into, batch)
         else:
             # Create a batch table, and ingest into it
             batch_metadata = sa.MetaData()
             batch_table = sa.Table(
                 uuid.uuid4().hex,
@@ -315,26 +311,29 @@
                 updates=sql.SQL(',').join(sql.SQL('{} = EXCLUDED.{}').format(sql.Identifier(column.name), sql.Identifier(column.name)) for column in target_table.columns),
             )
             conn.execute(sa.text(insert_query.as_string(conn.connection.driver_connection)))
 
             # Drop the batch table
             batch_metadata.drop_all(conn)
 
-            # Swap with live table if it's needed (i.e a migration table)
-            swap_if_necessary(conn, target_table, table_to_ingest_into)
+        comment_parsed['pg-bulk-ingest'] = comment_parsed.get('pg-bulk-ingest', {})
+        comment_parsed['pg-bulk-ingest']['high-watermark'] = high_watermark_value
+        conn.execute(sa.text(sql.SQL('''
+             COMMENT ON TABLE {schema}.{table} IS {comment}
+        ''').format(
+            schema=sql.Identifier(table_to_ingest_into.schema),
+            table=sql.Identifier(table_to_ingest_into.name),
+            comment=sql.Literal(json.dumps(comment_parsed))
+        ).as_string(conn.connection.driver_connection)))
 
-            comment_parsed['pg-bulk-ingest'] = comment_parsed.get('pg-bulk-ingest', {})
-            comment_parsed['pg-bulk-ingest']['high-watermark'] = high_watermark_value
-            conn.execute(sa.text(sql.SQL('''
-                 COMMENT ON TABLE {schema}.{table} IS {comment}
-            ''').format(
-                schema=sql.Identifier(target_table.schema),
-                table=sql.Identifier(target_table.name),
-                comment=sql.Literal(json.dumps(comment_parsed))
-            ).as_string(conn.connection.driver_connection)))
+        # Swap with live table if it's needed (i.e a migration table)
+        swap_if_necessary(conn, target_table, table_to_ingest_into)
+
+        table_to_ingest_into = target_table
+        at_least_one_batch = True
 
         conn.commit()
         conn.begin()
 
     if not at_least_one_batch:
         migrate_table = migrate_and_delete_if_necessary(conn, target_table, delete)
         swap_if_necessary(conn, target_table, migrate_table)
```

### Comparing `pg_bulk_ingest-0.0.8/.gitignore` & `pg_bulk_ingest-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.8/LICENSE` & `pg_bulk_ingest-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.8/README.md` & `pg_bulk_ingest-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 
 
 ## Usage
 
 The API is made of a single function, `ingest` that can be used to insert data into a table. This:
 
 - creates the table if necessary
-- migrates any existing table if necessary
+- migrates any existing table if necessary, minimising locking
 - inserts the incoming data into the table
 - if the table has a primary key, performs an "upsert" based matching on this primary key
+- handles "high-watermarking" to carry on from where the previous ingest finished
 - optionally deletes all existing rows before ingestion
 
 For example:
 
 ```python
 import sqlalchemy as sa
 from pg_bulk_ingest import HighWatermark, Visibility, Delete, ingest
@@ -34,15 +35,15 @@
 
 # A SQLAlchemy Metadata of a single table definition
 metadata = sa.MetaData()
 my_table = sa.Table(
     "my_table",
     metadata,
     sa.Column("id", sa.INTEGER, primary_key=True),
-    sa.Column("value", sa.STRING(16), nullable=False),
+    sa.Column("value", sa.VARCHAR(16), nullable=False),
     schema="my_schema",
 )
 
 # A function that yields batches of data, where each batch is a tuple of of (high watermark, data rows).
 # The batches must all be strictly _after_ the high watermark passed into the function
 # Each high watermark must be JSON-encodable
 # Each row must have the SQLAlchemy table associated with it
@@ -82,15 +83,15 @@
 
 - `conn` - A [SQLAlchemy connection](https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Connection) not in a transaction, i.e. started by `connection` rather than `begin`.
 
 - `metadata` - A SQLAlchemy metadata of a single table.
 
 - `batches` - A function that takes a high watermark, returning an iterable that yields data batches that are strictly after this high watermark. See Usage above for an example.
 
-- `high_watermark` (optional) - The high watermark passed into the `batches` function. If this is the `HighWatermark.LATEST`, the default, then the most high watermark that has most recently been ingested is passed into the `batches` function.
+- `high_watermark` (optional) - The high watermark passed into the `batches` function. If this is the `HighWatermark.LATEST`, then the most recent high watermark that been returned from a previous ingest's `batch` function whose corresponding batch has been succesfully ingested is passed into the `batches` function.
 
 - `visibility` (optional) - When ingests will be visible to other clients.
 
 - `delete` (optional) - If existing rows are to be deleted.
 
 ---
 
@@ -131,15 +132,15 @@
 
 
 ## Under the hood
 
 - Ingestion is done exclusively with `COPY FROM`.
 - Ingestion is transactional, each batch is ingested completely or not at all
 - The table is migrated to match the definition, using techniques to avoid exclusively locking the table to allow parallel SELECT queries.
-- If the table has a primary key, then an "upsert" is performed. Data is ingested into an intermediate table, and an `INSERT ... ON CONFICT(...) DO UPDATE` is performed to copy rows from this intermediate table to the existing table. This doesn't involve an exclusive lock on the live table, unless a migration requires it.
+- If the table has a primary key, then an "upsert" is performed. Data is ingested into an intermediate table, and an `INSERT ... ON CONFLICT(...) DO UPDATE` is performed to copy rows from this intermediate table to the existing table. This doesn't involve an exclusive lock on the live table.
 - If there is no known technique for a migration without a long-running exclusive lock, then an intermediate table is used, swapped with the live table at the end of the first batch. This swap does require an exclusive lock, but only for a short time. Backends that hold locks that conflict with this lock are forcably terminated after a delay.
 - The high watermark is stored on the table as a COMMENT, JSON-encoded.
 
 
 ## Compatibility
 
 - Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
```

### Comparing `pg_bulk_ingest-0.0.8/pyproject.toml` & `pg_bulk_ingest-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-bulk-ingest"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_bulk_ingest-0.0.8/PKG-INFO` & `pg_bulk_ingest-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-bulk-ingest
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking
 Project-URL: Source, https://github.com/uktrade/pg-bulk-ingest
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -43,17 +43,18 @@
 
 
 ## Usage
 
 The API is made of a single function, `ingest` that can be used to insert data into a table. This:
 
 - creates the table if necessary
-- migrates any existing table if necessary
+- migrates any existing table if necessary, minimising locking
 - inserts the incoming data into the table
 - if the table has a primary key, performs an "upsert" based matching on this primary key
+- handles "high-watermarking" to carry on from where the previous ingest finished
 - optionally deletes all existing rows before ingestion
 
 For example:
 
 ```python
 import sqlalchemy as sa
 from pg_bulk_ingest import HighWatermark, Visibility, Delete, ingest
@@ -64,15 +65,15 @@
 
 # A SQLAlchemy Metadata of a single table definition
 metadata = sa.MetaData()
 my_table = sa.Table(
     "my_table",
     metadata,
     sa.Column("id", sa.INTEGER, primary_key=True),
-    sa.Column("value", sa.STRING(16), nullable=False),
+    sa.Column("value", sa.VARCHAR(16), nullable=False),
     schema="my_schema",
 )
 
 # A function that yields batches of data, where each batch is a tuple of of (high watermark, data rows).
 # The batches must all be strictly _after_ the high watermark passed into the function
 # Each high watermark must be JSON-encodable
 # Each row must have the SQLAlchemy table associated with it
@@ -112,15 +113,15 @@
 
 - `conn` - A [SQLAlchemy connection](https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Connection) not in a transaction, i.e. started by `connection` rather than `begin`.
 
 - `metadata` - A SQLAlchemy metadata of a single table.
 
 - `batches` - A function that takes a high watermark, returning an iterable that yields data batches that are strictly after this high watermark. See Usage above for an example.
 
-- `high_watermark` (optional) - The high watermark passed into the `batches` function. If this is the `HighWatermark.LATEST`, the default, then the most high watermark that has most recently been ingested is passed into the `batches` function.
+- `high_watermark` (optional) - The high watermark passed into the `batches` function. If this is the `HighWatermark.LATEST`, then the most recent high watermark that been returned from a previous ingest's `batch` function whose corresponding batch has been succesfully ingested is passed into the `batches` function.
 
 - `visibility` (optional) - When ingests will be visible to other clients.
 
 - `delete` (optional) - If existing rows are to be deleted.
 
 ---
 
@@ -161,15 +162,15 @@
 
 
 ## Under the hood
 
 - Ingestion is done exclusively with `COPY FROM`.
 - Ingestion is transactional, each batch is ingested completely or not at all
 - The table is migrated to match the definition, using techniques to avoid exclusively locking the table to allow parallel SELECT queries.
-- If the table has a primary key, then an "upsert" is performed. Data is ingested into an intermediate table, and an `INSERT ... ON CONFICT(...) DO UPDATE` is performed to copy rows from this intermediate table to the existing table. This doesn't involve an exclusive lock on the live table, unless a migration requires it.
+- If the table has a primary key, then an "upsert" is performed. Data is ingested into an intermediate table, and an `INSERT ... ON CONFLICT(...) DO UPDATE` is performed to copy rows from this intermediate table to the existing table. This doesn't involve an exclusive lock on the live table.
 - If there is no known technique for a migration without a long-running exclusive lock, then an intermediate table is used, swapped with the live table at the end of the first batch. This swap does require an exclusive lock, but only for a short time. Backends that hold locks that conflict with this lock are forcably terminated after a delay.
 - The high watermark is stored on the table as a COMMENT, JSON-encoded.
 
 
 ## Compatibility
 
 - Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
```

