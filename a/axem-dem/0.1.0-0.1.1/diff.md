# Comparing `tmp/axem_dem-0.1.0.tar.gz` & `tmp/axem_dem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axem_dem-0.1.0.tar", max compression
+gzip compressed data, was "axem_dem-0.1.1.tar", max compression
```

## Comparing `axem_dem-0.1.0.tar` & `axem_dem-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    13291 2023-03-29 12:37:24.312474 axem_dem-0.1.0/LICENSE
--rw-r--r--   0        0        0     1373 2023-04-26 14:09:57.148630 axem_dem-0.1.0/README.md
--rw-r--r--   0        0        0      210 2023-02-17 13:29:58.234451 axem_dem-0.1.0/dem/__init__.py
--rw-r--r--   0        0        0      423 2023-05-02 07:11:36.902063 axem_dem-0.1.0/dem/__main__.py
--rw-r--r--   0        0        0     1884 2023-04-30 14:05:41.793486 axem_dem-0.1.0/dem/cli/command/clone_cmd.py
--rw-r--r--   0        0        0     2554 2023-04-19 08:55:43.195068 axem_dem-0.1.0/dem/cli/command/create_cmd.py
--rw-r--r--   0        0        0     2051 2023-04-19 09:09:24.159218 axem_dem-0.1.0/dem/cli/command/delete_cmd.py
--rw-r--r--   0        0        0     1826 2023-04-24 11:11:58.058824 axem_dem-0.1.0/dem/cli/command/info_cmd.py
--rw-r--r--   0        0        0     5150 2023-04-24 11:11:58.058824 axem_dem-0.1.0/dem/cli/command/list_cmd.py
--rw-r--r--   0        0        0     3571 2023-04-19 08:55:43.195068 axem_dem-0.1.0/dem/cli/command/modify_cmd.py
--rw-r--r--   0        0        0     4106 2023-04-24 11:11:58.058824 axem_dem-0.1.0/dem/cli/command/pull_cmd.py
--rw-r--r--   0        0        0     1389 2023-04-19 08:56:04.295193 axem_dem-0.1.0/dem/cli/command/rename_cmd.py
--rw-r--r--   0        0        0      152 2023-03-06 12:12:01.699246 axem_dem-0.1.0/dem/cli/console.py
--rw-r--r--   0        0        0     4005 2023-04-30 14:07:08.678170 axem_dem-0.1.0/dem/cli/main.py
--rw-r--r--   0        0        0     6328 2023-04-19 08:55:43.195068 axem_dem-0.1.0/dem/cli/menu.py
--rw-r--r--   0        0        0     1493 2023-04-19 09:09:24.159218 axem_dem-0.1.0/dem/core/container_engine.py
--rw-r--r--   0        0        0     2279 2023-04-24 11:11:58.058824 axem_dem-0.1.0/dem/core/data_management.py
--rwxr-xr-x   0        0        0     7667 2023-04-24 11:11:58.058824 axem_dem-0.1.0/dem/core/dev_env_setup.py
--rw-r--r--   0        0        0      412 2023-04-24 11:11:58.058824 axem_dem-0.1.0/dem/core/exceptions.py
--rw-r--r--   0        0        0       87 2023-03-06 12:12:01.699246 axem_dem-0.1.0/dem/core/properties.py
--rw-r--r--   0        0        0      952 2023-04-24 11:11:58.058824 axem_dem-0.1.0/dem/core/registry.py
--rw-r--r--   0        0        0     1539 2023-04-24 11:11:58.058824 axem_dem-0.1.0/dem/core/tool_images.py
--rw-r--r--   0        0        0      739 2023-05-02 07:48:43.801922 axem_dem-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 axem_dem-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13291 2023-03-29 12:37:24.312474 axem_dem-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1260 2023-05-17 09:22:38.112265 axem_dem-0.1.1/README.md
+-rw-r--r--   0        0        0      210 2023-02-17 13:29:58.234451 axem_dem-0.1.1/dem/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-03 10:20:26.853532 axem_dem-0.1.1/dem/__main__.py
+-rw-r--r--   0        0        0     1884 2023-05-03 10:20:26.853532 axem_dem-0.1.1/dem/cli/command/clone_cmd.py
+-rw-r--r--   0        0        0     4291 2023-05-17 09:22:38.112265 axem_dem-0.1.1/dem/cli/command/create_cmd.py
+-rw-r--r--   0        0        0     2051 2023-04-19 09:09:24.159218 axem_dem-0.1.1/dem/cli/command/delete_cmd.py
+-rw-r--r--   0        0        0     1826 2023-04-24 11:11:58.058824 axem_dem-0.1.1/dem/cli/command/info_cmd.py
+-rw-r--r--   0        0        0     5150 2023-04-24 11:11:58.058824 axem_dem-0.1.1/dem/cli/command/list_cmd.py
+-rw-r--r--   0        0        0     3571 2023-04-19 08:55:43.195068 axem_dem-0.1.1/dem/cli/command/modify_cmd.py
+-rw-r--r--   0        0        0     4106 2023-04-24 11:11:58.058824 axem_dem-0.1.1/dem/cli/command/pull_cmd.py
+-rw-r--r--   0        0        0     1389 2023-04-19 08:56:04.295193 axem_dem-0.1.1/dem/cli/command/rename_cmd.py
+-rw-r--r--   0        0        0      152 2023-03-06 12:12:01.699246 axem_dem-0.1.1/dem/cli/console.py
+-rw-r--r--   0        0        0     4005 2023-05-03 10:20:26.853532 axem_dem-0.1.1/dem/cli/main.py
+-rw-r--r--   0        0        0     6328 2023-04-19 08:55:43.195068 axem_dem-0.1.1/dem/cli/menu.py
+-rw-r--r--   0        0        0     1493 2023-04-19 09:09:24.159218 axem_dem-0.1.1/dem/core/container_engine.py
+-rw-r--r--   0        0        0     2476 2023-05-17 09:22:38.112265 axem_dem-0.1.1/dem/core/data_management.py
+-rwxr-xr-x   0        0        0     7667 2023-04-24 11:11:58.058824 axem_dem-0.1.1/dem/core/dev_env_setup.py
+-rw-r--r--   0        0        0      412 2023-04-24 11:11:58.058824 axem_dem-0.1.1/dem/core/exceptions.py
+-rw-r--r--   0        0        0       87 2023-03-06 12:12:01.699246 axem_dem-0.1.1/dem/core/properties.py
+-rw-r--r--   0        0        0      952 2023-04-24 11:11:58.058824 axem_dem-0.1.1/dem/core/registry.py
+-rw-r--r--   0        0        0     1539 2023-04-24 11:11:58.058824 axem_dem-0.1.1/dem/core/tool_images.py
+-rw-r--r--   0        0        0      739 2023-05-17 10:15:11.907014 axem_dem-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 axem_dem-0.1.1/PKG-INFO
```

### Comparing `axem_dem-0.1.0/LICENSE` & `axem_dem-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/cli/command/clone_cmd.py` & `axem_dem-0.1.1/dem/cli/command/clone_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/cli/command/create_cmd.py` & `axem_dem-0.1.1/dem/cli/command/create_cmd.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """create CLI command implementation."""
 # dem/cli/command/create_cmd.py
 
 import typer
-import dem.core.container_engine as container_engine
-import dem.core.registry as registry
 import dem.core.data_management as data_management
 from dem.core.dev_env_setup import DevEnv, DevEnvLocal, DevEnvLocalSetup
-from dem.cli.menu import ToolTypeMenu, ToolImageMenu
+from dem.core.container_engine import ContainerEngine
 from dem.core.tool_images import ToolImages
+from dem.cli.menu import ToolTypeMenu, ToolImageMenu
+from dem.cli.console import stdout, stderr
 
 tool_image_statuses = {
     ToolImages.LOCAL_ONLY: "local",
     ToolImages.REGISTRY_ONLY: "registry",
     ToolImages.LOCAL_AND_REGISTRY: "local and registry"
 }
 
@@ -38,24 +38,64 @@
             "type": tool_type,
             "image_name": selected_tool_image[0],
             "image_version": selected_tool_image[1]
         }
         dev_env_descriptor["tools"].append(tool_descriptor)
     return dev_env_descriptor
 
-def execute(dev_env_name: str) -> None:
-    derserialized_local_dev_nev = data_management.read_deserialized_dev_env_json()
-    dev_env_local_setup = DevEnvLocalSetup(derserialized_local_dev_nev)
+def overwrite_existing_dev_env(original_dev_env: DevEnvLocal, new_dev_env_descriptor: dict) -> None:
+    original_dev_env.tools = new_dev_env_descriptor["tools"]
+
+def create_new_dev_env(dev_env_local_setup: DevEnvLocalSetup, new_dev_env_descriptor: dict) -> DevEnvLocal:
+    new_dev_env = DevEnvLocal(new_dev_env_descriptor)
+    dev_env_local_setup.dev_envs.append(new_dev_env)
+
+    return new_dev_env
+
+def pull_registry_only_images(new_dev_env: DevEnvLocal) -> None:
+    """Pull images that are only present in the registry.
+    
+    Args:
+        new_dev_env -- the new local Dev Env instance
+    """
+    container_engine = ContainerEngine()
+    for tool in new_dev_env.tools:
+        if tool["image_status"] == ToolImages.REGISTRY_ONLY:
+            image_to_pull = tool["image_name" ] + ':' + tool["image_version"]
+            stdout.print("Pulling image: " + image_to_pull)
+            container_engine.pull(image_to_pull)
+
+def create_dev_env(dev_env_local_setup: DevEnvLocalSetup, dev_env_name: str) -> DevEnvLocal:
     dev_env_original = dev_env_local_setup.get_dev_env_by_name(dev_env_name)
     if dev_env_original is not None:
         typer.confirm("The input name is already used by a Development Environment. Overwrite it?", 
                       abort=True)
 
-    dev_env_descriptor = get_dev_env_descriptor_from_user(dev_env_name)
+    new_dev_env_descriptor = get_dev_env_descriptor_from_user(dev_env_name)
     
     if dev_env_original is not None:
-        dev_env_original.tools = dev_env_descriptor["tools"]
+        overwrite_existing_dev_env(dev_env_original, new_dev_env_descriptor)
+        new_dev_env = dev_env_original
+    else:
+        new_dev_env = create_new_dev_env(dev_env_local_setup, new_dev_env_descriptor)
+
+    new_dev_env.check_image_availability(dev_env_local_setup.tool_images)
+    pull_registry_only_images(new_dev_env)
+
+    return new_dev_env
+
+def execute(dev_env_name: str) -> None:
+    derserialized_local_dev_nev = data_management.read_deserialized_dev_env_json()
+    dev_env_local_setup = DevEnvLocalSetup(derserialized_local_dev_nev)
+
+    dev_env = create_dev_env(dev_env_local_setup, dev_env_name)
+
+    # Validate the Dev Env creation
+    image_statuses = dev_env.check_image_availability(dev_env_local_setup.tool_images, 
+                                                      update_tool_images=True)
+
+    if (ToolImages.NOT_AVAILABLE in image_statuses) or (ToolImages.REGISTRY_ONLY in image_statuses):
+        stderr.print("The installation failed.")
     else:
-        new_dev_env = DevEnvLocal(dev_env_descriptor)
-        dev_env_local_setup.dev_envs.append(new_dev_env)
-    derserialized_local_dev_nev = dev_env_local_setup.get_deserialized()
-    data_management.write_deserialized_dev_env_json(derserialized_local_dev_nev)
+        stdout.print("The [yellow]" + dev_env.name + "[/] Development Environment is ready!")
+        derserialized_local_dev_nev = dev_env_local_setup.get_deserialized()
+        data_management.write_deserialized_dev_env_json(derserialized_local_dev_nev)
```

### Comparing `axem_dem-0.1.0/dem/cli/command/delete_cmd.py` & `axem_dem-0.1.1/dem/cli/command/delete_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/cli/command/info_cmd.py` & `axem_dem-0.1.1/dem/cli/command/info_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/cli/command/list_cmd.py` & `axem_dem-0.1.1/dem/cli/command/list_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/cli/command/modify_cmd.py` & `axem_dem-0.1.1/dem/cli/command/modify_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/cli/command/pull_cmd.py` & `axem_dem-0.1.1/dem/cli/command/pull_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/cli/command/rename_cmd.py` & `axem_dem-0.1.1/dem/cli/command/rename_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/cli/main.py` & `axem_dem-0.1.1/dem/cli/main.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/cli/menu.py` & `axem_dem-0.1.1/dem/cli/menu.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/core/container_engine.py` & `axem_dem-0.1.1/dem/core/container_engine.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/core/data_management.py` & `axem_dem-0.1.1/dem/core/data_management.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,17 +15,22 @@
     "development_environments": []
 }
 """
 
 class DevEnvJSON():
     """ Serialize and deserialize the dev_env.json file."""
     _path = PurePath(os.path.expanduser('~') + "/.config/axem/dev_env.json")
+    _directory = PurePath(os.path.expanduser('~') + "/.config/axem")
 
     def _create_empty_dev_env_json(self) -> None:
         """ If the dev_env.json doesn't exist, then create an emmpty one."""
+        is_path_exist = os.path.exists(self._directory)
+        if not is_path_exist:
+            os.makedirs(self._directory)
+
         dev_env_json = open(self._path, "w")
         dev_env_json.write(_empty_dev_env_json)
         dev_env_json.close()
 
     def __init__(self) -> None:
         """ Init the class with an empty placeholder for the deserialized dev_env.json file. 
             Later the variable can be to access the deserialized data, until the dev_env.json file
```

### Comparing `axem_dem-0.1.0/dem/core/dev_env_setup.py` & `axem_dem-0.1.1/dem/core/dev_env_setup.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/core/registry.py` & `axem_dem-0.1.1/dem/core/registry.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/dem/core/tool_images.py` & `axem_dem-0.1.1/dem/core/tool_images.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.1.0/pyproject.toml` & `axem_dem-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "axem-dem"
-version = "0.1.0"
+version = "0.1.1"
 description = "Manager for Containerized Development Environments"
 authors = ["janosmurai <murai.janos@gmail.com>"]
 license = "Eclipse Public License - v2.0"
 readme = "README.md"
 packages = [{include = "dem"}]
 
 [tool.poetry.scripts]
```

