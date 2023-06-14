# Comparing `tmp/barbari-3.0.1.tar.gz` & `tmp/barbari-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barbari-3.0.1.tar", last modified: Fri Mar 12 03:06:43 2021, max compression
+gzip compressed data, was "barbari-3.0.2.tar", last modified: Wed Jun 14 04:17:45 2023, max compression
```

## Comparing `barbari-3.0.1.tar` & `barbari-3.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2021-03-12 03:06:43.103983 barbari-3.0.1/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       31 2021-02-21 05:33:40.000000 barbari-3.0.1/MANIFEST.in
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      459 2021-03-12 03:06:43.103983 barbari-3.0.1/PKG-INFO
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2021-03-12 03:06:43.099983 barbari-3.0.1/barbari/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       22 2021-03-12 03:04:31.000000 barbari-3.0.1/barbari/__init__.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2021-03-12 03:06:43.099983 barbari-3.0.1/barbari/commands/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2039 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/commands/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1422 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/commands/build.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2516 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/commands/build_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      710 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/commands/display_config.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      828 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/commands/generate_config.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2057 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/commands/list_configs.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1648 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/commands/setup_flatcam.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    11564 2021-03-12 03:04:08.000000 barbari-3.0.1/barbari/config.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2021-03-12 03:06:43.103983 barbari-3.0.1/barbari/configs/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1352 2021-03-12 02:17:57.000000 barbari-3.0.1/barbari/configs/coddingtonbear.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      216 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/configs/copper_wire_vias.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      177 2021-02-21 04:25:09.000000 barbari-3.0.1/barbari/configs/default_alignment_holes.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      175 2021-02-21 04:31:22.000000 barbari-3.0.1/barbari/configs/default_edge_cuts.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      137 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/configs/default_isolation_routing.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      217 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/configs/drilled_04_10.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      365 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/configs/drilled_pth_04_11.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1467 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/configs/example.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      250 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/configs/milled_10.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      250 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/configs/milled_11.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      544 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/configs/rivets.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      375 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/configs/simple.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      248 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/configs/slots_10.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      590 2021-02-14 05:13:51.000000 barbari-3.0.1/barbari/constants.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      246 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/exceptions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    16774 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/flatcam.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1873 2021-02-14 05:13:51.000000 barbari-3.0.1/barbari/gerbers.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1625 2021-03-06 22:56:06.000000 barbari-3.0.1/barbari/main.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2021-03-12 03:06:43.099983 barbari-3.0.1/barbari.egg-info/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      459 2021-03-12 03:06:42.000000 barbari-3.0.1/barbari.egg-info/PKG-INFO
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1025 2021-03-12 03:06:42.000000 barbari-3.0.1/barbari.egg-info/SOURCES.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2021-03-12 03:06:42.000000 barbari-3.0.1/barbari.egg-info/dependency_links.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      383 2021-03-12 03:06:42.000000 barbari-3.0.1/barbari.egg-info/entry_points.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       72 2021-03-12 03:06:42.000000 barbari-3.0.1/barbari.egg-info/requires.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        8 2021-03-12 03:06:42.000000 barbari-3.0.1/barbari.egg-info/top_level.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       38 2021-03-12 03:06:43.103983 barbari-3.0.1/setup.cfg
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1777 2021-03-06 22:56:06.000000 barbari-3.0.1/setup.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-14 04:17:45.392457 barbari-3.0.2/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       31 2021-02-21 05:33:40.000000 barbari-3.0.2/MANIFEST.in
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      403 2023-06-14 04:17:45.392457 barbari-3.0.2/PKG-INFO
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-14 04:17:45.392457 barbari-3.0.2/barbari/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       22 2023-06-14 04:16:38.000000 barbari-3.0.2/barbari/__init__.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-14 04:17:45.392457 barbari-3.0.2/barbari/commands/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2039 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/commands/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1422 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/commands/build.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2517 2023-06-14 04:11:40.000000 barbari-3.0.2/barbari/commands/build_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      710 2023-06-14 03:39:42.000000 barbari-3.0.2/barbari/commands/display_config.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      968 2023-06-14 04:10:46.000000 barbari-3.0.2/barbari/commands/generate_config.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2056 2023-06-14 04:11:53.000000 barbari-3.0.2/barbari/commands/list_configs.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1702 2023-06-14 04:13:17.000000 barbari-3.0.2/barbari/commands/setup_flatcam.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    11564 2023-06-14 04:09:43.000000 barbari-3.0.2/barbari/config.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-14 04:17:45.392457 barbari-3.0.2/barbari/configs/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1352 2021-03-12 02:17:57.000000 barbari-3.0.2/barbari/configs/coddingtonbear.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      216 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/configs/copper_wire_vias.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      177 2021-02-21 04:25:09.000000 barbari-3.0.2/barbari/configs/default_alignment_holes.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      175 2021-02-21 04:31:22.000000 barbari-3.0.2/barbari/configs/default_edge_cuts.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      137 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/configs/default_isolation_routing.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      217 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/configs/drilled_04_10.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      365 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/configs/drilled_pth_04_11.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1467 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/configs/example.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      250 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/configs/milled_10.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      250 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/configs/milled_11.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      544 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/configs/rivets.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      375 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/configs/simple.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      248 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/configs/slots_10.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      590 2021-02-14 05:13:51.000000 barbari-3.0.2/barbari/constants.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      246 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/exceptions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    16732 2023-06-14 04:14:21.000000 barbari-3.0.2/barbari/flatcam.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1873 2021-02-14 05:13:51.000000 barbari-3.0.2/barbari/gerbers.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1625 2021-03-06 22:56:06.000000 barbari-3.0.2/barbari/main.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-14 04:17:45.392457 barbari-3.0.2/barbari.egg-info/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      403 2023-06-14 04:17:45.000000 barbari-3.0.2/barbari.egg-info/PKG-INFO
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1025 2023-06-14 04:17:45.000000 barbari-3.0.2/barbari.egg-info/SOURCES.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-06-14 04:17:45.000000 barbari-3.0.2/barbari.egg-info/dependency_links.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      382 2023-06-14 04:17:45.000000 barbari-3.0.2/barbari.egg-info/entry_points.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       72 2023-06-14 04:17:45.000000 barbari-3.0.2/barbari.egg-info/requires.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        8 2023-06-14 04:17:45.000000 barbari-3.0.2/barbari.egg-info/top_level.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       38 2023-06-14 04:17:45.392457 barbari-3.0.2/setup.cfg
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1777 2021-03-06 22:56:06.000000 barbari-3.0.2/setup.py
```

### Comparing `barbari-3.0.1/barbari/commands/__init__.py` & `barbari-3.0.2/barbari/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/barbari/commands/build.py` & `barbari-3.0.2/barbari/commands/build.py`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/barbari/commands/build_script.py` & `barbari-3.0.2/barbari/commands/build_script.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from rich.prompt import Confirm
 
 from .. import config, gerbers, flatcam
 from . import BaseCommand
 
 
 class Command(BaseCommand):
-    OUTPUT_PATTERN = re.compile("^\d+\..*\.gcode$")
+    OUTPUT_PATTERN = re.compile(r"^\d+\..*\.gcode$")
 
     @classmethod
     def add_arguments(cls, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "directory", help="Path to a directory holding your gerber/drl exports."
         )
         parser.add_argument(
```

### Comparing `barbari-3.0.1/barbari/commands/display_config.py` & `barbari-3.0.2/barbari/commands/display_config.py`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/barbari/commands/generate_config.py` & `barbari-3.0.2/barbari/commands/generate_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import argparse
 import os
-
-import yaml
+import shutil
 
 from .. import config
 from . import BaseCommand
 
 
 class Command(BaseCommand):
+    DEFAULT_CONFIG = "example.yaml"
+
     @classmethod
     def add_arguments(cls, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "name", help="Name of the configuration you would like to generate."
         )
         return super().add_arguments(parser)
 
     def handle(self) -> None:
         final_path = f"{self.options.name}.yaml"
 
         os.makedirs(
-            os.path.dirname(config.get_user_config_path(final_path)), exist_ok=True
+            config.get_user_config_dir(), exist_ok=True
+        )
+        shutil.copyfile(
+            os.path.join(
+                config.get_default_config_dir(),
+                self.DEFAULT_CONFIG,
+            ),
+            os.path.join(
+                config.get_user_config_dir(),
+                final_path,
+            )
         )
-        with open(config.get_user_config_path(final_path), "w") as outf:
-            outf.write(yaml.safe_dump(config.get_default_config_dict()))
 
         self.console.print(
             f"Configuration '{self.options.name}' written to '{final_path}'."
         )
```

### Comparing `barbari-3.0.1/barbari/commands/list_configs.py` & `barbari-3.0.2/barbari/commands/list_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         for config_name, conf in to_show.items():
             formatted = Markdown(conf.description or "")
 
             self.console.print(f"[blue][b]{config_name}[/b][/blue]")
             if formatted:
                 self.console.print(formatted, style="italic")
             if conf.alignment_holes:
-                self.console.print(f"- Alignment Holes")
+                self.console.print("- Alignment Holes")
             if conf.isolation_routing:
                 self.console.print("- Isolation Routing")
             if conf.edge_cuts:
                 self.console.print("- Edge Cuts")
             if conf.drill:
                 self.console.print("- Drill Profiles")
                 for k, v in conf.drill.items():
```

### Comparing `barbari-3.0.1/barbari/commands/setup_flatcam.py` & `barbari-3.0.2/barbari/commands/setup_flatcam.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         stdout, stderr = proc.communicate()
         if "--shellfile" not in stdout.decode("utf-8"):
             raise BarbariFlatcamError(
                 "Could not start FlatCam using the provided parameters: "
-                f"stdout: {stdout}, stderr: {stderr}"
+                f"stdout: {stdout.decode('utf-8', 'replace')}, stderr: {stderr.decode('utf-8', 'replace')}"
             )
 
         self.config.flatcam_path = self.options.flatcam
         self.config.python_bin = self.options.python_bin
 
         config.save_environment_config(self.config)
         self.console.print("[green]Flatcam found. [b]Configuration saved[/b][/green]")
```

### Comparing `barbari-3.0.1/barbari/config.py` & `barbari-3.0.2/barbari/config.py`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/barbari/configs/coddingtonbear.yaml` & `barbari-3.0.2/barbari/configs/coddingtonbear.yaml`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/barbari/configs/example.yaml` & `barbari-3.0.2/barbari/configs/example.yaml`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/barbari/configs/rivets.yaml` & `barbari-3.0.2/barbari/configs/rivets.yaml`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/barbari/constants.py` & `barbari-3.0.2/barbari/constants.py`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/barbari/flatcam.py` & `barbari-3.0.2/barbari/flatcam.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         input_layer: Union[FlatcamLayer, str],
         output_layer: Union[FlatcamLayer, str],
     ):
         extra_kwargs = {}
         if config.multi_depth or config.depth_per_pass:
             extra_kwargs["dpp"] = config.depth_per_pass
 
-        return super().__init__(
+        super().__init__(
             "cncjob",
             self.get_layer_name(input_layer),
             z_cut=config.cut_z,
             z_move=config.travel_z,
             feedrate=config.feed_rate,
             dia=config.tool_size,
             spindlespeed=config.spindle_speed,
@@ -76,15 +76,15 @@
     def __init__(
         self,
         config: DrillHolesJobSpec,
         input_layer: Union[FlatcamLayer, str],
         output_layer: Union[FlatcamLayer, str],
         drilled_dias: List[float],
     ):
-        return super().__init__(
+        super().__init__(
             "drillcncjob",
             self.get_layer_name(input_layer),
             drilled_dias=",".join(str(dia) for dia in drilled_dias),
             drillz=config.drill_z,
             travelz=config.travel_z,
             feedrate_z=config.feed_rate,
             spindlespeed=config.spindle_speed,
@@ -96,15 +96,15 @@
     def __init__(
         self,
         config: MillHolesJobSpec,
         input_layer: Union[FlatcamLayer, str],
         output_layer: Union[FlatcamLayer, str],
         milled_dias: List[float],
     ):
-        return super().__init__(
+        super().__init__(
             "milldrills",
             self.get_layer_name(input_layer),
             tooldia=config.tool_size,
             milled_dias=",".join(str(dia) for dia in milled_dias),
             outname=self.get_layer_name(output_layer),
         )
 
@@ -113,15 +113,15 @@
     def __init__(
         self,
         config: MillSlotsJobSpec,
         input_layer: Union[FlatcamLayer, str],
         output_layer: Union[FlatcamLayer, str],
         milled_dias: List[float],
     ):
-        return super().__init__(
+        super().__init__(
             "millslots",
             self.get_layer_name(input_layer),
             tooldia=config.tool_size,
             milled_dias=",".join(str(dia) for dia in milled_dias),
             outname=self.get_layer_name(output_layer),
         )
 
@@ -129,15 +129,15 @@
 class FlatcamIsolate(FlatcamProcess):
     def __init__(
         self,
         config: IsolationRoutingJobSpec,
         input_layer: Union[FlatcamLayer, str],
         output_layer: Union[FlatcamLayer, str],
     ):
-        return super().__init__(
+        super().__init__(
             "isolate",
             self.get_layer_name(input_layer),
             dia=config.tool_size,
             passes=int(config.passes),
             overlap=config.pass_overlap,
             combine=1,
             outname=self.get_layer_name(output_layer),
@@ -150,15 +150,15 @@
         layer: Union[FlatcamLayer, str],
         path: str,
         counter: int,
         name: str,
         tool_name: str,
         tool_size: float,
     ):
-        return super().__init__(
+        super().__init__(
             "write_gcode",
             self.get_layer_name(layer),
             os.path.join(
                 path,
                 "{counter}.{name}.{tool_size}.{tool_name}.gcode".format(
                     counter=str(counter).zfill(2),
                     name=name,
```

### Comparing `barbari-3.0.1/barbari/gerbers.py` & `barbari-3.0.2/barbari/gerbers.py`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/barbari/main.py` & `barbari-3.0.2/barbari/main.py`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/barbari.egg-info/SOURCES.txt` & `barbari-3.0.2/barbari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `barbari-3.0.1/setup.py` & `barbari-3.0.2/setup.py`

 * *Files identical despite different names*

