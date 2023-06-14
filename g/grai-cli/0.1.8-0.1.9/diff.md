# Comparing `tmp/grai_cli-0.1.8.tar.gz` & `tmp/grai_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_cli-0.1.8.tar", max compression
+gzip compressed data, was "grai_cli-0.1.9.tar", max compression
```

## Comparing `grai_cli-0.1.8.tar` & `grai_cli-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0        0 2022-07-19 07:50:36.524781 grai_cli-0.1.8/README.md
--rw-r--r--   0        0        0      293 2023-01-03 17:11:14.004310 grai_cli-0.1.8/grai_cli/__init__.py
--rw-r--r--   0        0        0       23 2023-01-03 17:11:14.004356 grai_cli-0.1.8/grai_cli/__version__.py
--rw-r--r--   0        0        0       63 2022-11-09 15:55:13.272679 grai_cli-0.1.8/grai_cli/api/__init__.py
--rw-r--r--   0        0        0       51 2022-07-24 08:00:09.094234 grai_cli-0.1.8/grai_cli/api/config/__init__.py
--rw-r--r--   0        0        0     2005 2023-03-16 04:12:39.223918 grai_cli-0.1.8/grai_cli/api/config/config.py
--rw-r--r--   0        0        0     2193 2023-03-16 04:12:39.224233 grai_cli-0.1.8/grai_cli/api/config/set.py
--rw-r--r--   0        0        0      463 2023-02-13 20:16:22.656762 grai_cli-0.1.8/grai_cli/api/config/setup.py
--rw-r--r--   0        0        0     1026 2023-02-13 20:16:22.656984 grai_cli-0.1.8/grai_cli/api/entrypoint.py
--rw-r--r--   0        0        0       49 2022-07-24 08:00:09.100216 grai_cli-0.1.8/grai_cli/api/server/__init__.py
--rw-r--r--   0        0        0     4372 2023-03-16 04:12:39.224788 grai_cli-0.1.8/grai_cli/api/server/endpoints.py
--rw-r--r--   0        0        0     1141 2023-03-16 04:12:39.225042 grai_cli-0.1.8/grai_cli/api/server/setup.py
--rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273574 grai_cli-0.1.8/grai_cli/api/telemetry/__init__.py
--rw-r--r--   0        0        0      300 2023-02-13 20:16:22.657393 grai_cli-0.1.8/grai_cli/api/telemetry/commands.py
--rw-r--r--   0        0        0       89 2023-03-16 04:12:39.225317 grai_cli-0.1.8/grai_cli/config_default.yaml
--rw-r--r--   0        0        0        0 2022-07-24 06:33:14.647347 grai_cli-0.1.8/grai_cli/py.typed
--rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273862 grai_cli-0.1.8/grai_cli/settings/__init__.py
--rw-r--r--   0        0        0     2098 2023-03-16 04:12:39.225733 grai_cli-0.1.8/grai_cli/settings/cache.py
--rw-r--r--   0        0        0     5772 2023-03-16 04:12:39.226132 grai_cli-0.1.8/grai_cli/settings/config.py
--rw-r--r--   0        0        0       88 2023-01-10 17:15:31.923336 grai_cli-0.1.8/grai_cli/utilities/__init__.py
--rw-r--r--   0        0        0     1233 2023-03-16 04:12:39.226578 grai_cli-0.1.8/grai_cli/utilities/headers.py
--rw-r--r--   0        0        0      783 2023-02-13 20:16:22.657964 grai_cli-0.1.8/grai_cli/utilities/styling.py
--rw-r--r--   0        0        0      541 2023-01-03 17:11:14.005048 grai_cli-0.1.8/grai_cli/utilities/telemetry.py
--rw-r--r--   0        0        0      488 2023-03-16 04:12:39.226900 grai_cli-0.1.8/grai_cli/utilities/test.py
--rw-r--r--   0        0        0     3529 2023-03-16 04:12:39.227159 grai_cli-0.1.8/grai_cli/utilities/utilities.py
--rw-r--r--   0        0        0     1393 2023-03-16 04:12:39.227474 grai_cli-0.1.8/grai_cli/utilities/validators.py
--rw-r--r--   0        0        0      861 2023-03-19 22:01:50.171444 grai_cli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 grai_cli-0.1.8/setup.py
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 grai_cli-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-19 07:50:36.524781 grai_cli-0.1.9/README.md
+-rw-r--r--   0        0        0      293 2023-01-03 17:11:14.004310 grai_cli-0.1.9/grai_cli/__init__.py
+-rw-r--r--   0        0        0       23 2023-01-03 17:11:14.004356 grai_cli-0.1.9/grai_cli/__version__.py
+-rw-r--r--   0        0        0       63 2022-11-09 15:55:13.272679 grai_cli-0.1.9/grai_cli/api/__init__.py
+-rw-r--r--   0        0        0       51 2022-07-24 08:00:09.094234 grai_cli-0.1.9/grai_cli/api/config/__init__.py
+-rw-r--r--   0        0        0     2012 2023-03-19 22:15:28.568351 grai_cli-0.1.9/grai_cli/api/config/config.py
+-rw-r--r--   0        0        0     2193 2023-03-16 04:12:39.224233 grai_cli-0.1.9/grai_cli/api/config/set.py
+-rw-r--r--   0        0        0      463 2023-02-13 20:16:22.656762 grai_cli-0.1.9/grai_cli/api/config/setup.py
+-rw-r--r--   0        0        0     1026 2023-02-13 20:16:22.656984 grai_cli-0.1.9/grai_cli/api/entrypoint.py
+-rw-r--r--   0        0        0       49 2022-07-24 08:00:09.100216 grai_cli-0.1.9/grai_cli/api/server/__init__.py
+-rw-r--r--   0        0        0     4372 2023-03-16 04:12:39.224788 grai_cli-0.1.9/grai_cli/api/server/endpoints.py
+-rw-r--r--   0        0        0     1141 2023-03-16 04:12:39.225042 grai_cli-0.1.9/grai_cli/api/server/setup.py
+-rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273574 grai_cli-0.1.9/grai_cli/api/telemetry/__init__.py
+-rw-r--r--   0        0        0      300 2023-02-13 20:16:22.657393 grai_cli-0.1.9/grai_cli/api/telemetry/commands.py
+-rw-r--r--   0        0        0       89 2023-03-16 04:12:39.225317 grai_cli-0.1.9/grai_cli/config_default.yaml
+-rw-r--r--   0        0        0        0 2022-07-24 06:33:14.647347 grai_cli-0.1.9/grai_cli/py.typed
+-rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273862 grai_cli-0.1.9/grai_cli/settings/__init__.py
+-rw-r--r--   0        0        0     2098 2023-03-16 04:12:39.225733 grai_cli-0.1.9/grai_cli/settings/cache.py
+-rw-r--r--   0        0        0     5772 2023-03-16 04:12:39.226132 grai_cli-0.1.9/grai_cli/settings/config.py
+-rw-r--r--   0        0        0       88 2023-01-10 17:15:31.923336 grai_cli-0.1.9/grai_cli/utilities/__init__.py
+-rw-r--r--   0        0        0     1233 2023-03-16 04:12:39.226578 grai_cli-0.1.9/grai_cli/utilities/headers.py
+-rw-r--r--   0        0        0      783 2023-02-13 20:16:22.657964 grai_cli-0.1.9/grai_cli/utilities/styling.py
+-rw-r--r--   0        0        0      541 2023-01-03 17:11:14.005048 grai_cli-0.1.9/grai_cli/utilities/telemetry.py
+-rw-r--r--   0        0        0      488 2023-03-16 04:12:39.226900 grai_cli-0.1.9/grai_cli/utilities/test.py
+-rw-r--r--   0        0        0     3529 2023-03-16 04:12:39.227159 grai_cli-0.1.9/grai_cli/utilities/utilities.py
+-rw-r--r--   0        0        0     1663 2023-03-19 22:16:09.155405 grai_cli-0.1.9/grai_cli/utilities/validators.py
+-rw-r--r--   0        0        0      861 2023-03-19 22:19:53.661091 grai_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 grai_cli-0.1.9/setup.py
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 grai_cli-0.1.9/PKG-INFO
```

### Comparing `grai_cli-0.1.8/grai_cli/api/config/config.py` & `grai_cli-0.1.9/grai_cli/api/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,28 @@
         default=default_styler(config.server.port),
         prompt="Server port",
         prompt_required=True,
         callback=strip_style(port_callback),
     ),
     insecure: str = typer.Option(
         default=default_styler("False"),
-        prompt="insecure connection",
+        prompt="Insecure connection (i.e. http)?",
         prompt_required=True,
         callback=strip_style(insecure_callback),
     ),
     workspace: str = typer.Option(
         default=default_styler(config.server.workspace),
         prompt="The Grai workspace for this config",
         prompt_required=True,
         callback=strip_style(workspace_callback),
     ),
 ):
     """Initialize a new config file"""
     config.auth = BasicAuthSettings(username=username, password=password)
-    config.server = ServerSettingsV1(host=host, port=port, insecure=bool(insecure), workspace=workspace)
+    config.server = ServerSettingsV1(host=host, port=port, insecure=insecure, workspace=workspace)
     config.save()
 
 
 @config_app.command(help="Print config to console")
 def view():
     """View the current config file"""
     utilities.print(config.view())
```

### Comparing `grai_cli-0.1.8/grai_cli/api/config/set.py` & `grai_cli-0.1.9/grai_cli/api/config/set.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.1.8/grai_cli/api/entrypoint.py` & `grai_cli-0.1.9/grai_cli/api/entrypoint.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.1.8/grai_cli/api/server/endpoints.py` & `grai_cli-0.1.9/grai_cli/api/server/endpoints.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.1.8/grai_cli/api/server/setup.py` & `grai_cli-0.1.9/grai_cli/api/server/setup.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.1.8/grai_cli/settings/cache.py` & `grai_cli-0.1.9/grai_cli/settings/cache.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.1.8/grai_cli/settings/config.py` & `grai_cli-0.1.9/grai_cli/settings/config.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.1.8/grai_cli/utilities/headers.py` & `grai_cli-0.1.9/grai_cli/utilities/headers.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.1.8/grai_cli/utilities/styling.py` & `grai_cli-0.1.9/grai_cli/utilities/styling.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.1.8/grai_cli/utilities/telemetry.py` & `grai_cli-0.1.9/grai_cli/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.1.8/grai_cli/utilities/utilities.py` & `grai_cli-0.1.9/grai_cli/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.1.8/grai_cli/utilities/validators.py` & `grai_cli-0.1.9/grai_cli/utilities/validators.py`

 * *Files 21% similar despite different names*

```diff
@@ -46,15 +46,19 @@
         int_inp = int(inp)
         if 1 > int_inp < 65535:
             raise error
 
     return str(int_inp)
 
 
-def insecure_callback(inp: str):
+def insecure_callback(inp: str) -> str:
     error = typer.BadParameter(f"{inp} is not a valid value for insecure, should be either True or False.")
-    try:
-        bool(inp)
-    except:
+    TRUE = {"true", "yes", "y"}
+    FALSE = {"false", "no", "n"}
+    lowered_inp = inp.lower()
+    if lowered_inp in TRUE:
+        return "True"
+    elif lowered_inp in FALSE:
+        return "False"
+    else:
+        error = typer.BadParameter(f"'{inp}' is not a valid value for insecure, should be either True or False.")
         raise error
-
-    return str(inp)
```

### Comparing `grai_cli-0.1.8/pyproject.toml` & `grai_cli-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-cli"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 readme = "README.md"
 packages = [{include = "grai_cli"}]
 
 [tool.poetry.scripts]
```

### Comparing `grai_cli-0.1.8/setup.py` & `grai_cli-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['grai = grai_cli.api.entrypoint:app']}
 
 setup_kwargs = {
     'name': 'grai-cli',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_cli-0.1.8/PKG-INFO` & `grai_cli-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

