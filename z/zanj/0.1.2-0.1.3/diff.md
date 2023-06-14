# Comparing `tmp/zanj-0.1.2.tar.gz` & `tmp/zanj-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zanj-0.1.2.tar", max compression
+gzip compressed data, was "zanj-0.1.3.tar", max compression
```

## Comparing `zanj-0.1.2.tar` & `zanj-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 zanj-0.1.2/LICENSE
--rw-r--r--   0        0        0      937 2023-06-13 22:17:51.834629 zanj-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4291 2023-05-28 07:47:30.325865 zanj-0.1.2/README.md
--rw-r--r--   0        0        0      146 2023-06-13 22:17:56.392498 zanj-0.1.2/zanj/__init__.py
--rw-r--r--   0        0        0     1468 2023-05-28 05:22:18.527493 zanj-0.1.2/zanj/externals.py
--rw-r--r--   0        0        0    15618 2023-05-28 05:22:18.537492 zanj-0.1.2/zanj/loading.py
--rw-r--r--   0        0        0        0 2023-06-13 22:16:55.290434 zanj-0.1.2/zanj/py.typed
--rw-r--r--   0        0        0     4143 2023-05-28 05:13:20.057826 zanj-0.1.2/zanj/readme.md
--rw-r--r--   0        0        0     8121 2023-05-28 05:22:18.541492 zanj-0.1.2/zanj/serializing.py
--rw-r--r--   0        0        0     9696 2023-05-28 05:22:18.549492 zanj-0.1.2/zanj/torchutil.py
--rw-r--r--   0        0        0     8468 2023-05-28 05:22:18.555490 zanj-0.1.2/zanj/zanj.py
--rw-r--r--   0        0        0     5167 1970-01-01 00:00:00.000000 zanj-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 zanj-0.1.3/LICENSE
+-rw-r--r--   0        0        0      985 2023-06-14 03:59:17.522477 zanj-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9859 2023-06-14 03:53:30.481952 zanj-0.1.3/README.md
+-rw-r--r--   0        0        0      146 2023-06-14 03:59:11.003706 zanj-0.1.3/zanj/__init__.py
+-rw-r--r--   0        0        0     1468 2023-05-28 05:22:18.527493 zanj-0.1.3/zanj/externals.py
+-rw-r--r--   0        0        0    15618 2023-05-28 05:22:18.537492 zanj-0.1.3/zanj/loading.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:16:55.290434 zanj-0.1.3/zanj/py.typed
+-rw-r--r--   0        0        0     4143 2023-05-28 05:13:20.057826 zanj-0.1.3/zanj/readme.md
+-rw-r--r--   0        0        0     8121 2023-05-28 05:22:18.541492 zanj-0.1.3/zanj/serializing.py
+-rw-r--r--   0        0        0     9778 2023-06-14 03:53:30.489964 zanj-0.1.3/zanj/torchutil.py
+-rw-r--r--   0        0        0     8468 2023-05-28 05:22:18.555490 zanj-0.1.3/zanj/zanj.py
+-rw-r--r--   0        0        0    10735 1970-01-01 00:00:00.000000 zanj-0.1.3/PKG-INFO
```

### Comparing `zanj-0.1.2/LICENSE` & `zanj-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zanj-0.1.2/pyproject.toml` & `zanj-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zanj"
-version = "0.1.2"
+version = "0.1.3"
 description = "save and load complex objects to disk without pickling"
 license = "GPL-3.0-only"
 authors = ["mivanit <mivanits@umich.edu>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -24,14 +24,16 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 black = "^23.1.0"
 pylint = "^2.16.4"
 pycln = "^2.1.3"
 isort = "^5.12.0"
 mypy = "^1.0.1"
+pytest-cov = "^4.1.0"
+coverage-badge = "^1.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pycln]
 all = true
```

### Comparing `zanj-0.1.2/README.md` & `zanj-0.1.3/zanj/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-# ZANJ
-
-# installation
-PyPi: https://pypi.org/project/zanj/
-
-```
-pip install zanj
-```
 
 # Overview
 
 The `ZANJ` format is meant to be a way of saving arbitrary objects to disk, in a way that is flexible, allows to keep configuration and data together, and is human readable. It is loosely inspired by HDF5 and the derived `exdir` format, and the implementation is similar to `npz` files. The on-disk format is as follows:
 
 a file `<filename>.zanj` is a zip file containing:
 
@@ -22,20 +14,20 @@
 		- `.npy` for numpy arrays or torch tensors
 		- `.jsonl` for pandas dataframes or large sequences
 	- list of external files stored in `__zanj_meta__.json`
 	- "$ref" key will have value pointing to external file
 	- `__format__` key will detail an external format type
 
 
-This library was originally a module in [muutils](https://github.com/mivanit/muutils/)
-
 # Implementation
 
 ## `ZANJ`
 
+> located in `zanj.zanj`
+
 main class for saving and loading zanj files
 
 contains some configuration info about saving, such as:
 
 - thresholds for how big an array/table has to be before moving to external file
 - compression settings
 - error modes
@@ -66,8 +58,8 @@
 - Lazy loading: Can I inspect the file without loading everything ? And loading only some tensors in it without scanning the whole file (distributed setting) ?
 - Layout control: Lazy loading, is not necessarily enough since if the information about tensors is spread out in your file, then even if the information is lazily accessible you might have to access most of your file to read the available tensors (incurring many DISK -> RAM copies). Controlling the layout to keep fast access to single tensors is important.
 - No file size limit: Is there a limit to the file size ?
 - Flexibility: Can I save custom code in the format and be able to use it later with zero extra code ? (~ means we can store more than pure tensors, but no custom code)
 - Bfloat16: Does the format support native bfloat16 (meaning no weird workarounds are necessary)? This is becoming increasingly important in the ML world.
 
 
-(This table was stolen from [safetensors](https://github.com/huggingface/safetensors/blob/main/README.md))
+(This table was Stolen from [safetensors](https://github.com/huggingface/safetensors/blob/main/README.md))
```

### Comparing `zanj-0.1.2/zanj/externals.py` & `zanj-0.1.3/zanj/externals.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.2/zanj/loading.py` & `zanj-0.1.3/zanj/loading.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.2/zanj/serializing.py` & `zanj-0.1.3/zanj/serializing.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.2/zanj/torchutil.py` & `zanj-0.1.3/zanj/torchutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,23 +31,26 @@
     unique: list[torch.nn.Parameter] = list(
         {p.data_ptr(): p for p in parameters}.values()
     )
 
     return sum(p.numel() for p in unique)
 
 
-def get_device(
+def get_module_device(
     m: torch.nn.Module,
-) -> tuple[bool, torch.device | dict[str, torch.device],]:
+) -> tuple[bool, torch.device | dict[str, torch.device]]:
     """get the current devices"""
 
     devs: dict[str, torch.device] = {name: p.device for name, p in m.named_parameters()}
 
-    # check if all devices are the same
-    dev_uni: torch.device = list(devs.values())[0]
+    if len(devs) == 0:
+        return False, devs
+
+    # check if all devices are the same by getting one device
+    dev_uni: torch.device = next(iter(devs.values()))
 
     if all(dev == dev_uni for dev in devs.values()):
         return True, dev_uni
     else:
         return False, devs
```

### Comparing `zanj-0.1.2/zanj/zanj.py` & `zanj-0.1.3/zanj/zanj.py`

 * *Files identical despite different names*

