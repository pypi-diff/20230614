# Comparing `tmp/panda_utils-1.2.1.tar.gz` & `tmp/panda_utils-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.2.1.tar", last modified: Tue Jun 13 13:13:23 2023, max compression
+gzip compressed data, was "panda_utils-1.3.tar", last modified: Wed Jun 14 19:27:38 2023, max compression
```

## Comparing `panda_utils-1.2.1.tar` & `panda_utils-1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.414693 panda_utils-1.2.1/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1080 2022-08-12 11:48:21.000000 panda_utils-1.2.1/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    19196 2023-06-13 13:13:23.414693 panda_utils-1.2.1/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    18466 2023-06-13 13:12:03.000000 panda_utils-1.2.1/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.2.1/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.411359 panda_utils-1.2.1/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.2.1/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.2.1/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.414693 panda_utils-1.2.1/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.2.1/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3712 2023-06-13 13:13:16.000000 panda_utils-1.2.1/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      256 2023-06-13 10:12:15.000000 panda_utils-1.2.1/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.2.1/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     9059 2023-06-13 12:08:12.000000 panda_utils-1.2.1/panda_utils/assetpipeline/models.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.2.1/panda_utils/assetpipeline/textures.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.414693 panda_utils-1.2.1/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.2.1/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.2.1/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.2.1/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.414693 panda_utils-1.2.1/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.2.1/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5178 2023-06-12 15:26:37.000000 panda_utils-1.2.1/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.2.1/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.414693 panda_utils-1.2.1/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.2.1/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.2.1/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.2.1/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.2.1/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.2.1/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.2.1/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2482 2023-06-12 19:50:06.000000 panda_utils-1.2.1/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.411359 panda_utils-1.2.1/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    19196 2023-06-13 13:13:23.000000 panda_utils-1.2.1/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      916 2023-06-13 13:13:23.000000 panda_utils-1.2.1/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-06-13 13:13:23.000000 panda_utils-1.2.1/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-06-13 13:13:23.000000 panda_utils-1.2.1/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-06-13 13:13:23.000000 panda_utils-1.2.1/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-06-13 10:37:23.000000 panda_utils-1.2.1/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.2.1/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-06-13 13:13:23.414693 panda_utils-1.2.1/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.510842 panda_utils-1.3/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1080 2022-08-12 11:48:21.000000 panda_utils-1.3/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    20931 2023-06-14 19:27:38.510842 panda_utils-1.3/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    20203 2023-06-14 19:27:28.000000 panda_utils-1.3/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.3/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.467509 panda_utils-1.3/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.3/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.510842 panda_utils-1.3/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.3/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3715 2023-06-13 13:14:07.000000 panda_utils-1.3/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      256 2023-06-13 10:12:15.000000 panda_utils-1.3/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.3/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    10820 2023-06-14 19:20:04.000000 panda_utils-1.3/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.3/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.510842 panda_utils-1.3/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.3/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.3/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.3/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.510842 panda_utils-1.3/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.3/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5179 2023-06-14 17:29:22.000000 panda_utils-1.3/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.3/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.510842 panda_utils-1.3/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.3/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.3/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.3/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.3/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.3/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2482 2023-06-12 19:50:06.000000 panda_utils-1.3/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.470842 panda_utils-1.3/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    20931 2023-06-14 19:27:38.000000 panda_utils-1.3/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      916 2023-06-14 19:27:38.000000 panda_utils-1.3/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-06-14 19:27:38.000000 panda_utils-1.3/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-06-14 19:27:38.000000 panda_utils-1.3/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-06-14 19:27:38.000000 panda_utils-1.3/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1021 2023-06-14 19:20:10.000000 panda_utils-1.3/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.3/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-06-14 19:27:38.510842 panda_utils-1.3/setup.cfg
```

### Comparing `panda_utils-1.2.1/LICENSE` & `panda_utils-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/PKG-INFO` & `panda_utils-1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,8 @@
-Metadata-Version: 2.1
-Name: panda_utils
-Version: 1.2.1
-Summary: PandaUtils includes multiple tools for basic Panda3D automation
-Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
-Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
-Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: imagery
-Provides-Extra: autopath
-Provides-Extra: runnable
-Provides-Extra: pipeline
-Provides-Extra: everything
-License-File: LICENSE
-
-# Panda3D Utils v1.2.1
+# Panda3D Utils v1.3
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -202,15 +183,16 @@
 in order, first the node will be rescaled, and then it will be rotated.
 When a `collide[]` action is encountered, it will be called once with the given
 arguments. If a different `[]` action is encountered, it will not run.
 This method is used for easy interaction with Makefiles (if the input folder 
 is set as the makefile dependency, changing this file will cause the task
 building a given asset to be rerun).
 
-The pipeline will normally hide 
+The pipeline will normally hide all outputs unless the environmental variable
+`PANDA_UTILS_LOGGING`  is not empty.
 
 The list of all currently existing steps is below.
 
 ### Preblend
 
 This step will convert OBJ or FBX models into BLEND. It requires installing
 Blender on the machine. Note that due to specifics of various modeling software,
@@ -270,35 +252,96 @@
 
 ### Optimize
 
 This step will do the following transformations to every EGG model it finds:
 
 * Removes the default cube `Cube.N` and camera `Camera` groups from the file
   if they're found inside.
-* Creates a group with the same name as the model name, containing everything
-  inside of the model. This is useful if the Panda3D code is using `find()`
-  while loading this model.
 * Renames all textures to follow a consistent naming pattern. For example,
   if textures `file1.png`, `Randomfile.jpg` and `otherFile.png` are provided,
   they will be renamed into `input_folder.png`, `input_folder-1.jpg` and
   `input_folder-2.png` (the order is not guaranteed, but it will be consistent
   if this step is launched multiple times).
 
-This function takes one required parameter `profile`. However, the profile
-is currently ignored. In the future, there will be multiple profiles that can
-(for example) run egg-optchar, etc.
+This function takes no parameters.
 
 **Changelog**
+* 1.3 - no longer takes parameters, no longer sets model parents
+  (see: `model_parent`)
 * 1.2 - no longer changes the texture path prefix (now done by egg2bam)
 * 1.1 - initial implementation
 
 **Examples**
-* `optimize:stiffchar`
-* `optimize:actorchar`
-* `optimize:prop`
+* `optimize`
+
+### Model Parent
+This step creates a group with the same name as the model name, containing
+the entire model inside itself. This can be useful if the Panda3D code is using
+`find()` while loading this model.
+
+This step takes no parameters.
+
+**Changelog**
+* 1.3 - initial implementation
+
+*Examples**
+* `model_parent`
+
+### Group rename
+This step renames all collections with the given name into a different name.
+
+This step uses keyword arguments, which means it can only be run through `[]`.
+Setting a name to `__delete__` will delete the node. For example:
+
+```yaml
+group_rename:
+  hands.003: hands
+  useless-node: __delete__
+```
+
+**Changelog**
+* 1.3 - initial implementation
+
+*Examples**
+* `group_rename[]`
+
+### Group remove
+This step removes all collections with the given name. Unlike group rename,
+allows using fnmatch syntax to find the collections.
+
+Accepts one argument equal to the fnmatch pattern that is removed. Can be
+run multiple times if desired.
+
+```yaml
+group_rename:
+  hands.003: hands
+  useless-node: __delete__
+```
+
+**Changelog**
+* 1.3 - initial implementation
+
+*Examples**
+* `group_remove[]`
+* `group_remove:*useless*`
+
+### Optchar
+This step runs `egg-optchar`, setting the exposed joints and the flagged nodes.
+Note that changing the dart is currently not supported.
+
+This model takes two parameters. Both of them can be comma-separated strings,
+or lists of strings (only if the `[]` syntax is used). The first parameter is
+the flagged nodes, the second parameter is the exposed joints.
+
+**Changelog**
+* 1.3 - initial implementation
+
+**Examples**
+* `optchar[]`
+* `optchar:this-node-has-texture-set:joint_whatever`
 
 ### Transform
 
 This step will apply the given transforms to every egg file it encounters.
 Each transform is a combination of scale, rotate, and translate. For example:
 
 * `transform:10:0,0,180:0,-0.25,1`
@@ -406,20 +449,25 @@
 * `texture_cards:512`
 
 ### Palettize
 
 This step is used to join multiple texture files on a model into one palette.
 It will palettize every EGG model in the folder.
 
-This step takes one parameter, the desired texture size. It must be a power
-of two. The default value is 1024, which means each produced palette will be
-1024x1024.
+This step takes up to two parameters. The first parameter is required: the
+desired texture size. It must be a power of two. The default value is 1024,
+which means each produced palette will be 1024x1024.
+
+The second parameter is optional and includes zero or more comma-separated
+words, defaults to empty:
+* `ordered` - if the palettized images were named `{number}-{name}`, changes
+  the palettized node name to `name`. Primarily used with texture-cards stage.
 
 **Changelog**
-* 1.2.1 - renamed from `3d_palettize` to `palettize`
+* 1.2.1 - renamed from `3d_palettize` to `palettize`, added `ordered` flag
 * 1.2 - initial implementation
 
 **Examples**
 * `palettize`
 * `palettize:2048`
 
 ### Egg2Bam
```

### Comparing `panda_utils-1.2.1/README.md` & `panda_utils-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,27 @@
-# Panda3D Utils v1.2.1
+Metadata-Version: 2.1
+Name: panda_utils
+Version: 1.3
+Summary: PandaUtils includes multiple tools for basic Panda3D automation
+Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
+Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
+Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: imagery
+Provides-Extra: autopath
+Provides-Extra: runnable
+Provides-Extra: pipeline
+Provides-Extra: everything
+License-File: LICENSE
+
+# Panda3D Utils v1.3
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -183,15 +202,16 @@
 in order, first the node will be rescaled, and then it will be rotated.
 When a `collide[]` action is encountered, it will be called once with the given
 arguments. If a different `[]` action is encountered, it will not run.
 This method is used for easy interaction with Makefiles (if the input folder 
 is set as the makefile dependency, changing this file will cause the task
 building a given asset to be rerun).
 
-The pipeline will normally hide 
+The pipeline will normally hide all outputs unless the environmental variable
+`PANDA_UTILS_LOGGING`  is not empty.
 
 The list of all currently existing steps is below.
 
 ### Preblend
 
 This step will convert OBJ or FBX models into BLEND. It requires installing
 Blender on the machine. Note that due to specifics of various modeling software,
@@ -251,35 +271,96 @@
 
 ### Optimize
 
 This step will do the following transformations to every EGG model it finds:
 
 * Removes the default cube `Cube.N` and camera `Camera` groups from the file
   if they're found inside.
-* Creates a group with the same name as the model name, containing everything
-  inside of the model. This is useful if the Panda3D code is using `find()`
-  while loading this model.
 * Renames all textures to follow a consistent naming pattern. For example,
   if textures `file1.png`, `Randomfile.jpg` and `otherFile.png` are provided,
   they will be renamed into `input_folder.png`, `input_folder-1.jpg` and
   `input_folder-2.png` (the order is not guaranteed, but it will be consistent
   if this step is launched multiple times).
 
-This function takes one required parameter `profile`. However, the profile
-is currently ignored. In the future, there will be multiple profiles that can
-(for example) run egg-optchar, etc.
+This function takes no parameters.
 
 **Changelog**
+* 1.3 - no longer takes parameters, no longer sets model parents
+  (see: `model_parent`)
 * 1.2 - no longer changes the texture path prefix (now done by egg2bam)
 * 1.1 - initial implementation
 
 **Examples**
-* `optimize:stiffchar`
-* `optimize:actorchar`
-* `optimize:prop`
+* `optimize`
+
+### Model Parent
+This step creates a group with the same name as the model name, containing
+the entire model inside itself. This can be useful if the Panda3D code is using
+`find()` while loading this model.
+
+This step takes no parameters.
+
+**Changelog**
+* 1.3 - initial implementation
+
+*Examples**
+* `model_parent`
+
+### Group rename
+This step renames all collections with the given name into a different name.
+
+This step uses keyword arguments, which means it can only be run through `[]`.
+Setting a name to `__delete__` will delete the node. For example:
+
+```yaml
+group_rename:
+  hands.003: hands
+  useless-node: __delete__
+```
+
+**Changelog**
+* 1.3 - initial implementation
+
+*Examples**
+* `group_rename[]`
+
+### Group remove
+This step removes all collections with the given name. Unlike group rename,
+allows using fnmatch syntax to find the collections.
+
+Accepts one argument equal to the fnmatch pattern that is removed. Can be
+run multiple times if desired.
+
+```yaml
+group_rename:
+  hands.003: hands
+  useless-node: __delete__
+```
+
+**Changelog**
+* 1.3 - initial implementation
+
+*Examples**
+* `group_remove[]`
+* `group_remove:*useless*`
+
+### Optchar
+This step runs `egg-optchar`, setting the exposed joints and the flagged nodes.
+Note that changing the dart is currently not supported.
+
+This model takes two parameters. Both of them can be comma-separated strings,
+or lists of strings (only if the `[]` syntax is used). The first parameter is
+the flagged nodes, the second parameter is the exposed joints.
+
+**Changelog**
+* 1.3 - initial implementation
+
+**Examples**
+* `optchar[]`
+* `optchar:this-node-has-texture-set:joint_whatever`
 
 ### Transform
 
 This step will apply the given transforms to every egg file it encounters.
 Each transform is a combination of scale, rotate, and translate. For example:
 
 * `transform:10:0,0,180:0,-0.25,1`
@@ -387,20 +468,25 @@
 * `texture_cards:512`
 
 ### Palettize
 
 This step is used to join multiple texture files on a model into one palette.
 It will palettize every EGG model in the folder.
 
-This step takes one parameter, the desired texture size. It must be a power
-of two. The default value is 1024, which means each produced palette will be
-1024x1024.
+This step takes up to two parameters. The first parameter is required: the
+desired texture size. It must be a power of two. The default value is 1024,
+which means each produced palette will be 1024x1024.
+
+The second parameter is optional and includes zero or more comma-separated
+words, defaults to empty:
+* `ordered` - if the palettized images were named `{number}-{name}`, changes
+  the palettized node name to `name`. Primarily used with texture-cards stage.
 
 **Changelog**
-* 1.2.1 - renamed from `3d_palettize` to `palettize`
+* 1.2.1 - renamed from `3d_palettize` to `palettize`, added `ordered` flag
 * 1.2 - initial implementation
 
 **Examples**
 * `palettize`
 * `palettize:2048`
 
 ### Egg2Bam
```

### Comparing `panda_utils-1.2.1/panda_utils/__main__.py` & `panda_utils-1.3/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.3/panda_utils/assetpipeline/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,8 +103,8 @@
             if use_config:
                 ctx.run_action_through_config(action, method_name)
             else:
                 action(ctx, *args)
 
 
 if __name__ == "__main__":
-    main(os.getenv("PIPELINE_LOGGING") != "")
+    main(os.getenv("PANDA_UTILS_LOGGING") != "")
```

### Comparing `panda_utils-1.2.1/panda_utils/assetpipeline/models.py` & `panda_utils-1.3/panda_utils/assetpipeline/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import fnmatch
 import logging
 import os
 import re
 import shutil
 import subprocess
 from pathlib import Path
 
@@ -86,17 +87,15 @@
 def action_bam2egg(ctx):
     for file in ctx.files:
         if file.endswith(".bam"):
             logger.info("%s: Converting %s from Bam to Egg", ctx.name, file)
             bam2egg(ctx.putil_ctx, file)
 
 
-def action_optimize(ctx, mechanism):
-    logger.info("%s: Using optimization mechanism: %s", ctx.name, mechanism)
-
+def action_optimize(ctx):
     all_eggs = {}
     textures = set()
     for file in ctx.files:
         if file.endswith(".egg"):
             with open(file) as f:
                 all_eggs[file] = tree = eggparse.egg_tokenize(f.readlines())
                 for tex in tree.findall("Texture"):
@@ -117,16 +116,26 @@
         nodeset = set()
         for node in eggtree.children:
             if isinstance(node, eggparse.EggBranch) and node.node_type == "Group":
                 if node.node_name == "Camera" or node.node_name.startswith("Cube."):
                     nodeset.add(node)
         eggtree.remove_nodes(nodeset)
 
-        # For now we're also going to rename the top node into the model name, even though it's not
-        # strictly correct to do
+        with open(file, "w") as f:
+            f.write(str(eggtree))
+
+
+def action_model_parent(ctx):
+    for file in ctx.files:
+        if not file.endswith(".egg"):
+            continue
+
+        with open(file) as f:
+            eggtree = eggparse.egg_tokenize(f.readlines())
+
         if not any(group for group in eggtree.findall("Group") if group.node_name == ctx.model_name):
             group_node = eggparse.EggBranch("Group", ctx.model_name, [])
             removed_children = set()
             for node in eggtree.children:
                 if isinstance(node, eggparse.EggBranch) and node.node_type == "Group":
                     group_node.children.append(node)
                     removed_children.add(node)
@@ -211,14 +220,70 @@
     )
 
     if "ordered" in flag_list:
         for file in all_eggs:
             remove_palette_indices(file)
 
 
+def action_optchar(ctx, flags, expose):
+    if isinstance(flags, str):
+        flags = flags.split(",")
+    if isinstance(expose, str):
+        expose = expose.split(",")
+
+    for file in ctx.files:
+        if file.endswith(".egg"):
+            command = ["egg-optchar", file, "-inplace", "-keepall"]
+
+            for flag in flags:
+                command.append("-flag")
+                command.append(flag)
+
+            for joint in expose:
+                command.append("-expose")
+                command.append(joint)
+
+            util.run_panda(ctx.putil_ctx, *command)
+
+
+def action_group_rename(ctx, **kwargs):
+    for file in ctx.files:
+        if file.endswith(".egg"):
+            with open(file) as f:
+                tree = eggparse.egg_tokenize(f.readlines())
+
+            removals = set()
+            for group in tree.findall("Group"):
+                if new_name := kwargs.get(group.node_name):
+                    if new_name == "__delete__":
+                        removals.add(group)
+                    else:
+                        group.node_name = new_name
+
+            tree.remove_nodes(removals)
+            with open(file, "w") as f:
+                f.write(str(tree))
+
+
+def action_group_remove(ctx, pattern):
+    for file in ctx.files:
+        if file.endswith(".egg"):
+            with open(file) as f:
+                tree = eggparse.egg_tokenize(f.readlines())
+
+            removals = set()
+            for group in tree.findall("Group"):
+                if fnmatch.fnmatch(group.node_name, pattern):
+                    removals.add(group)
+
+            tree.remove_nodes(removals)
+            with open(file, "w") as f:
+                f.write(str(tree))
+
+
 def action_egg2bam(ctx):
     files = []
     for file in ctx.files:
         if file.endswith(".egg"):
             logger.info("%s: Copying %s into the dist directory", ctx.name, file)
             files.append(file)
```

### Comparing `panda_utils-1.2.1/panda_utils/assetpipeline/textures.py` & `panda_utils-1.3/panda_utils/assetpipeline/textures.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/panda_utils/blender/import_model.py` & `panda_utils-1.3/panda_utils/blender/import_model.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/panda_utils/eggtree/eggparse.py` & `panda_utils-1.3/panda_utils/eggtree/eggparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 def sanitize_string(val):
     if val and val[0] in '"\'':
         return val[1:-1]
     return val
 
 
 single_line_leaf_regex = re.compile(r"<([A-Za-z0-9_$]+)> ([-a-z0-9A-Z_.]+ )?\{ ?(.+) ?}")
-preline_regex = re.compile(r"<([A-Za-z0-9_$]+)> ([-a-z0-9A-Z_.<>\"]+ )?\{([^\n]*)")
+preline_regex = re.compile(r"<([A-Za-z0-9_$]+)> ([-a-z0-9A-Z_.<>\" ]+ )?\{([^\n]*)")
 
 
 def subtree_tokenize(lines: List[str]):
     last_line = lines[-1].strip()
     if len(lines) == 1:
         match = single_line_leaf_regex.match(last_line)
         if not match:
```

### Comparing `panda_utils-1.2.1/panda_utils/eggtree/operations.py` & `panda_utils-1.3/panda_utils/eggtree/operations.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/panda_utils/tools/animconvert.py` & `panda_utils-1.3/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/panda_utils/tools/convert.py` & `panda_utils-1.3/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/panda_utils/tools/downscale.py` & `panda_utils-1.3/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/panda_utils/tools/palettize.py` & `panda_utils-1.3/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/panda_utils/tools/toontown.py` & `panda_utils-1.3/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/panda_utils/util.py` & `panda_utils-1.3/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.3/panda_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-utils
-Version: 1.2.1
+Version: 1.3
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: imagery
 Provides-Extra: autopath
 Provides-Extra: runnable
 Provides-Extra: pipeline
 Provides-Extra: everything
 License-File: LICENSE
 
-# Panda3D Utils v1.2.1
+# Panda3D Utils v1.3
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -202,15 +202,16 @@
 in order, first the node will be rescaled, and then it will be rotated.
 When a `collide[]` action is encountered, it will be called once with the given
 arguments. If a different `[]` action is encountered, it will not run.
 This method is used for easy interaction with Makefiles (if the input folder 
 is set as the makefile dependency, changing this file will cause the task
 building a given asset to be rerun).
 
-The pipeline will normally hide 
+The pipeline will normally hide all outputs unless the environmental variable
+`PANDA_UTILS_LOGGING`  is not empty.
 
 The list of all currently existing steps is below.
 
 ### Preblend
 
 This step will convert OBJ or FBX models into BLEND. It requires installing
 Blender on the machine. Note that due to specifics of various modeling software,
@@ -270,35 +271,96 @@
 
 ### Optimize
 
 This step will do the following transformations to every EGG model it finds:
 
 * Removes the default cube `Cube.N` and camera `Camera` groups from the file
   if they're found inside.
-* Creates a group with the same name as the model name, containing everything
-  inside of the model. This is useful if the Panda3D code is using `find()`
-  while loading this model.
 * Renames all textures to follow a consistent naming pattern. For example,
   if textures `file1.png`, `Randomfile.jpg` and `otherFile.png` are provided,
   they will be renamed into `input_folder.png`, `input_folder-1.jpg` and
   `input_folder-2.png` (the order is not guaranteed, but it will be consistent
   if this step is launched multiple times).
 
-This function takes one required parameter `profile`. However, the profile
-is currently ignored. In the future, there will be multiple profiles that can
-(for example) run egg-optchar, etc.
+This function takes no parameters.
 
 **Changelog**
+* 1.3 - no longer takes parameters, no longer sets model parents
+  (see: `model_parent`)
 * 1.2 - no longer changes the texture path prefix (now done by egg2bam)
 * 1.1 - initial implementation
 
 **Examples**
-* `optimize:stiffchar`
-* `optimize:actorchar`
-* `optimize:prop`
+* `optimize`
+
+### Model Parent
+This step creates a group with the same name as the model name, containing
+the entire model inside itself. This can be useful if the Panda3D code is using
+`find()` while loading this model.
+
+This step takes no parameters.
+
+**Changelog**
+* 1.3 - initial implementation
+
+*Examples**
+* `model_parent`
+
+### Group rename
+This step renames all collections with the given name into a different name.
+
+This step uses keyword arguments, which means it can only be run through `[]`.
+Setting a name to `__delete__` will delete the node. For example:
+
+```yaml
+group_rename:
+  hands.003: hands
+  useless-node: __delete__
+```
+
+**Changelog**
+* 1.3 - initial implementation
+
+*Examples**
+* `group_rename[]`
+
+### Group remove
+This step removes all collections with the given name. Unlike group rename,
+allows using fnmatch syntax to find the collections.
+
+Accepts one argument equal to the fnmatch pattern that is removed. Can be
+run multiple times if desired.
+
+```yaml
+group_rename:
+  hands.003: hands
+  useless-node: __delete__
+```
+
+**Changelog**
+* 1.3 - initial implementation
+
+*Examples**
+* `group_remove[]`
+* `group_remove:*useless*`
+
+### Optchar
+This step runs `egg-optchar`, setting the exposed joints and the flagged nodes.
+Note that changing the dart is currently not supported.
+
+This model takes two parameters. Both of them can be comma-separated strings,
+or lists of strings (only if the `[]` syntax is used). The first parameter is
+the flagged nodes, the second parameter is the exposed joints.
+
+**Changelog**
+* 1.3 - initial implementation
+
+**Examples**
+* `optchar[]`
+* `optchar:this-node-has-texture-set:joint_whatever`
 
 ### Transform
 
 This step will apply the given transforms to every egg file it encounters.
 Each transform is a combination of scale, rotate, and translate. For example:
 
 * `transform:10:0,0,180:0,-0.25,1`
@@ -406,20 +468,25 @@
 * `texture_cards:512`
 
 ### Palettize
 
 This step is used to join multiple texture files on a model into one palette.
 It will palettize every EGG model in the folder.
 
-This step takes one parameter, the desired texture size. It must be a power
-of two. The default value is 1024, which means each produced palette will be
-1024x1024.
+This step takes up to two parameters. The first parameter is required: the
+desired texture size. It must be a power of two. The default value is 1024,
+which means each produced palette will be 1024x1024.
+
+The second parameter is optional and includes zero or more comma-separated
+words, defaults to empty:
+* `ordered` - if the palettized images were named `{number}-{name}`, changes
+  the palettized node name to `name`. Primarily used with texture-cards stage.
 
 **Changelog**
-* 1.2.1 - renamed from `3d_palettize` to `palettize`
+* 1.2.1 - renamed from `3d_palettize` to `palettize`, added `ordered` flag
 * 1.2 - initial implementation
 
 **Examples**
 * `palettize`
 * `palettize:2048`
 
 ### Egg2Bam
```

### Comparing `panda_utils-1.2.1/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.3/panda_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2.1/pyproject.toml` & `panda_utils-1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.2.1"
+version = "1.3"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

