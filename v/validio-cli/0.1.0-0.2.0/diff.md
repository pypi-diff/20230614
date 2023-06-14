# Comparing `tmp/validio_cli-0.1.0.tar.gz` & `tmp/validio_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_cli-0.1.0.tar", max compression
+gzip compressed data, was "validio_cli-0.2.0.tar", max compression
```

## Comparing `validio_cli-0.1.0.tar` & `validio_cli-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0    11340 2023-06-12 09:21:56.805572 validio_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     1738 2023-06-12 09:22:07.597616 validio_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5347 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/__init__.py
--rw-r--r--   0        0        0     1327 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/channels.py
--rw-r--r--   0        0        0    11656 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/code.py
--rw-r--r--   0        0        0     3897 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/config.py
--rw-r--r--   0        0        0     1171 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/credentials.py
--rw-r--r--   0        0        0     1176 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/destinations.py
--rw-r--r--   0        0        0     1716 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/notification_rules.py
--rw-r--r--   0        0        0     3110 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/recommendations.py
--rw-r--r--   0        0        0     1726 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/segmentations.py
--rw-r--r--   0        0        0    25068 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/sources.py
--rw-r--r--   0        0        0     1174 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/users.py
--rw-r--r--   0        0        0     2470 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/validators.py
--rw-r--r--   0        0        0     1686 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/windows.py
--rw-r--r--   0        0        0     2747 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/main.py
--rw-r--r--   0        0        0     2587 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/components.py
--rw-r--r--   0        0        0      265 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/metadata.py
--rw-r--r--   0        0        0     1382 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/schema.py
--rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 validio_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-06-14 09:21:19.092511 validio_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0      227 2023-06-14 09:21:19.092511 validio_cli-0.2.0/README_PUBLIC.md
+-rw-r--r--   0        0        0     1805 2023-06-14 09:21:30.028421 validio_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5400 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/__init__.py
+-rw-r--r--   0        0        0     1514 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/channels.py
+-rw-r--r--   0        0        0    11640 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/code.py
+-rw-r--r--   0        0        0     4335 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/config.py
+-rw-r--r--   0        0        0     1418 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/credentials.py
+-rw-r--r--   0        0        0     1423 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/destinations.py
+-rw-r--r--   0        0        0     1961 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/notification_rules.py
+-rw-r--r--   0        0        0     3335 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/recommendations.py
+-rw-r--r--   0        0        0     2022 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/segmentations.py
+-rw-r--r--   0        0        0    26909 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/sources.py
+-rw-r--r--   0        0        0     1174 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/users.py
+-rw-r--r--   0        0        0     2861 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/validators.py
+-rw-r--r--   0        0        0     1933 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/entities/windows.py
+-rw-r--r--   0        0        0     2871 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/bin/main.py
+-rw-r--r--   0        0        0     2587 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/components.py
+-rw-r--r--   0        0        0      265 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/metadata.py
+-rw-r--r--   0        0        0      630 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/namespace.py
+-rw-r--r--   0        0        0     1382 2023-06-14 09:21:19.092511 validio_cli-0.2.0/validio_cli/schema.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.2.0/PKG-INFO
```

### Comparing `validio_cli-0.1.0/LICENSE` & `validio_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_cli-0.1.0/pyproject.toml` & `validio_cli-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "validio-cli"
-version = "0.1.0"
+version = "0.2.0"
 description = "CLI tool to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://docs.validio.io/"
 packages = [{include = "validio_cli"}]
+readme = "README_PUBLIC.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 camel-converter = "^3.0.0"
 classdiff = "^0.2.0"
 validio-sdk = "*"
 typer = {extras = ["all"], version = "^0.7.0"}
@@ -65,7 +66,10 @@
 # No need for documentation in these files
 "__init__.py" = [ "D" ]
 "*/bin/*.py" = [ "D" ]
 "examples/*.py" = [ "D" ]
 
 [tool.black]
 preview = true
+
+[tool.mypy]
+plugins = "pydantic.mypy"
```

### Comparing `validio_cli-0.1.0/validio_cli/__init__.py` & `validio_cli-0.2.0/validio_cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from camel_converter import to_snake
 from tabulate import tabulate
 from validio_sdk import config
 from validio_sdk.config import Config, ValidioConfig
 from validio_sdk.util import ClassJSONEncoder
 from validio_sdk.validio_client import ValidioAPIClient
 
+DEFAULT_NAMESPACE: str = "default"
+
 
 class OutputFormat(str, Enum):
     """Available output formats for the CLI"""
 
     JSON = "json"
     TEXT = "text"
 
@@ -28,16 +30,17 @@
 ConfigDir = typer.Option(
     config.default_config_dir,
     "--config-dir",
     "-c",
     help="Path to where config is stored",
 )
 OutputFormatOption = typer.Option(
-    OutputFormat.TEXT.value, "--output-format", "-o", help="Output format"
+    OutputFormat.TEXT.value, "--output", "-o", help="Output format"
 )
+Namespace = typer.Option(None, "--namespace", "-n", help="Namespace to target")
 Identifier = typer.Argument(
     default=None, help="Name or ID of the resource to get of this type"
 )
 
 
 class AsyncTyper(typer.Typer):
     """
@@ -59,17 +62,14 @@
         return decorator
 
 
 async def get_client_and_config(
     config_dir: str = ConfigDir,
 ) -> tuple[ValidioAPIClient, ValidioConfig]:
     cfg = Config(Path(config_dir)).read()
-    if cfg is None:
-        raise Exception("TODO...")
-
     vc = ValidioAPIClient(validio_config=cfg)
 
     return (vc, cfg)
 
 
 @dataclass
 class OutputSettings:
```

### Comparing `validio_cli-0.1.0/validio_cli/bin/entities/channels.py` & `validio_cli-0.2.0/validio_cli/bin/entities/channels.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import typer
 from camel_converter import to_snake
+from validio_sdk.graphql_client.input_types import ResourceFilter
 
 from validio_cli import (
     AsyncTyper,
     ConfigDir,
     Identifier,
+    Namespace,
     OutputFormat,
     OutputFormatOption,
     OutputSettings,
     get_client_and_config,
     output_json,
     output_text,
 )
+from validio_cli.namespace import get_namespace
 
 app = AsyncTyper(help="Channels used for notifications")
 
 
 @app.async_command(help="Get channels")
 async def get(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    namespace: str = Namespace,
     identifier: str = Identifier,
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
+    ns = get_namespace(namespace, cfg)
 
     if identifier is not None:
-        # TODO(VR-2078): Don't hard code namespace
         channels = await vc.get_channel_by_resource_name(
-            resource_name=identifier, resource_namespace="default"
+            resource_name=identifier, resource_namespace=ns
         )
     else:
-        channels = await vc.get_channels()
+        channels = await vc.get_channels(filter=ResourceFilter(resourceNamespace=ns))
 
     if output_format == OutputFormat.JSON:
         return output_json(channels)
 
     return output_text(
         channels,
         fields={
```

### Comparing `validio_cli-0.1.0/validio_cli/bin/entities/code.py` & `validio_cli-0.2.0/validio_cli/bin/entities/code.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,54 +37,54 @@
     ),
 )
 
 no_capture_option: bool = typer.Option(
     False,
     help=(
         "By default, the code program's stdout output is hidden; "
-        "the output can be recovered by enabling this parameter"
+        "enable this parameter to recover the output"
     ),
 )
 
 show_schema_option = typer.Option(
-    False, help="Show the JTD schema in the plan output for sources"
+    False, help="Show the JTD schema in the plan output for Sources"
 )
 
 diff_option = typer.Option(
     DiffOutput.CHANGES.value,
     "--diff",
-    help="Show only the changed lines (added, removed or modified)",
+    help="Show only the changed lines (added, removed, or modified)",
 )
 
 destroy_option = typer.Option(
-    False, help="Deletes all resources belonging to the project"
+    False, help="Deletes all resources associated with the project"
 )
 
 show_secrets_option = typer.Option(
     False,
     help=(
         "By default, secret values within credentials are not shown; "
-        "they will be shown by enabling this parameter"
+        "enable this parameter to show the values"
     ),
 )
 
 update_schema_option = typer.Option(
     None,
     help=(
         "Specify a Source name to update its schema. This checks the upstream data"
-        " source for any schema changes before planning. Multiple sources can be"
-        " specified by using --update-schema src1 --update-schema src2."
+        " source for any schema changes before planning. You can use"
+        " --update-schema src1 --update-schema src2 to specify multiple Sources."
     ),
 )
 
 update_all_schemas_option = typer.Option(
     False,
     help=(
         "Similar to --update-schema. Checks for schema "
-        "updates for all sources before planning"
+        "updates for all Sources before planning"
     ),
 )
 
 
 @app.command()
 def init(
     directory: str = directory_option,
@@ -169,15 +169,15 @@
     )
 
     if diff.num_operations() == 0:
         return
 
     print()
     print("Do you want to perform these operations?")
-    print("\tOnly 'yes' will be accepted to approve")
+    print("\tOnly 'yes' is accepted to approve")
 
     if not auto_approve:
         session: prompt_toolkit.PromptSession = prompt_toolkit.PromptSession()
         p = await session.prompt_async("Enter a value: ")
         if p != "yes":
             print("Cancelled")
             return
@@ -226,15 +226,15 @@
         schema_reinference=schema_reinference,
         destroy=destroy,
         no_capture=no_capture,
         show_secrets=show_secrets,
     )
 
     if diff.num_operations() == 0:
-        print("No changes. Configuration is up-to-date!")
+        print("No changes. The configuration is up-to-date!")
         return diff, manifest_ctx
 
     _show_resources_diff(
         diff=diff,
         show_schema=show_schema,
         show_secrets=show_secrets,
         escape=sys.stdout.isatty(),
```

### Comparing `validio_cli-0.1.0/validio_cli/bin/entities/config.py` & `validio_cli-0.2.0/validio_cli/bin/entities/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     except ConfigNotFoundError:
         if confirm("🚫 No configuration found - do you want to create one?"):
             return create_or_update(default_config_path)
 
         raise typer.Exit(code=1)
     except ConfigInvalidError:
         if confirm(
-            "🚨 Configuration found but is in valid - do you want to delete it and"
+            "🚨 Configuration found, but is not valid - do you want to delete it and"
             " create a new one?"
         ):
             cfg.remove()
             return create_or_update(default_config_path)
 
         raise typer.Exit(code=1)
 
@@ -76,24 +76,37 @@
         if not value:
             return "⚠️  \033[91m{}\033[0m".format("MISSING")
 
         return value
 
     table: Iterable[Iterable[Any]] = [
         ["Path", cfg.config_path],
+        ["Default namespace", validio_config.default_namespace],
         ["Endpoint", _highlight_if_missing(validio_config.endpoint)],
         ["Access key", _highlight_if_missing(validio_config.access_key)],
         ["Access secret", _highlight_if_missing(validio_config.access_secret)],
     ]
 
     print(tabulate(table))
 
     return None
 
 
+def set_default_namespace(namespace: str, default_config_path: str | None = None):
+    config_path = Path(default_config_path) if default_config_path is not None else None
+    cfg = Config(config_path)
+
+    validio_config = cfg.read()
+    validio_config.default_namespace = namespace
+
+    cfg.write(validio_config)
+
+    print(f"Default namespace set to '{namespace}'")
+
+
 def _prompt_for_config(current_config: ValidioConfig | None) -> ValidioConfig:
     if current_config is None:
         current_config = ValidioConfig()
 
     endpoint_completer = WordCompleter(["http://localhost:8889"])
 
     current_config.endpoint = prompt(
```

### Comparing `validio_cli-0.1.0/validio_cli/bin/entities/notification_rules.py` & `validio_cli-0.2.0/validio_cli/bin/entities/notification_rules.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 import typer
 from camel_converter import to_snake
+from validio_sdk.graphql_client.input_types import ResourceFilter
 
 from validio_cli import (
     AsyncTyper,
     ConfigDir,
     Identifier,
+    Namespace,
     OutputFormat,
     OutputFormatOption,
     OutputSettings,
     _single_resource_if_specified,
     get_client_and_config,
     output_json,
     output_text,
 )
+from validio_cli.namespace import get_namespace
 
 app = AsyncTyper(help="Notification rules for incidents")
 
 
 @app.async_command(help="Get notification rules")
 async def get(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    namespace: str = Namespace,
     identifier: str = Identifier,
     source: str = typer.Option(
-        None, help="List notification rules for this source (id)"
+        None, help="List notification rules for this source (ID)"
     ),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
     # TODO: Get a single resource by id/name to not have to list.
-    notification_rules = await vc.get_notification_rules_v2()
+    notification_rules = await vc.get_notification_rules(
+        filter=ResourceFilter(resource_namespace=get_namespace(namespace, cfg))
+    )
     notification_rules = [
         nr
         for nr in notification_rules
         if source is None or (nr is not None and source in nr.sources)
     ]
     notification_rules = _single_resource_if_specified(notification_rules, identifier)
```

### Comparing `validio_cli-0.1.0/validio_cli/bin/entities/recommendations.py` & `validio_cli-0.2.0/validio_cli/bin/entities/recommendations.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import typer
 from validio_sdk.graphql_client import input_types
 
 from validio_cli import (
     AsyncTyper,
     ConfigDir,
     Identifier,
+    Namespace,
     OutputFormat,
     OutputFormatOption,
     OutputSettings,
     _single_resource_if_specified,
     get_client_and_config,
     output_json,
     output_text,
 )
 from validio_cli.bin.entities import sources
 
-app = AsyncTyper(help="Recommended validators for your sources")
+app = AsyncTyper(help="Recommended validators for your Sources")
 
 APPLY_RESULT_SUCCEEDED = "SUCCEEDED"
 APPLY_RESULT_FAILED = "FAILED"
 
 
 @dataclass
 class ApplyResult:
@@ -31,25 +32,28 @@
     state: str
 
 
 @app.async_command(help="List all recommendations")
 async def get(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    # ruff: noqa:  ARG001
+    namespace: str = Namespace,
     identifier: str = Identifier,
     source: str = typer.Option(
-        ..., help="List recommendations for this source (id or name)"
+        ..., help="List recommendations for this Source (ID or name)"
     ),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    source_id = await sources._get_source_id(vc, source)
+    source_id = await sources._get_source_id(vc, cfg, source, namespace)
     if source_id is None:
         return None
 
+    # TODO: Add namespace support in API
     recommendations = await vc.get_source_recommended_validators(id=source_id)
 
     # TODO: Add endpoint to get a single recommendation by id
     if recommendations is not None:
         recommendations = _single_resource_if_specified(
             recommendations.recommended_validators, identifier
         )
@@ -70,20 +74,23 @@
     )
 
 
 @app.async_command(help="Apply recommendations")
 async def apply(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    # ruff: noqa:  ARG001
+    namespace: str = Namespace,
     ids: list[str] = typer.Option(
-        ..., "--id", help="Recommendations to apply (ids), can supports multiple values"
+        ..., "--id", help="Recommendations to apply (IDs), supports multiple values"
     ),
 ):
     vc, _ = await get_client_and_config(config_dir)
 
+    # TODO: Add support for namespace.
     api_result = await vc.apply_validator_recommendation(
         input=input_types.ValidatorRecommendationApplyInput(ids=ids)
     )
 
     result = []
     seen_ids = set()
```

### Comparing `validio_cli-0.1.0/validio_cli/bin/entities/segmentations.py` & `validio_cli-0.2.0/validio_cli/bin/entities/segmentations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from typing import Any
 
 import typer
+from validio_sdk.graphql_client.input_types import ResourceFilter
 
 import validio_cli
 from validio_cli import (
     AsyncTyper,
     ConfigDir,
     Identifier,
+    Namespace,
     OutputFormat,
     OutputFormatOption,
     OutputSettings,
     _single_resource_if_specified,
     get_client_and_config,
     output_json,
     output_text,
 )
+from validio_cli.namespace import get_namespace
 
 app = AsyncTyper(help="Segmentation to group data")
 
 
-@app.async_command(help="List all segmentations")
+@app.async_command(help="List all Segmentations")
 async def get(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    namespace: str = Namespace,
     identifier: str = Identifier,
     source: str = typer.Option(
-        None, help="List segmentations for this source (id or name)"
+        None, help="List Segmentations for this Source (ID or name)"
     ),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
     segmentations: list[Any] = []
 
     # TODO: UI-1957
     # We don't want to get all resources if identifier is not id.
+    # TODO: Add namespace support in API
     if identifier is not None and identifier.startswith("SGM_"):
         segmentations = [await vc.get_segmentation(id=identifier)]
     else:
-        segmentations = await vc.list_segmentations()
+        segmentations = await vc.list_segmentations(
+            filter=ResourceFilter(resourceNamespace=get_namespace(namespace, cfg))
+        )
 
     segmentations = [
         segmentation
         for segmentation in segmentations
         if segmentation is not None
         and validio_cli._resource_filter(segmentation, ["source"], source)
     ]
```

### Comparing `validio_cli-0.1.0/validio_cli/bin/entities/sources.py` & `validio_cli-0.2.0/validio_cli/bin/entities/sources.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,74 +4,84 @@
 from pathlib import Path
 from typing import Any
 
 import click
 import typer
 from prompt_toolkit import PromptSession
 from prompt_toolkit.completion import WordCompleter
+from validio_sdk.config import ValidioConfig
 from validio_sdk.graphql_client.input_types import (
     AwsKinesisInferSchemaInput,
     AwsRedshiftInferSchemaInput,
     AwsS3InferSchemaInput,
     CsvParserInput,
     GcpBigQueryInferSchemaInput,
     GcpStorageInferSchemaInput,
     PostgreSqlInferSchemaInput,
+    ResourceFilter,
     SnowflakeInferSchemaInput,
 )
 from validio_sdk.validio_client import ValidioAPIClient
 
 import validio_cli
 from validio_cli import (
     AsyncTyper,
     ConfigDir,
     Identifier,
+    Namespace,
     OutputFormat,
     OutputFormatOption,
     OutputSettings,
     _single_resource_if_specified,
     components,
     get_client_and_config,
     output_json,
     output_text,
 )
+from validio_cli.namespace import get_namespace
 
-app = AsyncTyper(help="Sources where data is ingested from")
+app = AsyncTyper(help="Sources that Validio reads data from")
 
 infer_schema_app = AsyncTyper(help="Infer schema")
 app.add_typer(infer_schema_app, no_args_is_help=True, name="infer-schema")
 
 
-def schema_output_option(schema_type: str):
+def schema_filename_option(schema_type: str):
     return typer.Option(
         Path(Path.cwd(), f"{schema_type}_{uuid.uuid4()}.json"),
-        help="Output path for inferred schema",
+        "--filename",
+        "-f",
+        help="Filename including path for where to write inferred schema",
     )
 
 
-@app.async_command(help="List all sources")
+@app.async_command(help="List all Sources")
 async def get(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    namespace: str = Namespace,
     identifier: str = Identifier,
-    credential_id: str = typer.Option(None, help="List sources for this credential id"),
+    credential_id: str = typer.Option(None, help="List Sources for this credential ID"),
     credential_name: str = typer.Option(
-        None, help="List sources for this credential name"
+        None, help="List Sources for this credential name"
     ),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
     sources: list[Any] = []
 
     # TODO: UI-1957
     # We don't want to get all resources if identifier is not id.
+    # TODO: Add support for namespace
     if identifier is not None and identifier.startswith("SRC_"):
         sources = [await vc.get_source(id=identifier)]
     else:
-        sources = await vc.list_sources()
+        sources = await vc.list_sources(
+            filter=ResourceFilter(resource_namespace=get_namespace(namespace, cfg))
+        )
 
     sources = [
         source
         for source in sources
         if _resource_filter(source, credential_id, credential_name)
     ]
     sources = _single_resource_if_specified(sources, identifier)
@@ -90,102 +100,116 @@
     )
 
 
 @app.async_command(help="Start source")
 async def start(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    # ruff: noqa: ARG001
+    namespace: str = Namespace,
     identifier: str = Identifier,
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    source_id = await _get_source_id(vc, identifier)
+    source_id = await _get_source_id(vc, cfg, identifier, namespace)
     if source_id is None:
         return None
 
+    # TODO: Add support for namespace
     result = await vc.start_source(id=source_id)
 
     if output_format == OutputFormat.JSON:
         return output_json(result)
 
     return print(result.state.value)
 
 
 @app.async_command(help="Stop source")
 async def stop(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    # ruff: noqa: ARG001
+    namespace: str = Namespace,
     identifier: str = Identifier,
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    source_id = await _get_source_id(vc, identifier)
+    source_id = await _get_source_id(vc, cfg, identifier, namespace)
     if source_id is None:
         return None
 
+    # TODO: Add support for namespace
     result = await vc.stop_source(id=source_id)
 
     if output_format == OutputFormat.JSON:
         return output_json(result)
 
     return print(result.state.value)
 
 
 @app.async_command(help="Backfill source")
 async def backfill(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    # ruff: noqa: ARG001
+    namespace: str = Namespace,
     identifier: str = Identifier,
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    source_id = await _get_source_id(vc, identifier)
+    source_id = await _get_source_id(vc, cfg, identifier, namespace)
     if source_id is None:
         return None
 
+    # TODO: Add support for namespace
     result = await vc.backfill_source(id=source_id)
 
     if output_format == OutputFormat.JSON:
         return output_json(result)
 
     return print(result.state.value)
 
 
 @infer_schema_app.callback(invoke_without_command=True)
 def main(
     interactive: bool = typer.Option(
         False, "--interactive", "-i", help="Infer schema with an interactive prompt"
     ),
     config_dir: str = ConfigDir,
-    output: Path = schema_output_option("schema"),
+    filename: Path = schema_filename_option("schema"),
+    namespace: str = Namespace,
 ) -> None:
     ctx = click.get_current_context()
 
     # A subcommand was run prior to this, nothing todo
     if ctx.invoked_subcommand is not None:
         return None
 
     # The interactive flag was used, run the interactive version
     if interactive:
-        return asyncio.run(_interactive(config_dir, output))
+        return asyncio.run(_interactive(config_dir, filename, namespace))
 
     # A flag for this command was used but not interactive, print the help as if
     # no command was given
     click.echo(ctx.get_help())
 
     return None
 
 
-async def _interactive(
-    config_dir: str,
-    output: Path,
-):
-    vc, _ = await get_client_and_config(config_dir)
+async def _interactive(config_dir: str, filename: Path, namespace: str):
+    vc, cfg = await get_client_and_config(config_dir)
+
+    credentials = await vc.list_credentials(
+        filter=ResourceFilter(resourceNamespace=get_namespace(namespace, cfg))
+    )
+
+    if len(credentials) == 0:
+        print(f"No credentials found in namespace {namespace}")
+        raise typer.Exit(code=0)
 
-    credentials = await vc.list_credentials()
     credential_name_to_id = [(c.id, c.name) for c in credentials]
 
     credential_id = await components.radiolist_dialog(
         title="Credentials to use",
         values=credential_name_to_id,
         navigation_help=True,
     )
@@ -231,15 +255,15 @@
         inference_type = credential_type_to_source_type[credential_type][0][0]
 
     if inference_type is None:
         return
 
     match inference_type:
         case "demo":
-            await _infer_schema_demo(vc, output)
+            await _infer_schema_demo(vc, filename)
         case "kinesis":
             info = await _multip_prompt(
                 [
                     (
                         "Region",
                         # https://docs.aws.amazon.com/general/latest/gr/ak.html
                         [
@@ -276,15 +300,15 @@
                         "",
                     ),
                     ("Stream name", [], ""),
                 ]
             )
             await _infer_schema_kinesis(
                 vc,
-                output,
+                filename,
                 credential_id,
                 info.get("region", ""),
                 info.get("stream_name", ""),
             )
         case "s3":
             info = await _multip_prompt(
                 [
@@ -296,15 +320,15 @@
             )
 
             print()
             null_marker = await _get_null_marker()
 
             await _infer_schema_s3(
                 vc,
-                output,
+                filename,
                 credential_id,
                 info.get("bucket", ""),
                 info.get("file_pattern", ""),
                 info.get("prefix", ""),
                 info.get("csv_delimiter", ""),
                 null_marker,
             )
@@ -314,15 +338,15 @@
                     ("Schema", [], ""),
                     ("Database", [], ""),
                     ("Table", [], ""),
                 ]
             )
             await _infer_schema_postgresql(
                 vc,
-                output,
+                filename,
                 credential_id,
                 info.get("schema", ""),
                 info.get("database", ""),
                 info.get("table", ""),
             )
         case "redshift":
             info = await _multip_prompt(
@@ -330,15 +354,15 @@
                     ("Schema", [], ""),
                     ("Database", [], ""),
                     ("Table", [], ""),
                 ]
             )
             await _infer_schema_redshift(
                 vc,
-                output,
+                filename,
                 credential_id,
                 info.get("schema", ""),
                 info.get("database", ""),
                 info.get("table", ""),
             )
         case "snowflake":
             info = await _multip_prompt(
@@ -348,15 +372,15 @@
                     ("Table", [], ""),
                     ("Warehouse", [], ""),
                     ("Role", [], ""),
                 ]
             )
             await _infer_schema_snowflake(
                 vc,
-                output,
+                filename,
                 credential_id,
                 info.get("schema", ""),
                 info.get("database", ""),
                 info.get("table", ""),
                 info.get("role", ""),
                 info.get("warehouse", ""),
             )
@@ -366,15 +390,15 @@
                     ("Project", [], ""),
                     ("Dataset", [], ""),
                     ("Table", [], ""),
                 ]
             )
             await _infer_schema_bigquery(
                 vc,
-                output,
+                filename,
                 credential_id,
                 info.get("project", ""),
                 info.get("dataset", ""),
                 info.get("table", ""),
             )
         case "gcs":
             info = await _multip_prompt(
@@ -388,15 +412,15 @@
             )
 
             print()
             null_marker = await _get_null_marker()
 
             await _infer_schema_gcs(
                 vc,
-                output,
+                filename,
                 credential_id,
                 info.get("project", ""),
                 info.get("bucket", ""),
                 info.get("folder", ""),
                 info.get("file_pattern", ""),
                 info.get("csv_delimiter", ""),
                 null_marker,
@@ -405,342 +429,351 @@
             print("Not yet implemented...")
             return
 
 
 @infer_schema_app.async_command(help="Infer Demo schema")
 async def demo(
     config_dir: str = ConfigDir,
-    output: Path = schema_output_option("demo"),
+    filename: Path = schema_filename_option("demo"),
 ):
     vc, _ = await get_client_and_config(config_dir)
-    await _infer_schema_demo(vc, output)
+    await _infer_schema_demo(vc, filename)
 
 
 @infer_schema_app.async_command(help="Infer Amazon S3 schema")
 async def s3(
     config_dir: str = ConfigDir,
-    output: Path = schema_output_option("s3"),
+    filename: Path = schema_filename_option("s3"),
+    namespace: str = Namespace,
     credential_id: str = typer.Option(..., help="Credential name or ID"),
     bucket: str = typer.Option(..., help="S3 bucket name"),
     file_pattern: str = typer.Option(
         "*.csv", help="File glob pattern - files to use for inference"
     ),
     prefix: str = typer.Option("", help="Prefix in the bucket, a directory"),
     csv_delimiter: str = typer.Option(",", help="Delimiter between columns in file"),
     null_marker: str = typer.Option(None, help="Null marker (values to treat as NULL)"),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    resolved_credential_id = await _get_credential_id(vc, credential_id)
+    resolved_credential_id = await _get_credential_id(vc, cfg, credential_id, namespace)
     if resolved_credential_id is None:
         return
 
     await _infer_schema_s3(
         vc,
-        output,
+        filename,
         resolved_credential_id,
         bucket,
         file_pattern,
         prefix,
         csv_delimiter,
         null_marker,
     )
 
 
 @infer_schema_app.async_command(help="Infer Amazon Kinesis schema")
 async def kinesis(
     config_dir: str = ConfigDir,
-    output: Path = schema_output_option("kinesis"),
+    filename: Path = schema_filename_option("kinesis"),
     credential_id: str = typer.Option(..., help="Credential name or ID"),
     region: str = typer.Option(..., help="AWS region"),
     stream_name: str = typer.Option(..., help="AWS Kinesis stream name"),
+    namespace: str = Namespace,
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    resolved_credential_id = await _get_credential_id(vc, credential_id)
+    resolved_credential_id = await _get_credential_id(vc, cfg, credential_id, namespace)
     if resolved_credential_id is None:
         return
 
-    await _infer_schema_kinesis(vc, output, resolved_credential_id, region, stream_name)
+    await _infer_schema_kinesis(
+        vc, filename, resolved_credential_id, region, stream_name
+    )
 
 
 @infer_schema_app.async_command(help="Infer PostgreSQL schema")
 async def postgresql(
     config_dir: str = ConfigDir,
-    output: Path = schema_output_option("postgresql"),
+    filename: Path = schema_filename_option("postgresql"),
+    namespace: str = Namespace,
     credential_id: str = typer.Option(..., help="Credential name or ID"),
     schema: str = typer.Option(..., help="Schema name"),
     database: str = typer.Option(..., help="Database name"),
     table: str = typer.Option(..., help="Table name"),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    resolved_credential_id = await _get_credential_id(vc, credential_id)
+    resolved_credential_id = await _get_credential_id(vc, cfg, credential_id, namespace)
     if resolved_credential_id is None:
         return
 
     await _infer_schema_postgresql(
-        vc, output, resolved_credential_id, schema, database, table
+        vc, filename, resolved_credential_id, schema, database, table
     )
 
 
 @infer_schema_app.async_command(help="Infer Amazon Redshift schema")
 async def redshift(
     config_dir: str = ConfigDir,
-    output: Path = schema_output_option("redshift"),
+    filename: Path = schema_filename_option("redshift"),
+    namespace: str = Namespace,
     credential_id: str = typer.Option(..., help="Credential name or ID"),
     schema: str = typer.Option(..., help="Schema name"),
     database: str = typer.Option(..., help="Database name"),
     table: str = typer.Option(..., help="Table name"),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    resolved_credential_id = await _get_credential_id(vc, credential_id)
+    resolved_credential_id = await _get_credential_id(vc, cfg, credential_id, namespace)
     if resolved_credential_id is None:
         return
 
     await _infer_schema_redshift(
-        vc, output, resolved_credential_id, schema, database, table
+        vc, filename, resolved_credential_id, schema, database, table
     )
 
 
 @infer_schema_app.async_command(help="Infer Snowflake schema")
 async def snowflake(
     config_dir: str = ConfigDir,
-    output: Path = schema_output_option("snowflake"),
+    filename: Path = schema_filename_option("snowflake"),
+    namespace: str = Namespace,
     credential_id: str = typer.Option(..., help="Credential name or ID"),
     schema: str = typer.Option(..., help="Schema name"),
     database: str = typer.Option(..., help="Database name"),
     table: str = typer.Option(..., help="Table name"),
     role: str = typer.Option(..., help="Role name"),
     warehouse: str = typer.Option(..., help="Warehouse name"),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    resolved_credential_id = await _get_credential_id(vc, credential_id)
+    resolved_credential_id = await _get_credential_id(vc, cfg, credential_id, namespace)
     if resolved_credential_id is None:
         return
 
     await _infer_schema_snowflake(
-        vc, output, credential_id, schema, database, table, role, warehouse
+        vc, filename, credential_id, schema, database, table, role, warehouse
     )
 
 
 @infer_schema_app.async_command(help="Infer Google BigQuery schema")
 async def bigquery(
     config_dir: str = ConfigDir,
-    output: Path = schema_output_option("bigquery"),
+    filename: Path = schema_filename_option("bigquery"),
+    namespace: str = Namespace,
     credential_id: str = typer.Option(..., help="Credential name or ID"),
     project: str = typer.Option(..., help="Google project name"),
     dataset: str = typer.Option(..., help="Dataset name"),
     table: str = typer.Option(..., help="Table name"),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    resolved_credential_id = await _get_credential_id(vc, credential_id)
+    resolved_credential_id = await _get_credential_id(vc, cfg, credential_id, namespace)
     if resolved_credential_id is None:
         return
 
     await _infer_schema_bigquery(
-        vc, output, resolved_credential_id, project, dataset, table
+        vc, filename, resolved_credential_id, project, dataset, table
     )
 
 
 @infer_schema_app.async_command(help="Infer Google Cloud Storage schema")
 async def gcs(
     config_dir: str = ConfigDir,
-    output: Path = schema_output_option("gcs"),
+    filename: Path = schema_filename_option("gcs"),
+    namespace: str = Namespace,
     credential_id: str = typer.Option(..., help="Credential name or ID"),
     project: str = typer.Option(..., help="Google project name"),
     bucket: str = typer.Option(..., help="GCS bucket"),
     folder: str = typer.Option("", help="Folder in the bucket"),
     file_pattern: str = typer.Option("*.csv", help="File glob"),
     csv_delimiter: str = typer.Option(",", help="Delimiter between columns in file"),
     null_marker: str = typer.Option(None, help="Null marker (values to treat as NULL)"),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
-    resolved_credential_id = await _get_credential_id(vc, credential_id)
+    resolved_credential_id = await _get_credential_id(vc, cfg, credential_id, namespace)
     if resolved_credential_id is None:
         return
 
     await _infer_schema_gcs(
         vc,
-        output,
+        filename,
         resolved_credential_id,
         project,
         bucket,
         folder,
         file_pattern,
         csv_delimiter,
         null_marker,
     )
 
 
 async def _infer_schema_demo(
     vc: ValidioAPIClient,
-    output: Path,
+    filename: Path,
 ):
     schema = await vc.infer_demo_schema()
-    _write_schema(output, schema)
+    _write_schema(filename, schema)
 
 
 async def _infer_schema_s3(
     vc: ValidioAPIClient,
-    output: Path,
+    filename: Path,
     credential_id: str,
     bucket: str,
     file_pattern: str,
     prefix: str,
     csv_delimiter: str,
     null_marker: str | None,
 ):
     schema = await vc.infer_aws_s3_schema(
         AwsS3InferSchemaInput(
-            credentialId=credential_id,
+            credential_id=credential_id,
             bucket=bucket,
-            filePattern=file_pattern,
+            file_pattern=file_pattern,
             prefix=prefix,
             csv=CsvParserInput(
                 delimiter=csv_delimiter,
-                nullMarker=null_marker,
+                null_marker=null_marker,
             ),
         )
     )
-    _write_schema(output, schema)
+    _write_schema(filename, schema)
 
 
 async def _infer_schema_kinesis(
     vc: ValidioAPIClient,
-    output: Path,
+    filename: Path,
     credential_id: str,
     region: str,
     stream_name: str,
 ):
     schema = await vc.infer_aws_kinesis_schema(
         AwsKinesisInferSchemaInput(
-            credentialId=credential_id,
+            credential_id=credential_id,
             region=region,
-            streamName=stream_name,
+            stream_name=stream_name,
         )
     )
-    _write_schema(output, schema)
+    _write_schema(filename, schema)
 
 
 async def _infer_schema_postgresql(
     vc: ValidioAPIClient,
-    output: Path,
+    filename: Path,
     credential_id: str,
     db_schema: str,
     database: str,
     table: str,
 ):
     schema = await vc.infer_postgre_sql_schema(
         PostgreSqlInferSchemaInput(
-            credentialId=credential_id,
-            schema=db_schema,
+            credential_id=credential_id,
+            db_schema=db_schema,
             database=database,
             table=table,
         )
     )
-    _write_schema(output, schema)
+    _write_schema(filename, schema)
 
 
 async def _infer_schema_redshift(
     vc: ValidioAPIClient,
-    output: Path,
+    filename: Path,
     credential_id: str,
     db_schema: str,
     database: str,
     table: str,
 ):
     schema = await vc.infer_aws_redshift_schema(
         AwsRedshiftInferSchemaInput(
-            credentialId=credential_id,
-            schema=db_schema,
+            credential_id=credential_id,
+            db_schema=db_schema,
             database=database,
             table=table,
         )
     )
-    _write_schema(output, schema)
+    _write_schema(filename, schema)
 
 
 async def _infer_schema_snowflake(
     vc: ValidioAPIClient,
-    output: Path,
+    filename: Path,
     credential_id: str,
     db_schema: str,
     database: str,
     table: str,
     role: str,
     warehouse: str,
 ):
     schema = await vc.infer_snowflake_schema(
         SnowflakeInferSchemaInput(
-            credentialId=credential_id,
-            schema=db_schema,
+            credential_id=credential_id,
+            db_schema=db_schema,
             database=database,
             table=table,
             role=role,
             warehouse=warehouse,
         )
     )
-    _write_schema(output, schema)
+    _write_schema(filename, schema)
 
 
 async def _infer_schema_bigquery(
     vc: ValidioAPIClient,
-    output: Path,
+    filename: Path,
     credential_id: str,
     project: str,
     dataset: str,
     table: str,
 ):
     schema = await vc.infer_gcp_big_query_schema(
         GcpBigQueryInferSchemaInput(
-            credentialId=credential_id,
+            credential_id=credential_id,
             project=project,
             dataset=dataset,
             table=table,
         )
     )
-    _write_schema(output, schema)
+    _write_schema(filename, schema)
 
 
 async def _infer_schema_gcs(
     vc: ValidioAPIClient,
-    output: Path,
+    filename: Path,
     credential_id: str,
     project: str,
     bucket: str,
     folder: str,
     file_pattern: str,
     csv_delimiter: str,
     null_marker: str | None,
 ):
     schema = await vc.infer_gcp_storage_schema(
         GcpStorageInferSchemaInput(
-            credentialId=credential_id,
+            credential_id=credential_id,
             project=project,
             bucket=bucket,
             folder=folder,
-            filePattern=file_pattern,
+            file_pattern=file_pattern,
             csv=CsvParserInput(
                 delimiter=csv_delimiter,
-                nullMarker=null_marker,
+                null_marker=null_marker,
             ),
         )
     )
-    _write_schema(output, schema)
+    _write_schema(filename, schema)
 
 
-def _write_schema(output: Path, schema: Any):
-    output.write_text(json.dumps(schema, indent=2))
+def _write_schema(filename: Path, schema: Any):
+    filename.write_text(json.dumps(schema, indent=2))
 
-    print(f"Schema written to {output}")
+    print(f"Schema written to {filename}")
 
 
 async def _multip_prompt(questions: list[tuple[str, list[str], str]]) -> dict[str, str]:
     answers = {}
     session: PromptSession = PromptSession()
     for f in questions:
         title, values, default = f
@@ -787,52 +820,63 @@
         return ""
 
     return null_marker
 
 
 # TODO: UI-1957
 # We don't want to get _all_ resources just to find the id.
-async def _get_source_id(vc: ValidioAPIClient, identifier: str | None) -> str | None:
+async def _get_source_id(
+    vc: ValidioAPIClient, cfg: ValidioConfig, identifier: str, namespace: str
+) -> str | None:
     if identifier is None:
-        print("Missing source id or name")
+        print("Missing source ID or name")
         return None
 
     source_id: str | None = identifier
     if not identifier.startswith("SRC_"):
         source_id = next(
             (
                 source.id
-                for source in await vc.list_sources()
+                for source in await vc.list_sources(
+                    filter=ResourceFilter(
+                        resource_namespace=get_namespace(namespace, cfg)
+                    )
+                )
                 if source.resource_name == identifier
             ),
             None,
         )
 
     if source_id is None:
-        print(f"No source with name or id {identifier} found")
+        print(f"No source with name or ID {identifier} found")
         return None
 
     return source_id
 
 
-async def _get_credential_id(vc: ValidioAPIClient, identifier: str) -> str | None:
+async def _get_credential_id(
+    vc: ValidioAPIClient, cfg: ValidioConfig, identifier: str, namespace: str
+) -> str | None:
     if identifier.startswith("CRD_"):
         return identifier
 
+    # TODO: UI-1957 - Get a single resource by name
     resolved_id = next(
         (
             credential.id
-            for credential in await vc.list_credentials()
+            for credential in await vc.list_credentials(
+                filter=ResourceFilter(resource_namespace=get_namespace(namespace, cfg))
+            )
             if credential.resource_name == identifier
         ),
         None,
     )
 
     if resolved_id is None:
-        print(f"No credential with name or id {identifier} found")
+        print(f"No credential with name or ID {identifier} found")
         return None
     return None
 
 
 def _resource_filter(
     source: Any, credential_id: str | None, credential_name: str | None
 ) -> bool:
```

### Comparing `validio_cli-0.1.0/validio_cli/bin/entities/users.py` & `validio_cli-0.2.0/validio_cli/bin/entities/users.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.1.0/validio_cli/bin/entities/validators.py` & `validio_cli-0.2.0/validio_cli/bin/entities/validators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 from typing import Any
 
 import typer
+from validio_sdk.graphql_client.input_types import ResourceFilter
 
 import validio_cli
 from validio_cli import (
     AsyncTyper,
     ConfigDir,
     Identifier,
+    Namespace,
     OutputFormat,
     OutputFormatOption,
     OutputSettings,
     _single_resource_if_specified,
     get_client_and_config,
     output_json,
     output_text,
 )
+from validio_cli.namespace import get_namespace
 
-app = AsyncTyper(help="Validators applied to data from different sources")
+app = AsyncTyper(help="Validators monitor data from your Source")
 
 
-@app.async_command(help="Get validators")
+@app.async_command(help="Get Validators")
 async def get(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    namespace: str = Namespace,
     identifier: str = Identifier,
     source: str = typer.Option(
-        None, help="List validators for this source (name or id)"
+        None, help="List Validators for this Source (name or ID)"
     ),
     destination: str = typer.Option(
-        None, help="List validators for this destination (name or id)"
+        None, help="List Validators for this Destination (name or ID)"
     ),
     window: str = typer.Option(
-        None, help="List validators for this window (name or id)"
+        None, help="List Validators for this Window (name or ID)"
     ),
     segmentation: str = typer.Option(
-        None, help="List validators for this segmentation (name or id)"
+        None, help="List Validators for this Segmentation (name or ID)"
     ),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
     validators: list[Any] = []
 
     # TODO: UI-1957
     # We don't want to get all resources if identifier is not id.
+    # TODO: Add support for namespace
     if identifier is not None and identifier.startswith("MTR_"):
         validators.append(await vc.get_validator(id=identifier))
     elif source is None or not source.startswith("SRC_"):
-        for s in await vc.list_sources():
+        for s in await vc.list_sources(
+            filter=ResourceFilter(resourceNamespace=get_namespace(namespace, cfg))
+        ):
             validators.extend(await vc.list_validators(s.id))
     else:
-        validators = await vc.list_validators(id=source)
+        validators = await vc.list_validators(
+            id=source,
+            filter=ResourceFilter(resourceNamespace=get_namespace(namespace, cfg)),
+        )
 
     validators = [
         validator
         for validator in validators
         if validio_cli._resource_filter(validator, ["source_config", "source"], source)
         and validio_cli._resource_filter(validator, ["source_config", "window"], window)
         and validio_cli._resource_filter(
```

### Comparing `validio_cli-0.1.0/validio_cli/bin/entities/windows.py` & `validio_cli-0.2.0/validio_cli/bin/entities/windows.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 import typer
 from camel_converter import to_snake
+from validio_sdk.graphql_client.input_types import ResourceFilter
 
 import validio_cli
 from validio_cli import (
     AsyncTyper,
     ConfigDir,
     Identifier,
+    Namespace,
     OutputFormat,
     OutputFormatOption,
     OutputSettings,
     _single_resource_if_specified,
     get_client_and_config,
     output_json,
     output_text,
 )
+from validio_cli.namespace import get_namespace
 
 app = AsyncTyper(help="Windows used to group data for calculations")
 
 
 @app.async_command(help="Get windows")
 async def get(
     config_dir: str = ConfigDir,
     output_format: OutputFormat = OutputFormatOption,
+    namespace: str = Namespace,
     identifier: str = Identifier,
-    source: str = typer.Option(None, help="List windows for this source (id or name)"),
+    source: str = typer.Option(None, help="List Windows for this source (ID or name)"),
 ):
-    vc, _ = await get_client_and_config(config_dir)
+    vc, cfg = await get_client_and_config(config_dir)
 
     # TODO: Get a single resource by id/name to not have to list.
-    windows = await vc.list_windows()
+    windows = await vc.list_windows(
+        filter=ResourceFilter(resourceNamespace=get_namespace(namespace, cfg))
+    )
     windows = [
         window
         for window in windows
         if window is not None
         and validio_cli._resource_filter(window, ["source"], source)
     ]
     windows = _single_resource_if_specified(windows, identifier)
```

### Comparing `validio_cli-0.1.0/validio_cli/bin/main.py` & `validio_cli-0.2.0/validio_cli/bin/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import sys
-from typing import Annotated
 
 import httpx
 import typer
 import validio_sdk.metadata
 from tabulate import tabulate
 from validio_sdk.validio_client import UnauthorizedError
 
@@ -41,27 +40,30 @@
 app.add_typer(validators.app, no_args_is_help=True, name="validators")
 app.add_typer(windows.app, no_args_is_help=True, name="windows")
 
 
 @app.command()
 def config(
     config_dir: str = ConfigDir,
-    show: Annotated[
-        bool,
-        typer.Option(
-            help="Show current configuration",
-            default=False,
-        ),
-    ] = False,
+    show: bool = typer.Option(
+        False,
+        help="Show current configuration",
+    ),
+    default_namespace: str = typer.Option(
+        None,
+        help="Set default namespace to target from CLI",
+    ),
 ):
     """
     Initialize the CLI tool to set endpoint, credentials and more.
     """
     if show:
         cfg.show(config_dir)
+    elif default_namespace:
+        cfg.set_default_namespace(default_namespace, config_dir)
     else:
         cfg.create_or_update(config_dir)
 
 
 @app.command(help="Show current version")
 def version():
     print(
@@ -79,15 +81,15 @@
 
     try:
         app()
         exit_code = 0
     except UnauthorizedError:
         print("🛑 Unauthorized!")
         print(
-            "Ensure you have proper credentials and re-run 'validio config' to add them"
+            "Make sure you have proper credentials and run 'validio config' to add them"
         )
 
     except httpx.ConnectError as e:
         print(f"🛑 Failed to connect to server: {e}")
         print(
             "Check your network environment or run 'validio config' to set a proper"
             " server endpoint"
```

### Comparing `validio_cli-0.1.0/validio_cli/components.py` & `validio_cli-0.2.0/validio_cli/components.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.1.0/validio_cli/schema.py` & `validio_cli-0.2.0/validio_cli/schema.py`

 * *Files identical despite different names*

