# Comparing `tmp/monarch_py-0.9.4.tar.gz` & `tmp/monarch_py-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.9.4.tar", max compression
+gzip compressed data, was "monarch_py-0.9.5.tar", max compression
```

## Comparing `monarch_py-0.9.4.tar` & `monarch_py-0.9.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      958 2023-06-13 21:39:38.786548 monarch_py-0.9.4/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-13 21:39:38.786548 monarch_py-0.9.4/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1150 2023-06-13 21:39:38.786548 monarch_py-0.9.4/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     7464 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0    11142 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     7317 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3321 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    20571 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     4630 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     1954 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     9254 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3330 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     3145 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3985 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4937 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 monarch_py-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      958 2023-06-13 23:20:16.128924 monarch_py-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1150 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     8330 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0    11142 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     7317 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3321 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    20571 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-13 23:20:16.128924 monarch_py-0.9.5/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     4630 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     1954 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     9891 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     4004 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     3145 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3985 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     5120 2023-06-13 23:20:16.132924 monarch_py-0.9.5/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 monarch_py-0.9.5/PKG-INFO
```

### Comparing `monarch_py-0.9.4/pyproject.toml` & `monarch_py-0.9.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.9.4"
+version = "0.9.5"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.9.4/src/monarch_py/association_type_mappings.yaml` & `monarch_py-0.9.5/src/monarch_py/association_type_mappings.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/cli.py` & `monarch_py-0.9.5/src/monarch_py/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 import importlib
 from pathlib import Path
 from typing import List, Optional
+from typing_extensions import Annotated
 
 import typer
 
 from monarch_py import solr_cli, sql_cli
+from monarch_py.utils.utils import set_log_level
 
 app = typer.Typer()
 app.add_typer(solr_cli.solr_app, name="solr")
 app.add_typer(sql_cli.sql_app, name="sql")
 
 
 @app.callback(invoke_without_command=True)
-def callback(version: Optional[bool] = typer.Option(None, "--version", is_eager=True)):
-    if version:
+def callback(
+    ctx: typer.Context,
+    version: Annotated[Optional[bool], typer.Option("--version", "-v", is_eager=True)] = None,
+    # verbose: Annotated[int, typer.Option("--verbose", "-v", count=True)] = 0,
+    quiet: Annotated[bool, typer.Option("--quiet", "-q", help="Set log level to warning")] = False,
+    debug: Annotated[bool, typer.Option("--debug", "-d", help="Set log level to debug")] = False,
+    ):
+    if version and ctx.invoked_subcommand is None:
         from monarch_py import __version__
-
         typer.echo(f"monarch_py version: {__version__}")
         raise typer.Exit()
+    if ctx.invoked_subcommand is None:
+        typer.secho(f"\n\tNo command specified\n\tTry `monarch --help` for more information.\n", fg=typer.colors.YELLOW)
+        raise typer.Exit()
+    log_level = "DEBUG" if debug else "WARNING" if quiet else "INFO"
+    set_log_level(log_level)
+
+
+@app.command("test")
+def test():
+    """Test the CLI"""
+    typer.secho("\n\tTesting monarch_py CLI\n", fg=typer.colors.GREEN)
 
 
 @app.command("schema")
 def schema():
     """
     Print the linkml schema for the data model
     """
@@ -33,15 +51,14 @@
     with open(schema_path, "r") as schema_file:
         print(schema_file.read())
     raise typer.Exit()
 
 
 ### "Aliases" for Solr CLI ###
 
-
 @app.command("entity")
 def entity(
     id: str = typer.Argument(None, help="The identifier of the entity to be retrieved"),
     fmt: str = typer.Option(
         "json",
         "--format",
         "-f",
```

### Comparing `monarch_py-0.9.4/src/monarch_py/datamodels/model.py` & `monarch_py-0.9.5/src/monarch_py/datamodels/model.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.9.5/src/monarch_py/datamodels/model.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/datamodels/solr.py` & `monarch_py-0.9.5/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.9.5/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.9.5/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.9.5/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.9.5/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.9.5/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.9.5/src/monarch_py/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/service/solr_service.py` & `monarch_py-0.9.5/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/solr_cli.py` & `monarch_py-0.9.5/src/monarch_py/solr_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 from typing import List
+from typing_extensions import Annotated
 
 import pystow
 import typer
 
 from monarch_py.datamodels.model import AssociationCountList
 from monarch_py.utils.solr_cli_utils import (
     check_solr_permissions,
     get_solr,
     solr_status,
     start_solr,
     stop_solr,
 )
-from monarch_py.utils.utils import console, format_output
+from monarch_py.utils.utils import console, format_output, set_log_level
 
 solr_app = typer.Typer()
 monarchstow = pystow.module("monarch")
 
+@solr_app.callback(invoke_without_command=True)
+def callback(
+    ctx: typer.Context,
+    quiet: Annotated[bool, typer.Option("--quiet", "-q", help="Set log level to warning")] = False,
+    debug: Annotated[bool, typer.Option("--debug", "-d", help="Set log level to debug")] = False,
+    ):
+    if ctx.invoked_subcommand is None:
+        typer.secho(f"\n\tNo command specified\n\tTry `monarch solr --help` for more information.\n", fg=typer.colors.YELLOW)
+        raise typer.Exit()
+    log_level = "DEBUG" if debug else "WARNING" if quiet else "INFO"
+    set_log_level(log_level)
+
 ############################
 ### SOLR DOCKER COMMANDS ###
 ############################
 
 
 @solr_app.command("start")
 def start(update: bool = False):
```

### Comparing `monarch_py-0.9.4/src/monarch_py/sql_cli.py` & `monarch_py-0.9.5/src/monarch_py/sql_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,29 @@
+from typing_extensions import Annotated
+
 import typer
 
 from monarch_py.implementations.sql.sql_implementation import SQLImplementation
-from monarch_py.utils.utils import console, format_output
+from monarch_py.utils.utils import console, format_output, set_log_level
 
 sql_app = typer.Typer()
+app_state = {"log_level": "WARNING"}
+
+
+@sql_app.callback(invoke_without_command=True)
+def callback(
+    ctx: typer.Context,
+    quiet: Annotated[bool, typer.Option("--quiet", "-q", help="Set log level to warning")] = False,
+    debug: Annotated[bool, typer.Option("--debug", "-d", help="Set log level to debug")] = False,
+    ):
+    if ctx.invoked_subcommand is None:
+        typer.secho(f"\n\tNo command specified\n\tTry `monarch sql --help` for more information.\n", fg=typer.colors.YELLOW)
+        raise typer.Exit()
+    log_level = "DEBUG" if debug else "WARNING" if quiet else "INFO"
+    set_log_level(log_level)
 
 
 @sql_app.command()
 def entity(
     id: str = typer.Argument(None, help="The identifier of the entity to be retrieved"),
     update: bool = typer.Option(
         False, "--update", "-u", help="Whether to re-download the Monarch KG"
```

### Comparing `monarch_py-0.9.4/src/monarch_py/utils/association_type_utils.py` & `monarch_py-0.9.5/src/monarch_py/utils/association_type_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.9.5/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.4/src/monarch_py/utils/utils.py` & `monarch_py-0.9.5/src/monarch_py/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,26 @@
 
 def dict_factory(cursor, row):
     """Converts a sqlite3 row to a dictionary."""
     fields = [column[0] for column in cursor.description]
     return {key: value for key, value in zip(fields, row)}
 
 
+def set_log_level(log_level: str):
+    """Sets the log level for the application."""
+    import loguru
+
+    loguru.logger.remove()
+    loguru.logger.add(sys.stderr, level=log_level)
+
+
 ### Output conversion methods ###
 
 FMT_INPUT_ERROR_MSG = "Text conversion method only accepts Entity, HistoPheno, AssociationCountList, or Results objects."
 
-
 def get_headers_from_obj(obj: ConfiguredBaseModel) -> list:
     """Return a list of headers from a pydantic model."""
     schema = type(obj).schema()
     definitions = schema["definitions"]
     this_ref = schema["properties"]["items"]["items"]["$ref"].split("/")[-1]
     headers = definitions[this_ref]["properties"].keys()
     return list(headers)
```

### Comparing `monarch_py-0.9.4/PKG-INFO` & `monarch_py-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.9.4
+Version: 0.9.5
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

