# Comparing `tmp/rtex-0.0.1.tar.gz` & `tmp/rtex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtex-0.0.1.tar", last modified: Wed Jun 14 21:21:54 2023, max compression
+gzip compressed data, was "rtex-0.0.2.tar", last modified: Wed Jun 14 21:45:39 2023, max compression
```

## Comparing `rtex-0.0.1.tar` & `rtex-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:54.621401 rtex-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:54.621401 rtex-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:54.621401 rtex-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-14 21:21:43.000000 rtex-0.0.1/.github/workflows/build-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-14 21:21:43.000000 rtex-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 21:21:43.000000 rtex-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 21:21:54.621401 rtex-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-14 21:21:43.000000 rtex-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 21:21:43.000000 rtex-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:54.621401 rtex-0.0.1/rtex/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 21:21:43.000000 rtex-0.0.1/rtex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-14 21:21:43.000000 rtex-0.0.1/rtex/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-14 21:21:43.000000 rtex-0.0.1/rtex/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-14 21:21:43.000000 rtex-0.0.1/rtex/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-14 21:21:43.000000 rtex-0.0.1/rtex/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:54.621401 rtex-0.0.1/rtex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 21:21:54.000000 rtex-0.0.1/rtex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-14 21:21:54.000000 rtex-0.0.1/rtex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:21:54.000000 rtex-0.0.1/rtex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 21:21:54.000000 rtex-0.0.1/rtex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 21:21:54.000000 rtex-0.0.1/rtex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:21:54.621401 rtex-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:45:39.211370 rtex-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:45:39.207370 rtex-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:45:39.207370 rtex-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-14 21:45:27.000000 rtex-0.0.2/.github/workflows/build-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-14 21:45:27.000000 rtex-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 21:45:27.000000 rtex-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-14 21:45:39.211370 rtex-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-14 21:45:27.000000 rtex-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-14 21:45:27.000000 rtex-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 21:45:27.000000 rtex-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:45:39.207370 rtex-0.0.2/rtex/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 21:45:27.000000 rtex-0.0.2/rtex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-06-14 21:45:27.000000 rtex-0.0.2/rtex/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-14 21:45:27.000000 rtex-0.0.2/rtex/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-14 21:45:27.000000 rtex-0.0.2/rtex/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-14 21:45:27.000000 rtex-0.0.2/rtex/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:45:39.211370 rtex-0.0.2/rtex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-14 21:45:39.000000 rtex-0.0.2/rtex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-14 21:45:39.000000 rtex-0.0.2/rtex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:45:39.000000 rtex-0.0.2/rtex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 21:45:39.000000 rtex-0.0.2/rtex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 21:45:39.000000 rtex-0.0.2/rtex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:45:39.211370 rtex-0.0.2/setup.cfg
```

### Comparing `rtex-0.0.1/.github/workflows/build-and-publish.yml` & `rtex-0.0.2/.github/workflows/build-and-publish.yml`

 * *Files identical despite different names*

### Comparing `rtex-0.0.1/.gitignore` & `rtex-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rtex-0.0.1/LICENSE` & `rtex-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rtex-0.0.1/pyproject.toml` & `rtex-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rtex-0.0.1/rtex/client.py` & `rtex-0.0.2/rtex/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,20 +140,26 @@
         return buf
 
     @validate_arguments
     async def render_math(
         self,
         code: str,
         format: RenderFormat = "png",
+        documentclass: str = "minimal",
+        quality: Optional[RenderQuality] = None,
+        density: Optional[RenderDensity] = None,
     ):
         final_doc = rf"\({code}\)"
 
         res = await self.create_render(
             code=final_doc,
             format=format,
+            documentclass=documentclass,
+            quality=quality,
+            density=density,
         )
 
         if res.status == "error":
             raise RuntimeError("Failed to render code")
 
         return await self.get_render(
             filename=res.filename,
```

### Comparing `rtex-0.0.1/rtex/models.py` & `rtex-0.0.2/rtex/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Annotated, Literal, Optional, Union
 
 from pydantic import BaseModel, Field, conint
 
 RenderFormat = Literal["png", "jpg", "pdf"]
-RenderQuality = Annotated[int, conint(ge=0, le=100)]
+RenderQuality = Annotated[int, conint(gt=0, le=100)]
 RenderDensity = int
 
 
 class CreateLaTeXDocumentRequest(BaseModel):
     code: str
     format: RenderFormat
     quality: Optional[RenderQuality]
```

