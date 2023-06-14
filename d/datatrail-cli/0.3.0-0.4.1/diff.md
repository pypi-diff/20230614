# Comparing `tmp/datatrail_cli-0.3.0.tar.gz` & `tmp/datatrail_cli-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.3.0.tar", max compression
+gzip compressed data, was "datatrail_cli-0.4.1.tar", max compression
```

## Comparing `datatrail_cli-0.3.0.tar` & `datatrail_cli-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1080 2023-06-05 15:36:00.935159 datatrail_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0     3558 2023-06-05 15:36:00.935159 datatrail_cli-0.3.0/README.md
--rw-r--r--   0        0        0      214 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/__init__.py
--rw-r--r--   0        0        0     3862 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/clear.py
--rw-r--r--   0        0        0      929 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/cli.py
--rw-r--r--   0        0        0     3714 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/config.py
--rw-r--r--   0        0        0     1062 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/config.yaml
--rw-r--r--   0        0        0     3442 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/ls.py
--rw-r--r--   0        0        0     4415 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/ps.py
--rw-r--r--   0        0        0     4066 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/pull.py
--rw-r--r--   0        0        0    12027 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/src/functions.py
--rw-r--r--   0        0        0     9241 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/utilities/cadcclient.py
--rw-r--r--   0        0        0     1493 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/utilities/utilities.py
--rw-r--r--   0        0        0     1048 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 datatrail_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-08 00:04:53.466117 datatrail_cli-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3558 2023-06-08 00:04:53.466117 datatrail_cli-0.4.1/README.md
+-rw-r--r--   0        0        0      214 2023-06-08 00:04:53.474117 datatrail_cli-0.4.1/dtcli/__init__.py
+-rw-r--r--   0        0        0     4399 2023-06-08 00:04:53.474117 datatrail_cli-0.4.1/dtcli/clear.py
+-rw-r--r--   0        0        0      929 2023-06-08 00:04:53.474117 datatrail_cli-0.4.1/dtcli/cli.py
+-rw-r--r--   0        0        0     3714 2023-06-08 00:04:53.474117 datatrail_cli-0.4.1/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2023-06-08 00:04:53.474117 datatrail_cli-0.4.1/dtcli/config.yaml
+-rw-r--r--   0        0        0     3442 2023-06-08 00:04:53.474117 datatrail_cli-0.4.1/dtcli/ls.py
+-rw-r--r--   0        0        0     6101 2023-06-08 00:04:53.474117 datatrail_cli-0.4.1/dtcli/ps.py
+-rw-r--r--   0        0        0     4336 2023-06-08 00:04:53.474117 datatrail_cli-0.4.1/dtcli/pull.py
+-rw-r--r--   0        0        0    14068 2023-06-08 00:04:53.478117 datatrail_cli-0.4.1/dtcli/src/functions.py
+-rw-r--r--   0        0        0     9241 2023-06-08 00:04:53.478117 datatrail_cli-0.4.1/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     1493 2023-06-08 00:04:53.478117 datatrail_cli-0.4.1/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1048 2023-06-08 00:04:53.478117 datatrail_cli-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 datatrail_cli-0.4.1/PKG-INFO
```

### Comparing `datatrail_cli-0.3.0/LICENSE` & `datatrail_cli-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.3.0/README.md` & `datatrail_cli-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.3.0/dtcli/clear.py` & `datatrail_cli-0.4.1/dtcli/clear.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,45 +24,54 @@
     "-d",
     type=click.Path(
         exists=True, file_okay=False, dir_okay=True, writable=True, resolve_path=True
     ),
     default=None,
     help="Directory to clear data from.",
 )
+@click.option(
+    "--clear-parents",
+    is_flag=True,
+    help="Clear all empty parent directories of dataset.",
+)
 @click.option("-v", "--verbose", count=True, help="Verbosity: v=INFO, vv=DEBUG.")
 @click.option("-q", "--quiet", is_flag=True, help="Set log level to ERROR.")
 @click.option("--force", "-f", is_flag=True, help="Do not prompt for confirmation.")
 def clear(
     scope: str,
     dataset: str,
     directory: str,
+    clear_parents: bool,
     verbose: int = 0,
     quiet: bool = False,
     force: bool = False,
 ) -> None:
     """Clear a dataset.
 
     Args:
         scope (str): Scope of dataset.
         dataset (str): Name of dataset.
         directory (str): Directory to clear data from.
+        clear_parents (bool): Clear all empty parent directories of dataset.
         verbose (int): Verbosity: v=INFO, vv=DUBUG.
         quiet (bool): Minimal logging.
         force (bool): Automatically download files.
     """
     logger.setLevel("WARNING")
     if verbose == 1:
         logger.setLevel("INFO")
     elif verbose > 1:
         logger.setLevel("DEBUG")
     elif quiet:
         logger.setLevel("ERROR")
     logger.debug("`clear` called with:")
     logger.debug(f"scope: {scope} [{type(scope)}]")
     logger.debug(f"dataset: {dataset} [{type(dataset)}]")
+    logger.debug(f"directory: {directory} [{type(directory)}]")
+    logger.debug(f"clear_parents: {clear_parents} [{type(clear_parents)}]")
     logger.debug(f"verbose: {verbose} [{type(verbose)}]")
     logger.debug(f"quiet: {quiet} [{type(quiet)}]")
 
     # Load configuration.
     try:
         logger.debug("Loading configuration.")
         config = procure()
@@ -96,21 +105,26 @@
             f"Path {common_path} does not exist. No files to clear.", style="bold red"
         )
         raise click.Abort()
     files = os.listdir(common_path)
     size = sum(os.path.getsize(os.path.join(common_path, f)) for f in files)
 
     console.print(f"Directory: {common_path}", style="bold")
-    console.print(f"Found {len(files)} files.")
-    console.print(f"Total size: {size / 1024**3:.2f} GB.\n")
+    console.print(f" - Found {len(files)} files.")
+    console.print(f" - Total size: {size / 1024**3:.2f} GB.\n")
 
     # Confirm deletion.
     if force:
         is_delete = True
     else:
-        is_delete = Confirm.ask("Delete files?")
+        message = (
+            "⚠️  Delete files and empty parent directories?"
+            if clear_parents
+            else "⚠️  Delete files?"
+        )
+        is_delete = Confirm.ask(message)
 
     # Delete files.
     if is_delete:
-        clear_dataset_path(common_path, verbose, quiet)
+        clear_dataset_path(common_path, clear_parents, verbose, quiet)
     else:
         console.print("Roger roger, no files deleted.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `datatrail_cli-0.3.0/dtcli/cli.py` & `datatrail_cli-0.4.1/dtcli/cli.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.3.0/dtcli/config.py` & `datatrail_cli-0.4.1/dtcli/config.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.3.0/dtcli/config.yaml` & `datatrail_cli-0.4.1/dtcli/config.yaml`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.3.0/dtcli/ls.py` & `datatrail_cli-0.4.1/dtcli/ls.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.3.0/dtcli/pull.py` & `datatrail_cli-0.4.1/dtcli/pull.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Datatrail Pull Command."""
 
 import logging
 from os import cpu_count, path
 
 import click
+from requests.exceptions import SSLError
 from rich.console import Console
 from rich.prompt import Confirm
 
 from dtcli.config import procure
 from dtcli.src.functions import find_missing_dataset_files, get_files
 from dtcli.utilities.cadcclient import size
 from dtcli.utilities.utilities import validate_scope
 
 logger = logging.getLogger("pull")
 
 console = Console()
+error_console = Console(stderr=True, style="bold red")
 
 
 @click.command(name="pull", help="Download a dataset.")
 @click.argument("scope", type=click.STRING, required=True, nargs=1)
 @click.argument("dataset", type=click.STRING, required=True, nargs=1)
 @click.option(
     "--directory",
@@ -93,18 +95,26 @@
 
     # Find files missing from localhost.
     console.print(f"\nSearching for files for {dataset} {scope}...\n")
     files = find_missing_dataset_files(scope, dataset)
     if len(files["missing"]) == 0:
         console.print("No files found at minoc.", style="bold red")
         return None
-    common_path = path.commonpath(files["missing"])
-    if common_path.startswith("cadc:CHIMEFRB"):
-        common_path = common_path.replace("cadc:CHIMEFRB", "")
-    to_download_size = size(common_path)
+    files_paths = [f.replace("cadc:CHIMEFRB", "") for f in files["missing"]]
+    common_path = path.commonpath(["/" + f for f in files_paths])
+    try:
+        to_download_size = size(common_path)
+    except SSLError:
+        error_console.print(
+            """
+No valid CADC certificate found.
+Create one using 'cadc-get-cert -u <USERNAME>'.
+"""
+        )
+        return None
     console.print(
         f" - {len(files['existing'])} files found at {site}.",
         style="green",
     )
     console.print(
         f" - {len(files['missing'])} files can be downloaded from minoc.",
         style="yellow",
```

### Comparing `datatrail_cli-0.3.0/dtcli/src/functions.py` & `datatrail_cli-0.4.1/dtcli/src/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Functions for CLI."""
 
 import logging
 import os
 import shutil
+import time
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 
 from dtcli.config import procure
 from dtcli.utilities import cadcclient, utilities
@@ -98,77 +99,118 @@
             return {"error": "Datatrail Server at CHIME is not responding."}
 
     else:
         return {}
 
 
 def ps(
-    scope: str, dataset: str, base_url: Optional[str] = None
+    scope: str,
+    dataset: str,
+    verbose: int = 0,
+    quiet: bool = False,
+    base_url: Optional[str] = None,
 ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
     """List detailed information about a dataset.
 
     Args:
         scope (Optional[str], optional): Scope of dataset. Defaults to None.
         dataset (Optional[str], optional): Name of dataset. Defaults to None.
+        verbose (int, optional): Verbosity. Defaults to 0.
+        quiet (bool, optional): Minimal logging. Defaults to False.
         base_url (Optional[str], optional): Datatrail URL. Defaults to None.
 
     Returns:
         Tuple[Dict[str, Any], Dict[str, Any]]: Dictionary of dataset files,
             and dictionary of dataset's policies.
     """
+    # Set logging level.
+    logger.setLevel("WARNING")
+    if verbose == 1:
+        logger.setLevel("INFO")
+    elif verbose > 1:
+        logger.setLevel("DEBUG")
+    elif quiet:
+        logger.setLevel("ERROR")
+
     # Load configuration.
+    logger.debug("Loading configuration.")
     try:
         config = procure()
         server = config["server"]
+        logger.debug("Configuration loaded successfully.")
     except Exception:
         raise FileNotFoundError(
             "No configuration file found. Create one with `datatrail config init`."
         )
     if not base_url:
+        logger.debug(f"Setting base_url to {server}.")
         base_url = server
     try:
         files_response = get_dataset_file_info(scope, dataset)
 
+        logger.info(f"Getting policy for {dataset} in {scope}.")
         url: str = str(base_url) + f"/query/dataset/{scope}/{dataset}"
+        logger.debug(f"URL: {url}")
         r = requests.get(url)
+        logger.debug(f"Status: {r.status_code}.")
         policy_response = utilities.decode_response(r)
         if "object has no attribute" in policy_response or isinstance(
             files_response, str
         ):
             raise Exception(f"Could not find {dataset} {scope} in Datatrail.")
 
         return files_response, policy_response  # type: ignore
 
     except requests.exceptions.ConnectionError as e:
         logger.error(e)
         raise ConnectionError("Datatrail Server at CHIME is not responding.")
 
 
 def get_dataset_file_info(
-    scope: str, dataset: str, base_url: Optional[str] = None
+    scope: str,
+    dataset: str,
+    verbose: int = 0,
+    quiet: bool = False,
+    base_url: Optional[str] = None,
 ) -> Dict[str, Any]:
     """List detailed information about a dataset.
 
     Args:
         scope (Optional[str], optional): Scope of dataset. Defaults to None.
         dataset (Optional[str], optional): Name of dataset. Defaults to None.
+        verbose (int, optional): Verbosity. Defaults to 0.
+        quiet (bool, optional): Minimal logging. Defaults to False.
         base_url (Optional[str], optional): Datatrail URL. Defaults to None.
 
     Returns:
         Dict[str, Any]: JSON response from server or error string.
     """
+    # Set logging level.
+    logger.setLevel("WARNING")
+    if verbose == 1:
+        logger.setLevel("INFO")
+    elif verbose > 1:
+        logger.setLevel("DEBUG")
+    elif quiet:
+        logger.setLevel("ERROR")
+
     # Load configuration.
     config = procure()
     server = config["server"]
     if not base_url:
         base_url = server
     try:
+        logger.info(f"Finding files for {dataset} in {scope}.")
         payload = {"scope": scope, "name": dataset}
+        logger.debug(f"Payload: {payload}")
         url = str(base_url) + "/query/dataset/find"
+        logger.debug(f"URL: {url}")
         r = requests.post(url, json=payload)
+        logger.debug(f"Status: {r.status_code}.")
+        logger.debug("Decoding response.")
         response = utilities.decode_response(r)
         if "object has no attribute" in response:
             return {"error": f"Could not find {dataset} {scope} in Datatrail."}
         return response  # type: ignore
     except requests.exceptions.ConnectionError as e:
         logger.error(e)
         return {"error": "Datatrail Server at CHIME is not responding."}
@@ -262,46 +304,69 @@
             os.makedirs(folder, exist_ok=True)
         cadcclient.pget(
             source=files, destination=destinations, processors=cores, verbose=verbose
         )
     return None
 
 
-def clear_dataset_path(path: str, verbose: int, quiet: bool) -> bool:
+def clear_dataset_path(
+    path: str, clear_parents: bool, verbose: int, quiet: bool
+) -> bool:
     """Delete a path provided.
 
     Args:
         path (str): Path to delete.
+        clear_parents (bool): Clear empty parent directories recursively.
         verbose (int): Verbosity level.
         quiet (bool): Quiet mode.
 
     Returns:
         bool: True if path was deleted.
     """
     logger.setLevel("WARNING")
     if verbose == 1:
         logger.setLevel("INFO")
     elif verbose > 1:
         logger.setLevel("DEBUG")
     elif quiet:
         logger.setLevel("ERROR")
 
+    logger.debug(f"clear_parents: {clear_parents}")
+
     # Check if path exists.
+    p = Path(path)
     logger.debug(f"Checking if path {path} exists.")
-    exists = os.path.exists(path)
+    exists = p.exists()
 
     # Delete files.
     if exists:
-        shutil.rmtree(path)
+        shutil.rmtree(p)
         logger.info("Path successfully removed.")
-        return True
+        time.sleep(0.1)
     else:
         logger.info(f"Path {path} not found.")
         return False
 
+    # Clear empty parent directories.
+    parent = p.parent
+    if clear_parents:
+        logger.debug(f"Clearing parent directories of {parent}.")
+    while clear_parents:
+        files: List[Path] = [f for f in parent.iterdir()]
+        logger.debug(f"files: {files}")
+        if files:
+            logger.debug(f"{parent}: ✗")
+            clear_parents = False
+        else:
+            logger.debug(f"{parent}: ✔")
+            parent.rmdir()
+            time.sleep(0.1)
+        parent = parent.parent
+    return True
+
 
 def find_dataset_common_path(
     scope: str, dataset: str, site: str, verbose: int, quiet: bool
 ) -> Optional[str]:
     """Find common path for a dataset.
 
     Args:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `datatrail_cli-0.3.0/dtcli/utilities/cadcclient.py` & `datatrail_cli-0.4.1/dtcli/utilities/cadcclient.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.3.0/dtcli/utilities/utilities.py` & `datatrail_cli-0.4.1/dtcli/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.3.0/pyproject.toml` & `datatrail_cli-0.4.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datatrail-cli"
-version = "0.3.0"
+version = "0.4.1"
 description = "CHIME/FRB Datatrail CLI"
 authors = ["CHIME FRB Project Office"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dtcli" }]
 
 [tool.poetry.dependencies]
```

### Comparing `datatrail_cli-0.3.0/PKG-INFO` & `datatrail_cli-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrail-cli
-Version: 0.3.0
+Version: 0.4.1
 Summary: CHIME/FRB Datatrail CLI
 License: MIT
 Author: CHIME FRB Project Office
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datatrail-cli Version: 0.3.0 Summary: CHIME/FRB
+Metadata-Version: 2.1 Name: datatrail-cli Version: 0.4.1 Summary: CHIME/FRB
 Datatrail CLI License: MIT Author: CHIME FRB Project Office Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: cadcdata (>=2.4,<3.0) Requires-Dist: cadctap
 (>=0.9.11,<0.10.0) Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0) Requires-Dist:
```

