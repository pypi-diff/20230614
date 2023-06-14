# Comparing `tmp/wand-ai-client-0.0.7.tar.gz` & `tmp/wand-ai-client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wand-ai-client-0.0.7.tar", last modified: Mon May 29 14:04:04 2023, max compression
+gzip compressed data, was "wand-ai-client-0.0.8.tar", last modified: Wed Jun 14 14:58:25 2023, max compression
```

## Comparing `wand-ai-client-0.0.7.tar` & `wand-ai-client-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 14:04:04.260552 wand-ai-client-0.0.7/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 14:04:04.260552 wand-ai-client-0.0.7/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.7/README.md
--rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.7/pyproject.toml
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1859 2023-05-29 14:04:04.260552 wand-ai-client-0.0.7/setup.cfg
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 14:04:04.257218 wand-ai-client-0.0.7/wand_ai_client.egg-info/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)      508 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/entry_points.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/not-zip-safe
--rw-r--r--   0 romasku   (1000) romasku   (1000)      227 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/requires.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/top_level.txt
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 14:04:04.257218 wand-ai-client-0.0.7/wand_client/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.7/wand_client/__init__.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 14:04:04.257218 wand-ai-client-0.0.7/wand_client/cli/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.7/wand_client/cli/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1148 2023-05-28 09:03:50.000000 wand-ai-client-0.0.7/wand_client/cli/config.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     3043 2023-05-29 13:18:26.000000 wand-ai-client-0.0.7/wand_client/cli/formatters.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5091 2023-05-29 13:07:09.000000 wand-ai-client-0.0.7/wand_client/cli/main.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     2773 2023-05-29 14:03:37.000000 wand-ai-client-0.0.7/wand_client/jupyter.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 14:04:04.260552 wand-ai-client-0.0.7/wand_client/sdk/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.7/wand_client/sdk/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5635 2023-05-29 13:18:12.000000 wand-ai-client-0.0.7/wand_client/sdk/core.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      344 2023-06-12 15:17:19.000000 wand-ai-client-0.0.8/README.md
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.8/pyproject.toml
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1859 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/setup.cfg
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/wand_ai_client.egg-info/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      508 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      227 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/requires.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/top_level.txt
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/wand_client/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       21 2023-06-14 14:03:00.000000 wand-ai-client-0.0.8/wand_client/__init__.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/wand_client/cli/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.8/wand_client/cli/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1161 2023-06-01 09:24:47.000000 wand-ai-client-0.0.8/wand_client/cli/config.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     3043 2023-05-29 13:18:26.000000 wand-ai-client-0.0.8/wand_client/cli/formatters.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     5512 2023-06-14 14:04:35.000000 wand-ai-client-0.0.8/wand_client/cli/main.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     2773 2023-05-29 14:03:37.000000 wand-ai-client-0.0.8/wand_client/jupyter.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/wand_client/sdk/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.8/wand_client/sdk/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     5795 2023-06-13 13:52:34.000000 wand-ai-client-0.0.8/wand_client/sdk/core.py
```

### Comparing `wand-ai-client-0.0.7/PKG-INFO` & `wand-ai-client-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.7/setup.cfg` & `wand-ai-client-0.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wand-ai-client
-version = 0.0.7
+version = 0.0.8
 description = Wand AI API client
 author = Wand.AI Team
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `wand-ai-client-0.0.7/wand_ai_client.egg-info/PKG-INFO` & `wand-ai-client-0.0.8/wand_ai_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.7/wand_client/cli/config.py` & `wand-ai-client-0.0.8/wand_client/cli/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from pathlib import Path
 from typing import Any, Dict, Optional, Sequence
 
 from pydantic import BaseSettings
 
-CONFIG_PATH = Path("~/.wand/config.json")
+CONFIG_PATH = Path("~/.wand/config.json").expanduser()
 
 
 def json_config_settings_source(settings: BaseSettings) -> Dict[str, Any]:
     encoding = settings.__config__.env_file_encoding
     if CONFIG_PATH.exists():
         return json.loads(CONFIG_PATH.read_text(encoding))
     return {}
```

### Comparing `wand-ai-client-0.0.7/wand_client/cli/formatters.py` & `wand-ai-client-0.0.8/wand_client/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.7/wand_client/cli/main.py` & `wand-ai-client-0.0.8/wand_client/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import click
 import rich
 from click import Context
 from prompt_toolkit import PromptSession
 from rich.progress import Progress
 
+from wand_client import __version__
 from wand_client.cli.config import CONFIG_PATH, WandCliSettings
 from wand_client.cli.formatters import (
     ModelFormatter,
     ModelsFormatter,
     SettingsFormatter,
     SourceFormatter,
 )
@@ -31,14 +32,15 @@
         return WandClient(
             base_url=settings.WAND_API_URL,  # type: ignore
             token=settings.WAND_TOKEN,  # type: ignore
         )
 
 
 @click.group()
+@click.version_option(__version__)
 @click.option("--api_url", type=str, default=None)
 @click.option("--token", type=str, default=None)
 @click.pass_context
 def cli(ctx: Context, api_url: Optional[str], token: Optional[str]) -> None:
     option_settings = {
         "WAND_API_URL": api_url,
         "WAND_TOKEN": token,
@@ -68,14 +70,15 @@
         json.dumps(
             {
                 "WAND_API_URL": api_url,
                 "WAND_TOKEN": token,
             }
         )
     )
+    print(f"Wrote config to: {CONFIG_PATH.absolute()}")
 
 
 @config.command()
 @click.pass_context
 def show(ctx: Context) -> None:
     """
     Show current settings
@@ -148,14 +151,24 @@
 def get(ctx: Context, model_id: str) -> None:
     """Get info about model by ID"""
     client: WandClient = ctx.obj.get_client()
     model = client.models.get(model_id=model_id)
     rich.print(ModelFormatter()(model))
 
 
+@model.command()
+@click.argument("model_id", type=click.STRING)
+@click.pass_context
+def delete(ctx: Context, model_id: str) -> None:
+    """Get info about model by ID"""
+    client: WandClient = ctx.obj.get_client()
+    client.models.delete(model_id=model_id)
+    rich.print("Model deleted")
+
+
 @model.command(name="list")
 @click.pass_context
 def list_(ctx: Context) -> None:
     """List all models"""
     client: WandClient = ctx.obj.get_client()
     models = client.models.list_all()
     rich.print(ModelsFormatter()(models))
```

### Comparing `wand-ai-client-0.0.7/wand_client/jupyter.py` & `wand-ai-client-0.0.8/wand_client/jupyter.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.7/wand_client/sdk/core.py` & `wand-ai-client-0.0.8/wand_client/sdk/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,20 @@
     def get(self, model_id: str) -> Model:
         res = self._core.request(
             method="GET",
             path=f"/models/{model_id}",
         ).json()
         return self._parse_model_payload(res)
 
+    def delete(self, model_id: str) -> None:
+        self._core.request(
+            method="DELETE",
+            path=f"/models/{model_id}",
+        ).json()
+
     def list_all(self) -> List[Model]:
         res = self._core.request(
             method="GET",
             path=f"/models",
         ).json()
         return [self._parse_model_payload(it) for it in res]
```

