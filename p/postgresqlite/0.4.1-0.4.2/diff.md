# Comparing `tmp/postgresqlite-0.4.1.tar.gz` & `tmp/postgresqlite-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgresqlite-0.4.1.tar", max compression
+gzip compressed data, was "postgresqlite-0.4.2.tar", max compression
```

## Comparing `postgresqlite-0.4.1.tar` & `postgresqlite-0.4.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    15321 2023-06-14 10:26:48.369503 postgresqlite-0.4.1/README.md
--rw-r--r--   0        0        0    19586 2023-06-14 15:03:34.771430 postgresqlite-0.4.1/postgresqlite/__init__.py
--rw-r--r--   0        0        0       27 2022-10-12 06:58:47.552893 postgresqlite-0.4.1/postgresqlite/__main__.py
--rw-r--r--   0        0        0      822 2023-06-14 15:03:54.088019 postgresqlite-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    16362 1970-01-01 00:00:00.000000 postgresqlite-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    15321 2023-06-14 10:26:48.369503 postgresqlite-0.4.2/README.md
+-rw-r--r--   0        0        0    19608 2023-06-14 15:08:20.630314 postgresqlite-0.4.2/postgresqlite/__init__.py
+-rw-r--r--   0        0        0       27 2022-10-12 06:58:47.552893 postgresqlite-0.4.2/postgresqlite/__main__.py
+-rw-r--r--   0        0        0      822 2023-06-14 15:07:46.957110 postgresqlite-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    16362 1970-01-01 00:00:00.000000 postgresqlite-0.4.2/PKG-INFO
```

### Comparing `postgresqlite-0.4.1/README.md` & `postgresqlite-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `postgresqlite-0.4.1/postgresqlite/__init__.py` & `postgresqlite-0.4.2/postgresqlite/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     def query_column(self, sql, **kwparams):
         cursor = self.cursor()
         result = cursor.query_column(sql, **kwparams)
         cursor.close()
         return result
 
 
-mark_start = "\u001b[31m"
-mark_end = "\u001b[0m"
+error_start_marker = "\u001b[31m"
+error_end_marker = "\u001b[0m"
 
 def get_exception_message(query, args, org_exception):
     msg = str(org_exception)
     
     match_m = re.search("'M': '((\\\\.|[^'])+)'", msg) # message
     if match_m:
         match_h = re.search("'H': '((\\\\.|[^'])+)'", msg) # hint
@@ -54,15 +54,15 @@
             start_pos = int(match_p.group(1))-1
             match_word = re.search('^[a-zA-Z_.]+|[^a-zA-Z_.]+', query[start_pos:])
             if match_word and match_word.group(0).strip():
                 end_pos = start_pos + len(match_word.group(0))
             else:
                 query = query[:start_pos] + "⚠" + query[start_pos:]
                 end_pos = start_pos + 1
-            query = query[0:start_pos] + self.mark_start  + query[start_pos:end_pos] + self.mark_end + query[end_pos:]
+            query = query[0:start_pos] + error_start_marker  + query[start_pos:end_pos] + error_end_marker + query[end_pos:]
 
     msg = f"{msg}\nFor query:\n\t" + query.replace("\n","\n\t")
     if args:
         msg += f"\nWith arguments: {args}"
     return msg
```

### Comparing `postgresqlite-0.4.1/pyproject.toml` & `postgresqlite-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgresqlite"
-version = "0.4.1"
+version = "0.4.2"
 description = "Python package that gives you the power of a PostgreSQL server, with the convenience of the sqlite3 package."
 authors = ["Frank van Viegen <pp@vanviegen.net>"]
 readme = "README.md"
 repository = "https://github.com/vanviegen/postgresqlite"
 documentation = "https://github.com/vanviegen/postgresqlite/blob/master/README.md#Documentation"
 classifiers = [
     'Development Status :: 4 - Beta',
```

### Comparing `postgresqlite-0.4.1/PKG-INFO` & `postgresqlite-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgresqlite
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python package that gives you the power of a PostgreSQL server, with the convenience of the sqlite3 package.
 Home-page: https://github.com/vanviegen/postgresqlite
 Author: Frank van Viegen
 Author-email: pp@vanviegen.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

