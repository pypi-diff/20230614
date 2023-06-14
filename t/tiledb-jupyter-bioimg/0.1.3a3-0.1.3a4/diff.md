# Comparing `tmp/tiledb_jupyter_bioimg-0.1.3a3.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.3a3.tar", last modified: Thu Jun  8 12:25:29 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.3a4.tar", last modified: Wed Jun 14 14:16:01 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.3a3.tar` & `tiledb_jupyter_bioimg-0.1.3a4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:29.458397 tiledb_jupyter_bioimg-0.1.3a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-08 12:25:29.458397 tiledb_jupyter_bioimg-0.1.3a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-08 12:21:06.000000 tiledb_jupyter_bioimg-0.1.3a3/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:25:29.458397 tiledb_jupyter_bioimg-0.1.3a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:29.450397 tiledb_jupyter_bioimg-0.1.3a3/src/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/src/embed.ts
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:29.450397 tiledb_jupyter_bioimg-0.1.3a3/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:29.454397 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:29.454397 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:29.458397 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/241.7a42393c28911f92f6c6.js
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)   760758 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/556.2c70ba3b8c5599c82503.js
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/556.2c70ba3b8c5599c82503.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   516688 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/744.cd9879bb199b94dec1b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/remoteEntry.2fd765b4b184cbb0da17.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-08 12:24:20.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    85173 2023-06-08 12:24:50.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:29.454397 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-08 12:25:29.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-08 12:25:29.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:25:29.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:22:54.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 12:25:29.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 12:25:29.000000 tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-08 12:17:31.000000 tiledb_jupyter_bioimg-0.1.3a3/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:16:01.489960 tiledb_jupyter_bioimg-0.1.3a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-14 14:16:01.489960 tiledb_jupyter_bioimg-0.1.3a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-14 14:12:29.000000 tiledb_jupyter_bioimg-0.1.3a4/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 14:16:01.489960 tiledb_jupyter_bioimg-0.1.3a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:16:01.481959 tiledb_jupyter_bioimg-0.1.3a4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/src/embed.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:16:01.485960 tiledb_jupyter_bioimg-0.1.3a4/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:16:01.485960 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:16:01.485960 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:16:01.489960 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)   763992 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/556.06e35fefdb145d6110cd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/556.06e35fefdb145d6110cd.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/744.189af4ed2998fcfe7556.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/79.06e38572ee0f6236bd5c.js
+-rw-r--r--   0 runner    (1001) docker     (123)   520338 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/995.ed09fb94a4cde32b3298.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/995.ed09fb94a4cde32b3298.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/remoteEntry.a7cbc27a79641454b2f4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-14 14:15:06.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86073 2023-06-14 14:15:28.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:16:01.485960 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-14 14:16:01.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-14 14:16:01.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:16:01.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:13:56.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 14:16:01.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 14:16:01.000000 tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-14 14:09:36.000000 tiledb_jupyter_bioimg-0.1.3a4/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/LICENSE` & `tiledb_jupyter_bioimg-0.1.3a4/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.3a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.3a3
+Version: 0.1.3a4
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/README.md` & `tiledb_jupyter_bioimg-0.1.3a4/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/package.json` & `tiledb_jupyter_bioimg-0.1.3a4/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.968560606060606%*

 * *Differences: {"'dependencies'": "{'@tiledb-inc/bioimage-viewer': '^0.1.4'}",*

 * * "'devDependencies'": "{'ts-loader': '^9.2.5'}",*

 * * "'version'": "'0.1.3-alpha.4'"}*

```diff
@@ -2,27 +2,28 @@
     "author": "TileDB",
     "bugs": {
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
         "@jupyterlab/application": "^3.4.5",
-        "@tiledb-inc/bioimage-viewer": "^0.1.3"
+        "@tiledb-inc/bioimage-viewer": "^0.1.4"
     },
     "description": "A jupyterlab extension to visualize bioimages in TileDB format",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.0",
         "@typescript-eslint/eslint-plugin": "^2.27.0",
         "@typescript-eslint/parser": "^2.27.0",
         "eslint": "^7.5.0",
         "eslint-config-prettier": "^6.10.1",
         "eslint-plugin-prettier": "^3.1.2",
         "npm-run-all": "^4.1.5",
         "prettier": "^1.19.0",
         "rimraf": "^3.0.2",
+        "ts-loader": "^9.2.5",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/*.css",
         "style/index.js",
@@ -97,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3-alpha.3"
+    "version": "0.1.3-alpha.4"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/setup.py` & `tiledb_jupyter_bioimg-0.1.3a4/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/src/index.ts` & `tiledb_jupyter_bioimg-0.1.3a4/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/src/version.ts` & `tiledb_jupyter_bioimg-0.1.3a4/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.3a4/src/widget.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9681439393939394%*

 * *Differences: {"'dependencies'": "{'@tiledb-inc/bioimage-viewer': '^0.1.4'}",*

 * * "'devDependencies'": "{'ts-loader': '^9.2.5'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.a7cbc27a79641454b2f4.js'}}",*

 * * "'version'": "'0.1.3-alpha.4'"}*

```diff
@@ -2,41 +2,42 @@
     "author": "TileDB",
     "bugs": {
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
         "@jupyterlab/application": "^3.4.5",
-        "@tiledb-inc/bioimage-viewer": "^0.1.3"
+        "@tiledb-inc/bioimage-viewer": "^0.1.4"
     },
     "description": "A jupyterlab extension to visualize bioimages in TileDB format",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.0",
         "@typescript-eslint/eslint-plugin": "^2.27.0",
         "@typescript-eslint/parser": "^2.27.0",
         "eslint": "^7.5.0",
         "eslint-config-prettier": "^6.10.1",
         "eslint-plugin-prettier": "^3.1.2",
         "npm-run-all": "^4.1.5",
         "prettier": "^1.19.0",
         "rimraf": "^3.0.2",
+        "ts-loader": "^9.2.5",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/*.css",
         "style/index.js",
         "dist/*.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.2fd765b4b184cbb0da17.js",
+            "load": "static/remoteEntry.a7cbc27a79641454b2f4.js",
             "style": "./style"
         },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
@@ -102,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3-alpha.3"
+    "version": "0.1.3-alpha.4"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/241.7a42393c28911f92f6c6.js` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/79.06e38572ee0f6236bd5c.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,17 @@
 (() => {
     var e, t, r = {
-            7219: (e, t, r) => {
+            3281: (e, t, r) => {
                 "use strict";
                 var a = r(3578),
                     n = r.n(a),
                     o = r(4551),
-                    s = r(9757);
-                const l = {
+                    s = r(9757),
+                    l = r(8399);
+                const i = {
                     uint8: {
                         bytes: Uint8Array.BYTES_PER_ELEMENT,
                         format: s.Z.RED_INTEGER,
                         internalFormat: s.Z.R8UI,
                         type: s.Z.UNSIGNED_BYTE,
                         filtering: s.Z.NEAREST,
                         samplerType: "usampler2DArray",
@@ -48,180 +49,221 @@
                         filtering: s.Z.NEAREST,
                         samplerType: "sampler2DArray",
                         create: function(e) {
                             return new Float32Array(e)
                         }
                     }
                 };
-                class i {
+                class c {
                     constructor(e, t) {
                         this.baseAxes = e, this.targetAxes = t, this.permutationMatrix = new Array(e.length);
                         for (let e = 0; e < this.baseAxes.length; ++e) {
                             const t = this.targetAxes.indexOf(this.baseAxes[e]);
                             this.permutationMatrix[e] = t
                         }
                     }
                     reshape(e) {
                         const t = new Array(this.baseAxes.length);
                         for (let r = 0; r < this.baseAxes.length; ++r) t[this.targetAxes.indexOf(this.baseAxes[r])] = e[r];
                         return t
                     }
                 }
 
-                function c(e) {
+                function f(e) {
                     if (2 === e.length) return e;
                     const t = [];
                     for (let r = 0; r < e.length; r += 2) t.push([e[r], e[r + 1]]);
                     return t
                 }
 
-                function f(...e) {
+                function u(...e) {
                     const t = [],
                         r = e.length - 1;
                     return function a(n, o) {
                         for (let s = 0, l = e[o].length; s < l; s++) {
                             const l = n.slice(0);
                             l.push(e[o][s]), o === r ? t.push(l) : a(l, o + 1)
                         }
                     }([], 0), t
                 }
 
-                function u(e) {
+                function h(e) {
                     let t = 1;
                     const r = [];
                     if (0 === e.length) return r;
                     for (let a = 1; a <= e.length; a++) a === e.length || e[a] - e[a - 1] != 1 ? (1 === t ? r.push([e[a - t], e[a - t]]) : r.push([e[a - t], e[a - 1]]), t = 1) : t++;
                     return r
                 }
+                const d = "TILEDB_BIOIMAGE_CACHE";
+                let g = 1;
+                const p = async e => {
+                    const t = await (0, l.X3)(d);
+                    return t.objectStoreNames.contains(e + "_1") ? t : (t.close(), g = t.version + 1, (0, l.X3)(d, g, {
+                        upgrade(t) {
+                            for (let r = 0; r < 1; ++r) t.objectStoreNames.contains(e + "_" + r) && t.deleteObjectStore(e + "_" + r);
+                            t.createObjectStore(e + "_1", {
+                                autoIncrement: !0
+                            }).createIndex("timestamp", "__timestamp")
+                        }
+                    }))
+                }, y = async (e, t) => {
+                    const r = await p(e),
+                        a = await r.get(e + "_1", t);
+                    return r.close(), a
+                }, m = async (e, t, r) => {
+                    const a = await p(e),
+                        n = Date.now();
+                    await a.put(e + "_1", Object.assign(r, {
+                        __timestamp: n
+                    }), t), a.close()
+                };
                 self.onmessage = async function(e) {
                     const t = {
                             apiKey: e.data.token,
                             basePath: e.data.basePath
                         },
                         r = new(n())(t),
                         a = e.data.levelRecord.dimensions[e.data.levelRecord.axes.indexOf("X")],
                         s = e.data.levelRecord.dimensions[e.data.levelRecord.axes.indexOf("Y")],
-                        h = e.data.levelRecord.downsample,
-                        p = e.data.index.x,
+                        l = e.data.levelRecord.downsample,
+                        d = e.data.index.x,
                         g = e.data.index.y,
-                        d = e.data.tileSize,
-                        y = e.data.attribute.type.toLowerCase(),
-                        x = e.data.levelRecord.axesMapping,
-                        A = new i(e.data.levelRecord.arrayAxes.map((t => e.data.levelRecord.axesMapping.get(t))).flat(), ["C", "Y", "X"]),
-                        b = new Array(A.baseAxes.length);
+                        p = e.data.tileSize,
+                        b = e.data.attribute.type.toLowerCase(),
+                        v = e.data.levelRecord.axesMapping,
+                        A = new c(e.data.levelRecord.arrayAxes.map((t => e.data.levelRecord.axesMapping.get(t))).flat(), ["C", "Y", "X"]),
+                        x = new Array(A.baseAxes.length);
                     for (let e = 0; e < A.baseAxes.length; ++e) {
                         const t = A.baseAxes[e];
-                        b[e] = "X" === t || "Y" === t ? h : 1
+                        x[e] = "X" === t || "Y" === t ? l : 1
                     }
-                    const m = new Map;
-                    m.set("C", e.data.channelRanges), m.set("Y", [g * d * h, Math.min((g + 1) * d * h, s) - 1]), m.set("X", [p * d * h, Math.min((p + 1) * d * h, a) - 1]);
-                    const E = ~~((m.get("X")[1] - m.get("X")[0] + 1) / h),
-                        v = ~~((m.get("Y")[1] - m.get("Y")[0] + 1) / h);
-                    let R = 0;
-                    for (let e = 0; e < m.get("C").length; e += 2) R += m.get("C")[e + 1] - m.get("C")[e] + 1;
-                    const w = function(e, t, r, a, n, o) {
-                        const s = [];
-                        for (const l of r) {
-                            const i = a.get(l);
-                            if (1 === i.length) s.push(c(n.get(i[0])));
-                            else {
-                                const a = [];
-                                for (const r of i) a.push(e[t.indexOf(r)]);
-                                const c = new Array(i.length).fill(1);
-                                for (let e = 0; e < a.length; ++e)
-                                    for (let t = e + 1; t < a.length; ++t) c[e] *= a[t];
-                                const h = [],
-                                    p = [];
-                                for (const e of i) {
-                                    const t = [],
-                                        r = [],
-                                        a = n.get(e);
-                                    for (let e = 0; e < a.length; e += 2) t.push(a[e + 1] - a[e] + 1), r.push(a[e]);
-                                    h.push(t), p.push(r)
-                                }
-                                const g = f(...h),
-                                    d = f(...p),
-                                    y = [],
-                                    x = [];
-                                for (const e of d) {
-                                    let t = 0;
-                                    for (let r = 0; r < e.length; ++r) t += e[r] * c[r];
-                                    y.push(t)
-                                }
-                                for (const e of g) {
-                                    const t = new Array(i.length + 1).fill(Number.MAX_SAFE_INTEGER, 0, 1).fill(1, 1);
-                                    for (let r = 0; r < e.length; ++r)
-                                        for (let a = r + 1; a < e.length; ++a) t[r + 1] *= e[a];
-                                    x.push(t)
-                                }
-                                let A = 0;
-                                const b = new Array(i.length),
-                                    m = [],
-                                    E = o[r.indexOf(l)];
-                                for (let e = 0; e < g.length; ++e) {
-                                    const t = g[e].reduce(((e, t) => e * t), 1);
-                                    for (let r = 0; r < t; ++r) {
-                                        A = y[e];
-                                        for (let t = 0; t < x[e].length - 1; ++t) b[t] = ~~(r % x[e][t] / x[e][t + 1]), A += b[t] * c[t];
-                                        if (A >= E) return console.error("OOB"), [];
-                                        m.push(A)
+                    const E = new Map,
+                        _ = [];
+                    for (let t = 0; t <= e.data.channelRanges.length; t += 2)
+                        for (let r = e.data.channelRanges[t]; r <= e.data.channelRanges[t + 1]; ++r) {
+                            const t = await y(`${e.data.levelRecord.id}_${p}`, `${r}_${e.data.levelRecord.zoomLevel}_${d}_${g}`);
+                            t ? E.set(r, t) : _.push(r)
+                        }
+                    const R = new Map;
+                    R.set("Y", [g * p * l, Math.min((g + 1) * p * l, s) - 1]), R.set("X", [d * p * l, Math.min((d + 1) * p * l, a) - 1]);
+                    const w = ~~((R.get("X")[1] - R.get("X")[0] + 1) / l),
+                        S = ~~((R.get("Y")[1] - R.get("Y")[0] + 1) / l);
+                    if (R.get("X")[1] = R.get("X")[0] + w * l - 1, R.get("Y")[1] = R.get("Y")[0] + S * l - 1, 0 !== _.length) {
+                        const t = [];
+                        for (const [e, r] of _.entries()) 0 === t.length ? t.push(r) : r - _[e - 1] != 1 && t.push(_[e - 1], r);
+                        t.push(_.at(-1)), R.set("C", t);
+                        const a = function(e, t, r, a, n, o) {
+                            const s = [];
+                            for (const l of r) {
+                                const i = a.get(l);
+                                if (1 === i.length) s.push(f(n.get(i[0])));
+                                else {
+                                    const a = [];
+                                    for (const r of i) a.push(e[t.indexOf(r)]);
+                                    const c = new Array(i.length).fill(1);
+                                    for (let e = 0; e < a.length; ++e)
+                                        for (let t = e + 1; t < a.length; ++t) c[e] *= a[t];
+                                    const f = [],
+                                        d = [];
+                                    for (const e of i) {
+                                        const t = [],
+                                            r = [],
+                                            a = n.get(e);
+                                        for (let e = 0; e < a.length; e += 2) t.push(a[e + 1] - a[e] + 1), r.push(a[e]);
+                                        f.push(t), d.push(r)
+                                    }
+                                    const g = u(...f),
+                                        p = u(...d),
+                                        y = [],
+                                        m = [];
+                                    for (const e of p) {
+                                        let t = 0;
+                                        for (let r = 0; r < e.length; ++r) t += e[r] * c[r];
+                                        y.push(t)
+                                    }
+                                    for (const e of g) {
+                                        const t = new Array(i.length + 1).fill(Number.MAX_SAFE_INTEGER, 0, 1).fill(1, 1);
+                                        for (let r = 0; r < e.length; ++r)
+                                            for (let a = r + 1; a < e.length; ++a) t[r + 1] *= e[a];
+                                        m.push(t)
                                     }
+                                    let b = 0;
+                                    const v = new Array(i.length),
+                                        A = [],
+                                        x = o[r.indexOf(l)];
+                                    for (let e = 0; e < g.length; ++e) {
+                                        const t = g[e].reduce(((e, t) => e * t), 1);
+                                        for (let r = 0; r < t; ++r) {
+                                            b = y[e];
+                                            for (let t = 0; t < m[e].length - 1; ++t) v[t] = ~~(r % m[e][t] / m[e][t + 1]), b += v[t] * c[t];
+                                            if (b >= x) return console.error("OOB"), [];
+                                            A.push(b)
+                                        }
+                                    }
+                                    A.sort(((e, t) => e - t)), s.push(h(A))
                                 }
-                                m.sort(((e, t) => e - t)), s.push(u(m))
                             }
+                            return s
+                        }(e.data.levelRecord.dimensions, e.data.levelRecord.axes, e.data.levelRecord.arrayAxes, v, R, e.data.levelRecord.arrayExtends);
+                        if (0 === a.length) return;
+                        const n = {
+                                layout: o.Layout.RowMajor,
+                                ranges: a,
+                                bufferSize: 12e7,
+                                attributes: [e.data.attribute.name],
+                                returnRawBuffers: !0
+                            },
+                            s = r.query.ReadQuery(e.data.namespace, e.data.levelRecord.id, n),
+                            l = i[b].create(await s.next().then((t => t.value[e.data.attribute.name]))),
+                            c = [];
+                        for (const t of e.data.levelRecord.arrayAxes)
+                            for (const r of e.data.levelRecord.axesMapping.get(t).flat()) switch (r) {
+                                case "X":
+                                case "Y":
+                                    c.push(R.get(r)[1] - R.get(r)[0] + 1);
+                                    break;
+                                case "C":
+                                    c.push(_.length)
+                            }
+                        const y = function(e, t, r, a) {
+                            if (t.baseAxes.toString() === t.targetAxes.toString() && 1 === Math.max(...a)) return e;
+                            const n = t.reshape(r),
+                                o = t.reshape(a);
+                            let s = 1;
+                            for (let e = 0; e < n.length; ++e) n[e] = ~~(n[e] / o[e]), s *= n[e];
+                            const l = new e.constructor(s),
+                                i = new Array(t.baseAxes.length + 1).fill(Number.MAX_SAFE_INTEGER, 0, 1).fill(1, 1),
+                                c = new Array(t.baseAxes.length).fill(1);
+                            for (let e = 0; e < r.length; ++e)
+                                for (let t = e + 1; t < r.length; ++t) i[e + 1] *= r[t], c[e] *= n[t];
+                            let f = 0;
+                            const u = a.reduce(((e, t) => e * t), 1),
+                                h = new Array(t.baseAxes.length);
+                            for (let r = 0; r < e.length; ++r) {
+                                f = 0;
+                                for (let e = 0; e < i.length - 1; ++e) h[e] = ~~(r % i[e] / i[e + 1]), f += ~~(h[e] / o[t.permutationMatrix[e]]) * c[t.permutationMatrix[e]];
+                                l[f] += e[r] / u
+                            }
+                            return l
+                        }(l, A, c, x);
+                        for (const [t, r] of _.entries()) {
+                            const a = y.slice(t * w * S, (t + 1) * w * S);
+                            E.set(r, a), await m(`${e.data.levelRecord.id}_${p}`, `${r}_${e.data.levelRecord.zoomLevel}_${d}_${g}`, a)
                         }
-                        return s
-                    }(e.data.levelRecord.dimensions, e.data.levelRecord.axes, e.data.levelRecord.arrayAxes, x, m, e.data.levelRecord.arrayExtends);
-                    if (0 === w.length) return;
-                    const S = {
-                            layout: o.Layout.RowMajor,
-                            ranges: w,
-                            bufferSize: 12e7,
-                            attributes: [e.data.attribute.name],
-                            returnRawBuffers: !0
-                        },
-                        _ = r.query.ReadQuery(e.data.namespace, e.data.levelRecord.id, S),
-                        T = l[y].create(await _.next().then((t => t.value[e.data.attribute.name]))),
-                        O = [];
-                    for (const t of e.data.levelRecord.arrayAxes)
-                        for (const r of e.data.levelRecord.axesMapping.get(t).flat()) switch (r) {
-                            case "X":
-                            case "Y":
-                                O.push(m.get(r)[1] - m.get(r)[0] + 1);
-                                break;
-                            case "C":
-                                O.push(R)
-                        }
-                    const M = function(e, t, r, a) {
-                        if (t.baseAxes.toString() === t.targetAxes.toString() && 1 === Math.max(...a)) return e;
-                        const n = t.reshape(r),
-                            o = t.reshape(a);
-                        let s = 1;
-                        for (let e = 0; e < n.length; ++e) n[e] = ~~(n[e] / o[e]), s *= n[e];
-                        const l = new e.constructor(s),
-                            i = new Array(t.baseAxes.length + 1).fill(Number.MAX_SAFE_INTEGER, 0, 1).fill(1, 1),
-                            c = new Array(t.baseAxes.length).fill(1);
-                        for (let e = 0; e < r.length; ++e)
-                            for (let t = e + 1; t < r.length; ++t) i[e + 1] *= r[t], c[e] *= n[t];
-                        let f = 0;
-                        const u = a.reduce(((e, t) => e * t), 1),
-                            h = new Array(t.baseAxes.length);
-                        for (let r = 0; r < e.length; ++r) {
-                            f = 0;
-                            for (let e = 0; e < i.length - 1; ++e) h[e] = ~~(r % i[e] / i[e + 1]), f += ~~(h[e] / o[t.permutationMatrix[e]]) * c[t.permutationMatrix[e]];
-                            l[f] += e[r] / u
-                        }
-                        return l
-                    }(T, A, O, b);
+                    }
+                    const T = i[b].create(E.size * w * S);
+                    let O = 0;
+                    for (let t = 0; t <= e.data.channelRanges.length; t += 2)
+                        for (let r = e.data.channelRanges[t]; r <= e.data.channelRanges[t + 1]; ++r) T.set(E.get(r), O * w * S), ++O;
                     self.postMessage({
-                        data: M,
-                        width: E,
-                        height: v,
-                        channels: R
-                    }, [M.buffer])
+                        data: T,
+                        width: w,
+                        height: S,
+                        channels: E.size
+                    }, [T.buffer])
                 }
             },
             8291: () => {},
             4447: () => {}
         },
         a = {};
 
@@ -230,15 +272,15 @@
         if (void 0 !== t) return t.exports;
         var o = a[e] = {
             exports: {}
         };
         return r[e].call(o.exports, o, o.exports, n), o.exports
     }
     n.m = r, n.c = a, n.x = () => {
-        var e = n.O(void 0, [635], (() => n(7219)));
+        var e = n.O(void 0, [995], (() => n(3281)));
         return n.O(e)
     }, e = [], n.O = (t, r, a, o) => {
         if (!r) {
             var s = 1 / 0;
             for (f = 0; f < e.length; f++) {
                 for (var [r, a, o] = e[f], l = !0, i = 0; i < r.length; i++)(!1 & o || s >= o) && Object.keys(n.O).every((e => n.O[e](r[i]))) ? r.splice(i--, 1) : (l = !1, o < s && (s = o));
                 if (l) {
@@ -258,15 +300,15 @@
             a: t
         }), t
     }, n.d = (e, t) => {
         for (var r in t) n.o(t, r) && !n.o(e, r) && Object.defineProperty(e, r, {
             enumerable: !0,
             get: t[r]
         })
-    }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, r) => (n.f[r](e, t), t)), [])), n.u = e => e + ".b2bedc962bcd82714540.js?v=b2bedc962bcd82714540", n.g = function() {
+    }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, r) => (n.f[r](e, t), t)), [])), n.u = e => e + ".ed09fb94a4cde32b3298.js?v=ed09fb94a4cde32b3298", n.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.r = e => {
@@ -298,22 +340,22 @@
             if (r.length)
                 for (var a = r.length - 1; a > -1 && !e;) e = r[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), n.p = e
     })(), (() => {
         var e = {
-            241: 1
+            79: 1
         };
         n.f.i = (t, r) => {
             e[t] || importScripts(n.p + n.u(t))
         };
         var t = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || [],
             r = t.push.bind(t);
         t.push = t => {
             var [a, o, s] = t;
             for (var l in o) n.o(o, l) && (n.m[l] = o[l]);
             for (s && s(n); a.length;) e[a.pop()] = 1;
             r(t)
         }
-    })(), t = n.x, n.x = () => n.e(635).then(t), n.x()
+    })(), t = n.x, n.x = () => n.e(995).then(t), n.x()
 })();
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/556.2c70ba3b8c5599c82503.js` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/556.06e35fefdb145d6110cd.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 556.2c70ba3b8c5599c82503.js.LICENSE.txt */
+/*! For license information please see 556.06e35fefdb145d6110cd.js.LICENSE.txt */
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
     [556], {
         9296: t => {
             "use strict";
             t.exports = n, t.exports.default = n;
             var e = 1e20;
 
@@ -75,15 +75,15 @@
             }, n.prototype.drawWithMetrics = function(t) {
                 return this._draw(t, !0)
             }
         },
         1556: (t, e, n) => {
             "use strict";
             n.r(e), n.d(e, {
-                default: () => pE
+                default: () => bE
             });
             var i = n(3379),
                 r = n.n(i),
                 s = n(4272);
             r()(s.Z, {
                 insert: "head",
                 singleton: !1
@@ -316,16 +316,16 @@
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
                         return n && t(e.prototype, n), i && t(e, i), e
                     }
                 }(),
-                P = [38, 40],
-                S = 1;
+                S = [38, 40],
+                P = 1;
             const C = function(t) {
                 function e(t) {
                     ! function(t, e) {
                         if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                     }(this, e);
                     var n = function(t, e) {
                         if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
@@ -338,15 +338,15 @@
                         })
                     }, n.handleChange = function(t) {
                         n.setUpdatedValue(t.target.value, t)
                     }, n.handleKeyDown = function(t) {
                         var e, i = function(t) {
                             return Number(String(t).replace(/%/g, ""))
                         }(t.target.value);
-                        if (!isNaN(i) && (e = t.keyCode, P.indexOf(e) > -1)) {
+                        if (!isNaN(i) && (e = t.keyCode, S.indexOf(e) > -1)) {
                             var r = n.getArrowOffset(),
                                 s = 38 === t.keyCode ? i + r : i - r;
                             n.setUpdatedValue(s, t)
                         }
                     }, n.handleDrag = function(t) {
                         if (n.props.dragLabel) {
                             var e = Math.round(n.props.value + t.movementX);
@@ -357,15 +357,15 @@
                     }, n.handleMouseUp = function() {
                         n.unbindEventListeners()
                     }, n.unbindEventListeners = function() {
                         window.removeEventListener("mousemove", n.handleDrag), window.removeEventListener("mouseup", n.handleMouseUp)
                     }, n.state = {
                         value: String(t.value).toUpperCase(),
                         blurValue: String(t.value).toUpperCase()
-                    }, n.inputId = "rc-editable-input-" + S++, n
+                    }, n.inputId = "rc-editable-input-" + P++, n
                 }
                 return function(t, e) {
                     if ("function" != typeof e && null !== e) throw new TypeError("Super expression must either be null or a function, not " + typeof e);
                     t.prototype = Object.create(e && e.prototype, {
                         constructor: {
                             value: t,
                             enumerable: !1,
@@ -594,63 +594,63 @@
                             style: i.pointer
                         }, this.props.pointer ? h().createElement(this.props.pointer, this.props) : h().createElement("div", {
                             style: i.slider
                         }))))
                     }
                 }]), e
             }(c.PureComponent || c.Component);
-            var L = n(5697),
-                O = n.n(L);
-            const R = function(t, e) {
+            var O = n(5697),
+                L = n.n(O);
+            const I = function(t, e) {
                     return t === e || t != t && e != e
                 },
                 k = function(t, e) {
                     for (var n = t.length; n--;)
-                        if (R(t[n][0], e)) return n;
+                        if (I(t[n][0], e)) return n;
                     return -1
                 };
-            var I = Array.prototype.splice;
+            var R = Array.prototype.splice;
 
             function j(t) {
                 var e = -1,
                     n = null == t ? 0 : t.length;
                 for (this.clear(); ++e < n;) {
                     var i = t[e];
                     this.set(i[0], i[1])
                 }
             }
             j.prototype.clear = function() {
                 this.__data__ = [], this.size = 0
             }, j.prototype.delete = function(t) {
                 var e = this.__data__,
                     n = k(e, t);
-                return !(n < 0 || (n == e.length - 1 ? e.pop() : I.call(e, n, 1), --this.size, 0))
+                return !(n < 0 || (n == e.length - 1 ? e.pop() : R.call(e, n, 1), --this.size, 0))
             }, j.prototype.get = function(t) {
                 var e = this.__data__,
                     n = k(e, t);
                 return n < 0 ? void 0 : e[n][1]
             }, j.prototype.has = function(t) {
                 return k(this.__data__, t) > -1
             }, j.prototype.set = function(t, e) {
                 var n = this.__data__,
                     i = k(n, t);
                 return i < 0 ? (++this.size, n.push([t, e])) : n[i][1] = e, this
             };
             const z = j;
             var F = n(6169);
             const B = F.Z.Symbol;
-            var D = Object.prototype,
-                N = D.hasOwnProperty,
-                V = D.toString,
+            var N = Object.prototype,
+                D = N.hasOwnProperty,
+                V = N.toString,
                 U = B ? B.toStringTag : void 0;
             var G = Object.prototype.toString;
             var W = B ? B.toStringTag : void 0;
             const H = function(t) {
                     return null == t ? void 0 === t ? "[object Undefined]" : "[object Null]" : W && W in Object(t) ? function(t) {
-                        var e = N.call(t, U),
+                        var e = D.call(t, U),
                             n = t[U];
                         try {
                             t[U] = void 0;
                             var i = !0
                         } catch (t) {}
                         var r = V.call(t);
                         return i && (e ? t[U] = n : delete t[U]), r
@@ -658,22 +658,22 @@
                         return G.call(t)
                     }(t)
                 },
                 Z = function(t) {
                     var e = typeof t;
                     return null != t && ("object" == e || "function" == e)
                 },
-                q = function(t) {
+                X = function(t) {
                     if (!Z(t)) return !1;
                     var e = H(t);
                     return "[object Function]" == e || "[object GeneratorFunction]" == e || "[object AsyncFunction]" == e || "[object Proxy]" == e
                 },
-                X = F.Z["__core-js_shared__"];
+                q = F.Z["__core-js_shared__"];
             var Y = function() {
-                var t = /[^.]+$/.exec(X && X.keys && X.keys.IE_PROTO || "");
+                var t = /[^.]+$/.exec(q && q.keys && q.keys.IE_PROTO || "");
                 return t ? "Symbol(src)_1." + t : ""
             }();
             var K = Function.prototype.toString;
             const $ = function(t) {
                 if (null != t) {
                     try {
                         return K.call(t)
@@ -687,15 +687,15 @@
             var J = /^\[object .+?Constructor\]$/,
                 Q = Function.prototype,
                 tt = Object.prototype,
                 et = Q.toString,
                 nt = tt.hasOwnProperty,
                 it = RegExp("^" + et.call(nt).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
             const rt = function(t) {
-                    return !(!Z(t) || (e = t, Y && Y in e)) && (q(t) ? it : J).test($(t));
+                    return !(!Z(t) || (e = t, Y && Y in e)) && (X(t) ? it : J).test($(t));
                     var e
                 },
                 st = function(t, e) {
                     var n = function(t, e) {
                         return null == t ? void 0 : t[e]
                     }(t, e);
                     return rt(n) ? n : void 0
@@ -801,15 +801,15 @@
                         configurable: !0,
                         enumerable: !0,
                         value: n,
                         writable: !0
                     }) : t[e] = n
                 },
                 yt = function(t, e, n) {
-                    (void 0 !== n && !R(t[e], n) || void 0 === n && !(e in t)) && bt(t, e, n)
+                    (void 0 !== n && !I(t[e], n) || void 0 === n && !(e in t)) && bt(t, e, n)
                 },
                 _t = function(t, e, n) {
                     for (var i = -1, r = Object(t), s = n(t), o = s.length; o--;) {
                         var a = s[++i];
                         if (!1 === e(r[a], a, r)) break
                     }
                     return t
@@ -819,20 +819,20 @@
                 Et = function(t, e) {
                     var n = e ? function(t) {
                         var e = new t.constructor(t.byteLength);
                         return new wt(e).set(new wt(t)), e
                     }(t.buffer) : t.buffer;
                     return new t.constructor(n, t.byteOffset, t.length)
                 };
-            var Pt = Object.create;
-            const St = function() {
+            var St = Object.create;
+            const Pt = function() {
                     function t() {}
                     return function(e) {
                         if (!Z(e)) return {};
-                        if (Pt) return Pt(e);
+                        if (St) return St(e);
                         t.prototype = e;
                         var n = new t;
                         return t.prototype = void 0, n
                     }
                 }(),
                 Ct = function(t, e) {
                     return function(n) {
@@ -841,70 +841,70 @@
                 },
                 Tt = Ct(Object.getPrototypeOf, Object);
             var At = Object.prototype;
             const Mt = function(t) {
                     var e = t && t.constructor;
                     return t === ("function" == typeof e && e.prototype || At)
                 },
-                Lt = function(t) {
+                Ot = function(t) {
                     return null != t && "object" == typeof t
                 },
-                Ot = function(t) {
-                    return Lt(t) && "[object Arguments]" == H(t)
+                Lt = function(t) {
+                    return Ot(t) && "[object Arguments]" == H(t)
                 };
-            var Rt = Object.prototype,
-                kt = Rt.hasOwnProperty,
-                It = Rt.propertyIsEnumerable;
-            const jt = Ot(function() {
+            var It = Object.prototype,
+                kt = It.hasOwnProperty,
+                Rt = It.propertyIsEnumerable;
+            const jt = Lt(function() {
                     return arguments
-                }()) ? Ot : function(t) {
-                    return Lt(t) && kt.call(t, "callee") && !It.call(t, "callee")
+                }()) ? Lt : function(t) {
+                    return Ot(t) && kt.call(t, "callee") && !Rt.call(t, "callee")
                 },
                 zt = Array.isArray,
                 Ft = function(t) {
                     return "number" == typeof t && t > -1 && t % 1 == 0 && t <= 9007199254740991
                 },
                 Bt = function(t) {
-                    return null != t && Ft(t.length) && !q(t)
+                    return null != t && Ft(t.length) && !X(t)
                 };
-            var Dt = n(4002),
-                Nt = Function.prototype,
+            var Nt = n(4002),
+                Dt = Function.prototype,
                 Vt = Object.prototype,
-                Ut = Nt.toString,
+                Ut = Dt.toString,
                 Gt = Vt.hasOwnProperty,
                 Wt = Ut.call(Object);
             var Ht = {};
             Ht["[object Float32Array]"] = Ht["[object Float64Array]"] = Ht["[object Int8Array]"] = Ht["[object Int16Array]"] = Ht["[object Int32Array]"] = Ht["[object Uint8Array]"] = Ht["[object Uint8ClampedArray]"] = Ht["[object Uint16Array]"] = Ht["[object Uint32Array]"] = !0, Ht["[object Arguments]"] = Ht["[object Array]"] = Ht["[object ArrayBuffer]"] = Ht["[object Boolean]"] = Ht["[object DataView]"] = Ht["[object Date]"] = Ht["[object Error]"] = Ht["[object Function]"] = Ht["[object Map]"] = Ht["[object Number]"] = Ht["[object Object]"] = Ht["[object RegExp]"] = Ht["[object Set]"] = Ht["[object String]"] = Ht["[object WeakMap]"] = !1;
             var Zt = n(9730),
-                qt = Zt.Z && Zt.Z.isTypedArray;
-            const Xt = qt ? (Yt = qt, function(t) {
+                Xt = Zt.Z && Zt.Z.isTypedArray;
+            const qt = Xt ? (Yt = Xt, function(t) {
                 return Yt(t)
             }) : function(t) {
-                return Lt(t) && Ft(t.length) && !!Ht[H(t)]
+                return Ot(t) && Ft(t.length) && !!Ht[H(t)]
             };
             var Yt;
             const Kt = function(t, e) {
                 if (("constructor" !== e || "function" != typeof t[e]) && "__proto__" != e) return t[e]
             };
             var $t = Object.prototype.hasOwnProperty;
             const Jt = function(t, e, n) {
                 var i = t[e];
-                $t.call(t, e) && R(i, n) && (void 0 !== n || e in t) || bt(t, e, n)
+                $t.call(t, e) && I(i, n) && (void 0 !== n || e in t) || bt(t, e, n)
             };
             var Qt = /^(?:0|[1-9]\d*)$/;
             const te = function(t, e) {
                 var n = typeof t;
                 return !!(e = null == e ? 9007199254740991 : e) && ("number" == n || "symbol" != n && Qt.test(t)) && t > -1 && t % 1 == 0 && t < e
             };
             var ee = Object.prototype.hasOwnProperty;
             const ne = function(t, e) {
                 var n = zt(t),
                     i = !n && jt(t),
-                    r = !n && !i && (0, Dt.Z)(t),
-                    s = !n && !i && !r && Xt(t),
+                    r = !n && !i && (0, Nt.Z)(t),
+                    s = !n && !i && !r && qt(t),
                     o = n || i || r || s,
                     a = o ? function(t, e) {
                         for (var n = -1, i = Array(t); ++n < t;) i[n] = e(n);
                         return i
                     }(t.length, String) : [],
                     l = a.length;
                 for (var c in t) !e && !ee.call(t, c) || o && ("length" == c || r && ("offset" == c || "parent" == c) || s && ("buffer" == c || "byteLength" == c || "byteOffset" == c) || te(c, l)) || a.push(c);
@@ -944,29 +944,29 @@
                         h = o.get(c);
                     if (h) yt(t, n, h);
                     else {
                         var u = s ? s(l, c, n + "", t, e, o) : void 0,
                             d = void 0 === u;
                         if (d) {
                             var p = zt(c),
-                                f = !p && (0, Dt.Z)(c),
-                                g = !p && !f && Xt(c);
-                            u = c, p || f || g ? zt(l) ? u = l : Lt(a = l) && Bt(a) ? u = function(t, e) {
+                                f = !p && (0, Nt.Z)(c),
+                                g = !p && !f && qt(c);
+                            u = c, p || f || g ? zt(l) ? u = l : Ot(a = l) && Bt(a) ? u = function(t, e) {
                                 var n = -1,
                                     i = t.length;
                                 for (e || (e = Array(i)); ++n < i;) e[n] = t[n];
                                 return e
                             }(l) : f ? (d = !1, u = (0, xt.Z)(c, !0)) : g ? (d = !1, u = Et(c, !0)) : u = [] : function(t) {
-                                if (!Lt(t) || "[object Object]" != H(t)) return !1;
+                                if (!Ot(t) || "[object Object]" != H(t)) return !1;
                                 var e = Tt(t);
                                 if (null === e) return !0;
                                 var n = Gt.call(e, "constructor") && e.constructor;
                                 return "function" == typeof n && n instanceof n && Ut.call(n) == Wt
-                            }(c) || jt(c) ? (u = l, jt(l) ? u = oe(l) : Z(l) && !q(l) || (u = function(t) {
-                                return "function" != typeof t.constructor || Mt(t) ? {} : St(Tt(t))
+                            }(c) || jt(c) ? (u = l, jt(l) ? u = oe(l) : Z(l) && !X(l) || (u = function(t) {
+                                return "function" != typeof t.constructor || Mt(t) ? {} : Pt(Tt(t))
                             }(c))) : d = !1
                         }
                         d && (o.set(c, u), r(u, c, i, s, o), o.delete(c)), yt(t, n, u)
                     }
                 },
                 le = function t(e, n, i, r, s) {
                     e !== n && _t(n, (function(o, a) {
@@ -1035,15 +1035,15 @@
                     var n = -1,
                         i = e.length,
                         r = i > 1 ? e[i - 1] : void 0,
                         s = i > 2 ? e[2] : void 0;
                     for (r = me.length > 3 && "function" == typeof r ? (i--, r) : void 0, s && function(t, e, n) {
                             if (!Z(n)) return !1;
                             var i = typeof e;
-                            return !!("number" == i ? Bt(n) && te(e, n.length) : "string" == i && e in n) && R(n[e], t)
+                            return !!("number" == i ? Bt(n) && te(e, n.length) : "string" == i && e in n) && I(n[e], t)
                         }(e[0], e[1], s) && (r = i < 3 ? void 0 : r, i = 1), t = Object(t); ++n < i;) {
                         var o = e[n];
                         o && me(t, o, n)
                     }
                     return t
                 })));
             var me, ve = function(t) {
@@ -1117,18 +1117,18 @@
                 }, h().createElement("div", {
                     style: a.bg
                 }), h().createElement("div", {
                     style: a.content
                 }, r))
             };
             ve.propTypes = {
-                background: O().string,
-                zDepth: O().oneOf([0, 1, 2, 3, 4, 5]),
-                radius: O().number,
-                styles: O().object
+                background: L().string,
+                zDepth: L().oneOf([0, 1, 2, 3, 4, 5]),
+                radius: L().number,
+                styles: L().object
             }, ve.defaultProps = {
                 background: "#fff",
                 zDepth: 1,
                 radius: 2,
                 styles: {}
             };
             const be = ve,
@@ -1140,35 +1140,35 @@
             const we = function(t) {
                     return t ? t.slice(0, function(t) {
                         for (var e = t.length; e-- && _e.test(t.charAt(e)););
                         return e
                     }(t) + 1).replace(xe, "") : t
                 },
                 Ee = function(t) {
-                    return "symbol" == typeof t || Lt(t) && "[object Symbol]" == H(t)
+                    return "symbol" == typeof t || Ot(t) && "[object Symbol]" == H(t)
                 };
-            var Pe = /^[-+]0x[0-9a-f]+$/i,
-                Se = /^0b[01]+$/i,
+            var Se = /^[-+]0x[0-9a-f]+$/i,
+                Pe = /^0b[01]+$/i,
                 Ce = /^0o[0-7]+$/i,
                 Te = parseInt;
             const Ae = function(t) {
                 if ("number" == typeof t) return t;
                 if (Ee(t)) return NaN;
                 if (Z(t)) {
                     var e = "function" == typeof t.valueOf ? t.valueOf() : t;
                     t = Z(e) ? e + "" : e
                 }
                 if ("string" != typeof t) return 0 === t ? t : +t;
                 t = we(t);
-                var n = Se.test(t);
-                return n || Ce.test(t) ? Te(t.slice(2), n ? 2 : 8) : Pe.test(t) ? NaN : +t
+                var n = Pe.test(t);
+                return n || Ce.test(t) ? Te(t.slice(2), n ? 2 : 8) : Se.test(t) ? NaN : +t
             };
             var Me = Math.max,
-                Le = Math.min;
-            const Oe = function(t, e, n) {
+                Oe = Math.min;
+            const Le = function(t, e, n) {
                 var i, r, s, o, a, l, c = 0,
                     h = !1,
                     u = !1,
                     d = !0;
                 if ("function" != typeof t) throw new TypeError("Expected a function");
 
                 function p(e) {
@@ -1183,15 +1183,15 @@
                 }
 
                 function g() {
                     var t = ye();
                     if (f(t)) return m(t);
                     a = setTimeout(g, function(t) {
                         var n = e - (t - l);
-                        return u ? Le(n, s - (t - c)) : n
+                        return u ? Oe(n, s - (t - c)) : n
                     }(t))
                 }
 
                 function m(t) {
                     return a = void 0, d && i ? p(t) : (i = r = void 0, o)
                 }
 
@@ -1208,15 +1208,15 @@
                 }
                 return e = Ae(e) || 0, Z(n) && (h = !!n.leading, s = (u = "maxWait" in n) ? Me(Ae(n.maxWait) || 0, e) : s, d = "trailing" in n ? !!n.trailing : d), v.cancel = function() {
                     void 0 !== a && clearTimeout(a), c = 0, i = l = r = a = void 0
                 }, v.flush = function() {
                     return void 0 === a ? o : m(ye())
                 }, v
             };
-            var Re = function() {
+            var Ie = function() {
                     function t(t, e) {
                         for (var n = 0; n < e.length; n++) {
                             var i = e[n];
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
@@ -1258,15 +1258,15 @@
                             e.addEventListener("mousemove", n.handleChange), e.addEventListener("mouseup", n.handleMouseUp)
                         }, n.handleMouseUp = function() {
                             n.unbindEventListeners()
                         }, n.throttle = function(t, e, n) {
                             var i = !0,
                                 r = !0;
                             if ("function" != typeof t) throw new TypeError("Expected a function");
-                            return Z(n) && (i = "leading" in n ? !!n.leading : i, r = "trailing" in n ? !!n.trailing : r), Oe(t, e, {
+                            return Z(n) && (i = "leading" in n ? !!n.leading : i, r = "trailing" in n ? !!n.trailing : r), Le(t, e, {
                                 leading: i,
                                 maxWait: e,
                                 trailing: r
                             })
                         }((function(t, e, n) {
                             t(e, n)
                         }), 50), n
@@ -1277,15 +1277,15 @@
                             constructor: {
                                 value: t,
                                 enumerable: !1,
                                 writable: !0,
                                 configurable: !0
                             }
                         }), e && (Object.setPrototypeOf ? Object.setPrototypeOf(t, e) : t.__proto__ = e)
-                    }(e, t), Re(e, [{
+                    }(e, t), Ie(e, [{
                         key: "componentWillUnmount",
                         value: function() {
                             this.throttle.cancel(), this.unbindEventListeners()
                         }
                     }, {
                         key: "getContainerRenderWindow",
                         value: function() {
@@ -1367,39 +1367,39 @@
                                 style: a.pointer
                             }, this.props.pointer ? h().createElement(this.props.pointer, this.props) : h().createElement("div", {
                                 style: a.circle
                             }))))
                         }
                     }]), e
                 }(c.PureComponent || c.Component);
-            const Ie = ke,
+            const Re = ke,
                 je = function(t, e) {
                     for (var n = -1, i = null == t ? 0 : t.length; ++n < i && !1 !== e(t[n], n, t););
                     return t
                 },
                 ze = Ct(Object.keys, Object);
             var Fe = Object.prototype.hasOwnProperty;
             const Be = function(t) {
                     return Bt(t) ? ne(t) : function(t) {
                         if (!Mt(t)) return ze(t);
                         var e = [];
                         for (var n in Object(t)) Fe.call(t, n) && "constructor" != n && e.push(n);
                         return e
                     }(t)
                 },
-                De = function(t, e) {
+                Ne = function(t, e) {
                     if (null == t) return t;
                     if (!Bt(t)) return function(t, e) {
                         return t && _t(t, e, Be)
                     }(t, e);
                     for (var n = t.length, i = -1, r = Object(t); ++i < n && !1 !== e(r[i], i, r););
                     return t
                 },
-                Ne = function(t, e) {
-                    return (zt(t) ? je : De)(t, "function" == typeof(n = e) ? n : ce);
+                De = function(t, e) {
+                    return (zt(t) ? je : Ne)(t, "function" == typeof(n = e) ? n : ce);
                     var n
                 };
 
             function Ve(t) {
                 return Ve = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
                     return typeof t
                 } : function(t) {
@@ -1581,20 +1581,20 @@
                 return {
                     h: i,
                     s: r,
                     v: a
                 }
             }
 
-            function qe(t, e, n, i) {
+            function Xe(t, e, n, i) {
                 var r = [fn(Math.round(t).toString(16)), fn(Math.round(e).toString(16)), fn(Math.round(n).toString(16))];
                 return i && r[0].charAt(0) == r[0].charAt(1) && r[1].charAt(0) == r[1].charAt(1) && r[2].charAt(0) == r[2].charAt(1) ? r[0].charAt(0) + r[1].charAt(0) + r[2].charAt(0) : r.join("")
             }
 
-            function Xe(t, e, n, i) {
+            function qe(t, e, n, i) {
                 return [fn(mn(i)), fn(Math.round(t).toString(16)), fn(Math.round(e).toString(16)), fn(Math.round(n).toString(16))].join("")
             }
 
             function Ye(t, e) {
                 e = 0 === e ? 0 : e || 10;
                 var n = We(t).toHsl();
                 return n.s -= e / 100, n.s = dn(n.s), We(n)
@@ -1740,15 +1740,15 @@
                     var t = He(this._r, this._g, this._b),
                         e = Math.round(360 * t.h),
                         n = Math.round(100 * t.s),
                         i = Math.round(100 * t.l);
                     return 1 == this._a ? "hsl(" + e + ", " + n + "%, " + i + "%)" : "hsla(" + e + ", " + n + "%, " + i + "%, " + this._roundA + ")"
                 },
                 toHex: function(t) {
-                    return qe(this._r, this._g, this._b, t)
+                    return Xe(this._r, this._g, this._b, t)
                 },
                 toHexString: function(t) {
                     return "#" + this.toHex(t)
                 },
                 toHex8: function(t) {
                     return function(t, e, n, i, r) {
                         var s = [fn(Math.round(t).toString(16)), fn(Math.round(e).toString(16)), fn(Math.round(n).toString(16)), fn(mn(i))];
@@ -1777,23 +1777,23 @@
                         a: this._a
                     }
                 },
                 toPercentageRgbString: function() {
                     return 1 == this._a ? "rgb(" + Math.round(100 * un(this._r, 255)) + "%, " + Math.round(100 * un(this._g, 255)) + "%, " + Math.round(100 * un(this._b, 255)) + "%)" : "rgba(" + Math.round(100 * un(this._r, 255)) + "%, " + Math.round(100 * un(this._g, 255)) + "%, " + Math.round(100 * un(this._b, 255)) + "%, " + this._roundA + ")"
                 },
                 toName: function() {
-                    return 0 === this._a ? "transparent" : !(this._a < 1) && (cn[qe(this._r, this._g, this._b, !0)] || !1)
+                    return 0 === this._a ? "transparent" : !(this._a < 1) && (cn[Xe(this._r, this._g, this._b, !0)] || !1)
                 },
                 toFilter: function(t) {
-                    var e = "#" + Xe(this._r, this._g, this._b, this._a),
+                    var e = "#" + qe(this._r, this._g, this._b, this._a),
                         n = e,
                         i = this._gradientType ? "GradientType = 1, " : "";
                     if (t) {
                         var r = We(t);
-                        n = "#" + Xe(r._r, r._g, r._b, r._a)
+                        n = "#" + qe(r._r, r._g, r._b, r._a)
                     }
                     return "progid:DXImageTransform.Microsoft.gradient(" + i + "startColorstr=" + e + ",endColorstr=" + n + ")"
                 },
                 toString: function(t) {
                     var e = !!t;
                     t = t || this._format;
                     var n = !1,
@@ -2119,41 +2119,41 @@
 
             function wn(t) {
                 return !!xn.CSS_UNIT.exec(t)
             }
             var En = function(t) {
                     var e = 0,
                         n = 0;
-                    return Ne(["r", "g", "b", "a", "h", "s", "l", "v"], (function(i) {
+                    return De(["r", "g", "b", "a", "h", "s", "l", "v"], (function(i) {
                         t[i] && (e += 1, isNaN(t[i]) || (n += 1), "s" === i || "l" === i) && /^\d+%$/.test(t[i]) && (n += 1)
                     })), e === n && t
                 },
-                Pn = function(t, e) {
+                Sn = function(t, e) {
                     var n = t.hex ? We(t.hex) : We(t),
                         i = n.toHsl(),
                         r = n.toHsv(),
                         s = n.toRgb(),
                         o = n.toHex();
                     return 0 === i.s && (i.h = e || 0, r.h = e || 0), {
                         hsl: i,
                         hex: "000000" === o && 0 === s.a ? "transparent" : "#" + o,
                         rgb: s,
                         hsv: r,
                         oldHue: t.h || e || i.h,
                         source: t.source
                     }
                 },
-                Sn = function(t) {
+                Pn = function(t) {
                     if ("transparent" === t) return !0;
                     var e = "#" === String(t).charAt(0) ? 1 : 0;
                     return t.length !== 4 + e && t.length < 7 + e && We(t).isValid()
                 },
                 Cn = function(t) {
                     if (!t) return "#fff";
-                    var e = Pn(t);
+                    var e = Sn(t);
                     return "transparent" === e.hex ? "rgba(0,0,0,0.4)" : (299 * e.rgb.r + 587 * e.rgb.g + 114 * e.rgb.b) / 1e3 >= 128 ? "#000" : "#fff"
                 },
                 Tn = function(t, e) {
                     return We(e + " (" + t.replace("°", "") + ")")._ok
                 },
                 An = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
@@ -2169,35 +2169,35 @@
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
                         return n && t(e.prototype, n), i && t(e, i), e
                     }
                 }();
-            const Ln = function(t) {
+            const On = function(t) {
                 var e = function(e) {
                     function n(t) {
                         ! function(t, e) {
                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                         }(this, n);
                         var e = function(t, e) {
                             if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return !e || "object" != typeof e && "function" != typeof e ? t : e
                         }(this, (n.__proto__ || Object.getPrototypeOf(n)).call(this));
                         return e.handleChange = function(t, n) {
                             if (En(t)) {
-                                var i = Pn(t, t.h || e.state.oldHue);
+                                var i = Sn(t, t.h || e.state.oldHue);
                                 e.setState(i), e.props.onChangeComplete && e.debounce(e.props.onChangeComplete, i, n), e.props.onChange && e.props.onChange(i, n)
                             }
                         }, e.handleSwatchHover = function(t, n) {
                             if (En(t)) {
-                                var i = Pn(t, t.h || e.state.oldHue);
+                                var i = Sn(t, t.h || e.state.oldHue);
                                 e.props.onSwatchHover && e.props.onSwatchHover(i, n)
                             }
-                        }, e.state = An({}, Pn(t.color, 0)), e.debounce = Oe((function(t, e, n) {
+                        }, e.state = An({}, Sn(t.color, 0)), e.debounce = Le((function(t, e, n) {
                             t(e, n)
                         }), 100), e
                     }
                     return function(t, e) {
                         if ("function" != typeof e && null !== e) throw new TypeError("Super expression must either be null or a function, not " + typeof e);
                         t.prototype = Object.create(e && e.prototype, {
                             constructor: {
@@ -2214,35 +2214,35 @@
                             return this.props.onSwatchHover && (e.onSwatchHover = this.handleSwatchHover), h().createElement(t, An({}, this.props, this.state, {
                                 onChange: this.handleChange
                             }, e))
                         }
                     }], [{
                         key: "getDerivedStateFromProps",
                         value: function(t, e) {
-                            return An({}, Pn(t.color, e.oldHue))
+                            return An({}, Sn(t.color, e.oldHue))
                         }
                     }]), n
                 }(c.PureComponent || c.Component);
                 return e.propTypes = An({}, t.propTypes), e.defaultProps = An({}, t.defaultProps, {
                     color: {
                         h: 250,
                         s: .5,
                         l: .2,
                         a: 1
                     }
                 }), e
             };
-            var On = Object.assign || function(t) {
+            var Ln = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
                         for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
                     }
                     return t
                 },
-                Rn = function() {
+                In = function() {
                     function t(t, e) {
                         for (var n = 0; n < e.length; n++) {
                             var i = e[n];
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
@@ -2250,15 +2250,15 @@
                     }
                 }();
 
             function kn(t, e) {
                 if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                 return !e || "object" != typeof e && "function" != typeof e ? t : e
             }
-            var In = Object.assign || function(t) {
+            var Rn = Object.assign || function(t) {
                 for (var e = 1; e < arguments.length; e++) {
                     var n = arguments[e];
                     for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
                 }
                 return t
             };
             const jn = function(t) {
@@ -2288,21 +2288,21 @@
                             constructor: {
                                 value: t,
                                 enumerable: !1,
                                 writable: !0,
                                 configurable: !0
                             }
                         }), e && (Object.setPrototypeOf ? Object.setPrototypeOf(t, e) : t.__proto__ = e)
-                    }(i, n), Rn(i, [{
+                    }(i, n), In(i, [{
                         key: "render",
                         value: function() {
                             return h().createElement(e, {
                                 onFocus: this.handleFocus,
                                 onBlur: this.handleBlur
-                            }, h().createElement(t, On({}, this.props, this.state)))
+                            }, h().createElement(t, Ln({}, this.props, this.state)))
                         }
                     }]), i
                 }(h().Component)
             }((function(t) {
                 var e = t.color,
                     n = t.style,
                     i = t.onClick,
@@ -2313,28 +2313,28 @@
                     l = t.children,
                     c = t.focus,
                     u = t.focusStyle,
                     d = void 0 === u ? {} : u,
                     f = "transparent" === e,
                     g = (0, p.ZP)({
                         default: {
-                            swatch: In({
+                            swatch: Rn({
                                 background: e,
                                 height: "100%",
                                 width: "100%",
                                 cursor: "pointer",
                                 position: "relative",
                                 outline: "none"
                             }, n, c ? d : {})
                         }
                     }),
                     m = {};
                 return s && (m.onMouseOver = function(t) {
                     return s(e, t)
-                }), h().createElement("div", In({
+                }), h().createElement("div", Rn({
                     style: g.swatch,
                     onClick: function(t) {
                         return r(e, t)
                     },
                     title: a,
                     tabIndex: 0,
                     onKeyDown: function(t) {
@@ -2414,31 +2414,31 @@
                         }, {
                             vertical: "vertical" === e
                         });
                     return h().createElement("div", {
                         style: n.picker
                     })
                 }
-            }, Ln(Fn);
+            }, On(Fn);
             const Bn = function(t, e) {
                 for (var n = -1, i = null == t ? 0 : t.length, r = Array(i); ++n < i;) r[n] = e(t[n], n, t);
                 return r
             };
 
-            function Dn(t) {
+            function Nn(t) {
                 var e = -1,
                     n = null == t ? 0 : t.length;
                 for (this.__data__ = new ft; ++e < n;) this.add(t[e])
             }
-            Dn.prototype.add = Dn.prototype.push = function(t) {
+            Nn.prototype.add = Nn.prototype.push = function(t) {
                 return this.__data__.set(t, "__lodash_hash_undefined__"), this
-            }, Dn.prototype.has = function(t) {
+            }, Nn.prototype.has = function(t) {
                 return this.__data__.has(t)
             };
-            const Nn = Dn,
+            const Dn = Nn,
                 Vn = function(t, e) {
                     for (var n = -1, i = null == t ? 0 : t.length; ++n < i;)
                         if (e(t[n], n, t)) return !0;
                     return !1
                 },
                 Un = function(t, e) {
                     return t.has(e)
@@ -2449,15 +2449,15 @@
                         l = e.length;
                     if (a != l && !(o && l > a)) return !1;
                     var c = s.get(t),
                         h = s.get(e);
                     if (c && h) return c == e && h == t;
                     var u = -1,
                         d = !0,
-                        p = 2 & n ? new Nn : void 0;
+                        p = 2 & n ? new Dn : void 0;
                     for (s.set(t, e), s.set(e, t); ++u < a;) {
                         var f = t[u],
                             g = e[u];
                         if (i) var m = o ? i(g, f, u, e, t, s) : i(f, g, u, t, e, s);
                         if (void 0 !== m) {
                             if (m) continue;
                             d = !1;
@@ -2488,26 +2488,26 @@
                     var e = -1,
                         n = Array(t.size);
                     return t.forEach((function(t) {
                         n[++e] = t
                     })), n
                 };
             var Zn = B ? B.prototype : void 0,
-                qn = Zn ? Zn.valueOf : void 0;
-            var Xn = Object.prototype.propertyIsEnumerable,
+                Xn = Zn ? Zn.valueOf : void 0;
+            var qn = Object.prototype.propertyIsEnumerable,
                 Yn = Object.getOwnPropertySymbols;
             const Kn = Yn ? function(t) {
                     return null == t ? [] : (t = Object(t), function(t, e) {
                         for (var n = -1, i = null == t ? 0 : t.length, r = 0, s = []; ++n < i;) {
                             var o = t[n];
                             e(o, n, t) && (s[r++] = o)
                         }
                         return s
                     }(Yn(t), (function(e) {
-                        return Xn.call(t, e)
+                        return qn.call(t, e)
                     })))
                 } : function() {
                     return []
                 },
                 $n = function(t) {
                     return function(t, e, n) {
                         var i = e(t);
@@ -2560,29 +2560,29 @@
                     var o = zt(t),
                         a = zt(e),
                         l = o ? mi : fi(t),
                         c = a ? mi : fi(e),
                         h = (l = l == gi ? vi : l) == vi,
                         u = (c = c == gi ? vi : c) == vi,
                         d = l == c;
-                    if (d && (0, Dt.Z)(t)) {
-                        if (!(0, Dt.Z)(e)) return !1;
+                    if (d && (0, Nt.Z)(t)) {
+                        if (!(0, Nt.Z)(e)) return !1;
                         o = !0, h = !1
                     }
-                    if (d && !h) return s || (s = new mt), o || Xt(t) ? Gn(t, e, n, i, r, s) : function(t, e, n, i, r, s, o) {
+                    if (d && !h) return s || (s = new mt), o || qt(t) ? Gn(t, e, n, i, r, s) : function(t, e, n, i, r, s, o) {
                         switch (n) {
                             case "[object DataView]":
                                 if (t.byteLength != e.byteLength || t.byteOffset != e.byteOffset) return !1;
                                 t = t.buffer, e = e.buffer;
                             case "[object ArrayBuffer]":
                                 return !(t.byteLength != e.byteLength || !s(new wt(t), new wt(e)));
                             case "[object Boolean]":
                             case "[object Date]":
                             case "[object Number]":
-                                return R(+t, +e);
+                                return I(+t, +e);
                             case "[object Error]":
                                 return t.name == e.name && t.message == e.message;
                             case "[object RegExp]":
                             case "[object String]":
                                 return t == e + "";
                             case "[object Map]":
                                 var a = Wn;
@@ -2591,15 +2591,15 @@
                                 if (a || (a = Hn), t.size != e.size && !l) return !1;
                                 var c = o.get(t);
                                 if (c) return c == e;
                                 i |= 2, o.set(t, e);
                                 var h = Gn(a(t), a(e), i, r, s, o);
                                 return o.delete(t), h;
                             case "[object Symbol]":
-                                if (qn) return qn.call(t) == qn.call(e)
+                                if (Xn) return Xn.call(t) == Xn.call(e)
                         }
                         return !1
                     }(t, e, l, n, i, r, s);
                     if (!(1 & n)) {
                         var p = h && bi.call(t, "__wrapped__"),
                             f = u && bi.call(e, "__wrapped__");
                         if (p || f) {
@@ -2637,15 +2637,15 @@
                                 y = e.constructor;
                             b == y || !("constructor" in t) || !("constructor" in e) || "function" == typeof b && b instanceof b && "function" == typeof y && y instanceof y || (p = !1)
                         }
                         return s.delete(t), s.delete(e), p
                     }(t, e, n, i, r, s))
                 },
                 _i = function t(e, n, i, r, s) {
-                    return e === n || (null == e || null == n || !Lt(e) && !Lt(n) ? e != e && n != n : yi(e, n, i, r, t, s))
+                    return e === n || (null == e || null == n || !Ot(e) && !Ot(n) ? e != e && n != n : yi(e, n, i, r, t, s))
                 },
                 xi = function(t) {
                     return t == t && !Z(t)
                 },
                 wi = function(t, e) {
                     return function(n) {
                         return null != n && n[t] === e && (void 0 !== e || t in Object(n))
@@ -2682,20 +2682,20 @@
                                     if (!(void 0 === d ? _i(h, c, 3, i, u) : d)) return !1
                                 }
                             }
                             return !0
                         }(n, t, e)
                     }
                 };
-            var Pi = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
-                Si = /^\w*$/;
+            var Si = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
+                Pi = /^\w*$/;
             const Ci = function(t, e) {
                 if (zt(t)) return !1;
                 var n = typeof t;
-                return !("number" != n && "symbol" != n && "boolean" != n && null != t && !Ee(t)) || Si.test(t) || !Pi.test(t) || null != e && t in Object(e)
+                return !("number" != n && "symbol" != n && "boolean" != n && null != t && !Ee(t)) || Pi.test(t) || !Si.test(t) || null != e && t in Object(e)
             };
 
             function Ti(t, e) {
                 if ("function" != typeof t || null != e && "function" != typeof e) throw new TypeError("Expected a function");
                 var n = function() {
                     var i = arguments,
                         r = e ? e.apply(this, i) : i[0],
@@ -2705,71 +2705,71 @@
                     return n.cache = s.set(r, o) || s, o
                 };
                 return n.cache = new(Ti.Cache || ft), n
             }
             Ti.Cache = ft;
             const Ai = Ti;
             var Mi = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
-                Li = /\\(\\)?/g;
-            const Oi = function(t) {
+                Oi = /\\(\\)?/g;
+            const Li = function(t) {
                 var e = Ai(t, (function(t) {
                         return 500 === n.size && n.clear(), t
                     })),
                     n = e.cache;
                 return e
             }((function(t) {
                 var e = [];
                 return 46 === t.charCodeAt(0) && e.push(""), t.replace(Mi, (function(t, n, i, r) {
-                    e.push(i ? r.replace(Li, "$1") : n || t)
+                    e.push(i ? r.replace(Oi, "$1") : n || t)
                 })), e
             }));
-            var Ri = B ? B.prototype : void 0,
-                ki = Ri ? Ri.toString : void 0;
-            const Ii = function t(e) {
+            var Ii = B ? B.prototype : void 0,
+                ki = Ii ? Ii.toString : void 0;
+            const Ri = function t(e) {
                     if ("string" == typeof e) return e;
                     if (zt(e)) return Bn(e, t) + "";
                     if (Ee(e)) return ki ? ki.call(e) : "";
                     var n = e + "";
                     return "0" == n && 1 / e == -1 / 0 ? "-0" : n
                 },
                 ji = function(t) {
-                    return null == t ? "" : Ii(t)
+                    return null == t ? "" : Ri(t)
                 },
                 zi = function(t, e) {
-                    return zt(t) ? t : Ci(t, e) ? [t] : Oi(ji(t))
+                    return zt(t) ? t : Ci(t, e) ? [t] : Li(ji(t))
                 },
                 Fi = function(t) {
                     if ("string" == typeof t || Ee(t)) return t;
                     var e = t + "";
                     return "0" == e && 1 / t == -1 / 0 ? "-0" : e
                 },
                 Bi = function(t, e) {
                     for (var n = 0, i = (e = zi(e, t)).length; null != t && n < i;) t = t[Fi(e[n++])];
                     return n && n == i ? t : void 0
                 },
-                Di = function(t, e) {
+                Ni = function(t, e) {
                     return null != t && e in Object(t)
                 },
-                Ni = function(t, e) {
+                Di = function(t, e) {
                     return null != t && function(t, e, n) {
                         for (var i = -1, r = (e = zi(e, t)).length, s = !1; ++i < r;) {
                             var o = Fi(e[i]);
                             if (!(s = null != t && n(t, o))) break;
                             t = t[o]
                         }
                         return s || ++i != r ? s : !!(r = null == t ? 0 : t.length) && Ft(r) && te(o, r) && (zt(t) || jt(t))
-                    }(t, e, Di)
+                    }(t, e, Ni)
                 },
                 Vi = function(t, e) {
                     return Ci(t) && xi(e) ? wi(Fi(t), e) : function(n) {
                         var i = function(t, e, n) {
                             var i = null == t ? void 0 : Bi(t, e);
                             return void 0 === i ? n : i
                         }(n, t);
-                        return void 0 === i && i === e ? Ni(n, t) : _i(e, i, 3)
+                        return void 0 === i && i === e ? Di(n, t) : _i(e, i, 3)
                     }
                 },
                 Ui = function(t) {
                     return Ci(t) ? (e = Fi(t), function(t) {
                         return null == t ? void 0 : t[e]
                     }) : function(t) {
                         return function(e) {
@@ -2777,15 +2777,15 @@
                         }
                     }(t);
                     var e
                 },
                 Gi = function(t, e) {
                     var n = -1,
                         i = Bt(t) ? Array(t.length) : [];
-                    return De(t, (function(t, r, s) {
+                    return Ne(t, (function(t, r, s) {
                         i[++n] = e(t, r, s)
                     })), i
                 },
                 Wi = function(t, e) {
                     return (zt(t) ? Bn : Gi)(t, "function" == typeof(n = e) ? n : null == n ? ce : "object" == typeof n ? zt(n) ? Vi(n[0], n[1]) : Ei(n) : Ui(n));
                     var n
                 },
@@ -2837,15 +2837,15 @@
                     o = t.triangle,
                     a = t.styles,
                     l = void 0 === a ? {} : a,
                     c = t.className,
                     u = void 0 === c ? "" : c,
                     d = "transparent" === i,
                     f = function(t, n) {
-                        Sn(t) && e({
+                        Pn(t) && e({
                             hex: t,
                             source: "hex"
                         }, n)
                     },
                     g = (0, p.ZP)(ge({
                         default: {
                             card: {
@@ -2926,26 +2926,26 @@
                         input: g.input
                     },
                     value: i,
                     onChange: f
                 })))
             };
             Zi.propTypes = {
-                width: O().oneOfType([O().string, O().number]),
-                colors: O().arrayOf(O().string),
-                triangle: O().oneOf(["top", "hide"]),
-                styles: O().object
+                width: L().oneOfType([L().string, L().number]),
+                colors: L().arrayOf(L().string),
+                triangle: L().oneOf(["top", "hide"]),
+                styles: L().object
             }, Zi.defaultProps = {
                 width: 170,
                 colors: ["#D9E3F0", "#F47373", "#697689", "#37D67A", "#2CCCE4", "#555555", "#dce775", "#ff8a65", "#ba68c8"],
                 triangle: "top",
                 styles: {}
-            }, Ln(Zi);
-            var qi = "#ffcdd2",
-                Xi = "#e57373",
+            }, On(Zi);
+            var Xi = "#ffcdd2",
+                qi = "#e57373",
                 Yi = "#f44336",
                 Ki = "#d32f2f",
                 $i = "#b71c1c",
                 Ji = "#f8bbd0",
                 Qi = "#f06292",
                 tr = "#e91e63",
                 er = "#c2185b",
@@ -2967,39 +2967,39 @@
                 vr = "#1a237e",
                 br = "#bbdefb",
                 yr = "#64b5f6",
                 _r = "#2196f3",
                 xr = "#1976d2",
                 wr = "#0d47a1",
                 Er = "#b3e5fc",
-                Pr = "#4fc3f7",
-                Sr = "#03a9f4",
+                Sr = "#4fc3f7",
+                Pr = "#03a9f4",
                 Cr = "#0288d1",
                 Tr = "#01579b",
                 Ar = "#b2ebf2",
                 Mr = "#4dd0e1",
-                Lr = "#00bcd4",
-                Or = "#0097a7",
-                Rr = "#006064",
+                Or = "#00bcd4",
+                Lr = "#0097a7",
+                Ir = "#006064",
                 kr = "#b2dfdb",
-                Ir = "#4db6ac",
+                Rr = "#4db6ac",
                 jr = "#009688",
                 zr = "#00796b",
                 Fr = "#004d40",
                 Br = "#c8e6c9",
-                Dr = "#81c784",
-                Nr = "#4caf50",
+                Nr = "#81c784",
+                Dr = "#4caf50",
                 Vr = "#388e3c",
                 Ur = "#dcedc8",
                 Gr = "#aed581",
                 Wr = "#8bc34a",
                 Hr = "#689f38",
                 Zr = "#33691e",
-                qr = "#f0f4c3",
-                Xr = "#dce775",
+                Xr = "#f0f4c3",
+                qr = "#dce775",
                 Yr = "#cddc39",
                 Kr = "#afb42b",
                 $r = "#827717",
                 Jr = "#fff9c4",
                 Qr = "#fff176",
                 ts = "#ffeb3b",
                 es = "#fbc02d",
@@ -3021,16 +3021,16 @@
                 vs = "#bf360c",
                 bs = "#d7ccc8",
                 ys = "#a1887f",
                 _s = "#795548",
                 xs = "#5d4037",
                 ws = "#3e2723",
                 Es = "#cfd8dc",
-                Ps = "#90a4ae",
-                Ss = "#607d8b",
+                Ss = "#90a4ae",
+                Ps = "#607d8b",
                 Cs = "#455a64",
                 Ts = "#263238",
                 As = function(t) {
                     var e = t.color,
                         n = t.onClick,
                         i = t.onSwatchHover,
                         r = t.hover,
@@ -3081,15 +3081,15 @@
                     }))
                 };
             As.defaultProps = {
                 circleSize: 28,
                 circleSpacing: 14
             };
             const Ms = (0, p.tz)(As);
-            var Ls = function(t) {
+            var Os = function(t) {
                 var e = t.width,
                     n = t.onChange,
                     i = t.onSwatchHover,
                     r = t.colors,
                     s = t.hex,
                     o = t.circleSize,
                     a = t.styles,
@@ -3125,42 +3125,42 @@
                         onSwatchHover: i,
                         active: s === t.toLowerCase(),
                         circleSize: o,
                         circleSpacing: c
                     })
                 })))
             };
-            Ls.propTypes = {
-                width: O().oneOfType([O().string, O().number]),
-                circleSize: O().number,
-                circleSpacing: O().number,
-                styles: O().object
-            }, Ls.defaultProps = {
+            Os.propTypes = {
+                width: L().oneOfType([L().string, L().number]),
+                circleSize: L().number,
+                circleSpacing: L().number,
+                styles: L().object
+            }, Os.defaultProps = {
                 width: 252,
                 circleSize: 28,
                 circleSpacing: 14,
-                colors: [Yi, tr, sr, hr, gr, _r, Sr, Lr, jr, Nr, Wr, Yr, ts, ss, hs, gs, _s, Ss],
+                colors: [Yi, tr, sr, hr, gr, _r, Pr, Or, jr, Dr, Wr, Yr, ts, ss, hs, gs, _s, Ps],
                 styles: {}
-            }, Ln(Ls);
-            const Os = function(t) {
+            }, On(Os);
+            const Ls = function(t) {
                 return void 0 === t
             };
-            var Rs = n(746),
+            var Is = n(746),
                 ks = function() {
                     function t(t, e) {
                         for (var n = 0; n < e.length; n++) {
                             var i = e[n];
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
                         return n && t(e.prototype, n), i && t(e, i), e
                     }
                 }(),
-                Is = function(t) {
+                Rs = function(t) {
                     function e(t) {
                         ! function(t, e) {
                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                         }(this, e);
                         var n = function(t, e) {
                             if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return !e || "object" != typeof e && "function" != typeof e ? t : e
@@ -3172,15 +3172,15 @@
                                 view: "hsl"
                             }) : "hsl" === n.state.view && (1 === n.props.hsl.a ? n.setState({
                                 view: "hex"
                             }) : n.setState({
                                 view: "rgb"
                             }))
                         }, n.handleChange = function(t, e) {
-                            t.hex ? Sn(t.hex) && n.props.onChange({
+                            t.hex ? Pn(t.hex) && n.props.onChange({
                                 hex: t.hex,
                                 source: "hex"
                             }, e) : t.r || t.g || t.b ? n.props.onChange({
                                 r: t.r || n.props.rgb.r,
                                 g: t.g || n.props.rgb.g,
                                 b: t.b || n.props.rgb.b,
                                 source: "rgb"
@@ -3188,16 +3188,16 @@
                                 h: n.props.hsl.h,
                                 s: n.props.hsl.s,
                                 l: n.props.hsl.l,
                                 a: Math.round(100 * t.a) / 100,
                                 source: "rgb"
                             }, e)) : (t.h || t.s || t.l) && ("string" == typeof t.s && t.s.includes("%") && (t.s = t.s.replace("%", "")), "string" == typeof t.l && t.l.includes("%") && (t.l = t.l.replace("%", "")), 1 == t.s ? t.s = .01 : 1 == t.l && (t.l = .01), n.props.onChange({
                                 h: t.h || n.props.hsl.h,
-                                s: Number(Os(t.s) ? n.props.hsl.s : t.s),
-                                l: Number(Os(t.l) ? n.props.hsl.l : t.l),
+                                s: Number(Ls(t.s) ? n.props.hsl.s : t.s),
+                                l: Number(Ls(t.l) ? n.props.hsl.l : t.l),
                                 source: "hsl"
                             }, e))
                         }, n.showHighlight = function(t) {
                             t.currentTarget.style.background = "#eee"
                         }, n.hideHighlight = function(t) {
                             t.currentTarget.style.background = "transparent"
                         }, 1 !== t.hsl.a && "hex" === t.view ? n.state = {
@@ -3402,15 +3402,15 @@
                                 style: e.toggle
                             }, h().createElement("div", {
                                 style: e.icon,
                                 onClick: this.toggleViews,
                                 ref: function(e) {
                                     return t.icon = e
                                 }
-                            }, h().createElement(Rs.Z, {
+                            }, h().createElement(Is.Z, {
                                 style: e.svg,
                                 onMouseOver: this.showHighlight,
                                 onMouseEnter: this.showHighlight,
                                 onMouseOut: this.hideHighlight
                             }))))
                         }
                     }], [{
@@ -3418,18 +3418,18 @@
                         value: function(t, e) {
                             return 1 !== t.hsl.a && "hex" === e.view ? {
                                 view: "rgb"
                             } : null
                         }
                     }]), e
                 }(h().Component);
-            Is.defaultProps = {
+            Rs.defaultProps = {
                 view: "hex"
             };
-            const js = Is,
+            const js = Rs,
                 zs = function() {
                     var t = (0, p.ZP)({
                         default: {
                             picker: {
                                 width: "12px",
                                 height: "12px",
                                 borderRadius: "6px",
@@ -3556,15 +3556,15 @@
                         disableAlpha: i
                     });
                 return h().createElement("div", {
                     style: m.picker,
                     className: "chrome-picker " + f
                 }, h().createElement("div", {
                     style: m.saturation
-                }, h().createElement(Ie, {
+                }, h().createElement(Re, {
                     style: m.Saturation,
                     hsl: s,
                     hsv: o,
                     pointer: Fs,
                     onChange: n
                 })), h().createElement("div", {
                     style: m.body
@@ -3603,24 +3603,24 @@
                     hex: a,
                     view: g,
                     onChange: n,
                     disableAlpha: i
                 })))
             };
             Bs.propTypes = {
-                width: O().oneOfType([O().string, O().number]),
-                disableAlpha: O().bool,
-                styles: O().object,
-                defaultView: O().oneOf(["hex", "rgb", "hsl"])
+                width: L().oneOfType([L().string, L().number]),
+                disableAlpha: L().bool,
+                styles: L().object,
+                defaultView: L().oneOf(["hex", "rgb", "hsl"])
             }, Bs.defaultProps = {
                 width: 225,
                 disableAlpha: !1,
                 styles: {}
-            }, Ln(Bs);
-            const Ds = function(t) {
+            }, On(Bs);
+            const Ns = function(t) {
                     var e = t.color,
                         n = t.onClick,
                         i = void 0 === n ? function() {} : n,
                         r = t.onSwatchHover,
                         s = t.active,
                         o = (0, p.ZP)({
                             default: {
@@ -3672,15 +3672,15 @@
                         focusStyle: {
                             boxShadow: "0 0 4px " + e
                         }
                     }, h().createElement("div", {
                         style: o.dot
                     }))
                 },
-                Ns = function(t) {
+                Ds = function(t) {
                     var e = t.hex,
                         n = t.rgb,
                         i = t.onChange,
                         r = (0, p.ZP)({
                             default: {
                                 fields: {
                                     display: "flex",
@@ -3818,48 +3818,48 @@
                             },
                             clear: {
                                 clear: "both"
                             }
                         }
                     }, a)),
                     d = function(t, n) {
-                        t.hex ? Sn(t.hex) && e({
+                        t.hex ? Pn(t.hex) && e({
                             hex: t.hex,
                             source: "hex"
                         }, n) : e(t, n)
                     };
                 return h().createElement(be, {
                     style: u.Compact,
                     styles: a
                 }, h().createElement("div", {
                     style: u.compact,
                     className: "compact-picker " + c
                 }, h().createElement("div", null, Wi(i, (function(t) {
-                    return h().createElement(Ds, {
+                    return h().createElement(Ns, {
                         key: t,
                         color: t,
                         active: t.toLowerCase() === r,
                         onClick: d,
                         onSwatchHover: n
                     })
                 })), h().createElement("div", {
                     style: u.clear
-                })), h().createElement(Ns, {
+                })), h().createElement(Ds, {
                     hex: r,
                     rgb: s,
                     onChange: d
                 })))
             };
             Vs.propTypes = {
-                colors: O().arrayOf(O().string),
-                styles: O().object
+                colors: L().arrayOf(L().string),
+                styles: L().object
             }, Vs.defaultProps = {
                 colors: ["#4D4D4D", "#999999", "#FFFFFF", "#F44E3B", "#FE9200", "#FCDC00", "#DBDF00", "#A4DD00", "#68CCCA", "#73D8FF", "#AEA1FF", "#FDA1FF", "#333333", "#808080", "#cccccc", "#D33115", "#E27300", "#FCC400", "#B0BC00", "#68BC00", "#16A5A5", "#009CE0", "#7B64FF", "#FA28FF", "#000000", "#666666", "#B3B3B3", "#9F0500", "#C45100", "#FB9E00", "#808900", "#194D33", "#0C797D", "#0062B1", "#653294", "#AB149E"],
                 styles: {}
-            }, Ln(Vs);
+            }, On(Vs);
             const Us = (0, p.tz)((function(t) {
                 var e = t.hover,
                     n = t.color,
                     i = t.onClick,
                     r = t.onSwatchHover,
                     s = {
                         position: "relative",
@@ -4002,24 +4002,24 @@
                         key: t,
                         onClick: d,
                         onSwatchHover: r
                     })
                 })))
             };
             Gs.propTypes = {
-                width: O().oneOfType([O().string, O().number]),
-                colors: O().arrayOf(O().string),
-                triangle: O().oneOf(["hide", "top-left", "top-right", "bottom-left", "bottom-right"]),
-                styles: O().object
+                width: L().oneOfType([L().string, L().number]),
+                colors: L().arrayOf(L().string),
+                triangle: L().oneOf(["hide", "top-left", "top-right", "bottom-left", "bottom-right"]),
+                styles: L().object
             }, Gs.defaultProps = {
                 width: 200,
                 colors: ["#B80000", "#DB3E00", "#FCCB00", "#008B02", "#006B76", "#1273DE", "#004DCF", "#5300EB", "#EB9694", "#FAD0C3", "#FEF3BD", "#C1E1C5", "#BEDADC", "#C4DEF6", "#BED3F3", "#D4C4FB"],
                 triangle: "top-left",
                 styles: {}
-            }, Ln(Gs);
+            }, On(Gs);
             var Ws = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
                         for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
                     }
                     return t
                 },
@@ -4060,15 +4060,15 @@
                                 s: 1
                             })
                         },
                         direction: s
                     })))
                 };
             Hs.propTypes = {
-                styles: O().object
+                styles: L().object
             }, Hs.defaultProps = {
                 width: "316px",
                 height: "16px",
                 direction: "horizontal",
                 pointer: function(t) {
                     var e = t.direction,
                         n = (0, p.ZP)({
@@ -4091,15 +4091,15 @@
                             vertical: "vertical" === e
                         });
                     return h().createElement("div", {
                         style: n.picker
                     })
                 },
                 styles: {}
-            }, Ln(Hs), Ln((function(t) {
+            }, On(Hs), On((function(t) {
                 var e = t.onChange,
                     n = t.hex,
                     i = t.rgb,
                     r = t.styles,
                     s = void 0 === r ? {} : r,
                     o = t.className,
                     a = void 0 === o ? "" : o,
@@ -4166,15 +4166,15 @@
                             third: {
                                 flex: "1",
                                 paddingRight: "10px"
                             }
                         }
                     }, s)),
                     c = function(t, n) {
-                        t.hex ? Sn(t.hex) && e({
+                        t.hex ? Pn(t.hex) && e({
                             hex: t.hex,
                             source: "hex"
                         }, n) : (t.r || t.g || t.b) && e({
                             r: t.r || i.r,
                             g: t.g || i.g,
                             b: t.b || i.b,
                             source: "rgb"
@@ -4305,15 +4305,15 @@
                                     height: "20px",
                                     lineHeight: "22px",
                                     paddingBottom: "7px"
                                 }
                             }
                         }),
                         o = function(t, r) {
-                            t["#"] ? Sn(t["#"]) && e({
+                            t["#"] ? Pn(t["#"]) && e({
                                 hex: t["#"],
                                 source: "hex"
                             }, r) : t.r || t.g || t.b ? e({
                                 r: t.r || n.r,
                                 g: t.g || n.g,
                                 b: t.b || n.b,
                                 source: "rgb"
@@ -4399,15 +4399,15 @@
                         style: s.symbol
                     }, "°"), h().createElement("div", {
                         style: s.symbol
                     }, "%"), h().createElement("div", {
                         style: s.symbol
                     }, "%")))
                 },
-                qs = function(t) {
+                Xs = function(t) {
                     var e = t.hsl,
                         n = (0, p.ZP)({
                             default: {
                                 picker: {
                                     width: "12px",
                                     height: "12px",
                                     borderRadius: "6px",
@@ -4423,15 +4423,15 @@
                         }, {
                             "black-outline": e.l > .5
                         });
                     return h().createElement("div", {
                         style: n.picker
                     })
                 },
-                Xs = function() {
+                qs = function() {
                     var t = (0, p.ZP)({
                         default: {
                             triangle: {
                                 width: 0,
                                 height: 0,
                                 borderStyle: "solid",
                                 borderWidth: "4px 0 4px 6px",
@@ -4655,25 +4655,25 @@
                             }, h().createElement("div", {
                                 style: s.head
                             }, this.props.header), h().createElement("div", {
                                 style: s.body,
                                 className: "flexbox-fix"
                             }, h().createElement("div", {
                                 style: s.saturation
-                            }, h().createElement(Ie, {
+                            }, h().createElement(Re, {
                                 hsl: this.props.hsl,
                                 hsv: this.props.hsv,
-                                pointer: qs,
+                                pointer: Xs,
                                 onChange: this.props.onChange
                             })), h().createElement("div", {
                                 style: s.hue
                             }, h().createElement(M, {
                                 direction: "vertical",
                                 hsl: this.props.hsl,
-                                pointer: Xs,
+                                pointer: qs,
                                 onChange: this.props.onChange
                             })), h().createElement("div", {
                                 style: s.controls
                             }, h().createElement("div", {
                                 style: s.top,
                                 className: "flexbox-fix"
                             }, h().createElement("div", {
@@ -4696,20 +4696,20 @@
                                 hsv: this.props.hsv,
                                 hex: this.props.hex
                             }))))))
                         }
                     }]), e
                 }(h().Component);
             Js.propTypes = {
-                header: O().string,
-                styles: O().object
+                header: L().string,
+                styles: L().object
             }, Js.defaultProps = {
                 header: "Color Picker",
                 styles: {}
-            }, Ln(Js);
+            }, On(Js);
             const Qs = function(t) {
                 var e = t.onChange,
                     n = t.rgb,
                     i = t.hsl,
                     r = t.hex,
                     s = t.disableAlpha,
                     o = (0, p.ZP)({
@@ -4751,15 +4751,15 @@
                                 display: "none"
                             }
                         }
                     }, {
                         disableAlpha: s
                     }),
                     a = function(t, r) {
-                        t.hex ? Sn(t.hex) && e({
+                        t.hex ? Pn(t.hex) && e({
                             hex: t.hex,
                             source: "hex"
                         }, r) : t.r || t.g || t.b ? e({
                             r: t.r || n.r,
                             g: t.g || n.g,
                             b: t.b || n.b,
                             a: n.a,
@@ -4899,17 +4899,17 @@
                             focusStyle: {
                                 boxShadow: "inset 0 0 0 1px rgba(0,0,0,.15), 0 0 4px " + e.color
                             }
                         })))
                     })))
                 };
             eo.propTypes = {
-                colors: O().arrayOf(O().oneOfType([O().string, O().shape({
-                    color: O().string,
-                    title: O().string
+                colors: L().arrayOf(L().oneOfType([L().string, L().shape({
+                    color: L().string,
+                    title: L().string
                 })])).isRequired
             };
             const no = eo;
             var io = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
                         for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
@@ -5007,15 +5007,15 @@
                             disableAlpha: l
                         });
                     return h().createElement("div", {
                         style: v.picker,
                         className: "sketch-picker " + m
                     }, h().createElement("div", {
                         style: v.saturation
-                    }, h().createElement(Ie, {
+                    }, h().createElement(Re, {
                         style: v.Saturation,
                         hsl: s,
                         hsv: r,
                         onChange: o
                     })), h().createElement("div", {
                         style: v.controls,
                         className: "flexbox-fix"
@@ -5048,24 +5048,24 @@
                     }), h().createElement(no, {
                         colors: c,
                         onClick: o,
                         onSwatchHover: a
                     }))
                 };
             ro.propTypes = {
-                disableAlpha: O().bool,
-                width: O().oneOfType([O().string, O().number]),
-                styles: O().object
+                disableAlpha: L().bool,
+                width: L().oneOfType([L().string, L().number]),
+                styles: L().object
             }, ro.defaultProps = {
                 disableAlpha: !1,
                 width: 200,
                 styles: {},
                 presetColors: ["#D0021B", "#F5A623", "#F8E71C", "#8B572A", "#7ED321", "#417505", "#BD10E0", "#9013FE", "#4A90E2", "#50E3C2", "#B8E986", "#000000", "#4A4A4A", "#9B9B9B", "#FFFFFF"]
             };
-            const so = Ln(ro),
+            const so = On(ro),
                 oo = function(t) {
                     var e = t.hsl,
                         n = t.offset,
                         i = t.onClick,
                         r = void 0 === i ? function() {} : i,
                         s = t.active,
                         o = t.first,
@@ -5207,15 +5207,15 @@
                     style: l.swatches
                 }, h().createElement(ao, {
                     hsl: e,
                     onClick: n
                 })))
             };
             lo.propTypes = {
-                styles: O().object
+                styles: L().object
             }, lo.defaultProps = {
                 pointer: function() {
                     var t = (0, p.ZP)({
                         default: {
                             picker: {
                                 width: "14px",
                                 height: "14px",
@@ -5227,15 +5227,15 @@
                         }
                     });
                     return h().createElement("div", {
                         style: t.picker
                     })
                 },
                 styles: {}
-            }, Ln(lo);
+            }, On(lo);
             var co = n(9367);
             const ho = function(t) {
                     var e = t.color,
                         n = t.onClick,
                         i = void 0 === n ? function() {} : n,
                         r = t.onSwatchHover,
                         s = t.first,
@@ -5385,44 +5385,44 @@
                         onSwatchHover: r
                     })
                 })), h().createElement("div", {
                     style: d.clear
                 })))))
             };
             po.propTypes = {
-                width: O().oneOfType([O().string, O().number]),
-                height: O().oneOfType([O().string, O().number]),
-                colors: O().arrayOf(O().arrayOf(O().string)),
-                styles: O().object
+                width: L().oneOfType([L().string, L().number]),
+                height: L().oneOfType([L().string, L().number]),
+                colors: L().arrayOf(L().arrayOf(L().string)),
+                styles: L().object
             }, po.defaultProps = {
                 width: 320,
                 height: 240,
                 colors: [
-                    [$i, Ki, Yi, Xi, qi],
+                    [$i, Ki, Yi, qi, Xi],
                     [nr, er, tr, Qi, Ji],
                     [ar, or, sr, rr, ir],
                     [dr, ur, hr, cr, lr],
                     [vr, mr, gr, fr, pr],
                     [wr, xr, _r, yr, br],
-                    [Tr, Cr, Sr, Pr, Er],
-                    [Rr, Or, Lr, Mr, Ar],
-                    [Fr, zr, jr, Ir, kr],
-                    ["#194D33", Vr, Nr, Dr, Br],
+                    [Tr, Cr, Pr, Sr, Er],
+                    [Ir, Lr, Or, Mr, Ar],
+                    [Fr, zr, jr, Rr, kr],
+                    ["#194D33", Vr, Dr, Nr, Br],
                     [Zr, Hr, Wr, Gr, Ur],
-                    [$r, Kr, Yr, Xr, qr],
+                    [$r, Kr, Yr, qr, Xr],
                     [ns, es, ts, Qr, Jr],
                     [as, os, ss, rs, is],
                     [ds, us, hs, cs, ls],
                     [vs, ms, gs, fs, ps],
                     [ws, xs, _s, ys, bs],
-                    [Ts, Cs, Ss, Ps, Es],
+                    [Ts, Cs, Ps, Ss, Es],
                     ["#000000", "#525252", "#969696", "#D9D9D9", "#FFFFFF"]
                 ],
                 styles: {}
-            }, Ln(po);
+            }, On(po);
             var fo = function(t) {
                 var e = t.onChange,
                     n = t.onSwatchHover,
                     i = t.hex,
                     r = t.colors,
                     s = t.width,
                     o = t.triangle,
@@ -5528,15 +5528,15 @@
                         }
                     }, l), {
                         "hide-triangle": "hide" === o,
                         "top-left-triangle": "top-left" === o,
                         "top-right-triangle": "top-right" === o
                     }),
                     f = function(t, n) {
-                        Sn(t) && e({
+                        Pn(t) && e({
                             hex: t,
                             source: "hex"
                         }, n)
                     };
                 return h().createElement("div", {
                     style: d.card,
                     className: "twitter-picker " + u
@@ -5568,24 +5568,24 @@
                     value: i.replace("#", ""),
                     onChange: f
                 }), h().createElement("div", {
                     style: d.clear
                 })))
             };
             fo.propTypes = {
-                width: O().oneOfType([O().string, O().number]),
-                triangle: O().oneOf(["hide", "top-left", "top-right"]),
-                colors: O().arrayOf(O().string),
-                styles: O().object
+                width: L().oneOfType([L().string, L().number]),
+                triangle: L().oneOf(["hide", "top-left", "top-right"]),
+                colors: L().arrayOf(L().string),
+                styles: L().object
             }, fo.defaultProps = {
                 width: 276,
                 colors: ["#FF6900", "#FCB900", "#7BDCB5", "#00D084", "#8ED1FC", "#0693E3", "#ABB8C3", "#EB144C", "#F78DA7", "#9900EF"],
                 triangle: "top-left",
                 styles: {}
-            }, Ln(fo);
+            }, On(fo);
             var go = function(t) {
                 var e = (0, p.ZP)({
                     default: {
                         picker: {
                             width: "20px",
                             height: "20px",
                             borderRadius: "22px",
@@ -5596,19 +5596,19 @@
                     }
                 });
                 return h().createElement("div", {
                     style: e.picker
                 })
             };
             go.propTypes = {
-                hsl: O().shape({
-                    h: O().number,
-                    s: O().number,
-                    l: O().number,
-                    a: O().number
+                hsl: L().shape({
+                    h: L().number,
+                    s: L().number,
+                    l: L().number,
+                    a: L().number
                 })
             }, go.defaultProps = {
                 hsl: {
                     a: 1,
                     h: 249.94,
                     l: .2,
                     s: .5
@@ -5629,19 +5629,19 @@
                     }
                 });
                 return h().createElement("div", {
                     style: e.picker
                 })
             };
             vo.propTypes = {
-                hsl: O().shape({
-                    h: O().number,
-                    s: O().number,
-                    l: O().number,
-                    a: O().number
+                hsl: L().shape({
+                    h: L().number,
+                    s: L().number,
+                    l: L().number,
+                    a: L().number
                 })
             }, vo.defaultProps = {
                 hsl: {
                     a: 1,
                     h: 249.94,
                     l: .2,
                     s: .5
@@ -5651,15 +5651,15 @@
                 yo = function(t) {
                     var e = t.onChange,
                         n = t.rgb,
                         i = t.hsl,
                         r = t.hex,
                         s = t.hsv,
                         o = function(t, n) {
-                            if (t.hex) Sn(t.hex) && e({
+                            if (t.hex) Pn(t.hex) && e({
                                 hex: t.hex,
                                 source: "hex"
                             }, n);
                             else if (t.rgb) {
                                 var i = t.rgb.split(",");
                                 Tn(t.rgb, "rgb") && e({
                                     r: i[0],
@@ -5891,15 +5891,15 @@
                     className: "google-picker " + d
                 }, h().createElement("div", {
                     style: f.head
                 }, a), h().createElement("div", {
                     style: f.swatch
                 }), h().createElement("div", {
                     style: f.saturation
-                }, h().createElement(Ie, {
+                }, h().createElement(Re, {
                     hsl: r,
                     hsv: s,
                     pointer: mo,
                     onChange: n
                 })), h().createElement("div", {
                     style: f.body
                 }, h().createElement("div", {
@@ -5947,25 +5947,25 @@
                     value: n,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : t[e] = n, t
             }
             _o.propTypes = {
-                width: O().oneOfType([O().string, O().number]),
-                styles: O().object,
-                header: O().string
+                width: L().oneOfType([L().string, L().number]),
+                styles: L().object,
+                header: L().string
             }, _o.defaultProps = {
                 width: 652,
                 styles: {},
                 header: "Color picker"
-            }, Ln(_o);
+            }, On(_o);
             let Eo = 1,
-                Po = 1;
-            class So {
+                So = 1;
+            class Po {
                 constructor() {
                     this.time = 0, this.channels = new Map, this.animations = new Map, this.playing = !1, this.lastEngineTime = -1
                 }
                 addChannel(t) {
                     const {
                         delay: e = 0,
                         duration: n = Number.POSITIVE_INFINITY,
@@ -6012,15 +6012,15 @@
                 pause() {
                     this.playing = !1, this.lastEngineTime = -1
                 }
                 reset() {
                     this.setTime(0)
                 }
                 attachAnimation(t, e) {
-                    const n = Po++;
+                    const n = So++;
                     return this.animations.set(n, {
                         animation: t,
                         channel: e
                     }), t.setTime(this.getTime(e)), n
                 }
                 detachAnimation(t) {
                     this.animations.delete(t)
@@ -6033,29 +6033,29 @@
                     n >= t.duration * t.repeat ? t.time = t.duration * t.rate : (t.time = Math.max(0, n) % t.duration, t.time *= t.rate)
                 }
             }
             const Co = Symbol.for("component"),
                 To = Symbol.for("asyncPropDefaults"),
                 Ao = Symbol.for("asyncPropOriginal"),
                 Mo = Symbol.for("asyncPropResolved");
-            var Lo = n(4155);
+            var Oo = n(4155);
 
-            function Oo(t) {
+            function Lo(t) {
                 if ("undefined" != typeof window && "object" == typeof window.process && "renderer" === window.process.type) return !0;
-                if (void 0 !== Lo && "object" == typeof Lo.versions && Boolean(Lo.versions.electron)) return !0;
+                if (void 0 !== Oo && "object" == typeof Oo.versions && Boolean(Oo.versions.electron)) return !0;
                 const e = "object" == typeof navigator && "string" == typeof navigator.userAgent && navigator.userAgent,
                     n = t || e;
                 return !!(n && n.indexOf("Electron") >= 0)
             }
-            var Ro = n(4155);
+            var Io = n(4155);
 
             function ko() {
-                return !("object" == typeof Ro && "[object process]" === String(Ro) && !Ro.browser) || Oo()
+                return !("object" == typeof Io && "[object process]" === String(Io) && !Io.browser) || Lo()
             }
-            const Io = "undefined" != typeof __VERSION__ ? __VERSION__ : "untranspiled source";
+            const Ro = "undefined" != typeof __VERSION__ ? __VERSION__ : "untranspiled source";
             ko();
             class jo {
                 constructor(t, e) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "sessionStorage";
                     wo(this, "storage", void 0), wo(this, "id", void 0), wo(this, "config", void 0), this.storage = function(t) {
                         try {
                             const e = window[t],
@@ -6096,26 +6096,26 @@
             }
             let Fo;
 
             function Bo(t) {
                 return "string" == typeof t ? Fo[t.toUpperCase()] || Fo.WHITE : t
             }
 
-            function Do(t, e) {
+            function No(t, e) {
                 if (!t) throw new Error(e || "Assertion failed")
             }! function(t) {
                 t[t.BLACK = 30] = "BLACK", t[t.RED = 31] = "RED", t[t.GREEN = 32] = "GREEN", t[t.YELLOW = 33] = "YELLOW", t[t.BLUE = 34] = "BLUE", t[t.MAGENTA = 35] = "MAGENTA", t[t.CYAN = 36] = "CYAN", t[t.WHITE = 37] = "WHITE", t[t.BRIGHT_BLACK = 90] = "BRIGHT_BLACK", t[t.BRIGHT_RED = 91] = "BRIGHT_RED", t[t.BRIGHT_GREEN = 92] = "BRIGHT_GREEN", t[t.BRIGHT_YELLOW = 93] = "BRIGHT_YELLOW", t[t.BRIGHT_BLUE = 94] = "BRIGHT_BLUE", t[t.BRIGHT_MAGENTA = 95] = "BRIGHT_MAGENTA", t[t.BRIGHT_CYAN = 96] = "BRIGHT_CYAN", t[t.BRIGHT_WHITE = 97] = "BRIGHT_WHITE"
             }(Fo || (Fo = {}));
-            var No = n(4155);
+            var Do = n(4155);
             const Vo = {
                     self: "undefined" != typeof self && self,
                     window: "undefined" != typeof window && window,
                     global: void 0 !== n.g && n.g,
                     document: "undefined" != typeof document && document,
-                    process: "object" == typeof No && No
+                    process: "object" == typeof Do && Do
                 },
                 Uo = Vo.window || Vo.self || Vo.global,
                 Go = Vo.process || {};
 
             function Wo() {
                 let t;
                 var e, n;
@@ -6135,27 +6135,27 @@
                     error: console.error
                 },
                 Zo = {
                     enabled: !0,
                     level: 0
                 };
 
-            function qo() {}
-            const Xo = {},
+            function Xo() {}
+            const qo = {},
                 Yo = {
                     once: !0
                 };
             class Ko {
                 constructor() {
                     let {
                         id: t
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {
                         id: ""
                     };
-                    wo(this, "id", void 0), wo(this, "VERSION", Io), wo(this, "_startTs", Wo()), wo(this, "_deltaTs", Wo()), wo(this, "_storage", void 0), wo(this, "userData", {}), wo(this, "LOG_THROTTLE_TIMEOUT", 0), this.id = t, this.userData = {}, this._storage = new jo("__probe-".concat(this.id, "__"), Zo), this.timeStamp("".concat(this.id, " started")),
+                    wo(this, "id", void 0), wo(this, "VERSION", Ro), wo(this, "_startTs", Wo()), wo(this, "_deltaTs", Wo()), wo(this, "_storage", void 0), wo(this, "userData", {}), wo(this, "LOG_THROTTLE_TIMEOUT", 0), this.id = t, this.userData = {}, this._storage = new jo("__probe-".concat(this.id, "__"), Zo), this.timeStamp("".concat(this.id, " started")),
                         function(t) {
                             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : ["constructor"];
                             const n = Object.getPrototypeOf(t),
                                 i = Object.getOwnPropertyNames(n);
                             for (const n of i) "function" == typeof t[n] && (e.find((t => n === t)) || (t[n] = t[n].bind(t)))
                         }(this), Object.seal(this)
                 }
@@ -6205,15 +6205,15 @@
                         [t]: e
                     })
                 }
                 settings() {
                     console.table ? console.table(this._storage.config) : console.log(this._storage.config)
                 }
                 assert(t, e) {
-                    Do(t, e)
+                    No(t, e)
                 }
                 warn(t) {
                     return this._getLogFunction(0, t, Ho.warn, arguments, Yo)
                 }
                 error(t) {
                     return this._getLogFunction(0, t, Ho.error, arguments)
                 }
@@ -6236,17 +6236,17 @@
                     return this._getLogFunction(t, e, console.info, arguments)
                 }
                 once(t, e) {
                     for (var n = arguments.length, i = new Array(n > 2 ? n - 2 : 0), r = 2; r < n; r++) i[r - 2] = arguments[r];
                     return this._getLogFunction(t, e, Ho.debug || Ho.info, arguments, Yo)
                 }
                 table(t, e, n) {
-                    return e ? this._getLogFunction(t, e, console.table || qo, n && [n], {
+                    return e ? this._getLogFunction(t, e, console.table || Xo, n && [n], {
                         tag: Qo(e)
-                    }) : qo
+                    }) : Xo
                 }
                 image(t) {
                     let {
                         logLevel: e,
                         priority: n,
                         image: i,
                         message: r = "",
@@ -6259,48 +6259,48 @@
                             scale: i = 1
                         } = t;
                         if ("string" == typeof e) {
                             const t = new Image;
                             return t.onload = () => {
                                 const e = zo(t, n, i);
                                 console.log(...e)
-                            }, t.src = e, qo
+                            }, t.src = e, Xo
                         }
                         const r = e.nodeName || "";
-                        if ("img" === r.toLowerCase()) return console.log(...zo(e, n, i)), qo;
+                        if ("img" === r.toLowerCase()) return console.log(...zo(e, n, i)), Xo;
                         if ("canvas" === r.toLowerCase()) {
                             const t = new Image;
-                            return t.onload = () => console.log(...zo(t, n, i)), t.src = e.toDataURL(), qo
+                            return t.onload = () => console.log(...zo(t, n, i)), t.src = e.toDataURL(), Xo
                         }
-                        return qo
+                        return Xo
                     }({
                         image: i,
                         message: r,
                         scale: s
                     }) : function(t) {
                         let {
                             image: e,
                             message: n = "",
                             scale: i = 1
                         } = t;
-                        return console.warn("removed"), qo
+                        return console.warn("removed"), Xo
                     }({
                         image: i,
                         message: r,
                         scale: s
-                    }) : qo
+                    }) : Xo
                 }
                 time(t, e) {
                     return this._getLogFunction(t, e, console.time ? console.time : console.info)
                 }
                 timeEnd(t, e) {
                     return this._getLogFunction(t, e, console.timeEnd ? console.timeEnd : console.info)
                 }
                 timeStamp(t, e) {
-                    return this._getLogFunction(t, e, console.timeStamp || qo)
+                    return this._getLogFunction(t, e, console.timeStamp || Xo)
                 }
                 group(t, e) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
                         collapsed: !1
                     };
                     const i = Jo({
                             logLevel: t,
@@ -6315,15 +6315,15 @@
                 groupCollapsed(t, e) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
                     return this.group(t, e, Object.assign({}, n, {
                         collapsed: !0
                     }))
                 }
                 groupEnd(t) {
-                    return this._getLogFunction(t, "", console.groupEnd || qo)
+                    return this._getLogFunction(t, "", console.groupEnd || Xo)
                 }
                 withGroup(t, e, n) {
                     this.group(t, e)();
                     try {
                         n()
                     } finally {
                         this.groupEnd(t)()
@@ -6338,19 +6338,19 @@
                 _getLogFunction(t, e, n, i, r) {
                     if (this._shouldLog(t)) {
                         r = Jo({
                             logLevel: t,
                             message: e,
                             args: i,
                             opts: r
-                        }), Do(n = n || r.method), r.total = this.getTotal(), r.delta = this.getDelta(), this._deltaTs = Wo();
+                        }), No(n = n || r.method), r.total = this.getTotal(), r.delta = this.getDelta(), this._deltaTs = Wo();
                         const s = r.tag || r.message;
                         if (r.once) {
-                            if (Xo[s]) return qo;
-                            Xo[s] = Wo()
+                            if (qo[s]) return Xo;
+                            qo[s] = Wo()
                         }
                         return e = function(t, e, n) {
                             if ("string" == typeof e) {
                                 const o = n.time ? function(t) {
                                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 8;
                                     const n = Math.max(e - t.length, 0);
                                     return "".concat(" ".repeat(n)).concat(t)
@@ -6360,15 +6360,15 @@
                                 }(n.total)) : "";
                                 i = e = n.time ? "".concat(t, ": ").concat(o, "  ").concat(e) : "".concat(t, ": ").concat(e), r = n.color, s = n.background, ko || "string" != typeof i || (r && (r = Bo(r), i = "[".concat(r, "m").concat(i, "[39m")), s && (r = Bo(s), i = "[".concat(s + 10, "m").concat(i, "[49m"))), e = i
                             }
                             var i, r, s;
                             return e
                         }(this.id, r.message, r), n.bind(console, e, ...r.args)
                     }
-                    return qo
+                    return Xo
                 }
             }
 
             function $o(t) {
                 if (!t) return 0;
                 let e;
                 switch (typeof t) {
@@ -6377,15 +6377,15 @@
                         break;
                     case "object":
                         e = t.logLevel || t.priority || 0;
                         break;
                     default:
                         return 0
                 }
-                return Do(Number.isFinite(e) && e >= 0), e
+                return No(Number.isFinite(e) && e >= 0), e
             }
 
             function Jo(t) {
                 const {
                     logLevel: e,
                     message: n
                 } = t;
@@ -6398,25 +6398,25 @@
                         void 0 !== n && i.unshift(n), t.message = e;
                         break;
                     case "object":
                         Object.assign(t, e)
                 }
                 "function" == typeof t.message && (t.message = t.message());
                 const r = typeof t.message;
-                return Do("string" === r || "object" === r), Object.assign(t, {
+                return No("string" === r || "object" === r), Object.assign(t, {
                     args: i
                 }, t.opts)
             }
 
             function Qo(t) {
                 for (const e in t)
                     for (const n in t[e]) return n || "untitled";
                 return "empty"
             }
-            wo(Ko, "VERSION", Io);
+            wo(Ko, "VERSION", Ro);
             const ta = new Ko({
                 id: "deck"
             });
             let ea = {};
 
             function na(t, e, n, i) {
                 ta.level > 0 && ea[t] && ea[t].call(null, e, n, i)
@@ -6584,52 +6584,52 @@
                         ...t.options,
                         ...i
                     }
                 }), (null !== (e = t) && void 0 !== e && e.parseTextSync || null !== (n = t) && void 0 !== n && n.parseText) && (t.text = !0), t.text || (t.binary = !0), t
             }
             let wa = "";
             const Ea = {},
-                Pa = /^data:([-\w.]+\/[-\w.+]+)(;|,)/,
-                Sa = /^([-\w.]+\/[-\w.+]+)/;
+                Sa = /^data:([-\w.]+\/[-\w.+]+)(;|,)/,
+                Pa = /^([-\w.]+\/[-\w.+]+)/;
 
             function Ca(t) {
-                const e = Pa.exec(t);
+                const e = Sa.exec(t);
                 return e ? e[1] : ""
             }
             const Ta = /\?.*/;
 
             function Aa(t) {
                 return t.replace(Ta, "")
             }
 
             function Ma(t) {
                 return ga(t) ? t.url : ma(t) ? t.name || "" : "string" == typeof t ? t : ""
             }
 
-            function La(t) {
+            function Oa(t) {
                 if (ga(t)) {
                     const e = t,
                         n = e.headers.get("content-type") || "",
                         i = Aa(e.url);
                     return function(t) {
-                        const e = Sa.exec(t);
+                        const e = Pa.exec(t);
                         return e ? e[1] : t
                     }(n) || Ca(i)
                 }
                 return ma(t) ? t.type || "" : "string" == typeof t ? Ca(t) : ""
             }
-            async function Oa(t) {
+            async function La(t) {
                 if (ga(t)) return t;
                 const e = {},
                     n = function(t) {
                         return ga(t) ? t.headers["content-length"] || -1 : ma(t) ? t.size : "string" == typeof t ? t.length : t instanceof ArrayBuffer || ArrayBuffer.isView(t) ? t.byteLength : -1
                     }(t);
                 n >= 0 && (e["content-length"] = String(n));
                 const i = Ma(t),
-                    r = La(t);
+                    r = Oa(t);
                 r && (e["content-type"] = r);
                 const s = await async function(t) {
                     if ("string" == typeof t) return "data:,".concat(t.slice(0, 5));
                     if (t instanceof Blob) {
                         const e = t.slice(0, 5);
                         return await new Promise((t => {
                             const n = new FileReader;
@@ -6654,33 +6654,33 @@
                 const o = new Response(t, {
                     headers: e
                 });
                 return Object.defineProperty(o, "url", {
                     value: i
                 }), o
             }
-            async function Ra(t, e) {
+            async function Ia(t, e) {
                 if ("string" == typeof t) {
                     t = function(t) {
                         for (const e in Ea)
                             if (t.startsWith(e)) {
                                 const n = Ea[e];
                                 t = t.replace(e, n)
                             } return t.startsWith("http://") || t.startsWith("https://") || (t = "".concat(wa).concat(t)), t
                     }(t);
                     let n = e;
                     return null != e && e.fetch && "function" != typeof(null == e ? void 0 : e.fetch) && (n = e.fetch), await fetch(t, n)
                 }
-                return await Oa(t)
+                return await La(t)
             }
             var ka = n(4155),
-                Ia = n(4155);
+                Ra = n(4155);
 
             function ja() {
-                return !("object" == typeof Ia && "[object process]" === String(Ia) && !Ia.browser) || function(t) {
+                return !("object" == typeof Ra && "[object process]" === String(Ra) && !Ra.browser) || function(t) {
                     if ("undefined" != typeof window && "object" == typeof window.process && "renderer" === window.process.type) return !0;
                     if (void 0 !== ka && "object" == typeof ka.versions && Boolean(ka.versions.electron)) return !0;
                     const e = "object" == typeof navigator && "string" == typeof navigator.userAgent && navigator.userAgent;
                     return !!(e && e.indexOf("Electron") >= 0)
                 }()
             }
             const za = "undefined" != typeof __VERSION__ ? __VERSION__ : "untranspiled source";
@@ -6722,21 +6722,21 @@
                 const r = t.src.replace(/\(/g, "%28").replace(/\)/g, "%29");
                 t.width > i && (n = Math.min(n, i / t.width));
                 const s = t.width * n,
                     o = t.height * n,
                     a = ["font-size:1px;", "padding:".concat(Math.floor(o / 2), "px ").concat(Math.floor(s / 2), "px;"), "line-height:".concat(o, "px;"), "background:url(".concat(r, ");"), "background-size:".concat(s, "px ").concat(o, "px;"), "color:transparent;"].join("");
                 return ["".concat(e, " %c+"), a]
             }
-            let Da;
+            let Na;
             ! function(t) {
                 t[t.BLACK = 30] = "BLACK", t[t.RED = 31] = "RED", t[t.GREEN = 32] = "GREEN", t[t.YELLOW = 33] = "YELLOW", t[t.BLUE = 34] = "BLUE", t[t.MAGENTA = 35] = "MAGENTA", t[t.CYAN = 36] = "CYAN", t[t.WHITE = 37] = "WHITE", t[t.BRIGHT_BLACK = 90] = "BRIGHT_BLACK", t[t.BRIGHT_RED = 91] = "BRIGHT_RED", t[t.BRIGHT_GREEN = 92] = "BRIGHT_GREEN", t[t.BRIGHT_YELLOW = 93] = "BRIGHT_YELLOW", t[t.BRIGHT_BLUE = 94] = "BRIGHT_BLUE", t[t.BRIGHT_MAGENTA = 95] = "BRIGHT_MAGENTA", t[t.BRIGHT_CYAN = 96] = "BRIGHT_CYAN", t[t.BRIGHT_WHITE = 97] = "BRIGHT_WHITE"
-            }(Da || (Da = {}));
+            }(Na || (Na = {}));
 
-            function Na(t) {
-                return "string" != typeof t ? t : (t = t.toUpperCase(), Da[t] || Da.WHITE)
+            function Da(t) {
+                return "string" != typeof t ? t : (t = t.toUpperCase(), Na[t] || Na.WHITE)
             }
 
             function Va(t, e) {
                 if (!t) throw new Error(e || "Assertion failed")
             }
             globalThis.self || globalThis.window || globalThis.global;
             const Ua = globalThis.window || globalThis.self || globalThis.global,
@@ -6762,16 +6762,16 @@
                     error: console.error
                 },
                 Za = {
                     enabled: !0,
                     level: 0
                 };
 
-            function qa() {}
-            const Xa = {},
+            function Xa() {}
+            const qa = {},
                 Ya = {
                     once: !0
                 };
             class Ka {
                 constructor() {
                     let {
                         id: t
@@ -6866,17 +6866,17 @@
                 info(t, e) {
                     return this._getLogFunction(t, e, console.info, arguments)
                 }
                 once(t, e) {
                     return this._getLogFunction(t, e, Ha.debug || Ha.info, arguments, Ya)
                 }
                 table(t, e, n) {
-                    return e ? this._getLogFunction(t, e, console.table || qa, n && [n], {
+                    return e ? this._getLogFunction(t, e, console.table || Xa, n && [n], {
                         tag: Qa(e)
-                    }) : qa
+                    }) : Xa
                 }
                 image(t) {
                     let {
                         logLevel: e,
                         priority: n,
                         image: i,
                         message: r = "",
@@ -6889,48 +6889,48 @@
                             scale: i = 1
                         } = t;
                         if ("string" == typeof e) {
                             const t = new Image;
                             return t.onload = () => {
                                 const e = Ba(t, n, i);
                                 console.log(...e)
-                            }, t.src = e, qa
+                            }, t.src = e, Xa
                         }
                         const r = e.nodeName || "";
-                        if ("img" === r.toLowerCase()) return console.log(...Ba(e, n, i)), qa;
+                        if ("img" === r.toLowerCase()) return console.log(...Ba(e, n, i)), Xa;
                         if ("canvas" === r.toLowerCase()) {
                             const t = new Image;
-                            return t.onload = () => console.log(...Ba(t, n, i)), t.src = e.toDataURL(), qa
+                            return t.onload = () => console.log(...Ba(t, n, i)), t.src = e.toDataURL(), Xa
                         }
-                        return qa
+                        return Xa
                     }({
                         image: i,
                         message: r,
                         scale: s
                     }) : function(t) {
                         let {
                             image: e,
                             message: n = "",
                             scale: i = 1
                         } = t;
-                        return console.warn("removed"), qa
+                        return console.warn("removed"), Xa
                     }({
                         image: i,
                         message: r,
                         scale: s
-                    }) : qa
+                    }) : Xa
                 }
                 time(t, e) {
                     return this._getLogFunction(t, e, console.time ? console.time : console.info)
                 }
                 timeEnd(t, e) {
                     return this._getLogFunction(t, e, console.timeEnd ? console.timeEnd : console.info)
                 }
                 timeStamp(t, e) {
-                    return this._getLogFunction(t, e, console.timeStamp || qa)
+                    return this._getLogFunction(t, e, console.timeStamp || Xa)
                 }
                 group(t, e) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
                         collapsed: !1
                     };
                     const i = Ja({
                             logLevel: t,
@@ -6945,15 +6945,15 @@
                 groupCollapsed(t, e) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
                     return this.group(t, e, Object.assign({}, n, {
                         collapsed: !0
                     }))
                 }
                 groupEnd(t) {
-                    return this._getLogFunction(t, "", console.groupEnd || qa)
+                    return this._getLogFunction(t, "", console.groupEnd || Xa)
                 }
                 withGroup(t, e, n) {
                     this.group(t, e)();
                     try {
                         n()
                     } finally {
                         this.groupEnd(t)()
@@ -6971,45 +6971,45 @@
                             logLevel: t,
                             message: e,
                             args: i,
                             opts: r
                         }), Va(n = n || r.method), r.total = this.getTotal(), r.delta = this.getDelta(), this._deltaTs = Wa();
                         const s = r.tag || r.message;
                         if (r.once && s) {
-                            if (Xa[s]) return qa;
-                            Xa[s] = Wa()
+                            if (qa[s]) return Xa;
+                            qa[s] = Wa()
                         }
                         return e = function(t, e, n) {
                             if ("string" == typeof e) {
                                 const i = n.time ? function(t) {
                                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 8;
                                     const n = Math.max(e - t.length, 0);
                                     return "".concat(" ".repeat(n)).concat(t)
                                 }(function(t) {
                                     let e;
                                     return e = t < 10 ? "".concat(t.toFixed(2), "ms") : t < 100 ? "".concat(t.toFixed(1), "ms") : t < 1e3 ? "".concat(t.toFixed(0), "ms") : "".concat((t / 1e3).toFixed(2), "s"), e
                                 }(n.total)) : "";
                                 e = function(t, e, n) {
                                     if (!ja && "string" == typeof t) {
                                         if (e) {
-                                            const n = Na(e);
+                                            const n = Da(e);
                                             t = "[".concat(n, "m").concat(t, "[39m")
                                         }
                                         if (n) {
-                                            const e = Na(n);
+                                            const e = Da(n);
                                             t = "[".concat(e + 10, "m").concat(t, "[49m")
                                         }
                                     }
                                     return t
                                 }(e = n.time ? "".concat(t, ": ").concat(i, "  ").concat(e) : "".concat(t, ": ").concat(e), n.color, n.background)
                             }
                             return e
                         }(this.id, r.message, r), n.bind(console, e, ...r.args)
                     }
-                    return qa
+                    return Xa
                 }
             }
 
             function $a(t) {
                 if (!t) return 0;
                 let e;
                 switch (typeof t) {
@@ -7203,15 +7203,15 @@
                         } : t[n] = e[n]
                     }
             }
 
             function pl(t, e) {
                 const n = ll(),
                     i = t || n;
-                return "function" == typeof i.fetch ? i.fetch : ua(i.fetch) ? t => Ra(t, i) : null != e && e.fetch ? null == e ? void 0 : e.fetch : Ra
+                return "function" == typeof i.fetch ? i.fetch : ua(i.fetch) ? t => Ia(t, i) : null != e && e.fetch ? null == e ? void 0 : e.fetch : Ia
             }
 
             function fl(t, e) {
                 if (!t) throw new Error(e || "loaders.gl assertion failed.")
             }
             var gl = n(4155);
             "undefined" != typeof self && self, "undefined" != typeof window && window, void 0 !== n.g && n.g, "undefined" != typeof document && document;
@@ -7243,30 +7243,30 @@
                     for (const n in t) wl(t[n], e, i);
                 return void 0 === n ? Array.from(i) : []
             }
 
             function El(t) {
                 return !!t && (t instanceof ArrayBuffer || "undefined" != typeof MessagePort && t instanceof MessagePort || "undefined" != typeof ImageBitmap && t instanceof ImageBitmap || "undefined" != typeof OffscreenCanvas && t instanceof OffscreenCanvas)
             }
-            const Pl = () => {};
-            class Sl {
+            const Sl = () => {};
+            class Pl {
                 static isSupported() {
                     return "undefined" != typeof Worker && ml || void 0 !== yl && !ml
                 }
                 constructor(t) {
                     wo(this, "name", void 0), wo(this, "source", void 0), wo(this, "url", void 0), wo(this, "terminated", !1), wo(this, "worker", void 0), wo(this, "onMessage", void 0), wo(this, "onError", void 0), wo(this, "_loadableURL", "");
                     const {
                         name: e,
                         source: n,
                         url: i
                     } = t;
-                    fl(n || i), this.name = e, this.source = n, this.url = i, this.onMessage = Pl, this.onError = t => console.log(t), this.worker = ml ? this._createBrowserWorker() : this._createNodeWorker()
+                    fl(n || i), this.name = e, this.source = n, this.url = i, this.onMessage = Sl, this.onError = t => console.log(t), this.worker = ml ? this._createBrowserWorker() : this._createNodeWorker()
                 }
                 destroy() {
-                    this.onMessage = Pl, this.onError = Pl, this.worker.terminate(), this.terminated = !0
+                    this.onMessage = Sl, this.onError = Sl, this.worker.terminate(), this.terminated = !0
                 }
                 get isRunning() {
                     return Boolean(this.onMessage)
                 }
                 postMessage(t, e) {
                     e = e || wl(t), this.worker.postMessage(t, e)
                 }
@@ -7331,15 +7331,15 @@
                 }
                 error(t) {
                     fl(this.isRunning), this.isRunning = !1, this._reject(t)
                 }
             }
             class Tl {
                 static isSupported() {
-                    return Sl.isSupported()
+                    return Pl.isSupported()
                 }
                 constructor(t) {
                     wo(this, "name", "unnamed"), wo(this, "source", void 0), wo(this, "url", void 0), wo(this, "maxConcurrency", 1), wo(this, "maxMobileConcurrency", 1), wo(this, "onDebug", (() => {})), wo(this, "reuseWorkers", !0), wo(this, "props", {}), wo(this, "jobQueue", []), wo(this, "idleQueue", []), wo(this, "count", 0), wo(this, "isDestroyed", !1), this.source = t.source, this.url = t.url, this.setProps(t)
                 }
                 destroy() {
                     this.idleQueue.forEach((t => t.destroy())), this.isDestroyed = !0
                 }
@@ -7385,15 +7385,15 @@
                     this.isDestroyed || !this.reuseWorkers || this.count > this._getMaxConcurrency() ? (t.destroy(), this.count--) : this.idleQueue.push(t), this.isDestroyed || this._startQueuedJob()
                 }
                 _getAvailableWorker() {
                     if (this.idleQueue.length > 0) return this.idleQueue.shift() || null;
                     if (this.count < this._getMaxConcurrency()) {
                         this.count++;
                         const t = "".concat(this.name.toLowerCase(), " (#").concat(this.count, " of ").concat(this.maxConcurrency, ")");
-                        return new Sl({
+                        return new Pl({
                             name: t,
                             source: this.source,
                             url: this.url
                         })
                     }
                     return null
                 }
@@ -7405,15 +7405,15 @@
                 maxConcurrency: 3,
                 maxMobileConcurrency: 1,
                 reuseWorkers: !0,
                 onDebug: () => {}
             };
             class Ml {
                 static isSupported() {
-                    return Sl.isSupported()
+                    return Pl.isSupported()
                 }
                 static getWorkerFarm() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return Ml._workerFarm = Ml._workerFarm || new Ml({}), Ml._workerFarm.setProps(t), Ml._workerFarm
                 }
                 constructor(t) {
                     wo(this, "props", void 0), wo(this, "workerPools", new Map), this.props = {
@@ -7450,45 +7450,45 @@
                         maxMobileConcurrency: this.props.maxMobileConcurrency,
                         reuseWorkers: this.props.reuseWorkers,
                         onDebug: this.props.onDebug
                     }
                 }
             }
             wo(Ml, "_workerFarm", void 0);
-            const Ll = "latest";
-            async function Ol(t, e, n, i, r) {
+            const Ol = "latest";
+            async function Ll(t, e, n, i, r) {
                 const s = t.id,
                     o = function(t) {
                         let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                         const n = e[t.id] || {},
                             i = "".concat(t.id, "-worker.js");
                         let r = n.workerUrl;
                         if (r || "compression" !== t.id || (r = e.workerUrl), "test" === e._workerType && (r = "modules/".concat(t.module, "/dist/").concat(i)), !r) {
                             let e = t.version;
-                            "latest" === e && (e = Ll);
+                            "latest" === e && (e = Ol);
                             const n = e ? "@".concat(e) : "";
                             r = "https://unpkg.com/@loaders.gl/".concat(t.module).concat(n, "/dist/").concat(i)
                         }
                         return fl(r), r
                     }(t, n),
                     a = Ml.getWorkerFarm(n).getWorkerPool({
                         name: s,
                         url: o
                     });
                 n = JSON.parse(JSON.stringify(n)), i = JSON.parse(JSON.stringify(i || {}));
-                const l = await a.startJob("process-on-worker", Rl.bind(null, r));
+                const l = await a.startJob("process-on-worker", Il.bind(null, r));
                 l.postMessage("process", {
                     input: e,
                     options: n,
                     context: i
                 });
                 const c = await l.result;
                 return await c.result
             }
-            async function Rl(t, e, n, i) {
+            async function Il(t, e, n, i) {
                 switch (n) {
                     case "done":
                         e.done(i);
                         break;
                     case "error":
                         e.error(new Error(i.error));
                         break;
@@ -7511,15 +7511,15 @@
                         }
                         break;
                     default:
                         console.warn("parse-with-worker unknown message ".concat(n))
                 }
             }
             const kl = 262144,
-                Il = 262144,
+                Rl = 262144,
                 jl = 1048576;
 
             function zl(t) {
                 if ((e = t) && "object" == typeof e && e.isBuffer) return t;
                 var e;
                 if (t instanceof ArrayBuffer) return t;
                 if (ArrayBuffer.isView(t)) return 0 === t.byteOffset && t.byteLength === t.buffer.byteLength ? t.buffer : t.buffer.slice(t.byteOffset, t.byteOffset + t.byteLength);
@@ -7550,15 +7550,15 @@
                         n.releaseLock()
                     }
                 }(t, e): async function*(t, e) {
                     for await (const e of t) yield zl(e)
                 }(t)
             }
             const Bl = "Cannot convert supplied data type";
-            async function Dl(t, e, n) {
+            async function Nl(t, e, n) {
                 const i = t instanceof ArrayBuffer || ArrayBuffer.isView(t);
                 if ("string" == typeof t || i) return function(t, e, n) {
                     if (e.text && "string" == typeof t) return t;
                     if (va(t) && (t = t.buffer), t instanceof ArrayBuffer) {
                         const n = t;
                         return e.text && !e.binary ? new TextDecoder("utf8").decode(n) : n
                     }
@@ -7566,15 +7566,15 @@
                         if (e.text && !e.binary) return new TextDecoder("utf8").decode(t);
                         let n = t.buffer;
                         const i = t.byteLength || t.length;
                         return 0 === t.byteOffset && i === n.byteLength || (n = n.slice(t.byteOffset, t.byteOffset + i)), n
                     }
                     throw new Error(Bl)
                 }(t, e);
-                if (ma(t) && (t = await Oa(t)), ga(t)) {
+                if (ma(t) && (t = await La(t)), ga(t)) {
                     const n = t;
                     return await async function(t) {
                         if (!t.ok) {
                             const e = await async function(t) {
                                 let e = "Failed to fetch resource ".concat(t.url, " (").concat(t.status, "): ");
                                 try {
                                     const n = t.headers.get("Content-Type");
@@ -7598,15 +7598,15 @@
                                 i += e, yield r.encode(s)
                             }
                         }(t, e);
                         if (t instanceof ArrayBuffer) return function(t) {
                             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                             return function*() {
                                 const {
-                                    chunkSize: n = Il
+                                    chunkSize: n = Rl
                                 } = e;
                                 let i = 0;
                                 for (; i < t.byteLength;) {
                                     const e = Math.min(t.byteLength - i, n),
                                         r = new ArrayBuffer(e),
                                         s = new Uint8Array(t, i, e);
                                     new Uint8Array(r).set(s), i += e, yield r
@@ -7637,15 +7637,15 @@
                         for (const t of i) s.set(t, o), o += t.byteLength;
                         return s.buffer
                     }(...e)
                 }(t);
                 throw new Error(Bl)
             }
 
-            function Nl(t) {
+            function Dl(t) {
                 const e = t ? t.lastIndexOf("/") : -1;
                 return e >= 0 ? t.substr(e + 1) : ""
             }
             const Vl = new Ka({
                     id: "loaders.gl"
                 }),
                 Ul = () => {
@@ -7663,66 +7663,66 @@
                 let r = [];
                 e && (r = r.concat(e)), null != n && n.ignoreRegisteredLoaders || r.push(...Ul()),
                     function(t) {
                         for (const e of t) xa(e)
                     }(r);
                 const s = function(t, e, n, i) {
                     const r = Ma(t),
-                        s = La(t),
+                        s = Oa(t),
                         o = Aa(r) || (null == i ? void 0 : i.url);
                     let a = null,
                         l = "";
                     var c;
-                    return null != n && n.mimeType && (a = ql(e, null == n ? void 0 : n.mimeType), l = "match forced by supplied MIME type ".concat(null == n ? void 0 : n.mimeType)), a = a || function(t, e) {
+                    return null != n && n.mimeType && (a = Xl(e, null == n ? void 0 : n.mimeType), l = "match forced by supplied MIME type ".concat(null == n ? void 0 : n.mimeType)), a = a || function(t, e) {
                         const n = e && Gl.exec(e),
                             i = n && n[1];
                         return i ? function(t, e) {
                             e = e.toLowerCase();
                             for (const n of t)
                                 for (const t of n.extensions)
                                     if (t.toLowerCase() === e) return n;
                             return null
                         }(t, i) : null
-                    }(e, o), l = l || (a ? "matched url ".concat(o) : ""), a = a || ql(e, s), l = l || (a ? "matched MIME type ".concat(s) : ""), a = a || function(t, e) {
+                    }(e, o), l = l || (a ? "matched url ".concat(o) : ""), a = a || Xl(e, s), l = l || (a ? "matched MIME type ".concat(s) : ""), a = a || function(t, e) {
                         if (!e) return null;
                         for (const n of t)
                             if ("string" == typeof e) {
-                                if (Xl(e, n)) return n
+                                if (ql(e, n)) return n
                             } else if (ArrayBuffer.isView(e)) {
                             if (Yl(e.buffer, e.byteOffset, n)) return n
                         } else if (e instanceof ArrayBuffer && Yl(e, 0, n)) return n;
                         return null
-                    }(e, t), l = l || (a ? "matched initial data ".concat(Kl(t)) : ""), a = a || ql(e, null == n ? void 0 : n.fallbackMimeType), l = l || (a ? "matched fallback MIME type ".concat(s) : ""), l && Vl.log(1, "selectLoader selected ".concat(null === (c = a) || void 0 === c ? void 0 : c.name, ": ").concat(l, ".")), a
+                    }(e, t), l = l || (a ? "matched initial data ".concat(Kl(t)) : ""), a = a || Xl(e, null == n ? void 0 : n.fallbackMimeType), l = l || (a ? "matched fallback MIME type ".concat(s) : ""), l && Vl.log(1, "selectLoader selected ".concat(null === (c = a) || void 0 === c ? void 0 : c.name, ": ").concat(l, ".")), a
                 }(t, r, n, i);
                 if (!(s || null != n && n.nothrow)) throw new Error(Zl(t));
                 return s
             }
 
             function Hl(t) {
                 return !(t instanceof Response && 204 === t.status)
             }
 
             function Zl(t) {
                 const e = Ma(t),
-                    n = La(t);
+                    n = Oa(t);
                 let i = "No valid loader found (";
-                i += e ? "".concat(Nl(e), ", ") : "no url provided, ", i += "MIME type: ".concat(n ? '"'.concat(n, '"') : "not provided", ", ");
+                i += e ? "".concat(Dl(e), ", ") : "no url provided, ", i += "MIME type: ".concat(n ? '"'.concat(n, '"') : "not provided", ", ");
                 const r = t ? Kl(t) : "";
                 return i += r ? ' first bytes: "'.concat(r, '"') : "first bytes: not available", i += ")", i
             }
 
-            function ql(t, e) {
+            function Xl(t, e) {
                 for (const n of t) {
                     if (n.mimeTypes && n.mimeTypes.includes(e)) return n;
                     if (e === "application/x.".concat(n.id)) return n
                 }
                 return null
             }
 
-            function Xl(t, e) {
+            function ql(t, e) {
                 return e.testText ? e.testText(t) : (Array.isArray(e.tests) ? e.tests : [e.tests]).some((e => t.startsWith(e)))
             }
 
             function Yl(t, e, n) {
                 return (Array.isArray(n.tests) ? n.tests : [n.tests]).some((i => function(t, e, n, i) {
                     if (i instanceof ArrayBuffer) return function(t, e, n) {
                         if (n = n || t.byteLength, t.byteLength < n || e.byteLength < n) return !1;
@@ -7787,15 +7787,15 @@
                         ...t
                     };
                     if (i.url) {
                         const t = Aa(i.url);
                         i.baseUrl = t, i.queryString = function(t) {
                             const e = t.match(Ta);
                             return e && e[0]
-                        }(i.url), i.filename = Nl(t), i.baseUrl = function(t) {
+                        }(i.url), i.filename = Dl(t), i.baseUrl = function(t) {
                             const e = t ? t.lastIndexOf("/") : -1;
                             return e >= 0 ? t.substr(0, e) : ""
                         }(t)
                     }
                     return Array.isArray(i.loaders) || (i.loaders = null), i
                 }({
                     url: r,
@@ -7822,18 +7822,18 @@
                             redirected: r,
                             status: s,
                             statusText: o,
                             type: a,
                             url: l
                         }
                     }
-                    if (e = await Dl(e, t, n), t.parseTextSync && "string" == typeof e) return n.dataType = "text", t.parseTextSync(e, n, i, t);
+                    if (e = await Nl(e, t, n), t.parseTextSync && "string" == typeof e) return n.dataType = "text", t.parseTextSync(e, n, i, t);
                     if (function(t, e) {
                             return !!Ml.isSupported() && !!(ml || null != e && e._nodeWorkers) && t.worker && (null == e ? void 0 : e.worker)
-                        }(t, n)) return await Ol(t, e, n, i, Jl);
+                        }(t, n)) return await Ll(t, e, n, i, Jl);
                     if (t.parseText && "string" == typeof e) return await t.parseText(e, n, i, t);
                     if (t.parse) return await t.parse(e, n, i, t);
                     throw fl(!t.parseSync), new Error("".concat(t.id, " loader - no parser found and worker is disabled"))
                 }(o, t, n, i)) : null
             }
             async function Ql(t, e, n, i) {
                 Array.isArray(e) || _a(e) || (n = e, e = void 0);
@@ -8369,21 +8369,21 @@
             Math.random, Math.PI, Math.hypot || (Math.hypot = function() {
                 for (var t = 0, e = arguments.length; e--;) t += arguments[e] * arguments[e];
                 return Math.sqrt(t)
             });
             var Ec = function(t, e, n) {
                     return t[0] = e[0] - n[0], t[1] = e[1] - n[1], t[2] = e[2] - n[2], t
                 },
-                Pc = function(t) {
+                Sc = function(t) {
                     var e = t[0],
                         n = t[1],
                         i = t[2];
                     return Math.hypot(e, n, i)
                 },
-                Sc = function(t) {
+                Pc = function(t) {
                     var e = t[0],
                         n = t[1],
                         i = t[2];
                     return e * e + n * n + i * i
                 };
 
             function Cc(t, e, n) {
@@ -8399,17 +8399,17 @@
                     r = e[1],
                     s = e[2];
                 return t[0] = n[0] * i + n[3] * r + n[6] * s, t[1] = n[1] * i + n[4] * r + n[7] * s, t[2] = n[2] * i + n[5] * r + n[8] * s, t[3] = e[3], t
             }
             mc();
             const Ac = [0, 0, 0];
             let Mc;
-            class Lc extends pc {
+            class Oc extends pc {
                 static get ZERO() {
-                    return Mc || (Mc = new Lc(0, 0, 0), Object.freeze(Mc)), Mc
+                    return Mc || (Mc = new Oc(0, 0, 0), Object.freeze(Mc)), Mc
                 }
                 constructor(t = 0, e = 0, n = 0) {
                     super(-0, -0, -0), 1 === arguments.length && sc(t) ? this.copy(t) : (ic.debug && (hc(t), hc(e), hc(n)), this[0] = t, this[1] = e, this[2] = n)
                 }
                 set(t, e, n) {
                     return this[0] = t, this[1] = e, this[2] = n, this.check()
                 }
@@ -8478,27 +8478,27 @@
                         t[0] = n[0] * i + n[2] * r, t[1] = n[1] * i + n[3] * r, t[2] = e[2]
                     }(this, this, t), this.check()
                 }
                 transformByQuaternion(t) {
                     return wc(this, this, t), this.check()
                 }
             }
-            const Oc = new Lc;
+            const Lc = new Oc;
 
-            function Rc(t, e, n, i) {
-                Oc.set(t, e, n);
-                const r = Oc.len();
+            function Ic(t, e, n, i) {
+                Lc.set(t, e, n);
+                const r = Lc.len();
                 return {
                     distance: i / r,
-                    normal: new Lc(-t / r, -e / r, -n / r)
+                    normal: new Oc(-t / r, -e / r, -n / r)
                 }
             }
             let kc;
 
-            function Ic(t, e) {
+            function Rc(t, e) {
                 const {
                     size: n = 1,
                     startIndex: i = 0
                 } = e, r = void 0 !== e.endIndex ? e.endIndex : t.length, s = (r - i) / n;
                 kc = nc.allocate(kc, s, {
                     type: Float32Array,
                     size: 2 * n
@@ -8568,22 +8568,22 @@
                     v = e[15],
                     b = n * a - i * o,
                     y = n * l - r * o,
                     _ = n * c - s * o,
                     x = i * l - r * a,
                     w = i * c - s * a,
                     E = r * c - s * l,
-                    P = h * g - u * f,
-                    S = h * m - d * f,
+                    S = h * g - u * f,
+                    P = h * m - d * f,
                     C = h * v - p * f,
                     T = u * m - d * g,
                     A = u * v - p * g,
                     M = d * v - p * m,
-                    L = b * M - y * A + _ * T + x * C - w * S + E * P;
-                return L ? (L = 1 / L, t[0] = (a * M - l * A + c * T) * L, t[1] = (r * A - i * M - s * T) * L, t[2] = (g * E - m * w + v * x) * L, t[3] = (d * w - u * E - p * x) * L, t[4] = (l * C - o * M - c * S) * L, t[5] = (n * M - r * C + s * S) * L, t[6] = (m * _ - f * E - v * y) * L, t[7] = (h * E - d * _ + p * y) * L, t[8] = (o * A - a * C + c * P) * L, t[9] = (i * C - n * A - s * P) * L, t[10] = (f * w - g * _ + v * b) * L, t[11] = (u * _ - h * w - p * b) * L, t[12] = (a * S - o * T - l * P) * L, t[13] = (n * T - i * S + r * P) * L, t[14] = (g * y - f * x - m * b) * L, t[15] = (h * x - u * y + d * b) * L, t) : null
+                    O = b * M - y * A + _ * T + x * C - w * P + E * S;
+                return O ? (O = 1 / O, t[0] = (a * M - l * A + c * T) * O, t[1] = (r * A - i * M - s * T) * O, t[2] = (g * E - m * w + v * x) * O, t[3] = (d * w - u * E - p * x) * O, t[4] = (l * C - o * M - c * P) * O, t[5] = (n * M - r * C + s * P) * O, t[6] = (m * _ - f * E - v * y) * O, t[7] = (h * E - d * _ + p * y) * O, t[8] = (o * A - a * C + c * S) * O, t[9] = (i * C - n * A - s * S) * O, t[10] = (f * w - g * _ + v * b) * O, t[11] = (u * _ - h * w - p * b) * O, t[12] = (a * P - o * T - l * S) * O, t[13] = (n * T - i * P + r * S) * O, t[14] = (g * y - f * x - m * b) * O, t[15] = (h * x - u * y + d * b) * O, t) : null
             }
 
             function Fc(t, e, n) {
                 var i = e[0],
                     r = e[1],
                     s = e[2],
                     o = e[3],
@@ -8609,22 +8609,22 @@
             function Bc(t, e, n) {
                 var i, r, s, o, a, l, c, h, u, d, p, f, g = n[0],
                     m = n[1],
                     v = n[2];
                 return e === t ? (t[12] = e[0] * g + e[4] * m + e[8] * v + e[12], t[13] = e[1] * g + e[5] * m + e[9] * v + e[13], t[14] = e[2] * g + e[6] * m + e[10] * v + e[14], t[15] = e[3] * g + e[7] * m + e[11] * v + e[15]) : (i = e[0], r = e[1], s = e[2], o = e[3], a = e[4], l = e[5], c = e[6], h = e[7], u = e[8], d = e[9], p = e[10], f = e[11], t[0] = i, t[1] = r, t[2] = s, t[3] = o, t[4] = a, t[5] = l, t[6] = c, t[7] = h, t[8] = u, t[9] = d, t[10] = p, t[11] = f, t[12] = i * g + a * m + u * v + e[12], t[13] = r * g + l * m + d * v + e[13], t[14] = s * g + c * m + p * v + e[14], t[15] = o * g + h * m + f * v + e[15]), t
             }
 
-            function Dc(t, e, n) {
+            function Nc(t, e, n) {
                 var i = n[0],
                     r = n[1],
                     s = n[2];
                 return t[0] = e[0] * i, t[1] = e[1] * i, t[2] = e[2] * i, t[3] = e[3] * i, t[4] = e[4] * r, t[5] = e[5] * r, t[6] = e[6] * r, t[7] = e[7] * r, t[8] = e[8] * s, t[9] = e[9] * s, t[10] = e[10] * s, t[11] = e[11] * s, t[12] = e[12], t[13] = e[13], t[14] = e[14], t[15] = e[15], t
             }
 
-            function Nc(t, e, n) {
+            function Dc(t, e, n) {
                 var i = Math.sin(n),
                     r = Math.cos(n),
                     s = e[4],
                     o = e[5],
                     a = e[6],
                     l = e[7],
                     c = e[8],
@@ -8663,15 +8663,15 @@
                 return t[0] = r + i * (n[0] - r), t[1] = s + i * (n[1] - s), t
             }
 
             function Zc(t, e, n) {
                 return t[0] = e[0] * n, t[1] = e[1] * n, t[2] = e[2] * n, t[3] = e[3] * n, t
             }
 
-            function qc(t, e, n) {
+            function Xc(t, e, n) {
                 var i = e[0],
                     r = e[1],
                     s = e[2],
                     o = e[3];
                 return t[0] = n[0] * i + n[4] * r + n[8] * s + n[12] * o, t[1] = n[1] * i + n[5] * r + n[9] * s + n[13] * o, t[2] = n[2] * i + n[6] * r + n[10] * s + n[14] * o, t[3] = n[3] * i + n[7] * r + n[11] * s + n[15] * o, t
             }! function() {
                 var t;
@@ -8680,15 +8680,15 @@
             function() {
                 var t;
                 t = new gc(4), gc != Float32Array && (t[0] = 0, t[1] = 0, t[2] = 0, t[3] = 0)
             }(),
             function(t) {
                 t[t.COL0ROW0 = 0] = "COL0ROW0", t[t.COL0ROW1 = 1] = "COL0ROW1", t[t.COL0ROW2 = 2] = "COL0ROW2", t[t.COL0ROW3 = 3] = "COL0ROW3", t[t.COL1ROW0 = 4] = "COL1ROW0", t[t.COL1ROW1 = 5] = "COL1ROW1", t[t.COL1ROW2 = 6] = "COL1ROW2", t[t.COL1ROW3 = 7] = "COL1ROW3", t[t.COL2ROW0 = 8] = "COL2ROW0", t[t.COL2ROW1 = 9] = "COL2ROW1", t[t.COL2ROW2 = 10] = "COL2ROW2", t[t.COL2ROW3 = 11] = "COL2ROW3", t[t.COL3ROW0 = 12] = "COL3ROW0", t[t.COL3ROW1 = 13] = "COL3ROW1", t[t.COL3ROW2 = 14] = "COL3ROW2", t[t.COL3ROW3 = 15] = "COL3ROW3"
             }(Uc || (Uc = {}));
-            const Xc = 45 * Math.PI / 180,
+            const qc = 45 * Math.PI / 180,
                 Yc = 1,
                 Kc = .1,
                 $c = 500,
                 Jc = Object.freeze([1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1]);
             class Qc extends jc {
                 static get IDENTITY() {
                     return eh || (eh = new Qc, Object.freeze(eh)), eh
@@ -8788,15 +8788,15 @@
                             l = 1 / (i - r),
                             c = 1 / (s - o);
                         t[0] = -2 * a, t[1] = 0, t[2] = 0, t[3] = 0, t[4] = 0, t[5] = -2 * l, t[6] = 0, t[7] = 0, t[8] = 0, t[9] = 0, t[10] = 2 * c, t[11] = 0, t[12] = (e + n) * a, t[13] = (r + i) * l, t[14] = (o + s) * c, t[15] = 1
                     }(this, e, n, i, r, s, o), this.check()
                 }
                 orthographic(t) {
                     const {
-                        fovy: e = Xc,
+                        fovy: e = qc,
                         aspect: n = Yc,
                         focalDistance: i = 1,
                         near: r = Kc,
                         far: s = $c
                     } = t;
                     nh(e);
                     const o = e / 2,
@@ -8869,43 +8869,43 @@
                 multiplyLeft(t) {
                     return Fc(this, t, this), this.check()
                 }
                 multiplyRight(t) {
                     return Fc(this, this, t), this.check()
                 }
                 rotateX(t) {
-                    return Nc(this, this, t), this.check()
+                    return Dc(this, this, t), this.check()
                 }
                 rotateY(t) {
                     var e, n, i, r, s, o, a, l, c, h, u, d, p;
                     return e = this, n = this, i = t, r = Math.sin(i), s = Math.cos(i), o = n[0], a = n[1], l = n[2], c = n[3], h = n[8], u = n[9], d = n[10], p = n[11], n !== e && (e[4] = n[4], e[5] = n[5], e[6] = n[6], e[7] = n[7], e[12] = n[12], e[13] = n[13], e[14] = n[14], e[15] = n[15]), e[0] = o * s - h * r, e[1] = a * s - u * r, e[2] = l * s - d * r, e[3] = c * s - p * r, e[8] = o * r + h * s, e[9] = a * r + u * s, e[10] = l * r + d * s, e[11] = c * r + p * s, this.check()
                 }
                 rotateZ(t) {
                     return Vc(this, this, t), this.check()
                 }
                 rotateXYZ(t) {
                     return this.rotateX(t[0]).rotateY(t[1]).rotateZ(t[2])
                 }
                 rotateAxis(t, e) {
                     return function(t, e, n, i) {
-                        var r, s, o, a, l, c, h, u, d, p, f, g, m, v, b, y, _, x, w, E, P, S, C, T, A = i[0],
+                        var r, s, o, a, l, c, h, u, d, p, f, g, m, v, b, y, _, x, w, E, S, P, C, T, A = i[0],
                             M = i[1],
-                            L = i[2],
-                            O = Math.hypot(A, M, L);
-                        O < fc || (A *= O = 1 / O, M *= O, L *= O, r = Math.sin(n), o = 1 - (s = Math.cos(n)), a = e[0], l = e[1], c = e[2], h = e[3], u = e[4], d = e[5], p = e[6], f = e[7], g = e[8], m = e[9], v = e[10], b = e[11], y = A * A * o + s, _ = M * A * o + L * r, x = L * A * o - M * r, w = A * M * o - L * r, E = M * M * o + s, P = L * M * o + A * r, S = A * L * o + M * r, C = M * L * o - A * r, T = L * L * o + s, t[0] = a * y + u * _ + g * x, t[1] = l * y + d * _ + m * x, t[2] = c * y + p * _ + v * x, t[3] = h * y + f * _ + b * x, t[4] = a * w + u * E + g * P, t[5] = l * w + d * E + m * P, t[6] = c * w + p * E + v * P, t[7] = h * w + f * E + b * P, t[8] = a * S + u * C + g * T, t[9] = l * S + d * C + m * T, t[10] = c * S + p * C + v * T, t[11] = h * S + f * C + b * T, e !== t && (t[12] = e[12], t[13] = e[13], t[14] = e[14], t[15] = e[15]))
+                            O = i[2],
+                            L = Math.hypot(A, M, O);
+                        L < fc || (A *= L = 1 / L, M *= L, O *= L, r = Math.sin(n), o = 1 - (s = Math.cos(n)), a = e[0], l = e[1], c = e[2], h = e[3], u = e[4], d = e[5], p = e[6], f = e[7], g = e[8], m = e[9], v = e[10], b = e[11], y = A * A * o + s, _ = M * A * o + O * r, x = O * A * o - M * r, w = A * M * o - O * r, E = M * M * o + s, S = O * M * o + A * r, P = A * O * o + M * r, C = M * O * o - A * r, T = O * O * o + s, t[0] = a * y + u * _ + g * x, t[1] = l * y + d * _ + m * x, t[2] = c * y + p * _ + v * x, t[3] = h * y + f * _ + b * x, t[4] = a * w + u * E + g * S, t[5] = l * w + d * E + m * S, t[6] = c * w + p * E + v * S, t[7] = h * w + f * E + b * S, t[8] = a * P + u * C + g * T, t[9] = l * P + d * C + m * T, t[10] = c * P + p * C + v * T, t[11] = h * P + f * C + b * T, e !== t && (t[12] = e[12], t[13] = e[13], t[14] = e[14], t[15] = e[15]))
                     }(this, this, t, e), this.check()
                 }
                 scale(t) {
-                    return Dc(this, this, Array.isArray(t) ? t : [t, t, t]), this.check()
+                    return Nc(this, this, Array.isArray(t) ? t : [t, t, t]), this.check()
                 }
                 translate(t) {
                     return Bc(this, this, t), this.check()
                 }
                 transform(t, e) {
-                    return 4 === t.length ? (uc(e = qc(e || [-0, -0, -0, -0], t, this), 4), e) : this.transformAsPoint(t, e)
+                    return 4 === t.length ? (uc(e = Xc(e || [-0, -0, -0, -0], t, this), 4), e) : this.transformAsPoint(t, e)
                 }
                 transformAsPoint(t, e) {
                     const {
                         length: n
                     } = t;
                     let i;
                     switch (n) {
@@ -8962,15 +8962,15 @@
             let th, eh;
 
             function nh(t) {
                 if (t > 2 * Math.PI) throw Error("expected radians")
             }
 
             function ih(t, e) {
-                const n = qc([], e, t);
+                const n = Xc([], e, t);
                 return Zc(n, n, 1 / n[3]), n
             }
 
             function rh(t, e) {
                 const n = t % e;
                 return n < 0 ? e + n : n
             }
@@ -9068,15 +9068,15 @@
                 const o = ih(e, [i, r, 0, 1]),
                     a = ih(e, [i, r, 1, 1]),
                     l = o[2],
                     c = a[2];
                 return Hc([], o, a, l === c ? 0 : ((n || 0) - l) / (c - l))
             }
 
-            function Ph(t) {
+            function Sh(t) {
                 const {
                     width: e,
                     height: n,
                     bounds: i,
                     minExtent: r = 0,
                     maxZoom: s = 24,
                     offset: o = [0, 0]
@@ -9100,15 +9100,15 @@
                     x = Math.min(s, oh(Math.abs(Math.min(m, v))));
                 return ah(Number.isFinite(x)), {
                     longitude: _[0],
                     latitude: _[1],
                     zoom: x
                 }
             }
-            const Sh = Math.PI / 180;
+            const Ph = Math.PI / 180;
 
             function Ch(t, e, n) {
                 const {
                     pixelUnprojectionMatrix: i
                 } = t, r = ih(i, [e, 0, 1, 1]), s = ih(i, [e, t.height, 1, 1]), o = vh(Hc([], r, s, (n * t.distanceScales.unitsPerMeter[2] - r[2]) / (s[2] - r[2])));
                 return o.push(n), o
             }
@@ -9129,32 +9129,32 @@
                     IDENTITY: 0
                 },
                 Mh = {
                     common: 0,
                     meters: 1,
                     pixels: 2
                 },
-                Lh = {
+                Oh = {
                     click: {
                         handler: "onClick"
                     },
                     panstart: {
                         handler: "onDragStart"
                     },
                     panmove: {
                         handler: "onDrag"
                     },
                     panend: {
                         handler: "onDragEnd"
                     }
                 },
-                Oh = "draw",
-                Rh = "mask",
+                Lh = "draw",
+                Ih = "mask",
                 kh = Math.PI / 180,
-                Ih = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1],
+                Rh = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1],
                 jh = [0, 0, 0],
                 zh = {
                     unitsPerMeter: [1, 1, 1],
                     metersPerUnit: [1, 1, 1]
                 };
             class Fh {
                 constructor(t = {}) {
@@ -9230,20 +9230,20 @@
                     width: n = 1,
                     height: i = 1
                 }) {
                     return t < this.x + this.width && this.x < t + n && e < this.y + this.height && this.y < e + i
                 }
                 getFrustumPlanes() {
                     return this._frustumPlanes.near || Object.assign(this._frustumPlanes, {
-                        left: Rc((t = this.viewProjectionMatrix)[3] + t[0], t[7] + t[4], t[11] + t[8], t[15] + t[12]),
-                        right: Rc(t[3] - t[0], t[7] - t[4], t[11] - t[8], t[15] - t[12]),
-                        bottom: Rc(t[3] + t[1], t[7] + t[5], t[11] + t[9], t[15] + t[13]),
-                        top: Rc(t[3] - t[1], t[7] - t[5], t[11] - t[9], t[15] - t[13]),
-                        near: Rc(t[3] + t[2], t[7] + t[6], t[11] + t[10], t[15] + t[14]),
-                        far: Rc(t[3] - t[2], t[7] - t[6], t[11] - t[10], t[15] - t[14])
+                        left: Ic((t = this.viewProjectionMatrix)[3] + t[0], t[7] + t[4], t[11] + t[8], t[15] + t[12]),
+                        right: Ic(t[3] - t[0], t[7] - t[4], t[11] - t[8], t[15] - t[12]),
+                        bottom: Ic(t[3] + t[1], t[7] + t[5], t[11] + t[9], t[15] + t[13]),
+                        top: Ic(t[3] - t[1], t[7] - t[5], t[11] - t[9], t[15] - t[13]),
+                        near: Ic(t[3] + t[2], t[7] + t[6], t[11] + t[10], t[15] + t[14]),
+                        far: Ic(t[3] - t[2], t[7] - t[6], t[11] - t[10], t[15] - t[14])
                     }), this._frustumPlanes;
                     var t
                 }
                 panByPosition(t, e) {
                     return null
                 }
                 _initProps(t) {
@@ -9267,30 +9267,30 @@
                     const {
                         position: r,
                         modelMatrix: s
                     } = t;
                     let o = jh;
                     if (r && (o = s ? new Qc(s).transformAsVector(r, []) : r), this.isGeospatial) {
                         const t = this.projectPosition([e, n, 0]);
-                        this.center = new Lc(o).scale(this.distanceScales.unitsPerMeter).add(t)
+                        this.center = new Oc(o).scale(this.distanceScales.unitsPerMeter).add(t)
                     } else this.center = this.projectPosition(o)
                 }
                 _initMatrices(t) {
                     const {
-                        viewMatrix: e = Ih,
+                        viewMatrix: e = Rh,
                         projectionMatrix: n = null,
                         orthographic: i = !1,
                         fovyRadians: r,
                         fovy: s = 75,
                         near: o = .1,
                         far: a = 1e3,
                         padding: l = null,
                         focalDistance: c = 1
                     } = t;
-                    this.viewMatrixUncentered = e, this.viewMatrix = (new Qc).multiplyRight(e).translate(new Lc(this.center).negate()), this.projectionMatrix = n || function({
+                    this.viewMatrixUncentered = e, this.viewMatrix = (new Qc).multiplyRight(e).translate(new Oc(this.center).negate()), this.projectionMatrix = n || function({
                         width: t,
                         height: e,
                         orthographic: n,
                         fovyRadians: i,
                         focalDistance: r,
                         padding: s,
                         near: o,
@@ -9330,22 +9330,22 @@
                         far: a
                     });
                     const h = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1];
                     var u;
                     Fc(h, h, this.projectionMatrix), Fc(h, h, this.viewMatrix), this.viewProjectionMatrix = h, this.viewMatrixInverse = zc([], this.viewMatrix) || this.viewMatrix, this.cameraPosition = [(u = this.viewMatrixInverse)[12], u[13], u[14]];
                     const d = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1],
                         p = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1];
-                    Dc(d, d, [this.width / 2, -this.height / 2, 1]), Bc(d, d, [1, -1, 0]), Fc(p, d, this.viewProjectionMatrix), this.pixelProjectionMatrix = p, this.pixelUnprojectionMatrix = zc([1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1], this.pixelProjectionMatrix), this.pixelUnprojectionMatrix || ta.warn("Pixel project matrix not invertible")()
+                    Nc(d, d, [this.width / 2, -this.height / 2, 1]), Bc(d, d, [1, -1, 0]), Fc(p, d, this.viewProjectionMatrix), this.pixelProjectionMatrix = p, this.pixelUnprojectionMatrix = zc([1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1], this.pixelProjectionMatrix), this.pixelUnprojectionMatrix || ta.warn("Pixel project matrix not invertible")()
                 }
             }
             wo(Fh, "displayName", "Viewport");
             const Bh = "vs",
-                Dh = "fs";
+                Nh = "fs";
 
-            function Nh(t, e) {
+            function Dh(t, e) {
                 if (!t) throw new Error(e || "shadertools: assertion failed.")
             }
             const Vh = {
                 number: {
                     validate: (t, e) => Number.isFinite(t) && (!("max" in e) || t <= e.max) && (!("min" in e) || t >= e.min)
                 },
                 array: {
@@ -9383,15 +9383,15 @@
                         getUniforms: o,
                         deprecations: a = [],
                         defines: l = {},
                         inject: c = {},
                         vertexShader: h,
                         fragmentShader: u
                     } = t;
-                    Nh("string" == typeof e), this.name = e, this.vs = n || h, this.fs = i || u, this.getModuleUniforms = o, this.dependencies = r, this.deprecations = this._parseDeprecationDefinitions(a), this.defines = l, this.injections = function(t) {
+                    Dh("string" == typeof e), this.name = e, this.vs = n || h, this.fs = i || u, this.getModuleUniforms = o, this.dependencies = r, this.deprecations = this._parseDeprecationDefinitions(a), this.defines = l, this.injections = function(t) {
                         const e = {
                             vs: {},
                             fs: {}
                         };
                         for (const n in t) {
                             let i = t[n];
                             "string" == typeof i && (i = {
@@ -9415,15 +9415,15 @@
                         case "vs":
                             e = this.vs || "";
                             break;
                         case "fs":
                             e = this.fs || "";
                             break;
                         default:
-                            Nh(!1)
+                            Dh(!1)
                     }
                     return "#define MODULE_".concat(this.name.toUpperCase().replace(/[^0-9a-z]/gi, "_"), "\n").concat(e, "// END MODULE_").concat(this.name, "\n\n")
                 }
                 getUniforms(t, e) {
                     return this.getModuleUniforms ? this.getModuleUniforms(t, e) : this.uniforms ? this._defaultGetUniforms(t) : {}
                 }
                 getDefines() {
@@ -9441,15 +9441,15 @@
                 }
                 _defaultGetUniforms() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const e = {},
                         n = this.uniforms;
                     for (const i in n) {
                         const r = n[i];
-                        i in t && !r.private ? (r.validate && Nh(r.validate(t[i], r), "".concat(this.name, ": invalid ").concat(i)), e[i] = t[i]) : e[i] = r.value
+                        i in t && !r.private ? (r.validate && Dh(r.validate(t[i], r), "".concat(this.name, ": invalid ").concat(i)), e[i] = t[i]) : e[i] = r.value
                     }
                     return e
                 }
             }
 
             function Hh(t) {
                 return function(t) {
@@ -9457,15 +9457,15 @@
                         n = {};
                     return Zh({
                         modules: t,
                         level: 0,
                         moduleMap: e,
                         moduleDepth: n
                     }), Object.keys(n).sort(((t, e) => n[e] - n[t])).map((t => e[t]))
-                }(qh(t))
+                }(Xh(t))
             }
 
             function Zh(t) {
                 let {
                     modules: e,
                     level: n,
                     moduleMap: i,
@@ -9477,18 +9477,18 @@
                     modules: t.dependencies,
                     level: n + 1,
                     moduleMap: i,
                     moduleDepth: r
                 })
             }
 
-            function qh(t, e) {
-                return t.map((t => (t instanceof Wh || (Nh("string" != typeof t, "Shader module use by name is deprecated. Import shader module '".concat(t, "' and use it directly.")), Nh(t.name, "shader module has no name"), (t = new Wh(t)).dependencies = qh(t.dependencies)), t)))
+            function Xh(t, e) {
+                return t.map((t => (t instanceof Wh || (Dh("string" != typeof t, "Shader module use by name is deprecated. Import shader module '".concat(t, "' and use it directly.")), Dh(t.name, "shader module has no name"), (t = new Wh(t)).dependencies = Xh(t.dependencies)), t)))
             }
-            const Xh = 7936,
+            const qh = 7936,
                 Yh = 7937,
                 Kh = 7938,
                 $h = 35724,
                 Jh = {
                     GLSL_FRAG_DATA: ["WEBGL_draw_buffers", !0],
                     GLSL_FRAG_DEPTH: ["EXT_frag_depth", !0],
                     GLSL_DERIVATIVES: ["OES_standard_derivatives", !0],
@@ -9499,15 +9499,15 @@
                 Qh[t] = t
             }));
             const tu = {};
 
             function eu(t, e) {
                 let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
                 const i = Jh[e];
-                if (Nh(i, e), ! function() {
+                if (Dh(i, e), ! function() {
                         let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                         const e = "undefined" != typeof window && window.navigator || {},
                             n = t.userAgent || e.userAgent || "",
                             i = -1 !== n.indexOf("MSIE "),
                             r = -1 !== n.indexOf("Trident/");
                         return i || r
                     }(n)) return !0;
@@ -9520,25 +9520,25 @@
                 const l = t.getShaderParameter(a, 35713);
                 return t.deleteShader(a), tu[e] = l, l
             }
 
             function nu(t, e) {
                 return (e = Array.isArray(e) ? e : [e]).every((e => function(t, e) {
                     const n = Jh[e];
-                    Nh(n, e);
+                    Dh(n, e);
                     const i = function(t) {
                             return "undefined" != typeof WebGL2RenderingContext && t instanceof WebGL2RenderingContext || Boolean(t && 2 === t._version)
                         }(t) && n[1] || n[0],
                         r = "string" == typeof i ? Boolean(t.getExtension(i)) : i;
-                    return Nh(!1 === r || !0 === r), r
+                    return Dh(!1 === r || !0 === r), r
                 }(t, e)))
             }
             const iu = {
                     [Bh]: "#ifdef MODULE_LOGDEPTH\n  logdepth_adjustPosition(gl_Position);\n#endif\n",
-                    [Dh]: "#ifdef MODULE_MATERIAL\n  gl_FragColor = material_filterColor(gl_FragColor);\n#endif\n\n#ifdef MODULE_LIGHTING\n  gl_FragColor = lighting_filterColor(gl_FragColor);\n#endif\n\n#ifdef MODULE_FOG\n  gl_FragColor = fog_filterColor(gl_FragColor);\n#endif\n\n#ifdef MODULE_PICKING\n  gl_FragColor = picking_filterHighlightColor(gl_FragColor);\n  gl_FragColor = picking_filterPickingColor(gl_FragColor);\n#endif\n\n#ifdef MODULE_LOGDEPTH\n  logdepth_setFragDepth();\n#endif\n"
+                    [Nh]: "#ifdef MODULE_MATERIAL\n  gl_FragColor = material_filterColor(gl_FragColor);\n#endif\n\n#ifdef MODULE_LIGHTING\n  gl_FragColor = lighting_filterColor(gl_FragColor);\n#endif\n\n#ifdef MODULE_FOG\n  gl_FragColor = fog_filterColor(gl_FragColor);\n#endif\n\n#ifdef MODULE_PICKING\n  gl_FragColor = picking_filterHighlightColor(gl_FragColor);\n  gl_FragColor = picking_filterPickingColor(gl_FragColor);\n#endif\n\n#ifdef MODULE_LOGDEPTH\n  logdepth_setFragDepth();\n#endif\n"
                 },
                 ru = "__LUMA_INJECT_DECLARATIONS__",
                 su = /void\s+main\s*\([^)]*\)\s*\{\n?/,
                 ou = /}\n?[^{}]*$/,
                 au = [];
 
             function lu(t, e, n) {
@@ -9573,15 +9573,15 @@
                     }
                 }
                 return t = t.replace(ru, ""), i && (t = t.replace(/\}\s*$/, (t => t + iu[e]))), t
             }
 
             function cu(t) {
                 const e = {};
-                return Nh(Array.isArray(t) && t.length > 1), t.forEach((t => {
+                return Dh(Array.isArray(t) && t.length > 1), t.forEach((t => {
                     for (const n in t) e[n] = e[n] ? "".concat(e[n], "\n").concat(t[n]) : t[n]
                 })), e
             }
 
             function hu(t) {
                 return new RegExp("\\b".concat(t, "[ \\t]+(\\w+[ \\t]+\\w+(\\[\\w+\\])?;)"), "g")
             }
@@ -9611,15 +9611,15 @@
             function _u(t, e) {
                 for (const [n, i] of e) t = t.replace(n, i);
                 return t
             }
             const xu = "\n\n".concat(ru, "\n\n"),
                 wu = {
                     [Bh]: "vertex",
-                    [Dh]: "fragment"
+                    [Nh]: "fragment"
                 };
 
             function Eu(t, e) {
                 let {
                     id: n,
                     source: i,
                     type: r,
@@ -9627,15 +9627,15 @@
                     defines: o = {},
                     hookFunctions: a = [],
                     inject: l = {},
                     transpileToGLSL100: c = !1,
                     prologue: h = !0,
                     log: u
                 } = e;
-                Nh("string" == typeof i, "shader source must be a string");
+                Dh("string" == typeof i, "shader source must be a string");
                 const d = r === Bh,
                     p = i.split("\n");
                 let f = 100,
                     g = "",
                     m = i;
                 0 === p[0].indexOf("#version ") ? (f = 300, g = p[0], m = p.slice(1).join("\n")) : g = "#version ".concat(f);
                 const v = {};
@@ -9659,15 +9659,15 @@
                     } = t;
                     return "\n#define SHADER_TYPE_".concat(wu[e].toUpperCase(), "\n")
                 }({
                     type: r
                 }), "\n").concat(function(t) {
                     const e = function(t) {
                         const e = t.getExtension("WEBGL_debug_renderer_info"),
-                            n = t.getParameter(e && e.UNMASKED_VENDOR_WEBGL || Xh),
+                            n = t.getParameter(e && e.UNMASKED_VENDOR_WEBGL || qh),
                             i = t.getParameter(e && e.UNMASKED_RENDERER_WEBGL || Yh);
                         return {
                             gpuVendor: function(t, e) {
                                 return t.match(/NVIDIA/i) || e.match(/NVIDIA/i) ? "NVIDIA" : t.match(/INTEL/i) || e.match(/INTEL/i) ? "INTEL" : t.match(/AMD/i) || e.match(/AMD/i) || t.match(/ATI/i) || e.match(/ATI/i) ? "AMD" : "UNKNOWN GPU"
                             }(n, i),
                             vendor: n,
                             renderer: i,
@@ -9778,25 +9778,25 @@
                             }(t);
                         default:
                             throw new Error("unknown GLSL version ".concat(e))
                     }
                 }(b, c ? 100 : f, d), b
             }
 
-            function Pu(t) {
+            function Su(t) {
                 return function(e) {
                     const n = {};
                     for (const i of t) {
                         const t = i.getUniforms(e, n);
                         Object.assign(n, t)
                     }
                     return n
                 }
             }
-            const Su = new Ko({
+            const Pu = new Ko({
                 id: "luma.gl"
             });
 
             function Cu(t, e) {
                 if (!t) throw new Error(e || "luma.gl: assertion failed.")
             }
             const Tu = "Requires WebGL2";
@@ -9805,48 +9805,48 @@
                 return "undefined" != typeof WebGLRenderingContext && t instanceof WebGLRenderingContext || "undefined" != typeof WebGL2RenderingContext && t instanceof WebGL2RenderingContext || Boolean(t && Number.isFinite(t._version))
             }
 
             function Mu(t) {
                 return "undefined" != typeof WebGL2RenderingContext && t instanceof WebGL2RenderingContext || Boolean(t && 2 === t._version)
             }
 
-            function Lu(t) {
+            function Ou(t) {
                 return Cu(Au(t), "Invalid WebGLRenderingContext"), t
             }
 
-            function Ou(t) {
+            function Lu(t) {
                 return Cu(Mu(t), Tu), t
             }
-            const Ru = {};
+            const Iu = {};
             const ku = function t(e) {
                 const n = e.gl;
                 this.ext = e, this.isAlive = !0, this.hasBeenBound = !1, this.elementArrayBuffer = null, this.attribs = new Array(e.maxVertexAttribs);
                 for (let e = 0; e < this.attribs.length; e++) {
                     const i = new t.VertexAttrib(n);
                     this.attribs[e] = i
                 }
                 this.maxAttrib = 0
             };
             (ku.VertexAttrib = function(t) {
                 this.enabled = !1, this.buffer = null, this.size = 4, this.type = 5126, this.normalized = !1, this.stride = 16, this.offset = 0, this.cached = "", this.recache()
             }).prototype.recache = function() {
                 this.cached = [this.size, this.type, this.normalized, this.stride, this.offset].join(":")
             };
-            const Iu = function(t) {
+            const Ru = function(t) {
                 const e = this;
                 this.gl = t,
                     function(t) {
                         const e = t.getError;
                         t.getError = function() {
                             let n;
                             do {
-                                n = e.apply(t), 0 !== n && (Ru[n] = !0)
+                                n = e.apply(t), 0 !== n && (Iu[n] = !0)
                             } while (0 !== n);
-                            for (n in Ru)
-                                if (Ru[n]) return delete Ru[n], parseInt(n, 10);
+                            for (n in Iu)
+                                if (Iu[n]) return delete Iu[n], parseInt(n, 10);
                             return 0
                         }
                     }(t);
                 const n = this.original = {
                     getParameter: t.getParameter,
                     enableVertexAttribArray: t.enableVertexAttribArray,
                     disableVertexAttribArray: t.disableVertexAttribArray,
@@ -9894,29 +9894,29 @@
                     l.maxAttrib = Math.max(l.maxAttrib, t);
                     const c = l.attribs[t];
                     return c.buffer = e.currentArrayBuffer, c.size = i, c.type = r, c.normalized = s, c.stride = o, c.offset = a, c.recache(), n.vertexAttribPointer.apply(this, arguments)
                 }, t.instrumentExtension && t.instrumentExtension(this, "OES_vertex_array_object"), t.canvas && t.canvas.addEventListener("webglcontextrestored", (() => {
                     globalThis.console && globalThis.console.log && globalThis.console.log("OESVertexArrayObject emulation library context restored"), e.reset_()
                 }), !0), this.reset_()
             };
-            Iu.prototype.VERTEX_ARRAY_BINDING_OES = 34229, Iu.prototype.reset_ = function() {
+            Ru.prototype.VERTEX_ARRAY_BINDING_OES = 34229, Ru.prototype.reset_ = function() {
                 if (void 0 !== this.vertexArrayObjects)
                     for (let t = 0; t < this.vertexArrayObjects.length; ++t) this.vertexArrayObjects.isAlive = !1;
                 const t = this.gl;
                 this.maxVertexAttribs = t.getParameter(34921), this.defaultVertexArrayObject = new ku(this), this.currentVertexArrayObject = null, this.currentArrayBuffer = null, this.vertexArrayObjects = [this.defaultVertexArrayObject], this.bindVertexArrayOES(null)
-            }, Iu.prototype.createVertexArrayOES = function() {
+            }, Ru.prototype.createVertexArrayOES = function() {
                 const t = new ku(this);
                 return this.vertexArrayObjects.push(t), t
-            }, Iu.prototype.deleteVertexArrayOES = function(t) {
+            }, Ru.prototype.deleteVertexArrayOES = function(t) {
                 t.isAlive = !1, this.vertexArrayObjects.splice(this.vertexArrayObjects.indexOf(t), 1), this.currentVertexArrayObject === t && this.bindVertexArrayOES(null)
-            }, Iu.prototype.isVertexArrayOES = function(t) {
+            }, Ru.prototype.isVertexArrayOES = function(t) {
                 return !!(t && t instanceof ku && t.hasBeenBound && t.ext === this)
-            }, Iu.prototype.bindVertexArrayOES = function(t) {
+            }, Ru.prototype.bindVertexArrayOES = function(t) {
                 const e = this.gl;
-                if (t && !t.isAlive) return n = "bindVertexArrayOES: attempt to bind deleted arrayObject", Ru[1282] = !0, void(void 0 !== n && (i = n, globalThis.console && globalThis.console.error && globalThis.console.error(i)));
+                if (t && !t.isAlive) return n = "bindVertexArrayOES: attempt to bind deleted arrayObject", Iu[1282] = !0, void(void 0 !== n && (i = n, globalThis.console && globalThis.console.error && globalThis.console.error(i)));
                 var n, i;
                 const r = this.original,
                     s = this.currentVertexArrayObject;
                 this.currentVertexArrayObject = t || this.defaultVertexArrayObject, this.currentVertexArrayObject.hasBeenBound = !0;
                 const o = this.currentVertexArrayObject;
                 if (s === o) return;
                 s && o.elementArrayBuffer === s.elementArrayBuffer || r.bindBuffer.call(e, 34963, o.elementArrayBuffer);
@@ -9932,15 +9932,15 @@
                 }
                 this.currentArrayBuffer !== a && r.bindBuffer.call(e, 34962, this.currentArrayBuffer)
             };
             const ju = "OES_element_index",
                 zu = "WEBGL_draw_buffers",
                 Fu = "WEBGL_debug_renderer_info",
                 Bu = t => Mu(t) ? void 0 : 0,
-                Du = {
+                Nu = {
                     3074: t => Mu(t) ? void 0 : 36064,
                     35723: t => Mu(t) ? void 0 : 4352,
                     35977: Bu,
                     32937: Bu,
                     36795: (t, e) => {
                         const n = Mu(t) ? t.getExtension("EXT_disjoint_timer_query_webgl2") : t.getExtension("EXT_disjoint_timer_query");
                         return n && n.GPU_DISJOINT_EXT ? e(n.GPU_DISJOINT_EXT) : 0
@@ -9993,28 +9993,28 @@
                     37154: Bu,
                     35371: Bu,
                     35658: Bu,
                     35076: Bu,
                     35077: Bu,
                     35380: Bu
                 },
-                Nu = "ANGLE_instanced_arrays",
+                Du = "ANGLE_instanced_arrays",
                 Vu = {
                     OES_vertex_array_object: {
                         meta: {
                             suffix: "OES"
                         },
                         createVertexArray: () => {
                             Cu(!1, "VertexArray requires WebGL2 or OES_vertex_array_object extension")
                         },
                         deleteVertexArray: () => {},
                         bindVertexArray: () => {},
                         isVertexArray: () => !1
                     },
-                    [Nu]: {
+                    [Du]: {
                         meta: {
                             suffix: "ANGLE"
                         },
                         vertexAttribDivisor(t, e) {
                             Cu(0 === e, "WebGL instanced rendering not supported")
                         },
                         drawElementsInstanced: () => {},
@@ -10060,15 +10060,15 @@
                             webgl2: r,
                             ext: s
                         } = function(t, e) {
                             return {
                                 webgl2: Mu(t),
                                 ext: t.getExtension(e)
                             }
-                        }(t, Nu);
+                        }(t, Du);
                         let o;
                         switch (i) {
                             case 35069:
                                 o = !!r && void 0;
                                 break;
                             case 35070:
                                 o = r || s ? void 0 : 0
@@ -10092,15 +10092,15 @@
                                 extensions: e
                             } = t.luma, n = e.EXT_texture_filter_anisotropic;
                             i = n && n.TEXTURE_MAX_ANISOTROPY_EXT || 34046
                         }
                         return e(n, i)
                     },
                     getParameter: function(t, e, n) {
-                        const i = Du[n],
+                        const i = Nu[n],
                             r = "function" == typeof i ? i(t, e, n) : i;
                         return void 0 !== r ? r : e(n)
                     },
                     hint: (t, e, n, i) => e(n, i)
                 };
 
             function Gu(t, e) {
@@ -10134,15 +10134,15 @@
                     const e = t.getSupportedExtensions;
                     t.getSupportedExtensions = function() {
                         const t = e.call(this) || [];
                         return t.indexOf("OES_vertex_array_object") < 0 && t.push("OES_vertex_array_object"), t
                     };
                     const n = t.getExtension;
                     t.getExtension = function(e) {
-                        return n.call(this, e) || ("OES_vertex_array_object" !== e ? null : (t.__OESVertexArrayObject || (this.__OESVertexArrayObject = new Iu(this)), this.__OESVertexArrayObject))
+                        return n.call(this, e) || ("OES_vertex_array_object" !== e ? null : (t.__OESVertexArrayObject || (this.__OESVertexArrayObject = new Ru(this)), this.__OESVertexArrayObject))
                     }
                 }(t), function(t) {
                     t.luma.extensions = {};
                     const e = t.getSupportedExtensions() || [];
                     for (const n of e) t.luma[n] = t.getExtension(n)
                 }(t), function(t, e) {
                     for (const n of Object.getOwnPropertyNames(e)) "overrides" !== n && Gu(t, {
@@ -10229,17 +10229,17 @@
                     32878: 0,
                     3316: 0,
                     3315: 0,
                     32877: 0
                 },
                 Hu = (t, e, n) => e ? t.enable(n) : t.disable(n),
                 Zu = (t, e, n) => t.hint(n, e),
-                qu = (t, e, n) => t.pixelStorei(n, e);
+                Xu = (t, e, n) => t.pixelStorei(n, e);
 
-            function Xu(t) {
+            function qu(t) {
                 return Array.isArray(t) || ArrayBuffer.isView(t)
             }
             const Yu = {
                 3042: Hu,
                 32773: (t, e) => t.blendColor(...e),
                 32777: "blendEquation",
                 34877: "blendEquation",
@@ -10286,39 +10286,39 @@
                 2964: "stencilOpFront",
                 2965: "stencilOpFront",
                 2966: "stencilOpFront",
                 34817: "stencilOpBack",
                 34818: "stencilOpBack",
                 34819: "stencilOpBack",
                 2978: (t, e) => t.viewport(...e),
-                3333: qu,
-                3317: qu,
-                37440: qu,
-                37441: qu,
-                37443: qu,
-                3330: qu,
-                3332: qu,
-                3331: qu,
+                3333: Xu,
+                3317: Xu,
+                37440: Xu,
+                37441: Xu,
+                37443: Xu,
+                3330: Xu,
+                3332: Xu,
+                3331: Xu,
                 36010: (t, e) => t.bindFramebuffer(36008, e),
-                3314: qu,
-                32878: qu,
-                3316: qu,
-                3315: qu,
-                32877: qu,
+                3314: Xu,
+                32878: Xu,
+                3316: Xu,
+                3315: Xu,
+                32877: Xu,
                 framebuffer: (t, e) => {
                     const n = e && "handle" in e ? e.handle : e;
                     return t.bindFramebuffer(36160, n)
                 },
                 blend: (t, e) => e ? t.enable(3042) : t.disable(3042),
                 blendColor: (t, e) => t.blendColor(...e),
                 blendEquation: (t, e) => {
-                    e = Xu(e) ? e : [e, e], t.blendEquationSeparate(...e)
+                    e = qu(e) ? e : [e, e], t.blendEquationSeparate(...e)
                 },
                 blendFunc: (t, e) => {
-                    e = Xu(e) && 2 === e.length ? [...e, ...e] : e, t.blendFuncSeparate(...e)
+                    e = qu(e) && 2 === e.length ? [...e, ...e] : e, t.blendFuncSeparate(...e)
                 },
                 clearColor: (t, e) => t.clearColor(...e),
                 clearDepth: (t, e) => t.clearDepth(e),
                 clearStencil: (t, e) => t.clearStencil(e),
                 colorMask: (t, e) => t.colorMask(...e),
                 cull: (t, e) => e ? t.enable(2884) : t.disable(2884),
                 cullFace: (t, e) => t.cullFace(e),
@@ -10336,25 +10336,25 @@
                 polygonOffsetFill: (t, e) => e ? t.enable(32823) : t.disable(32823),
                 polygonOffset: (t, e) => t.polygonOffset(...e),
                 sampleCoverage: (t, e) => t.sampleCoverage(...e),
                 scissorTest: (t, e) => e ? t.enable(3089) : t.disable(3089),
                 scissor: (t, e) => t.scissor(...e),
                 stencilTest: (t, e) => e ? t.enable(2960) : t.disable(2960),
                 stencilMask: (t, e) => {
-                    e = Xu(e) ? e : [e, e];
+                    e = qu(e) ? e : [e, e];
                     const [n, i] = e;
                     t.stencilMaskSeparate(1028, n), t.stencilMaskSeparate(1029, i)
                 },
                 stencilFunc: (t, e) => {
-                    e = Xu(e) && 3 === e.length ? [...e, ...e] : e;
+                    e = qu(e) && 3 === e.length ? [...e, ...e] : e;
                     const [n, i, r, s, o, a] = e;
                     t.stencilFuncSeparate(1028, n, i, r), t.stencilFuncSeparate(1029, s, o, a)
                 },
                 stencilOp: (t, e) => {
-                    e = Xu(e) && 3 === e.length ? [...e, ...e] : e;
+                    e = qu(e) && 3 === e.length ? [...e, ...e] : e;
                     const [n, i, r, s, o, a] = e;
                     t.stencilOpSeparate(1028, n, i, r), t.stencilOpSeparate(1029, s, o, a)
                 },
                 viewport: (t, e) => t.viewport(...e)
             };
 
             function Ku(t, e, n) {
@@ -10771,15 +10771,15 @@
                                 rendererMasked: n,
                                 version: t.getParameter(7938),
                                 shadingLanguageVersion: t.getParameter(35724)
                             }
                         }(t),
                         i = n ? "(".concat(n.vendor, ",").concat(n.renderer, ")") : "",
                         r = t.debug ? " debug" : "";
-                    Su.info(1, "".concat(e).concat(r, " context ").concat(i))()
+                    Pu.info(1, "".concat(e).concat(r, " context ").concat(i))()
                 }(r), r) : null
             }
 
             function bd(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 if (!t || t._instrumented) return t;
                 t._version = t._version || function(t) {
@@ -10789,17 +10789,17 @@
                     manageState: n,
                     debug: i
                 } = e;
                 return n && od(t, {
                     copyState: !1,
                     log: function() {
                         for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-                        return Su.log(1, ...e)()
+                        return Pu.log(1, ...e)()
                     }
-                }), fd && i && (globalThis.makeDebugContext ? (t = globalThis.makeDebugContext(t, e), Su.level = Math.max(Su.level, 1)) : Su.warn('WebGL debug mode not activated. import "@luma.gl/debug" to enable.')()), t._instrumented = !0, t
+                }), fd && i && (globalThis.makeDebugContext ? (t = globalThis.makeDebugContext(t, e), Pu.level = Math.max(Pu.level, 1)) : Pu.warn('WebGL debug mode not activated. import "@luma.gl/debug" to enable.')()), t._instrumented = !0, t
             }
             const yd = "8.5.16";
             class _d {
                 constructor() {
                     this.stats = new Map
                 }
                 get(t) {
@@ -10819,36 +10819,36 @@
                 if ("string" != typeof e) return e;
                 const n = Number(e);
                 if (!isNaN(n)) return n;
                 const i = t[e = e.replace(/^.*\./, "")];
                 return wd(void 0 !== i, "Accessing undefined constant GL.".concat(e)), i
             }
 
-            function Pd(t, e) {
+            function Sd(t, e) {
                 e = Number(e);
                 for (const n in t)
                     if (t[n] === e) return "GL.".concat(n);
                 return String(e)
             }
-            globalThis.luma || (ko() && Su.log(1, "luma.gl ".concat(yd, " - ").concat("set luma.log.level=1 (or higher) to trace rendering"))(), globalThis.luma = globalThis.luma || {
+            globalThis.luma || (ko() && Pu.log(1, "luma.gl ".concat(yd, " - ").concat("set luma.log.level=1 (or higher) to trace rendering"))(), globalThis.luma = globalThis.luma || {
                 VERSION: yd,
                 version: yd,
-                log: Su,
+                log: Pu,
                 stats: xd,
                 globals: {
                     modules: {},
                     nodeIO: {}
                 }
             }), globalThis.luma;
-            const Sd = {};
+            const Pd = {};
 
             function Cd() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "id";
-                Sd[t] = Sd[t] || 1;
-                const e = Sd[t]++;
+                Pd[t] = Pd[t] || 1;
+                const e = Pd[t]++;
                 return "".concat(t, "-").concat(e)
             }
 
             function Td(t) {
                 return wd("number" == typeof t, "Input must be a number"), t && 0 == (t & t - 1)
             }
 
@@ -10862,26 +10862,26 @@
             }
 
             function Md(t, e, n, i) {
                 const r = "See luma.gl ".concat(n, " Upgrade Guide at https://luma.gl/docs/upgrade-guide"),
                     s = Object.getPrototypeOf(t);
                 i.forEach((t => {
                     s.methodName || (s[t] = () => {
-                        throw Su.removed("Calling removed method ".concat(e, ".").concat(t, ": "), r)(), new Error(t)
+                        throw Pu.removed("Calling removed method ".concat(e, ".").concat(t, ": "), r)(), new Error(t)
                     })
                 }))
             }
-            const Ld = "Resource subclass must define virtual methods";
-            class Od {
+            const Od = "Resource subclass must define virtual methods";
+            class Ld {
                 get[Symbol.toStringTag]() {
                     return "Resource"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    Lu(t);
+                    Ou(t);
                     const {
                         id: n,
                         userData: i = {}
                     } = e;
                     this.gl = t, this.gl2 = t, this.id = n || Cd(this[Symbol.toStringTag]), this.userData = i, this._bound = !1, this._handle = e.handle, void 0 === this._handle && (this._handle = this._createHandle()), this.byteLength = 0, this._initStats(), this._addStats()
                 }
                 toString() {
@@ -10923,16 +10923,16 @@
                     const {
                         parameters: e,
                         keys: n
                     } = t, i = this.constructor.PARAMETERS || {}, r = Mu(this.gl), s = {}, o = e || Object.keys(i);
                     for (const e of o) {
                         const o = i[e];
                         if (o && (!("webgl2" in o) || r) && (!("extension" in o) || this.gl.getExtension(o.extension))) {
-                            const i = n ? Pd(this.gl, e) : e;
-                            s[i] = this.getParameter(e, t), n && "GLenum" === o.type && (s[i] = Pd(this.gl, s[i]))
+                            const i = n ? Sd(this.gl, e) : e;
+                            s[i] = this.getParameter(e, t), n && "GLenum" === o.type && (s[i] = Sd(this.gl, s[i]))
                         }
                     }
                     return s
                 }
                 setParameter(t, e) {
                     wd(t = Ed(this.gl, t));
                     const n = (this.constructor.PARAMETERS || {})[t];
@@ -10948,30 +10948,30 @@
                     return this
                 }
                 stubRemovedMethods(t, e, n) {
                     return Md(this, t, e, n)
                 }
                 initialize(t) {}
                 _createHandle() {
-                    throw new Error(Ld)
+                    throw new Error(Od)
                 }
                 _deleteHandle() {
-                    throw new Error(Ld)
+                    throw new Error(Od)
                 }
                 _bindHandle(t) {
-                    throw new Error(Ld)
+                    throw new Error(Od)
                 }
                 _getOptsFromHandle() {
-                    throw new Error(Ld)
+                    throw new Error(Od)
                 }
                 _getParameter(t, e) {
-                    throw new Error(Ld)
+                    throw new Error(Od)
                 }
                 _setParameter(t, e) {
-                    throw new Error(Ld)
+                    throw new Error(Od)
                 }
                 _context() {
                     return this.gl.luma = this.gl.luma || {}, this.gl.luma
                 }
                 _initStats() {
                     this.gl.stats = this.gl.stats || new _d
                 }
@@ -10999,15 +10999,15 @@
                 }
                 _doTrackDeallocatedMemory() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this[Symbol.toStringTag],
                         e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : xd.get("Memory Usage");
                     e.get("GPU Memory").subtractCount(this.byteLength), e.get("".concat(t, " Memory")).subtractCount(this.byteLength), this.byteLength = 0
                 }
             }
-            const Rd = "Failed to deduce GL constant from typed array";
+            const Id = "Failed to deduce GL constant from typed array";
 
             function kd(t) {
                 switch (ArrayBuffer.isView(t) ? t.constructor : t) {
                     case Float32Array:
                         return 5126;
                     case Uint16Array:
                         return 5123;
@@ -11019,19 +11019,19 @@
                     case Int8Array:
                         return 5120;
                     case Int16Array:
                         return 5122;
                     case Int32Array:
                         return 5124;
                     default:
-                        throw new Error(Rd)
+                        throw new Error(Id)
                 }
             }
 
-            function Id(t) {
+            function Rd(t) {
                 let {
                     clamped: e = !0
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 switch (t) {
                     case 5126:
                         return Float32Array;
                     case 5123:
@@ -11078,24 +11078,24 @@
                     removedProps: i = {},
                     deprecatedProps: r = {},
                     replacedProps: s = {}
                 } = n;
                 for (const n in i)
                     if (n in e) {
                         const e = i[n] ? "".concat(t, ".").concat(i[n]) : "N/A";
-                        Su.removed("".concat(t, ".").concat(n), e)()
+                        Pu.removed("".concat(t, ".").concat(n), e)()
                     } for (const n in r)
                     if (n in e) {
                         const e = r[n];
-                        Su.deprecated("".concat(t, ".").concat(n), "".concat(t, ".").concat(e))()
+                        Pu.deprecated("".concat(t, ".").concat(n), "".concat(t, ".").concat(e))()
                     } let o = null;
                 for (const n in s)
                     if (n in e) {
                         const i = s[n];
-                        Su.deprecated("".concat(t, ".").concat(n), "".concat(t, ".").concat(i))(), o = o || Object.assign({}, e), o[i] = e[n], delete o[n]
+                        Pu.deprecated("".concat(t, ".").concat(n), "".concat(t, ".").concat(i))(), o = o || Object.assign({}, e), o[i] = e[n], delete o[n]
                     } return o || e
             }
             const Fd = {
                     offset: 0,
                     stride: 0,
                     type: 5126,
                     size: 1,
@@ -11105,44 +11105,44 @@
                 },
                 Bd = {
                     deprecatedProps: {
                         instanced: "divisor",
                         isInstanced: "divisor"
                     }
                 };
-            class Dd {
+            class Nd {
                 static getBytesPerElement(t) {
-                    return Id(t.type || 5126).BYTES_PER_ELEMENT
+                    return Rd(t.type || 5126).BYTES_PER_ELEMENT
                 }
                 static getBytesPerVertex(t) {
-                    return wd(t.size), Id(t.type || 5126).BYTES_PER_ELEMENT * t.size
+                    return wd(t.size), Rd(t.type || 5126).BYTES_PER_ELEMENT * t.size
                 }
                 static resolve() {
                     for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-                    return new Dd(...[Fd, ...e])
+                    return new Nd(...[Fd, ...e])
                 }
                 constructor() {
                     for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                     e.forEach((t => this._assign(t))), Object.freeze(this)
                 }
                 toString() {
                     return JSON.stringify(this)
                 }
                 get BYTES_PER_ELEMENT() {
-                    return Dd.getBytesPerElement(this)
+                    return Nd.getBytesPerElement(this)
                 }
                 get BYTES_PER_VERTEX() {
-                    return Dd.getBytesPerVertex(this)
+                    return Nd.getBytesPerVertex(this)
                 }
                 _assign() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return t = zd("Accessor", t, Bd), void 0 !== t.type && (this.type = t.type, 5124 !== t.type && 5125 !== t.type || (this.integer = !0)), void 0 !== t.size && (this.size = t.size), void 0 !== t.offset && (this.offset = t.offset), void 0 !== t.stride && (this.stride = t.stride), void 0 !== t.normalized && (this.normalized = t.normalized), void 0 !== t.integer && (this.integer = t.integer), void 0 !== t.divisor && (this.divisor = t.divisor), void 0 !== t.buffer && (this.buffer = t.buffer), void 0 !== t.index && ("boolean" == typeof t.index ? this.index = t.index ? 1 : 0 : this.index = t.index), void 0 !== t.instanced && (this.divisor = t.instanced ? 1 : 0), void 0 !== t.isInstanced && (this.divisor = t.isInstanced ? 1 : 0), this
                 }
             }
-            const Nd = {
+            const Dd = {
                     offset: "accessor.offset",
                     stride: "accessor.stride",
                     type: "accessor.type",
                     size: "accessor.size",
                     divisor: "accessor.divisor",
                     normalized: "accessor.normalized",
                     integer: "accessor.integer",
@@ -11150,48 +11150,48 @@
                     isInstanced: "accessor.divisor"
                 },
                 Vd = {
                     removedProps: {},
                     replacedProps: {
                         bytes: "byteLength"
                     },
-                    deprecatedProps: Nd
+                    deprecatedProps: Dd
                 },
                 Ud = {
-                    removedProps: Nd
+                    removedProps: Dd
                 };
-            class Gd extends Od {
+            class Gd extends Ld {
                 get[Symbol.toStringTag]() {
                     return "Buffer"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     super(t, e), this.stubRemovedMethods("Buffer", "v6.0", ["layout", "setLayout", "getIndexedParameter"]), this.target = e.target || (this.gl.webgl2 ? 36662 : 34962), this.initialize(e), Object.seal(this)
                 }
                 getElementCount() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this.accessor;
-                    return Math.round(this.byteLength / Dd.getBytesPerElement(t))
+                    return Math.round(this.byteLength / Nd.getBytesPerElement(t))
                 }
                 getVertexCount() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this.accessor;
-                    return Math.round(this.byteLength / Dd.getBytesPerVertex(t))
+                    return Math.round(this.byteLength / Nd.getBytesPerVertex(t))
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return ArrayBuffer.isView(t) && (t = {
                         data: t
                     }), Number.isFinite(t) && (t = {
                         byteLength: t
                     }), t = zd("Buffer", t, Vd), this.usage = t.usage || 35044, this.debugData = null, this.setAccessor(Object.assign({}, t, t.accessor)), t.data ? this._setData(t.data, t.offset, t.byteLength) : this._setByteLength(t.byteLength || 0), this
                 }
                 setProps(t) {
                     return "accessor" in (t = zd("Buffer", t, Ud)) && this.setAccessor(t.accessor), this
                 }
                 setAccessor(t) {
-                    return delete(t = Object.assign({}, t)).buffer, this.accessor = new Dd(t), this
+                    return delete(t = Object.assign({}, t)).buffer, this.accessor = new Nd(t), this
                 }
                 reallocate(t) {
                     return t > this.byteLength ? (this._setByteLength(t), !0) : (this.bytesUsed = t, !1)
                 }
                 setData(t) {
                     return this.initialize(t)
                 }
@@ -11202,37 +11202,37 @@
                     const {
                         data: e,
                         offset: n = 0,
                         srcOffset: i = 0
                     } = t, r = t.byteLength || t.length;
                     wd(e);
                     const s = this.gl.webgl2 ? 36663 : this.target;
-                    return this.gl.bindBuffer(s, this.handle), 0 !== i || void 0 !== r ? (Ou(this.gl), this.gl.bufferSubData(this.target, n, e, i, r)) : this.gl.bufferSubData(s, n, e), this.gl.bindBuffer(s, null), this.debugData = null, this._inferType(e), this
+                    return this.gl.bindBuffer(s, this.handle), 0 !== i || void 0 !== r ? (Lu(this.gl), this.gl.bufferSubData(this.target, n, e, i, r)) : this.gl.bufferSubData(s, n, e), this.gl.bindBuffer(s, null), this.debugData = null, this._inferType(e), this
                 }
                 copyData(t) {
                     let {
                         sourceBuffer: e,
                         readOffset: n = 0,
                         writeOffset: i = 0,
                         size: r
                     } = t;
                     const {
                         gl: s
                     } = this;
-                    return Ou(s), s.bindBuffer(36662, e.handle), s.bindBuffer(36663, this.handle), s.copyBufferSubData(36662, 36663, n, i, r), s.bindBuffer(36662, null), s.bindBuffer(36663, null), this.debugData = null, this
+                    return Lu(s), s.bindBuffer(36662, e.handle), s.bindBuffer(36663, this.handle), s.copyBufferSubData(36662, 36663, n, i, r), s.bindBuffer(36662, null), s.bindBuffer(36663, null), this.debugData = null, this
                 }
                 getData() {
                     let {
                         dstData: t = null,
                         srcByteOffset: e = 0,
                         dstOffset: n = 0,
                         length: i = 0
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    Ou(this.gl);
-                    const r = Id(this.accessor.type || 5126, {
+                    Lu(this.gl);
+                    const r = Rd(this.accessor.type || 5126, {
                             clamped: !1
                         }),
                         s = this._getAvailableElementCount(e),
                         o = n;
                     let a, l;
                     t ? (l = t.length, a = l - o) : (a = Math.min(s, i || s), l = o + a);
                     const c = Math.min(s, a);
@@ -11271,15 +11271,15 @@
                 _setData(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0,
                         n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : t.byteLength + e;
                     wd(ArrayBuffer.isView(t)), this._trackDeallocatedMemory();
                     const i = this._getTarget();
                     this.gl.bindBuffer(i, this.handle), this.gl.bufferData(i, n, this.usage), this.gl.bufferSubData(i, e, t), this.gl.bindBuffer(i, null), this.debugData = t.slice(0, 10), this.bytesUsed = n, this._trackAllocatedMemory(n);
                     const r = kd(t);
-                    return wd(r), this.setAccessor(new Dd(this.accessor, {
+                    return wd(r), this.setAccessor(new Nd(this.accessor, {
                         type: r
                     })), this
                 }
                 _setByteLength(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.usage;
                     wd(t >= 0), this._trackDeallocatedMemory();
                     let n = t;
@@ -11287,21 +11287,21 @@
                     const i = this._getTarget();
                     return this.gl.bindBuffer(i, this.handle), this.gl.bufferData(i, n, e), this.gl.bindBuffer(i, null), this.usage = e, this.debugData = null, this.bytesUsed = t, this._trackAllocatedMemory(t), this
                 }
                 _getTarget() {
                     return this.gl.webgl2 ? 36663 : this.target
                 }
                 _getAvailableElementCount(t) {
-                    const e = t / Id(this.accessor.type || 5126, {
+                    const e = t / Rd(this.accessor.type || 5126, {
                         clamped: !1
                     }).BYTES_PER_ELEMENT;
                     return this.getElementCount() - e
                 }
                 _inferType(t) {
-                    this.accessor.type || this.setAccessor(new Dd(this.accessor, {
+                    this.accessor.type || this.setAccessor(new Nd(this.accessor, {
                         type: kd(t)
                     }))
                 }
                 _createHandle() {
                     return this.gl.createBuffer()
                 }
                 _deleteHandle() {
@@ -11309,24 +11309,24 @@
                 }
                 _getParameter(t) {
                     this.gl.bindBuffer(this.target, this.handle);
                     const e = this.gl.getBufferParameter(this.target, t);
                     return this.gl.bindBuffer(this.target, null), e
                 }
                 get type() {
-                    return Su.deprecated("Buffer.type", "Buffer.accessor.type")(), this.accessor.type
+                    return Pu.deprecated("Buffer.type", "Buffer.accessor.type")(), this.accessor.type
                 }
                 get bytes() {
-                    return Su.deprecated("Buffer.bytes", "Buffer.byteLength")(), this.byteLength
+                    return Pu.deprecated("Buffer.bytes", "Buffer.byteLength")(), this.byteLength
                 }
                 setByteLength(t) {
-                    return Su.deprecated("setByteLength", "reallocate")(), this.reallocate(t)
+                    return Pu.deprecated("setByteLength", "reallocate")(), this.reallocate(t)
                 }
                 updateAccessor(t) {
-                    return Su.deprecated("updateAccessor(...)", "setAccessor(new Accessor(buffer.accessor, ...)")(), this.accessor = new Dd(this.accessor, t), this
+                    return Pu.deprecated("updateAccessor(...)", "setAccessor(new Accessor(buffer.accessor, ...)")(), this.accessor = new Nd(this.accessor, t), this
                 }
             }
             const Wd = {
                     6407: {
                         dataFormat: 6407,
                         types: [5121, 33635]
                     },
@@ -11388,17 +11388,17 @@
                     5124: 4,
                     5123: 2,
                     5122: 2,
                     5131: 2,
                     5120: 1,
                     5121: 1
                 },
-                qd = [9729, 9728],
-                Xd = globalThis.WebGLBuffer || function() {};
-            class Yd extends Od {
+                Xd = [9729, 9728],
+                qd = globalThis.WebGLBuffer || function() {};
+            class Yd extends Ld {
                 get[Symbol.toStringTag]() {
                     return "Texture"
                 }
                 static isSupported(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const {
                         format: n,
@@ -11477,15 +11477,15 @@
                         format: r,
                         type: p,
                         dataFormat: d,
                         compressed: f,
                         data: e,
                         width: h,
                         height: u
-                    })), this.width = h, this.height = u, this.depth = m, this.format = r, this.type = p, this.dataFormat = d, this.border = s, this.textureUnit = c, Number.isFinite(this.textureUnit) && (this.gl.activeTexture(33984 + this.textureUnit), this.gl.bindTexture(this.target, this.handle)), g && this._isNPOT() && (Su.warn("texture: ".concat(this, " is Non-Power-Of-Two, disabling mipmaping"))(), g = !1, this._updateForNPOT(a)), this.mipmaps = g, this.setImageData({
+                    })), this.width = h, this.height = u, this.depth = m, this.format = r, this.type = p, this.dataFormat = d, this.border = s, this.textureUnit = c, Number.isFinite(this.textureUnit) && (this.gl.activeTexture(33984 + this.textureUnit), this.gl.bindTexture(this.target, this.handle)), g && this._isNPOT() && (Pu.warn("texture: ".concat(this, " is Non-Power-Of-Two, disabling mipmaping"))(), g = !1, this._updateForNPOT(a)), this.mipmaps = g, this.setImageData({
                         data: e,
                         width: h,
                         height: u,
                         depth: m,
                         format: r,
                         type: p,
                         dataFormat: d,
@@ -11527,15 +11527,15 @@
                         dataFormat: this.dataFormat,
                         border: this.border,
                         mipmaps: i
                     }) : this
                 }
                 generateMipmap() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    return this._isNPOT() ? (Su.warn("texture: ".concat(this, " is Non-Power-Of-Two, disabling mipmaping"))(), this) : (this.mipmaps = !0, this.gl.bindTexture(this.target, this.handle), cd(this.gl, t, (() => {
+                    return this._isNPOT() ? (Pu.warn("texture: ".concat(this, " is Non-Power-Of-Two, disabling mipmaping"))(), this) : (this.mipmaps = !0, this.gl.bindTexture(this.target, this.handle), cd(this.gl, t, (() => {
                         this.gl.generateMipmap(this.target)
                     })), this.gl.bindTexture(this.target, null), this)
                 }
                 setImageData(t) {
                     this._trackDeallocatedMemory("Texture");
                     const {
                         target: e = this.target,
@@ -11587,15 +11587,15 @@
                                 case "null":
                                     f.texImage2D(e, i, r, h, u, s, d, c, l);
                                     break;
                                 case "typed-array":
                                     f.texImage2D(e, i, r, h, u, s, d, c, l, o);
                                     break;
                                 case "buffer":
-                                    g = Ou(f), g.bindBuffer(35052, l.handle || l), g.texImage2D(e, i, r, h, u, s, d, c, o), g.bindBuffer(35052, null);
+                                    g = Lu(f), g.bindBuffer(35052, l.handle || l), g.texImage2D(e, i, r, h, u, s, d, c, o), g.bindBuffer(35052, null);
                                     break;
                                 case "browser-object":
                                     Mu(f) ? f.texImage2D(e, i, r, h, u, s, d, c, l) : f.texImage2D(e, i, r, d, c, l);
                                     break;
                                 case "compressed":
                                     for (const [t, n] of l.entries()) f.compressedTexImage2D(e, t, n.format, n.width, n.height, s, n.data), v += n.levelSize;
                                     break;
@@ -11647,22 +11647,22 @@
                         const t = i;
                         i = t.data, o = t.shape[0], a = t.shape[1]
                     }
                     i instanceof Gd && (i = i.handle), this.gl.bindTexture(this.target, this.handle), cd(this.gl, g, (() => {
                         if (d) this.gl.compressedTexSubImage2D(e, l, r, s, o, a, c, i);
                         else if (null === i) this.gl.texSubImage2D(e, l, r, s, o, a, u, h, null);
                         else if (ArrayBuffer.isView(i)) this.gl.texSubImage2D(e, l, r, s, o, a, u, h, i, p);
-                        else if (i instanceof Xd) {
-                            const t = Ou(this.gl);
+                        else if (i instanceof qd) {
+                            const t = Lu(this.gl);
                             t.bindBuffer(35052, i), t.texSubImage2D(e, l, r, s, o, a, u, h, p), t.bindBuffer(35052, null)
-                        } else Mu(this.gl) ? Ou(this.gl).texSubImage2D(e, l, r, s, o, a, u, h, i) : this.gl.texSubImage2D(e, l, r, s, u, h, i)
+                        } else Mu(this.gl) ? Lu(this.gl).texSubImage2D(e, l, r, s, o, a, u, h, i) : this.gl.texSubImage2D(e, l, r, s, u, h, i)
                     })), this.gl.bindTexture(this.target, null)
                 }
                 copyFramebuffer() {
-                    return Su.error("Texture.copyFramebuffer({...}) is no logner supported, use copyToTexture(source, target, opts})")(), null
+                    return Pu.error("Texture.copyFramebuffer({...}) is no logner supported, use copyToTexture(source, target, opts})")(), null
                 }
                 getActiveUnit() {
                     return this.gl.getParameter(34016) - 33984
                 }
                 bind() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this.textureUnit;
                     const {
@@ -11690,15 +11690,15 @@
                         dataType: "null"
                     } : ArrayBuffer.isView(e) ? {
                         data: e,
                         dataType: "typed-array"
                     } : e instanceof Gd ? {
                         data: e.handle,
                         dataType: "buffer"
-                    } : e instanceof Xd ? {
+                    } : e instanceof qd ? {
                         data: e,
                         dataType: "buffer"
                     } : {
                         data: e,
                         dataType: "browser-object"
                     }
                 }
@@ -11788,15 +11788,15 @@
                 }
                 _updateForNPOT(t) {
                     void 0 === t[this.gl.TEXTURE_MIN_FILTER] && (t[this.gl.TEXTURE_MIN_FILTER] = this.gl.LINEAR), void 0 === t[this.gl.TEXTURE_WRAP_S] && (t[this.gl.TEXTURE_WRAP_S] = this.gl.CLAMP_TO_EDGE), void 0 === t[this.gl.TEXTURE_WRAP_T] && (t[this.gl.TEXTURE_WRAP_T] = this.gl.CLAMP_TO_EDGE)
                 }
                 _getNPOTParam(t, e) {
                     if (this._isNPOT()) switch (t) {
                         case 10241:
-                            -1 === qd.indexOf(e) && (e = 9729);
+                            -1 === Xd.indexOf(e) && (e = 9729);
                             break;
                         case 10242:
                         case 10243:
                             33071 !== e && (e = 33071)
                     }
                     return e
                 }
@@ -11807,15 +11807,15 @@
                 }
                 static isSupported(t, e) {
                     return Yd.isSupported(t, e)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     var n;
-                    Lu(t), (e instanceof Promise || "string" == typeof e) && (e = {
+                    Ou(t), (e instanceof Promise || "string" == typeof e) && (e = {
                         data: e
                     }), "string" == typeof e.data && (e = Object.assign({}, e, {
                         data: (n = e.data, wd("string" == typeof n), n = "" + n, new Promise(((t, e) => {
                             try {
                                 const i = new Image;
                                 i.onload = () => t(i), i.onerror = () => e(new Error("Could not load image ".concat(n, "."))), i.crossOrigin = "anonymous", i.src = n
                             } catch (t) {
@@ -11984,15 +11984,15 @@
                         bpp: 16
                     },
                     35898: {
                         gl2: $d,
                         bpp: 4
                     }
                 };
-            class Qd extends Od {
+            class Qd extends Ld {
                 get[Symbol.toStringTag]() {
                     return "Renderbuffer"
                 }
                 static isSupported(t) {
                     let {
                         format: e
                     } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {
@@ -12072,15 +12072,15 @@
             const ip = [34069, 34070, 34071, 34072, 34073, 34074];
             class rp extends Yd {
                 get[Symbol.toStringTag]() {
                     return "TextureCube"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    Lu(t), super(t, Object.assign({}, e, {
+                    Ou(t), super(t, Object.assign({}, e, {
                         target: 34067
                     })), this.initialize(e), Object.seal(this)
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         mipmaps: e = !0,
@@ -12119,15 +12119,15 @@
                     const {
                         gl: l
                     } = this, c = i || r, h = await Promise.all(ip.map((t => {
                         const e = c[t];
                         return Promise.all(Array.isArray(e) ? e : [e])
                     })));
                     this.bind(), ip.forEach(((t, i) => {
-                        h[i].length > 1 && !1 !== this.opts.mipmaps && Su.warn("".concat(this.id, " has mipmap and multiple LODs."))(), h[i].forEach(((i, r) => {
+                        h[i].length > 1 && !1 !== this.opts.mipmaps && Pu.warn("".concat(this.id, " has mipmap and multiple LODs."))(), h[i].forEach(((i, r) => {
                             e && n ? l.texImage2D(t, r, o, e, n, s, o, a, i) : l.texImage2D(t, r, o, o, a, i)
                         }))
                     })), this.unbind()
                 }
                 setImageDataForFace(t) {
                     const {
                         face: e,
@@ -12154,15 +12154,15 @@
                     return "Texture3D"
                 }
                 static isSupported(t) {
                     return Mu(t)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    Ou(t), e = Object.assign({
+                    Lu(t), e = Object.assign({
                         depth: 1
                     }, e, {
                         target: 32879,
                         unpackFlipY: !1
                     }), super(t, e), this.initialize(e), Object.seal(this)
                 }
                 setImageData(t) {
@@ -12230,15 +12230,15 @@
                 const {
                     gl: d,
                     handle: p,
                     attachments: f
                 } = h;
                 a = a || h.width, l = l || h.height, 36064 === s && null === p && (s = 1028), wd(f[s]), c = c || f[s].type, o = function(t, e, n, i, r) {
                     if (t) return t;
-                    const s = Id(e = e || 5121, {
+                    const s = Rd(e = e || 5121, {
                             clamped: !1
                         }),
                         o = function(t) {
                             switch (t) {
                                 case 6406:
                                 case 33326:
                                 case 6403:
@@ -12372,18 +12372,18 @@
                     const r = Mu(t) && n[1] || n[0];
                     if ("function" == typeof r) i = r(t);
                     else if (Array.isArray(r)) {
                         i = !0;
                         for (const e of r) i = i && Boolean(t.getExtension(e))
                     } else "string" == typeof r ? i = Boolean(t.getExtension(r)) : "boolean" == typeof r ? i = r : wd(!1);
                     return i
-                }(t, e)), t.luma.caps[e] || Su.log(pp, "Feature: ".concat(e, " not supported"))(), t.luma.caps[e]
+                }(t, e)), t.luma.caps[e] || Pu.log(pp, "Feature: ".concat(e, " not supported"))(), t.luma.caps[e]
             }
             const mp = "Multiple render targets not supported";
-            class vp extends Od {
+            class vp extends Ld {
                 get[Symbol.toStringTag]() {
                     return "Framebuffer"
                 }
                 static isSupported(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const {
                         colorBufferFloat: n,
@@ -12396,19 +12396,19 @@
                     return t.luma = t.luma || {}, t.luma.defaultFramebuffer = t.luma.defaultFramebuffer || new vp(t, {
                         id: "default-framebuffer",
                         handle: null,
                         attachments: {}
                     }), t.luma.defaultFramebuffer
                 }
                 get MAX_COLOR_ATTACHMENTS() {
-                    const t = Ou(this.gl);
+                    const t = Lu(this.gl);
                     return t.getParameter(t.MAX_COLOR_ATTACHMENTS)
                 }
                 get MAX_DRAW_BUFFERS() {
-                    const t = Ou(this.gl);
+                    const t = Lu(this.gl);
                     return t.getParameter(t.MAX_DRAW_BUFFERS)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     super(t, e), this.width = null, this.height = null, this.attachments = {}, this.readBuffer = 36064, this.drawBuffers = [36064], this.ownResources = [], this.initialize(e), Object.seal(this)
                 }
                 get color() {
@@ -12474,15 +12474,15 @@
                 resize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                         {
                             width: e,
                             height: n
                         } = t;
                     if (null === this.handle) return wd(void 0 === e && void 0 === n), this.width = this.gl.drawingBufferWidth, this.height = this.gl.drawingBufferHeight, this;
-                    void 0 === e && (e = this.gl.drawingBufferWidth), void 0 === n && (n = this.gl.drawingBufferHeight), e !== this.width && n !== this.height && Su.log(2, "Resizing framebuffer ".concat(this.id, " to ").concat(e, "x").concat(n))();
+                    void 0 === e && (e = this.gl.drawingBufferWidth), void 0 === n && (n = this.gl.drawingBufferHeight), e !== this.width && n !== this.height && Pu.log(2, "Resizing framebuffer ".concat(this.id, " to ").concat(e, "x").concat(n))();
                     for (const t in this.attachments) this.attachments[t].resize({
                         width: e,
                         height: n
                     });
                     return this.width = e, this.height = n, this
                 }
                 attach(t) {
@@ -12560,15 +12560,15 @@
                         ! function(t) {
                             let {
                                 framebuffer: e = null,
                                 buffer: n = tp,
                                 drawBuffer: i = 0,
                                 value: r = [0, 0, 0, 0]
                             } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                            Ou(t), cd(t, {
+                            Lu(t), cd(t, {
                                 framebuffer: e
                             }, (() => {
                                 switch (n) {
                                     case tp:
                                         switch (r.constructor) {
                                             case Int32Array:
                                                 t.clearBufferiv(n, i, r);
@@ -12598,77 +12598,77 @@
                         }(this.gl, {
                             drawBuffer: e,
                             value: t
                         })
                     })), this.gl.bindFramebuffer(36160, s || null), this
                 }
                 readPixels() {
-                    return Su.error("Framebuffer.readPixels() is no logner supported, use readPixelsToArray(framebuffer)")(), null
+                    return Pu.error("Framebuffer.readPixels() is no logner supported, use readPixelsToArray(framebuffer)")(), null
                 }
                 readPixelsToBuffer() {
-                    return Su.error("Framebuffer.readPixelsToBuffer()is no logner supported, use readPixelsToBuffer(framebuffer)")(), null
+                    return Pu.error("Framebuffer.readPixelsToBuffer()is no logner supported, use readPixelsToBuffer(framebuffer)")(), null
                 }
                 copyToDataUrl() {
-                    return Su.error("Framebuffer.copyToDataUrl() is no logner supported, use copyToDataUrl(framebuffer)")(), null
+                    return Pu.error("Framebuffer.copyToDataUrl() is no logner supported, use copyToDataUrl(framebuffer)")(), null
                 }
                 copyToImage() {
-                    return Su.error("Framebuffer.copyToImage() is no logner supported, use copyToImage(framebuffer)")(), null
+                    return Pu.error("Framebuffer.copyToImage() is no logner supported, use copyToImage(framebuffer)")(), null
                 }
                 copyToTexture() {
-                    return Su.error("Framebuffer.copyToTexture({...}) is no logner supported, use copyToTexture(source, target, opts})")(), null
+                    return Pu.error("Framebuffer.copyToTexture({...}) is no logner supported, use copyToTexture(source, target, opts})")(), null
                 }
                 blit() {
-                    return Su.error("Framebuffer.blit({...}) is no logner supported, use blit(source, target, opts)")(), null
+                    return Pu.error("Framebuffer.blit({...}) is no logner supported, use blit(source, target, opts)")(), null
                 }
                 invalidate(t) {
                     let {
                         attachments: e = [],
                         x: n = 0,
                         y: i = 0,
                         width: r,
                         height: s
                     } = t;
-                    const o = Ou(this.gl),
+                    const o = Lu(this.gl),
                         a = o.bindFramebuffer(36008, this.handle);
                     return 0 === n && 0 === i && void 0 === r && void 0 === s ? o.invalidateFramebuffer(36008, e) : o.invalidateFramebuffer(36008, e, n, i, r, s), o.bindFramebuffer(36008, a), this
                 }
                 getAttachmentParameter(t, e, n) {
                     let i = this._getAttachmentParameterFallback(e);
-                    return null === i && (this.gl.bindFramebuffer(36160, this.handle), i = this.gl.getFramebufferAttachmentParameter(36160, t, e), this.gl.bindFramebuffer(36160, null)), n && i > 1e3 && (i = Pd(this.gl, i)), i
+                    return null === i && (this.gl.bindFramebuffer(36160, this.handle), i = this.gl.getFramebufferAttachmentParameter(36160, t, e), this.gl.bindFramebuffer(36160, null)), n && i > 1e3 && (i = Sd(this.gl, i)), i
                 }
                 getAttachmentParameters() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 36064,
                         e = arguments.length > 1 ? arguments[1] : void 0,
                         n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : this.constructor.ATTACHMENT_PARAMETERS || [];
                     const i = {};
-                    for (const r of n) i[e ? Pd(this.gl, r) : r] = this.getAttachmentParameter(t, r, e);
+                    for (const r of n) i[e ? Sd(this.gl, r) : r] = this.getAttachmentParameter(t, r, e);
                     return i
                 }
                 getParameters() {
                     let t = !(arguments.length > 0 && void 0 !== arguments[0]) || arguments[0];
                     const e = Object.keys(this.attachments),
                         n = {};
                     for (const i of e) {
                         const e = Number(i);
-                        n[t ? Pd(this.gl, e) : e] = this.getAttachmentParameters(e, t)
+                        n[t ? Sd(this.gl, e) : e] = this.getAttachmentParameters(e, t)
                     }
                     return n
                 }
                 show() {
                     return "undefined" != typeof window && window.open(lp(this), "luma-debug-texture"), this
                 }
                 log() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 0,
                         e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "";
-                    if (t > Su.level || "undefined" == typeof window) return this;
+                    if (t > Pu.level || "undefined" == typeof window) return this;
                     e = e || "Framebuffer ".concat(this.id);
                     const n = lp(this, {
                         targetMaxHeight: 100
                     });
-                    return Su.image({
+                    return Pu.image({
                         logLevel: t,
                         message: e,
                         image: n
                     }, e)(), this
                 }
                 bind() {
                     let {
@@ -12733,15 +12733,15 @@
                     } = t;
                     const {
                         gl: s
                     } = this;
                     switch (s.bindTexture(n.target, n.handle), n.target) {
                         case 35866:
                         case 32879:
-                            Ou(s).framebufferTextureLayer(36160, e, n.target, r, i);
+                            Lu(s).framebufferTextureLayer(36160, e, n.target, r, i);
                             break;
                         case 34067:
                             const t = function(t) {
                                 return t < 34069 ? t + 34069 : t
                             }(i);
                             s.framebufferTexture2D(36160, e, t, n.handle, r);
                             break;
@@ -12757,15 +12757,15 @@
                     const e = Mu(n = this.gl) ? n : null;
                     var n;
                     e ? e.readBuffer(t) : wd(36064 === t || 1029 === t, mp), this.readBuffer = t
                 }
                 _setDrawBuffers(t) {
                     const {
                         gl: e
-                    } = this, n = Ou(e);
+                    } = this, n = Lu(e);
                     if (n) n.drawBuffers(t);
                     else {
                         const n = e.getExtension("WEBGL_draw_buffers");
                         n ? n.drawBuffersWEBGL(t) : wd(1 === t.length && (36064 === t[0] || 1029 === t[0]), mp)
                     }
                     this.drawBuffers = t
                 }
@@ -12801,77 +12801,77 @@
                 }
                 _bindHandle(t) {
                     return this.gl.bindFramebuffer(36160, t)
                 }
             }
             vp.ATTACHMENT_PARAMETERS = [36049, 36048, 33296, 33298, 33299, 33300, 33301, 33302, 33303];
             const bp = {
-                    5126: Rp.bind(null, "uniform1fv", Pp, 1, kp),
-                    35664: Rp.bind(null, "uniform2fv", Pp, 2, kp),
-                    35665: Rp.bind(null, "uniform3fv", Pp, 3, kp),
-                    35666: Rp.bind(null, "uniform4fv", Pp, 4, kp),
-                    5124: Rp.bind(null, "uniform1iv", Sp, 1, kp),
-                    35667: Rp.bind(null, "uniform2iv", Sp, 2, kp),
-                    35668: Rp.bind(null, "uniform3iv", Sp, 3, kp),
-                    35669: Rp.bind(null, "uniform4iv", Sp, 4, kp),
-                    35670: Rp.bind(null, "uniform1iv", Sp, 1, kp),
-                    35671: Rp.bind(null, "uniform2iv", Sp, 2, kp),
-                    35672: Rp.bind(null, "uniform3iv", Sp, 3, kp),
-                    35673: Rp.bind(null, "uniform4iv", Sp, 4, kp),
-                    35674: Rp.bind(null, "uniformMatrix2fv", Pp, 4, Ip),
-                    35675: Rp.bind(null, "uniformMatrix3fv", Pp, 9, Ip),
-                    35676: Rp.bind(null, "uniformMatrix4fv", Pp, 16, Ip),
-                    35678: Op,
-                    35680: Op,
-                    5125: Rp.bind(null, "uniform1uiv", Cp, 1, kp),
-                    36294: Rp.bind(null, "uniform2uiv", Cp, 2, kp),
-                    36295: Rp.bind(null, "uniform3uiv", Cp, 3, kp),
-                    36296: Rp.bind(null, "uniform4uiv", Cp, 4, kp),
-                    35685: Rp.bind(null, "uniformMatrix2x3fv", Pp, 6, Ip),
-                    35686: Rp.bind(null, "uniformMatrix2x4fv", Pp, 8, Ip),
-                    35687: Rp.bind(null, "uniformMatrix3x2fv", Pp, 6, Ip),
-                    35688: Rp.bind(null, "uniformMatrix3x4fv", Pp, 12, Ip),
-                    35689: Rp.bind(null, "uniformMatrix4x2fv", Pp, 8, Ip),
-                    35690: Rp.bind(null, "uniformMatrix4x3fv", Pp, 12, Ip),
-                    35678: Op,
-                    35680: Op,
-                    35679: Op,
-                    35682: Op,
-                    36289: Op,
-                    36292: Op,
-                    36293: Op,
-                    36298: Op,
-                    36299: Op,
-                    36300: Op,
-                    36303: Op,
-                    36306: Op,
-                    36307: Op,
-                    36308: Op,
-                    36311: Op
+                    5126: Ip.bind(null, "uniform1fv", Sp, 1, kp),
+                    35664: Ip.bind(null, "uniform2fv", Sp, 2, kp),
+                    35665: Ip.bind(null, "uniform3fv", Sp, 3, kp),
+                    35666: Ip.bind(null, "uniform4fv", Sp, 4, kp),
+                    5124: Ip.bind(null, "uniform1iv", Pp, 1, kp),
+                    35667: Ip.bind(null, "uniform2iv", Pp, 2, kp),
+                    35668: Ip.bind(null, "uniform3iv", Pp, 3, kp),
+                    35669: Ip.bind(null, "uniform4iv", Pp, 4, kp),
+                    35670: Ip.bind(null, "uniform1iv", Pp, 1, kp),
+                    35671: Ip.bind(null, "uniform2iv", Pp, 2, kp),
+                    35672: Ip.bind(null, "uniform3iv", Pp, 3, kp),
+                    35673: Ip.bind(null, "uniform4iv", Pp, 4, kp),
+                    35674: Ip.bind(null, "uniformMatrix2fv", Sp, 4, Rp),
+                    35675: Ip.bind(null, "uniformMatrix3fv", Sp, 9, Rp),
+                    35676: Ip.bind(null, "uniformMatrix4fv", Sp, 16, Rp),
+                    35678: Lp,
+                    35680: Lp,
+                    5125: Ip.bind(null, "uniform1uiv", Cp, 1, kp),
+                    36294: Ip.bind(null, "uniform2uiv", Cp, 2, kp),
+                    36295: Ip.bind(null, "uniform3uiv", Cp, 3, kp),
+                    36296: Ip.bind(null, "uniform4uiv", Cp, 4, kp),
+                    35685: Ip.bind(null, "uniformMatrix2x3fv", Sp, 6, Rp),
+                    35686: Ip.bind(null, "uniformMatrix2x4fv", Sp, 8, Rp),
+                    35687: Ip.bind(null, "uniformMatrix3x2fv", Sp, 6, Rp),
+                    35688: Ip.bind(null, "uniformMatrix3x4fv", Sp, 12, Rp),
+                    35689: Ip.bind(null, "uniformMatrix4x2fv", Sp, 8, Rp),
+                    35690: Ip.bind(null, "uniformMatrix4x3fv", Sp, 12, Rp),
+                    35678: Lp,
+                    35680: Lp,
+                    35679: Lp,
+                    35682: Lp,
+                    36289: Lp,
+                    36292: Lp,
+                    36293: Lp,
+                    36298: Lp,
+                    36299: Lp,
+                    36300: Lp,
+                    36303: Lp,
+                    36306: Lp,
+                    36307: Lp,
+                    36308: Lp,
+                    36311: Lp
                 },
                 yp = {},
                 _p = {},
                 xp = {},
                 wp = [0];
 
             function Ep(t, e, n, i) {
                 1 === e && "boolean" == typeof t && (t = t ? 1 : 0), Number.isFinite(t) && (wp[0] = t, t = wp);
                 const r = t.length;
-                if (r % e && Su.warn("Uniform size should be multiples of ".concat(e), t)(), t instanceof n) return t;
+                if (r % e && Pu.warn("Uniform size should be multiples of ".concat(e), t)(), t instanceof n) return t;
                 let s = i[r];
                 s || (s = new n(r), i[r] = s);
                 for (let e = 0; e < r; e++) s[e] = t[e];
                 return s
             }
 
-            function Pp(t, e) {
+            function Sp(t, e) {
                 return Ep(t, e, Float32Array, yp)
             }
 
-            function Sp(t, e) {
+            function Pp(t, e) {
                 return Ep(t, e, Int32Array, _p)
             }
 
             function Cp(t, e) {
                 return Ep(t, e, Uint32Array, xp)
             }
 
@@ -12902,32 +12902,32 @@
                     const e = Math.min(t.length, 16);
                     for (let n = 0; n < e; ++n)
                         if (!Number.isFinite(t[n])) return !1;
                     return !0
                 }(t) : !!isFinite(t) || !0 === t || !1 === t || t instanceof Yd || t instanceof Qd || t instanceof vp && Boolean(t.texture)
             }
 
-            function Lp(t, e, n) {
+            function Op(t, e, n) {
                 if (Array.isArray(n) || ArrayBuffer.isView(n))
                     if (t[e]) {
                         const i = t[e];
                         for (let t = 0, e = n.length; t < e; ++t) i[t] = n[t]
                     } else t[e] = n.slice();
                 else t[e] = n
             }
 
-            function Op() {
+            function Lp() {
                 let t = null;
                 return (e, n, i) => {
                     const r = t !== i;
                     return r && (e.uniform1i(n, i), t = i), r
                 }
             }
 
-            function Rp(t, e, n, i) {
+            function Ip(t, e, n, i) {
                 let r = null,
                     s = null;
                 return (o, a, l) => {
                     const c = e(l, n),
                         h = c.length;
                     let u = !1;
                     if (null === r) r = new Float32Array(h), s = h, u = !0;
@@ -12943,15 +12943,15 @@
                 }
             }
 
             function kp(t, e, n, i) {
                 t[e](n, i)
             }
 
-            function Ip(t, e, n, i) {
+            function Rp(t, e, n, i) {
                 t[e](n, !1, i)
             }
 
             function jp(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "unnamed";
                 const n = t.match(/#define[\s*]SHADER_NAME[\s*]([A-Za-z0-9_-]+)[\s*]/);
                 return n ? n[1] : e
@@ -12974,30 +12974,30 @@
             }
 
             function Fp(t, e) {
                 let n = "";
                 for (let t = 0; t < e; ++t) n += " ";
                 return "".concat(n).concat(t)
             }
-            class Bp extends Od {
+            class Bp extends Ld {
                 get[Symbol.toStringTag]() {
                     return "Shader"
                 }
                 static getTypeName(t) {
                     switch (t) {
                         case 35633:
                             return "vertex-shader";
                         case 35632:
                             return "fragment-shader";
                         default:
                             return wd(!1), "unknown"
                     }
                 }
                 constructor(t, e) {
-                    Lu(t), wd("string" == typeof e.source, "Shader: GLSL source code must be a JavaScript string"), super(t, {
+                    Ou(t), wd("string" == typeof e.source, "Shader: GLSL source code must be a JavaScript string"), super(t, {
                         id: jp(e.source, null) || e.id || Cd("unnamed ".concat(Bp.getTypeName(e.shaderType)))
                     }), this.shaderType = e.shaderType, this.source = e.source, this.initialize(e)
                 }
                 initialize(t) {
                     let {
                         source: e
                     } = t;
@@ -13065,43 +13065,43 @@
                                 }(e);
                                 return {
                                     shaderName: l,
                                     errors: zp(s, c),
                                     warnings: zp(o, c)
                                 }
                             }(t, this.source, this.shaderType, this.id);
-                        throw Su.error("GLSL compilation errors in ".concat(e, "\n").concat(n))(), Su.warn("GLSL compilation warnings in ".concat(e, "\n").concat(i))(), new Error("GLSL compilation errors in ".concat(e))
+                        throw Pu.error("GLSL compilation errors in ".concat(e, "\n").concat(n))(), Pu.warn("GLSL compilation warnings in ".concat(e, "\n").concat(i))(), new Error("GLSL compilation errors in ".concat(e))
                     }
                 }
                 _deleteHandle() {
                     this.gl.deleteShader(this.handle)
                 }
                 _getOptsFromHandle() {
                     return {
                         type: this.getParameter(35663),
                         source: this.getSource()
                     }
                 }
             }
-            class Dp extends Bp {
+            class Np extends Bp {
                 get[Symbol.toStringTag]() {
                     return "VertexShader"
                 }
                 constructor(t, e) {
                     "string" == typeof e && (e = {
                         source: e
                     }), super(t, Object.assign({}, e, {
                         shaderType: 35633
                     }))
                 }
                 _createHandle() {
                     return this.gl.createShader(35633)
                 }
             }
-            class Np extends Bp {
+            class Dp extends Bp {
                 get[Symbol.toStringTag]() {
                     return "FragmentShader"
                 }
                 constructor(t, e) {
                     "string" == typeof e && (e = {
                         source: e
                     }), super(t, Object.assign({}, e, {
@@ -13114,28 +13114,28 @@
             }
             const Vp = 5120,
                 Up = 5121,
                 Gp = 5122,
                 Wp = 5123,
                 Hp = 5126,
                 Zp = 5124,
-                qp = 5125,
-                Xp = {
+                Xp = 5125,
+                qp = {
                     [Hp]: [Hp, 1, "float"],
                     35664: [Hp, 2, "vec2"],
                     35665: [Hp, 3, "vec3"],
                     35666: [Hp, 4, "vec4"],
                     [Zp]: [Zp, 1, "int"],
                     35667: [Zp, 2, "ivec2"],
                     35668: [Zp, 3, "ivec3"],
                     35669: [Zp, 4, "ivec4"],
-                    [qp]: [qp, 1, "uint"],
-                    36294: [qp, 2, "uvec2"],
-                    36295: [qp, 3, "uvec3"],
-                    36296: [qp, 4, "uvec4"],
+                    [Xp]: [Xp, 1, "uint"],
+                    36294: [Xp, 2, "uvec2"],
+                    36295: [Xp, 3, "uvec3"],
+                    36296: [Xp, 4, "uvec4"],
                     35670: [Hp, 1, "bool"],
                     35671: [Hp, 2, "bvec2"],
                     35672: [Hp, 3, "bvec3"],
                     35673: [Hp, 4, "bvec4"],
                     35674: [Hp, 8, "mat2"],
                     35685: [Hp, 8, "mat2x3"],
                     35686: [Hp, 8, "mat2x4"],
@@ -13144,15 +13144,15 @@
                     35688: [Hp, 12, "mat3x4"],
                     35676: [Hp, 16, "mat4"],
                     35689: [Hp, 16, "mat4x2"],
                     35690: [Hp, 16, "mat4x3"]
                 };
 
             function Yp(t) {
-                const e = Xp[t];
+                const e = qp[t];
                 if (!e) return null;
                 const [n, i] = e;
                 return {
                     type: n,
                     components: i
                 }
             }
@@ -13161,16 +13161,16 @@
                 switch (t) {
                     case Vp:
                     case Up:
                     case Gp:
                     case Wp:
                         t = Hp
                 }
-                for (const n in Xp) {
-                    const [i, r, s] = Xp[n];
+                for (const n in qp) {
+                    const [i, r, s] = qp[n];
                     if (i === t && r === e) return {
                         glType: n,
                         name: s
                     }
                 }
                 return null
             }
@@ -13240,39 +13240,39 @@
                         type: r,
                         size: i * s
                     };
                     this._inferProperties(t, e, o);
                     const a = {
                         location: t,
                         name: e,
-                        accessor: new Dd(o)
+                        accessor: new Nd(o)
                     };
                     this.attributeInfos.push(a), this.attributeInfosByLocation[t] = a, this.attributeInfosByName[a.name] = a
                 }
                 _inferProperties(t, e, n) {
                     /instance/i.test(e) && (n.divisor = 1)
                 }
                 _addVarying(t, e, n, i) {
                     const {
                         type: r,
                         components: s
                     } = Yp(n), o = {
                         location: t,
                         name: e,
-                        accessor: new Dd({
+                        accessor: new Nd({
                             type: r,
                             size: i * s
                         })
                     };
                     this.varyingInfos.push(o), this.varyingInfosByName[o.name] = o
                 }
             }
             const Jp = 35981,
                 Qp = ["setVertexArray", "setAttributes", "setBuffers", "unsetBuffers", "use", "getUniformCount", "getUniformInfo", "getUniformLocation", "getUniformValue", "getVarying", "getFragDataLocation", "getAttachedShaders", "getAttributeCount", "getAttributeLocation", "getAttributeInfo"];
-            class tf extends Od {
+            class tf extends Ld {
                 get[Symbol.toStringTag]() {
                     return "Program"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     super(t, e), this.stubRemovedMethods("Program", "v6.0", Qp), this._isCached = !1, this.initialize(e), Object.seal(this), this._setId(e.id)
                 }
@@ -13281,21 +13281,21 @@
                     const {
                         hash: e,
                         vs: n,
                         fs: i,
                         varyings: r,
                         bufferMode: s = Jp
                     } = t;
-                    return this.hash = e || "", this.vs = "string" == typeof n ? new Dp(this.gl, {
+                    return this.hash = e || "", this.vs = "string" == typeof n ? new Np(this.gl, {
                         id: "".concat(t.id, "-vs"),
                         source: n
-                    }) : n, this.fs = "string" == typeof i ? new Np(this.gl, {
+                    }) : n, this.fs = "string" == typeof i ? new Dp(this.gl, {
                         id: "".concat(t.id, "-fs"),
                         source: i
-                    }) : i, wd(this.vs instanceof Dp), wd(this.fs instanceof Np), this.uniforms = {}, this._textureUniforms = {}, r && r.length > 0 && (Ou(this.gl), this.varyings = r, this.gl2.transformFeedbackVaryings(this.handle, r, s)), this._compileAndLink(), this._readUniformLocationsFromLinkedProgram(), this.configuration = new $p(this), this.setProps(t)
+                    }) : i, wd(this.vs instanceof Np), wd(this.fs instanceof Dp), this.uniforms = {}, this._textureUniforms = {}, r && r.length > 0 && (Lu(this.gl), this.varyings = r, this.gl2.transformFeedbackVaryings(this.handle, r, s)), this._compileAndLink(), this._readUniformLocationsFromLinkedProgram(), this.configuration = new $p(this), this.setProps(t)
                 }
                 delete() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this._isCached ? this : super.delete(t)
                 }
                 setProps(t) {
                     return "uniforms" in t && this.setUniforms(t.uniforms), this
@@ -13315,18 +13315,18 @@
                         vertexArray: u = null,
                         transformFeedback: d,
                         framebuffer: p,
                         parameters: f = {},
                         uniforms: g,
                         samplers: m
                     } = t;
-                    if ((g || m) && (Su.deprecated("Program.draw({uniforms})", "Program.setUniforms(uniforms)")(), this.setUniforms(g || {})), Su.priority >= e) {
+                    if ((g || m) && (Pu.deprecated("Program.draw({uniforms})", "Program.setUniforms(uniforms)")(), this.setUniforms(g || {})), Pu.priority >= e) {
                         const t = p ? p.id : "default",
-                            r = "mode=".concat(Pd(this.gl, n), " verts=").concat(i, " ") + "instances=".concat(c, " indexType=").concat(Pd(this.gl, l), " ") + "isInstanced=".concat(h, " isIndexed=").concat(a, " ") + "Framebuffer=".concat(t);
-                        Su.log(e, r)()
+                            r = "mode=".concat(Sd(this.gl, n), " verts=").concat(i, " ") + "instances=".concat(c, " indexType=").concat(Sd(this.gl, l), " ") + "isInstanced=".concat(h, " isIndexed=").concat(a, " ") + "Framebuffer=".concat(t);
+                        Pu.log(e, r)()
                     }
                     return wd(u), this.gl.useProgram(this.handle), !(!this._areTexturesRenderable() || 0 === i || h && 0 === c || (u.bindForDraw(i, c, (() => {
                         if (void 0 !== p && (f = Object.assign({}, f, {
                                 framebuffer: p
                             })), d) {
                             const t = function(t) {
                                 switch (t) {
@@ -13349,15 +13349,15 @@
                         this._bindTextures(), cd(this.gl, f, (() => {
                             a && h ? this.gl2.drawElementsInstanced(n, i, l, r, c) : a && Mu(this.gl) && !isNaN(s) && !isNaN(o) ? this.gl2.drawRangeElements(n, s, o, i, l, r) : a ? this.gl.drawElements(n, i, l, r) : h ? this.gl2.drawArraysInstanced(n, r, i, c) : this.gl.drawArrays(n, r, i)
                         })), d && d.end()
                     })), 0))
                 }
                 setUniforms() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    Su.priority >= 2 && function(t, e, n) {
+                    Pu.priority >= 2 && function(t, e, n) {
                         for (const i in t) {
                             const r = t[i];
                             if ((!n || Boolean(n[i])) && !Mp(r)) throw e = e ? "".concat(e, " ") : "", console.error("".concat(e, " Bad uniform ").concat(i), r), new Error("".concat(e, " Bad uniform ").concat(i))
                         }
                     }(t, this.id, this._uniformSetters), this.gl.useProgram(this.handle);
                     for (const e in t) {
                         const n = t[e],
@@ -13371,15 +13371,15 @@
                                     const n = t,
                                         {
                                             textureIndex: r
                                         } = i;
                                     n.bind(r), t = r, this._textureUniforms[e] = n
                                 } else t = i.textureIndex;
                             else this._textureUniforms[e] && delete this._textureUniforms[e];
-                            (i(t) || r) && Lp(this.uniforms, e, n)
+                            (i(t) || r) && Op(this.uniforms, e, n)
                         }
                     }
                     return this
                 }
                 _areTexturesRenderable() {
                     let t = !0;
                     for (const e in this._textureUniforms) {
@@ -13401,20 +13401,20 @@
                     this.gl.deleteProgram(this.handle)
                 }
                 _getOptionsFromHandle(t) {
                     const e = this.gl.getAttachedShaders(t),
                         n = {};
                     for (const t of e) switch (this.gl.getShaderParameter(this.handle, 35663)) {
                         case 35633:
-                            n.vs = new Dp({
+                            n.vs = new Np({
                                 handle: t
                             });
                             break;
                         case 35632:
-                            n.fs = new Np({
+                            n.fs = new Dp({
                                 handle: t
                             })
                     }
                     return n
                 }
                 _getParameter(t) {
                     return this.gl.getProgramParameter(this.handle, t)
@@ -13429,15 +13429,15 @@
                     let t = this.vs.getName() || this.fs.getName();
                     return t = t.replace(/shader/i, ""), t = t ? "".concat(t, "-program") : "program", t
                 }
                 _compileAndLink() {
                     const {
                         gl: t
                     } = this;
-                    if (t.attachShader(this.handle, this.vs.handle), t.attachShader(this.handle, this.fs.handle), Su.time(4, "linkProgram for ".concat(this._getName()))(), t.linkProgram(this.handle), Su.timeEnd(4, "linkProgram for ".concat(this._getName()))(), t.debug || Su.level > 0) {
+                    if (t.attachShader(this.handle, this.vs.handle), t.attachShader(this.handle, this.fs.handle), Pu.time(4, "linkProgram for ".concat(this._getName()))(), t.linkProgram(this.handle), Pu.timeEnd(4, "linkProgram for ".concat(this._getName()))(), t.debug || Pu.level > 0) {
                         if (!t.getProgramParameter(this.handle, 35714)) throw new Error("Error linking: ".concat(t.getProgramInfoLog(this.handle)));
                         if (t.validateProgram(this.handle), !t.getProgramParameter(this.handle, 35715)) throw new Error("Error validating: ".concat(t.getProgramInfoLog(this.handle)))
                     }
                 }
                 _readUniformLocationsFromLinkedProgram() {
                     const {
                         gl: t
@@ -13511,18 +13511,18 @@
                                 vs: Eu(t, Object.assign({}, e, {
                                     source: n,
                                     type: Bh,
                                     modules: r
                                 })),
                                 fs: Eu(t, Object.assign({}, e, {
                                     source: i,
-                                    type: Dh,
+                                    type: Nh,
                                     modules: r
                                 })),
-                                getUniforms: Pu(r)
+                                getUniforms: Su(r)
                             }
                         }(this.gl, {
                             vs: e,
                             fs: n,
                             modules: l,
                             inject: r,
                             defines: i,
@@ -13628,24 +13628,24 @@
                             viewProjectionMatrix: o
                         } = t, a = uf, l = uf, c = t.cameraPosition;
                         const {
                             geospatialOrigin: h,
                             shaderCoordinateOrigin: u,
                             offsetMode: d
                         } = vf(t, e, n);
-                        return d && (l = t.projectPosition(h || u), c = [c[0] - l[0], c[1] - l[1], c[2] - l[2]], l[3] = 1, a = qc([], l, o), s = i || s, o = Fc([], r, s), o = Fc([], o, df)), {
+                        return d && (l = t.projectPosition(h || u), c = [c[0] - l[0], c[1] - l[1], c[2] - l[2]], l[3] = 1, a = Xc([], l, o), s = i || s, o = Fc([], r, s), o = Fc([], o, df)), {
                             viewMatrix: s,
                             viewProjectionMatrix: o,
                             projectionCenter: a,
                             originCommon: l,
                             cameraPosCommon: c,
                             shaderCoordinateOrigin: u,
                             geospatialOrigin: h
                         }
-                    }(t, n, i), h = t.getDistanceScales(), u = [t.width * e, t.height * e], d = qc([], [0, 0, -t.focalDistance, 1], t.projectionMatrix)[3] || 1, p = {
+                    }(t, n, i), h = t.getDistanceScales(), u = [t.width * e, t.height * e], d = Xc([], [0, 0, -t.focalDistance, 1], t.projectionMatrix)[3] || 1, p = {
                         project_uCoordinateSystem: n,
                         project_uProjectionMode: t.projectionMode,
                         project_uCoordinateOrigin: l,
                         project_uCommonOrigin: o.slice(0, 3),
                         project_uCenter: r,
                         project_uPseudoMeters: Boolean(t._pseudoMeters),
                         project_uViewportSize: u,
@@ -13762,15 +13762,15 @@
                         programManager: t && wf(t),
                         stats: n || new ca({
                             id: "deck.gl"
                         }),
                         viewport: i || new Fh({
                             id: "DEFAULT-INITIAL-VIEWPORT"
                         }),
-                        timeline: r || new So,
+                        timeline: r || new Po,
                         resourceManager: this.resourceManager,
                         onError: void 0
                     }, Object.seal(this)
                 }
                 finalize() {
                     this.resourceManager.finalize();
                     for (const t of this.layers) this._finalizeLayer(t)
@@ -13871,25 +13871,25 @@
                         t._finalize(), t.lifecycle = "Finalized! Awaiting garbage collection"
                     } catch (e) {
                         this._handleError("finalization", e, t)
                     }
                 }
             }
 
-            function Pf(t, e) {
+            function Sf(t, e) {
                 if (t === e) return !0;
                 if (!t || !e) return !1;
                 for (const n in t) {
                     const i = t[n],
                         r = e[n];
-                    if (!(i === r || Array.isArray(i) && Array.isArray(r) && Pf(i, r))) return !1
+                    if (!(i === r || Array.isArray(i) && Array.isArray(r) && Sf(i, r))) return !1
                 }
                 return !0
             }
-            class Sf {
+            class Pf {
                 constructor(t) {
                     wo(this, "width", void 0), wo(this, "height", void 0), wo(this, "views", void 0), wo(this, "viewState", void 0), wo(this, "controllers", void 0), wo(this, "timeline", void 0), wo(this, "_viewports", void 0), wo(this, "_viewportMap", void 0), wo(this, "_isUpdating", void 0), wo(this, "_needsRedraw", void 0), wo(this, "_needsUpdate", void 0), wo(this, "_eventManager", void 0), wo(this, "_eventCallbacks", void 0), this.views = [], this.width = 100, this.height = 100, this.viewState = {}, this.controllers = {}, this.timeline = t.timeline, this._viewports = [], this._viewportMap = {}, this._isUpdating = !1, this._needsRedraw = "First render", this._needsUpdate = "Initialize", this._eventManager = t.eventManager, this._eventCallbacks = {
                         onViewStateChange: t.onViewStateChange,
                         onInteractionStateChange: t.onInteractionStateChange
                     }, Object.seal(this), this.setProps(t)
                 }
                 finalize() {
@@ -13958,15 +13958,15 @@
                 _setSize(t, e) {
                     t === this.width && e === this.height || (this.width = t, this.height = e, this.setNeedsUpdate("Size changed"))
                 }
                 _setViews(t) {
                     t = ia(t, Boolean), this._diffViews(t, this.views) && this.setNeedsUpdate("views changed"), this.views = t
                 }
                 _setViewState(t) {
-                    t ? (!Pf(t, this.viewState) && this.setNeedsUpdate("viewState changed"), this.viewState = t) : ta.warn("missing `viewState` or `initialViewState`")()
+                    t ? (!Sf(t, this.viewState) && this.setNeedsUpdate("viewState changed"), this.viewState = t) : ta.warn("missing `viewState` or `initialViewState`")()
                 }
                 _onViewStateChange(t, e) {
                     this._eventCallbacks.onViewStateChange && this._eventCallbacks.onViewStateChange({
                         ...e,
                         viewId: t
                     })
                 }
@@ -14061,15 +14061,15 @@
             function Af(t, e) {
                 return t.relative ? Math.round(t.position * e) : t.position
             }
 
             function Mf(t, e) {
                 if (!t) throw new Error(e || "deck.gl: assertion failed.")
             }
-            class Lf {
+            class Of {
                 constructor(t) {
                     wo(this, "id", void 0), wo(this, "viewportInstance", void 0), wo(this, "_x", void 0), wo(this, "_y", void 0), wo(this, "_width", void 0), wo(this, "_height", void 0), wo(this, "_padding", void 0), wo(this, "props", void 0);
                     const {
                         id: e,
                         x: n = 0,
                         y: i = 0,
                         width: r = "100%",
@@ -14084,15 +14084,15 @@
                         left: Tf(o.left || 0),
                         right: Tf(o.right || 0),
                         top: Tf(o.top || 0),
                         bottom: Tf(o.bottom || 0)
                     }, this.equals = this.equals.bind(this), Object.seal(this)
                 }
                 equals(t) {
-                    return this === t || (this.viewportInstance ? !!t.viewportInstance && this.viewportInstance.equals(t.viewportInstance) : this.ViewportType === t.ViewportType && Pf(this.props, t.props))
+                    return this === t || (this.viewportInstance ? !!t.viewportInstance && this.viewportInstance.equals(t.viewportInstance) : this.ViewportType === t.ViewportType && Sf(this.props, t.props))
                 }
                 makeViewport({
                     width: t,
                     height: e,
                     viewState: n
                 }) {
                     if (this.viewportInstance) return this.viewportInstance;
@@ -14149,18 +14149,18 @@
                         type: t
                     } : {
                         type: this.ControllerType,
                         ...t
                     } : null
                 }
             }
-            const Of = Math.PI / 180;
+            const Lf = Math.PI / 180;
 
-            function Rf(t) {
-                return 512 / 4003e4 / Math.cos(t * Of)
+            function If(t) {
+                return 512 / 4003e4 / Math.cos(t * Lf)
             }
             class kf extends Fh {
                 constructor(t = {}) {
                     const {
                         latitude: e = 0,
                         longitude: n = 0,
                         zoom: i = 0,
@@ -14228,18 +14228,18 @@
                             height: e,
                             pitch: n,
                             bearing: i,
                             altitude: r,
                             scale: s,
                             center: o
                         } = t, a = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1];
-                        Bc(a, a, [0, 0, -r]), Nc(a, a, -n * hh), Vc(a, a, i * hh);
+                        Bc(a, a, [0, 0, -r]), Dc(a, a, -n * hh), Vc(a, a, i * hh);
                         const l = s / e;
                         var c, h;
-                        return Dc(a, a, [l, l, l]), o && Bc(a, a, ((c = [])[0] = -(h = o)[0], c[1] = -h[1], c[2] = -h[2], c)), a
+                        return Nc(a, a, [l, l, l]), o && Bc(a, a, ((c = [])[0] = -(h = o)[0], c[1] = -h[1], c[2] = -h[2], c)), a
                     }({
                         height: f,
                         pitch: r,
                         bearing: s,
                         scale: m,
                         altitude: g
                     });
@@ -14270,20 +14270,20 @@
                         }
                     }
                     return this._subViewports
                 }
                 projectPosition(t) {
                     if (this._pseudoMeters) return super.projectPosition(t);
                     const [e, n] = this.projectFlat(t);
-                    return [e, n, (t[2] || 0) * Rf(t[1])]
+                    return [e, n, (t[2] || 0) * If(t[1])]
                 }
                 unprojectPosition(t) {
                     if (this._pseudoMeters) return super.unprojectPosition(t);
                     const [e, n] = this.unprojectFlat(t);
-                    return [e, n, (t[2] || 0) / Rf(n)]
+                    return [e, n, (t[2] || 0) / If(n)]
                 }
                 addMetersToLngLat(t, e) {
                     return yh(t, e)
                 }
                 panByPosition(t, e) {
                     const n = Eh(e, this.pixelUnprojectionMatrix),
                         i = Gc([], this.projectFlat(t), Wc([], n)),
@@ -14300,27 +14300,27 @@
                             width: n,
                             height: i,
                             unproject: r
                         } = t, s = {
                             targetZ: e
                         }, o = r([0, i], s), a = r([n, i], s);
                         let l, c;
-                        return (t.fovy ? .5 * t.fovy * Sh : Math.atan(.5 / t.altitude)) > (90 - t.pitch) * Sh - .01 ? (l = Ch(t, 0, e), c = Ch(t, n, e)) : (l = r([0, 0], s), c = r([n, 0], s)), [o, a, c, l]
+                        return (t.fovy ? .5 * t.fovy * Ph : Math.atan(.5 / t.altitude)) > (90 - t.pitch) * Ph - .01 ? (l = Ch(t, 0, e), c = Ch(t, n, e)) : (l = r([0, 0], s), c = r([n, 0], s)), [o, a, c, l]
                     }(this, t.z || 0);
                     return [Math.min(e[0][0], e[1][0], e[2][0], e[3][0]), Math.min(e[0][1], e[1][1], e[2][1], e[3][1]), Math.max(e[0][0], e[1][0], e[2][0], e[3][0]), Math.max(e[0][1], e[1][1], e[2][1], e[3][1])]
                 }
                 fitBounds(t, e = {}) {
                     const {
                         width: n,
                         height: i
                     } = this, {
                         longitude: r,
                         latitude: s,
                         zoom: o
-                    } = Ph({
+                    } = Sh({
                         width: n,
                         height: i,
                         bounds: t,
                         ...e
                     });
                     return new kf({
                         width: n,
@@ -14328,15 +14328,15 @@
                         longitude: r,
                         latitude: s,
                         zoom: o
                     })
                 }
             }
             wo(kf, "displayName", "WebMercatorViewport");
-            class If {
+            class Rf {
                 constructor(t) {
                     wo(this, "_inProgress", void 0), wo(this, "_handle", void 0), wo(this, "_timeline", void 0), wo(this, "time", void 0), wo(this, "settings", void 0), this._inProgress = !1, this._handle = null, this._timeline = t, this.time = 0, this.settings = {
                         duration: 0
                     }
                 }
                 get inProgress() {
                     return this._inProgress
@@ -14388,15 +14388,15 @@
                         this.propsInTransition = this.getControllerState({
                             ...this.props,
                             ...l
                         }).getViewportProps(), this.onViewStateChange({
                             viewState: this.propsInTransition,
                             oldViewState: this.props
                         })
-                    })), this.getControllerState = t.getControllerState, this.propsInTransition = null, this.transition = new If(t.timeline), this.onViewStateChange = t.onViewStateChange || jf, this.onStateChange = t.onStateChange || jf
+                    })), this.getControllerState = t.getControllerState, this.propsInTransition = null, this.transition = new Rf(t.timeline), this.onViewStateChange = t.onViewStateChange || jf, this.onStateChange = t.onStateChange || jf
                 }
                 finalize() {
                     this.transition.cancel()
                 }
                 getViewportInTransition() {
                     return this.propsInTransition
                 }
@@ -14501,26 +14501,26 @@
                 _checkRequiredProps(t) {
                     this._requiredProps && this._requiredProps.forEach((e => {
                         const n = t[e];
                         Mf(Number.isFinite(n) || Array.isArray(n), "".concat(e, " is required for transition"))
                     }))
                 }
             }
-            const Df = ["longitude", "latitude", "zoom", "bearing", "pitch"],
-                Nf = ["longitude", "latitude", "zoom"];
+            const Nf = ["longitude", "latitude", "zoom", "bearing", "pitch"],
+                Df = ["longitude", "latitude", "zoom"];
             class Vf extends Bf {
                 constructor(t = {}) {
                     const e = Array.isArray(t) ? t : t.transitionProps,
                         n = Array.isArray(t) ? {} : t;
                     n.transitionProps = Array.isArray(e) ? {
                         compare: e,
                         required: e
                     } : e || {
-                        compare: Df,
-                        required: Nf
+                        compare: Nf,
+                        required: Df
                     }, super(n.transitionProps), wo(this, "opts", void 0), this.opts = n
                 }
                 initializeProps(t, e) {
                     const n = super.initializeProps(t, e),
                         {
                             makeViewport: i,
                             around: r
@@ -14554,16 +14554,16 @@
             const Uf = {
                     transitionDuration: 0
                 },
                 Gf = t => 1 - (1 - t) * (1 - t),
                 Wf = ["wheel"],
                 Hf = ["panstart", "panmove", "panend"],
                 Zf = ["pinchstart", "pinchmove", "pinchend"],
-                qf = ["tripanstart", "tripanmove", "tripanend"],
-                Xf = ["doubletap"],
+                Xf = ["tripanstart", "tripanmove", "tripanend"],
+                qf = ["doubletap"],
                 Yf = ["keydown"],
                 Kf = {};
             class $f {
                 constructor(t) {
                     wo(this, "props", void 0), wo(this, "state", {}), wo(this, "transitionManager", void 0), wo(this, "eventManager", void 0), wo(this, "onViewStateChange", void 0), wo(this, "onStateChange", void 0), wo(this, "makeViewport", void 0), wo(this, "_controllerState", void 0), wo(this, "_events", {}), wo(this, "_interactionState", {
                         isDragging: !1
                     }), wo(this, "_customEvents", []), wo(this, "_eventStartBlocked", null), wo(this, "_panMove", !1), wo(this, "invertPan", !1), wo(this, "dragMode", "rotate"), wo(this, "inertia", 0), wo(this, "scrollZoom", !0), wo(this, "dragPan", !0), wo(this, "dragRotate", !0), wo(this, "doubleClickZoom", !0), wo(this, "touchZoom", !0), wo(this, "touchRotate", !1), wo(this, "keyboard", !0), this.transitionManager = new Ff({
@@ -14666,15 +14666,15 @@
                         dragPan: i = !0,
                         dragRotate: r = !0,
                         doubleClickZoom: s = !0,
                         touchZoom: o = !0,
                         touchRotate: a = !1,
                         keyboard: l = !0
                     } = t, c = Boolean(this.onViewStateChange);
-                    this.toggleEvents(Wf, c && n), this.toggleEvents(Hf, c && (i || r)), this.toggleEvents(Zf, c && (o || a)), this.toggleEvents(qf, c && a), this.toggleEvents(Xf, c && s), this.toggleEvents(Yf, c && l), this.scrollZoom = n, this.dragPan = i, this.dragRotate = r, this.doubleClickZoom = s, this.touchZoom = o, this.touchRotate = a, this.keyboard = l
+                    this.toggleEvents(Wf, c && n), this.toggleEvents(Hf, c && (i || r)), this.toggleEvents(Zf, c && (o || a)), this.toggleEvents(Xf, c && a), this.toggleEvents(qf, c && s), this.toggleEvents(Yf, c && l), this.scrollZoom = n, this.dragPan = i, this.dragRotate = r, this.doubleClickZoom = s, this.touchZoom = o, this.touchRotate = a, this.keyboard = l
                 }
                 updateTransition() {
                     this.transitionManager.updateTransition()
                 }
                 toggleEvents(t, e) {
                     this.eventManager && t.forEach((t => {
                         this._events[t] !== e && (this._events[t] = e, e ? this.eventManager.on(t, this.handleEvent) : this.eventManager.off(t, this.handleEvent))
@@ -15347,15 +15347,15 @@
                     super.setProps(t), (!e || e.height !== t.height) && this.updateViewport(new this.ControllerState({
                         makeViewport: this.makeViewport,
                         ...t,
                         ...this.state
                     }))
                 }
             }
-            class eg extends Lf {
+            class eg extends Of {
                 get ViewportType() {
                     return kf
                 }
                 get ControllerType() {
                     return tg
                 }
             }
@@ -15386,15 +15386,15 @@
                     } = t, {
                         intensity: n = ag
                     } = t, {
                         direction: i = lg
                     } = t, {
                         _shadow: r = !1
                     } = t;
-                    this.id = t.id || "directional-".concat(cg++), this.color = e, this.intensity = n, this.type = "directional", this.direction = new Lc(i).normalize().toArray(), this.shadow = r
+                    this.id = t.id || "directional-".concat(cg++), this.color = e, this.intensity = n, this.type = "directional", this.direction = new Oc(i).normalize().toArray(), this.shadow = r
                 }
                 getProjectedLight(t) {
                     return this
                 }
             }
             class ug {
                 constructor(t, e = {
@@ -15694,15 +15694,15 @@
                             [0, t.height, -1],
                             [t.width, t.height, -1]
                         ].map((t => function(t, e) {
                             const [n, i, r] = t, s = Eh([n, i, r], e);
                             return Number.isFinite(r) ? s : [s[0], s[1], 0]
                         }(t, i)));
                     for (const i of e) {
-                        const e = i.clone().translate(new Lc(t.center).negate()),
+                        const e = i.clone().translate(new Oc(t.center).negate()),
                             r = s.map((t => e.transform(t))),
                             o = (new Qc).ortho({
                                 left: Math.min(...r.map((t => t[0]))),
                                 right: Math.max(...r.map((t => t[0]))),
                                 bottom: Math.min(...r.map((t => t[1]))),
                                 top: Math.max(...r.map((t => t[1]))),
                                 near: Math.min(...r.map((t => -t[2]))),
@@ -15745,15 +15745,15 @@
                             s = [],
                             o = mg({
                                 shadowMatrices: t.shadowMatrices,
                                 viewport: t.viewport
                             }).slice();
                         for (let n = 0; n < t.shadowMatrices.length; n++) {
                             const i = o[n],
-                                a = i.clone().translate(new Lc(t.viewport.center).negate());
+                                a = i.clone().translate(new Oc(t.viewport.center).negate());
                             e.project_uCoordinateSystem === Th.LNGLAT && e.project_uProjectionMode === Ah.WEB_MERCATOR ? (o[n] = a, s[n] = r) : (o[n] = i.clone().multiplyRight(bg), s[n] = a.transform(r))
                         }
                         for (let e = 0; e < o.length; e++) i["shadow_uViewProjectionMatrices[".concat(e, "]")] = o[e], i["shadow_uProjectCenters[".concat(e, "]")] = s[e], t.shadowMaps && t.shadowMaps.length > 0 ? i["shadow_uShadowMap".concat(e)] = t.shadowMaps[e] : i["shadow_uShadowMap".concat(e)] = t.dummyShadowMap;
                         return i
                     }(t, e) : {}
                 },
                 _g = {
@@ -15835,15 +15835,15 @@
                     for (const t of this.shadowPasses) t.delete();
                     this.shadowPasses.length = 0, this.shadowMaps.length = 0, this.dummyShadowMap && (this.dummyShadowMap.delete(), this.dummyShadowMap = null), this.shadow && this.programManager && (this.programManager.removeDefaultModule(yg), this.programManager = null)
                 }
                 _calculateMatrices() {
                     const t = [];
                     for (const e of this.directionalLights) {
                         const n = (new Qc).lookAt({
-                            eye: new Lc(e.direction).negate()
+                            eye: new Oc(e.direction).negate()
                         });
                         t.push(n)
                     }
                     return t
                 }
                 _createShadowPasses(t) {
                     for (let e = 0; e < this.directionalLights.length; e++) {
@@ -15856,15 +15856,15 @@
                         ambientLight: t,
                         pointLights: e,
                         directionalLights: n
                     } = this;
                     t || 0 !== e.length || 0 !== n.length || (this.ambientLight = new sg(_g), this.directionalLights.push(new hg(xg[0]), new hg(xg[1])))
                 }
             }
-            class Pg extends dg {
+            class Sg extends dg {
                 constructor(t, e) {
                     super(t, e), wo(this, "maskMap", void 0), wo(this, "fbo", void 0);
                     const {
                         mapSize: n = 2048
                     } = e;
                     this.maskMap = new Kd(t, {
                         width: n,
@@ -15897,21 +15897,21 @@
                     }, (() => super.render({
                         ...t,
                         target: this.fbo,
                         pass: "mask"
                     })))
                 }
                 shouldDrawLayer(t) {
-                    return t.props.operation === Rh
+                    return t.props.operation === Ih
                 }
                 delete() {
                     this.fbo.delete(), this.maskMap.delete()
                 }
             }
-            const Sg = (new Qc).lookAt({
+            const Pg = (new Qc).lookAt({
                 eye: [0, 0, 1]
             });
 
             function Cg({
                 width: t,
                 height: e,
                 near: n,
@@ -15961,15 +15961,15 @@
                             metersPerUnit: [d / t, d / e, 1]
                         }
                     }
                     super({
                         ...t,
                         longitude: void 0,
                         position: o,
-                        viewMatrix: Sg.clone().scale([d, d * (l ? -1 : 1), d]),
+                        viewMatrix: Pg.clone().scale([d, d * (l ? -1 : 1), d]),
                         projectionMatrix: Cg({
                             width: e || 1,
                             height: n || 1,
                             padding: a,
                             near: i,
                             far: r
                         }),
@@ -16270,52 +16270,52 @@
                                 e < i && (r += i - e), e = Math.max(t + r, s + r), e > n && (r += n - e), t += r, s += r
                         }
                         return [t, s]
                     }
                     return oc(e + r, i, n)
                 }
             }
-            class Lg extends $f {
+            class Og extends $f {
                 constructor(...t) {
                     super(...t), wo(this, "ControllerState", Mg), wo(this, "transition", {
                         transitionDuration: 300,
                         transitionInterpolator: new Vf(["target", "zoom"])
                     }), wo(this, "dragMode", "pan")
                 }
                 _onPanRotate() {
                     return !1
                 }
             }
-            class Og extends Lf {
+            class Lg extends Of {
                 get ViewportType() {
                     return Tg
                 }
                 get ControllerType() {
-                    return Lg
+                    return Og
                 }
             }
-            wo(Og, "displayName", "OrthographicView");
-            class Rg {
+            wo(Lg, "displayName", "OrthographicView");
+            class Ig {
                 constructor() {
                     wo(this, "id", "mask-effect"), wo(this, "props", null), wo(this, "useInPicking", !0), wo(this, "dummyMaskMap", void 0), wo(this, "channels", []), wo(this, "masks", null), wo(this, "maskPass", void 0), wo(this, "maskMap", void 0), wo(this, "lastViewport", void 0)
                 }
                 preRender(t, {
                     layers: e,
                     layerFilter: n,
                     viewports: i,
                     onViewportActive: r,
                     views: s
                 }) {
                     this.dummyMaskMap || (this.dummyMaskMap = new Kd(t, {
                         width: 1,
                         height: 1
                     }));
-                    const o = e.filter((t => t.props.visible && t.props.operation === Rh));
+                    const o = e.filter((t => t.props.visible && t.props.operation === Ih));
                     if (0 === o.length) return this.masks = null, void(this.channels.length = 0);
-                    this.masks = {}, this.maskPass || (this.maskPass = new Pg(t, {
+                    this.masks = {}, this.maskPass || (this.maskPass = new Sg(t, {
                         id: "default-mask"
                     }), this.maskMap = this.maskPass.maskMap);
                     const a = this._sortMaskChannels(o),
                         l = i[0],
                         c = !this.lastViewport || !this.lastViewport.equals(l);
                     for (const t in a) this._renderChannel(a[t], {
                         layerFilter: n,
@@ -16369,15 +16369,15 @@
                         }) {
                             if (t[2] <= t[0] || t[3] <= t[1]) return null;
                             if (n -= 2, i -= 2, e instanceof kf) {
                                 const {
                                     longitude: e,
                                     latitude: r,
                                     zoom: s
-                                } = Ph({
+                                } = Sh({
                                     width: n,
                                     height: i,
                                     bounds: [
                                         [t[0], t[1]],
                                         [t[2], t[3]]
                                     ],
                                     maxZoom: 20
@@ -16390,15 +16390,15 @@
                                     y: 1,
                                     width: n,
                                     height: i
                                 })
                             }
                             const r = [(t[0] + t[2]) / 2, (t[1] + t[3]) / 2, 0],
                                 s = Math.min(20, n / (t[2] - t[0]), i / (t[3] - t[1]));
-                            return new Og({
+                            return new Lg({
                                 x: 1,
                                 y: 1
                             }).makeViewport({
                                 width: n,
                                 height: i,
                                 viewState: {
                                     target: r,
@@ -16472,45 +16472,45 @@
                     }
                 }
                 cleanup() {
                     this.dummyMaskMap && (this.dummyMaskMap.delete(), this.dummyMaskMap = void 0), this.maskPass && (this.maskPass.delete(), this.maskPass = void 0, this.maskMap = void 0), this.lastViewport = void 0, this.masks = null, this.channels.length = 0
                 }
             }
             const kg = new Eg;
-            class Ig {
+            class Rg {
                 constructor() {
                     wo(this, "effects", void 0), wo(this, "_internalEffects", void 0), wo(this, "_needsRedraw", void 0), this.effects = [], this._internalEffects = [], this._needsRedraw = "Initial render", this.setEffects()
                 }
                 setProps(t) {
-                    "effects" in t && (t.effects.length === this.effects.length && Pf(t.effects, this.effects) || (this.setEffects(t.effects), this._needsRedraw = "effects changed"))
+                    "effects" in t && (t.effects.length === this.effects.length && Sf(t.effects, this.effects) || (this.setEffects(t.effects), this._needsRedraw = "effects changed"))
                 }
                 needsRedraw(t = {
                     clearRedrawFlags: !1
                 }) {
                     const e = this._needsRedraw;
                     return t.clearRedrawFlags && (this._needsRedraw = !1), e
                 }
                 getEffects() {
                     return this._internalEffects
                 }
                 finalize() {
                     this.cleanup()
                 }
                 setEffects(t = []) {
-                    this.cleanup(), this.effects = t, this._internalEffects = t.slice(), this._internalEffects.push(new Rg), t.some((t => t instanceof Eg)) || this._internalEffects.push(kg)
+                    this.cleanup(), this.effects = t, this._internalEffects = t.slice(), this._internalEffects.push(new Ig), t.some((t => t instanceof Eg)) || this._internalEffects.push(kg)
                 }
                 cleanup() {
                     for (const t of this.effects) t.cleanup();
                     for (const t of this._internalEffects) t.cleanup();
                     this.effects.length = 0, this._internalEffects.length = 0
                 }
             }
             class jg extends dg {
                 shouldDrawLayer(t) {
-                    return t.props.operation === Oh
+                    return t.props.operation === Lh
                 }
             }
             const zg = {
                 blendFunc: [1, 0, 32771, 0],
                 blendEquation: 32774
             };
             class Fg extends dg {
@@ -16568,15 +16568,15 @@
                     })));
                     return this._colors = null, {
                         decodePickingColor: g && Bg.bind(null, g),
                         stats: m
                     }
                 }
                 shouldDrawLayer(t) {
-                    return t.props.pickable && t.props.operation === Oh
+                    return t.props.pickable && t.props.operation === Lh
                 }
                 getModuleParameters() {
                     return {
                         pickingActive: 1,
                         pickingAttribute: this.pickZ,
                         lightSources: {}
                     }
@@ -16604,15 +16604,15 @@
                 const n = t.byAlpha[e[3]];
                 return n && {
                     pickedLayer: n.layer,
                     pickedViewports: n.viewports,
                     pickedObjectIndex: n.layer.decodePickingColor(e)
                 }
             }
-            class Dg {
+            class Ng {
                 constructor(t) {
                     this.gl = t, this.layerFilter = null, this.drawPickingColors = !1, this.drawLayersPass = new jg(t), this.pickLayersPass = new Fg(t), this.renderCount = 0, this._needsRedraw = "Initial render", this.renderBuffers = [], this.lastPostProcessEffect = null
                 }
                 setProps(t) {
                     "layerFilter" in t && this.layerFilter !== t.layerFilter && (this.layerFilter = t.layerFilter, this._needsRedraw = "layerFilter changed"), "drawPickingColors" in t && this.drawPickingColors !== t.drawPickingColors && (this.drawPickingColors = t.drawPickingColors, this._needsRedraw = "drawPickingColors changed")
                 }
                 renderLayers(t) {
@@ -16665,15 +16665,15 @@
                                 break
                             }
                             const t = r.postRender(this.gl, i);
                             i.inputBuffer = t, i.swapBuffer = t === n[0] ? n[1] : n[0]
                         }
                 }
             }
-            const Ng = {
+            const Dg = {
                 pickedColor: null,
                 pickedObjectIndex: -1
             };
 
             function Vg({
                 pickedColors: t,
                 decodePickingColor: e,
@@ -16716,15 +16716,15 @@
                             pickedColor: n,
                             pickedX: o + e,
                             pickedY: a + t
                         }
                     }
                     ta.error("Picked non-existent layer. Is picking buffer corrupt?")()
                 }
-                return Ng
+                return Dg
             }
 
             function Ug({
                 pickInfo: t,
                 viewports: e,
                 pixelRatio: n,
                 x: i,
@@ -17141,15 +17141,15 @@
                 color: "#a0a7b4",
                 backgroundColor: "#29323c",
                 padding: "10px",
                 top: "0",
                 left: "0",
                 display: "none"
             };
-            class qg {
+            class Xg {
                 constructor(t) {
                     wo(this, "el", null), wo(this, "isVisible", !1);
                     const e = t.parentElement;
                     e && (this.el = document.createElement("div"), this.el.className = "deck-tooltip", Object.assign(this.el.style, Zg), e.appendChild(this.el))
                 }
                 setTooltip(t, e, n) {
                     const i = this.el;
@@ -17163,16 +17163,16 @@
                     }
                 }
                 remove() {
                     this.el && (this.el.remove(), this.el = null)
                 }
             }
             const {
-                _parseImageNode: Xg
-            } = globalThis, Yg = "undefined" != typeof Image, Kg = "undefined" != typeof ImageBitmap, $g = Boolean(Xg), Jg = !!il || $g;
+                _parseImageNode: qg
+            } = globalThis, Yg = "undefined" != typeof Image, Kg = "undefined" != typeof ImageBitmap, $g = Boolean(qg), Jg = !!il || $g;
 
             function Qg(t) {
                 const e = function(t) {
                     return "undefined" != typeof ImageBitmap && t instanceof ImageBitmap ? "imagebitmap" : "undefined" != typeof Image && t instanceof Image ? "image" : t && "object" == typeof t && t.data && t.width && t.height ? "data" : null
                 }(t);
                 if (!e) throw new Error("Not an image");
                 return e
@@ -17443,23 +17443,23 @@
                 }
             }]]));
             const gm = globalThis.deck,
                 mm = globalThis;
 
             function vm(t) {
                 if (!t && !ko()) return "Node";
-                if (Oo(t)) return "Electron";
+                if (Lo(t)) return "Electron";
                 const e = "undefined" != typeof navigator ? navigator : {},
                     n = t || e.userAgent || "";
                 if (n.indexOf("Edge") > -1) return "Edge";
                 const i = -1 !== n.indexOf("MSIE "),
                     r = -1 !== n.indexOf("Trident/");
                 return i || r ? "IE" : mm.chrome ? "Chrome" : mm.safari ? "Safari" : mm.mozInnerScreenX ? "Firefox" : "Unknown"
             }
-            class bm extends Od {
+            class bm extends Ld {
                 get[Symbol.toStringTag]() {
                     return "Query"
                 }
                 static isSupported(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : [];
                     const n = Mu(t),
                         i = fp(t, hp);
@@ -17548,15 +17548,15 @@
                         autoResizeViewport: u = !0,
                         autoResizeDrawingBuffer: d = !0,
                         stats: p = xd.get("animation-loop-".concat(_m++))
                     } = t;
                     let {
                         useDevicePixels: f = !0
                     } = t;
-                    "useDevicePixelRatio" in t && (Su.deprecated("useDevicePixelRatio", "useDevicePixels")(), f = t.useDevicePixelRatio), this.props = {
+                    "useDevicePixelRatio" in t && (Pu.deprecated("useDevicePixelRatio", "useDevicePixels")(), f = t.useDevicePixelRatio), this.props = {
                         onCreateContext: e,
                         onAddHTML: n,
                         onInitialize: i,
                         onRender: r,
                         onFinalize: s,
                         onError: o,
                         gl: a,
@@ -17624,15 +17624,15 @@
                 }
                 getHTMLControlValue(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 1;
                     const n = document.getElementById(t);
                     return n ? Number(n.value) : e
                 }
                 setViewParameters() {
-                    return Su.removed("AnimationLoop.setViewParameters", "AnimationLoop.setProps")(), this
+                    return Pu.removed("AnimationLoop.setViewParameters", "AnimationLoop.setProps")(), this
                 }
                 _startLoop() {
                     const t = () => {
                         this._running && (this.redraw(), this._animationFrameId = this._requestAnimationFrame(t))
                     };
                     this._cancelAnimationFrame(this._animationFrameId), this._animationFrameId = this._requestAnimationFrame(t)
                 }
@@ -17729,21 +17729,21 @@
                 _resizeCanvasDrawingBuffer() {
                     this.autoResizeDrawingBuffer && function(t) {
                         let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                         if (t.canvas) return void
                         function(t, e, n) {
                             let i = "width" in n ? n.width : t.canvas.clientWidth,
                                 r = "height" in n ? n.height : t.canvas.clientHeight;
-                            i && r || (Su.log(1, "Canvas clientWidth/clientHeight is 0")(), e = 1, i = t.canvas.width || 1, r = t.canvas.height || 1), t.luma = t.luma || {}, t.luma.canvasSizeInfo = t.luma.canvasSizeInfo || {};
+                            i && r || (Pu.log(1, "Canvas clientWidth/clientHeight is 0")(), e = 1, i = t.canvas.width || 1, r = t.canvas.height || 1), t.luma = t.luma || {}, t.luma.canvasSizeInfo = t.luma.canvasSizeInfo || {};
                             const s = t.luma.canvasSizeInfo;
                             if (s.clientWidth !== i || s.clientHeight !== r || s.devicePixelRatio !== e) {
                                 let n = e;
                                 const s = Math.floor(i * n),
                                     o = Math.floor(r * n);
-                                t.canvas.width = s, t.canvas.height = o, t.drawingBufferWidth === s && t.drawingBufferHeight === o || (Su.warn("Device pixel ratio clamped")(), n = Math.min(t.drawingBufferWidth / i, t.drawingBufferHeight / r), t.canvas.width = Math.floor(i * n), t.canvas.height = Math.floor(r * n)), Object.assign(t.luma.canvasSizeInfo, {
+                                t.canvas.width = s, t.canvas.height = o, t.drawingBufferWidth === s && t.drawingBufferHeight === o || (Pu.warn("Device pixel ratio clamped")(), n = Math.min(t.drawingBufferWidth / i, t.drawingBufferHeight / r), t.canvas.width = Math.floor(i * n), t.canvas.height = Math.floor(r * n)), Object.assign(t.luma.canvasSizeInfo, {
                                     clientWidth: i,
                                     clientHeight: r,
                                     devicePixelRatio: e
                                 })
                             }
                         }(t, function(t) {
                             const e = "undefined" == typeof window ? 1 : window.devicePixelRatio || 1;
@@ -17804,88 +17804,88 @@
                 1 & e && t.button >= 0 && (this.pressed = !0), 2 & e && 0 === t.which && (e = 4), this.pressed && (4 & e && (this.pressed = !1), this.callback(this.manager, e, {
                     pointers: [t],
                     changedPointers: [t],
                     pointerType: "mouse",
                     srcEvent: t
                 }))
             };
-            const Pm = wm.Manager,
-                Sm = wm;
+            const Sm = wm.Manager,
+                Pm = wm;
             class Cm {
                 constructor(t, e, n) {
                     this.element = t, this.callback = e, this.options = {
                         enable: !0,
                         ...n
                     }
                 }
             }
-            const Tm = Sm ? [
-                    [Sm.Pan, {
+            const Tm = Pm ? [
+                    [Pm.Pan, {
                         event: "tripan",
                         pointers: 3,
                         threshold: 0,
                         enable: !1
                     }],
-                    [Sm.Rotate, {
+                    [Pm.Rotate, {
                         enable: !1
                     }],
-                    [Sm.Pinch, {
+                    [Pm.Pinch, {
                         enable: !1
                     }],
-                    [Sm.Swipe, {
+                    [Pm.Swipe, {
                         enable: !1
                     }],
-                    [Sm.Pan, {
+                    [Pm.Pan, {
                         threshold: 0,
                         enable: !1
                     }],
-                    [Sm.Press, {
+                    [Pm.Press, {
                         enable: !1
                     }],
-                    [Sm.Tap, {
+                    [Pm.Tap, {
                         event: "doubletap",
                         taps: 2,
                         enable: !1
                     }],
-                    [Sm.Tap, {
+                    [Pm.Tap, {
                         event: "anytap",
                         enable: !1
                     }],
-                    [Sm.Tap, {
+                    [Pm.Tap, {
                         enable: !1
                     }]
                 ] : null,
                 Am = {
                     tripan: ["rotate", "pinch", "pan"],
                     rotate: ["pinch"],
                     pinch: ["pan"],
                     pan: ["press", "doubletap", "anytap", "tap"],
                     doubletap: ["anytap"],
                     anytap: ["tap"]
                 },
                 Mm = {
                     doubletap: ["tap"]
                 },
-                Lm = {
+                Om = {
                     pointerdown: "pointerdown",
                     pointermove: "pointermove",
                     pointerup: "pointerup",
                     touchstart: "pointerdown",
                     touchmove: "pointermove",
                     touchend: "pointerup",
                     mousedown: "pointerdown",
                     mousemove: "pointermove",
                     mouseup: "pointerup"
                 },
-                Om = {
+                Lm = {
                     KEY_EVENTS: ["keydown", "keyup"],
                     MOUSE_EVENTS: ["mousedown", "mousemove", "mouseup", "mouseover", "mouseout", "mouseleave"],
                     WHEEL_EVENTS: ["wheel", "mousewheel"]
                 },
-                Rm = {
+                Im = {
                     tap: "tap",
                     anytap: "anytap",
                     doubletap: "doubletap",
                     press: "press",
                     pinch: "pinch",
                     pinchin: "pinch",
                     pinchout: "pinch",
@@ -17929,41 +17929,41 @@
                     mousedown: "pointerdown",
                     mousemove: "pointermove",
                     mouseup: "pointerup",
                     mouseover: "pointerover",
                     mouseout: "pointerout",
                     mouseleave: "pointerleave"
                 },
-                Im = "undefined" != typeof navigator && navigator.userAgent ? navigator.userAgent.toLowerCase() : "",
+                Rm = "undefined" != typeof navigator && navigator.userAgent ? navigator.userAgent.toLowerCase() : "",
                 jm = "undefined" != typeof window ? window : n.g;
             void 0 !== n.g ? n.g : window, "undefined" != typeof document && document;
             let zm = !1;
             try {
                 const t = {
                     get passive() {
                         return zm = !0, !0
                     }
                 };
                 jm.addEventListener("test", null, t), jm.removeEventListener("test", null)
             } catch (t) {
                 zm = !1
             }
-            const Fm = -1 !== Im.indexOf("firefox"),
+            const Fm = -1 !== Rm.indexOf("firefox"),
                 {
                     WHEEL_EVENTS: Bm
-                } = Om,
-                Dm = "wheel",
-                Nm = 4.000244140625;
+                } = Lm,
+                Nm = "wheel",
+                Dm = 4.000244140625;
             class Vm extends Cm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         if (!this.options.enable) return;
                         let e = t.deltaY;
-                        jm.WheelEvent && (Fm && t.deltaMode === jm.WheelEvent.DOM_DELTA_PIXEL && (e /= jm.devicePixelRatio), t.deltaMode === jm.WheelEvent.DOM_DELTA_LINE && (e *= 40)), 0 !== e && e % Nm == 0 && (e = Math.floor(e / Nm)), t.shiftKey && e && (e *= .25), this.callback({
-                            type: Dm,
+                        jm.WheelEvent && (Fm && t.deltaMode === jm.WheelEvent.DOM_DELTA_PIXEL && (e /= jm.devicePixelRatio), t.deltaMode === jm.WheelEvent.DOM_DELTA_LINE && (e *= 40)), 0 !== e && e % Dm == 0 && (e = Math.floor(e / Dm)), t.shiftKey && e && (e *= .25), this.callback({
+                            type: Nm,
                             center: {
                                 x: t.clientX,
                                 y: t.clientY
                             },
                             delta: -e,
                             srcEvent: t,
                             pointerType: "mouse",
@@ -17973,47 +17973,47 @@
                         passive: !1
                     })))
                 }
                 destroy() {
                     this.events.forEach((t => this.element.removeEventListener(t, this.handleEvent)))
                 }
                 enableEventType(t, e) {
-                    t === Dm && (this.options.enable = e)
+                    t === Nm && (this.options.enable = e)
                 }
             }
             const {
                 MOUSE_EVENTS: Um
-            } = Om, Gm = "pointermove", Wm = "pointerover", Hm = "pointerout", Zm = "pointerenter", qm = "pointerleave";
-            class Xm extends Cm {
+            } = Lm, Gm = "pointermove", Wm = "pointerover", Hm = "pointerout", Zm = "pointerenter", Xm = "pointerleave";
+            class qm extends Cm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         this.handleOverEvent(t), this.handleOutEvent(t), this.handleEnterEvent(t), this.handleLeaveEvent(t), this.handleMoveEvent(t)
                     }, this.pressed = !1;
                     const {
                         enable: i
                     } = this.options;
                     this.enableMoveEvent = i, this.enableLeaveEvent = i, this.enableEnterEvent = i, this.enableOutEvent = i, this.enableOverEvent = i, this.events = (this.options.events || []).concat(Um), this.events.forEach((e => t.addEventListener(e, this.handleEvent)))
                 }
                 destroy() {
                     this.events.forEach((t => this.element.removeEventListener(t, this.handleEvent)))
                 }
                 enableEventType(t, e) {
-                    t === Gm && (this.enableMoveEvent = e), t === Wm && (this.enableOverEvent = e), t === Hm && (this.enableOutEvent = e), t === Zm && (this.enableEnterEvent = e), t === qm && (this.enableLeaveEvent = e)
+                    t === Gm && (this.enableMoveEvent = e), t === Wm && (this.enableOverEvent = e), t === Hm && (this.enableOutEvent = e), t === Zm && (this.enableEnterEvent = e), t === Xm && (this.enableLeaveEvent = e)
                 }
                 handleOverEvent(t) {
                     this.enableOverEvent && "mouseover" === t.type && this._emit(Wm, t)
                 }
                 handleOutEvent(t) {
                     this.enableOutEvent && "mouseout" === t.type && this._emit(Hm, t)
                 }
                 handleEnterEvent(t) {
                     this.enableEnterEvent && "mouseenter" === t.type && this._emit(Zm, t)
                 }
                 handleLeaveEvent(t) {
-                    this.enableLeaveEvent && "mouseleave" === t.type && this._emit(qm, t)
+                    this.enableLeaveEvent && "mouseleave" === t.type && this._emit(Xm, t)
                 }
                 handleMoveEvent(t) {
                     if (this.enableMoveEvent) switch (t.type) {
                         case "mousedown":
                             t.button >= 0 && (this.pressed = !0);
                             break;
                         case "mousemove":
@@ -18034,15 +18034,15 @@
                         pointerType: "mouse",
                         target: e.target
                     })
                 }
             }
             const {
                 KEY_EVENTS: Ym
-            } = Om, Km = "keydown", $m = "keyup";
+            } = Lm, Km = "keydown", $m = "keyup";
             class Jm extends Cm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         const e = t.target || t.srcElement;
                         "INPUT" === e.tagName && "text" === e.type || "TEXTAREA" === e.tagName || (this.enableDownEvent && "keydown" === t.type && this.callback({
                             type: Km,
                             srcEvent: t,
@@ -18237,24 +18237,24 @@
                     }
                 }
             }
             const ov = {
                 events: null,
                 recognizers: null,
                 recognizerOptions: {},
-                Manager: Pm,
+                Manager: Sm,
                 touchAction: "none",
                 tabIndex: 0
             };
             class av {
                 constructor(t = null, e) {
                     this._onBasicInput = t => {
                         const {
                             srcEvent: e
-                        } = t, n = Lm[e.type];
+                        } = t, n = Om[e.type];
                         n && this.manager.emit(n, t)
                     }, this._onOtherEvent = t => {
                         this.manager.emit(t.type, t)
                     }, this.options = {
                         ...ov,
                         ...e
                     }, this.events = new Map, this.setElement(t);
@@ -18285,15 +18285,15 @@
                         if (n) {
                             const i = e.recognizerOptions[t];
                             delete i.enable, n.set(i)
                         }
                     }
                     this.wheelInput = new Vm(t, this._onOtherEvent, {
                         enable: !1
-                    }), this.moveInput = new Xm(t, this._onOtherEvent, {
+                    }), this.moveInput = new qm(t, this._onOtherEvent, {
                         enable: !1
                     }), this.keyInput = new Jm(t, this._onOtherEvent, {
                         enable: !1,
                         tabIndex: e.tabIndex
                     }), this.contextmenuInput = new tv(t, this._onOtherEvent, {
                         enable: !1
                     });
@@ -18339,15 +18339,15 @@
                         return
                     }
                     const {
                         manager: s,
                         events: o
                     } = this, a = km[t] || t;
                     let l = o.get(a);
-                    l || (l = new sv(this), o.set(a, l), l.recognizerName = Rm[a] || a, s && s.on(a, l.handleEvent)), l.add(t, e, n, i, r), l.isEmpty() || this._toggleRecognizer(l.recognizerName, !0)
+                    l || (l = new sv(this), o.set(a, l), l.recognizerName = Im[a] || a, s && s.on(a, l.handleEvent)), l.add(t, e, n, i, r), l.isEmpty() || this._toggleRecognizer(l.recognizerName, !0)
                 }
                 _removeEventHandler(t, e) {
                     if ("string" != typeof t) {
                         for (const e in t) this._removeEventHandler(e, t[e]);
                         return
                     }
                     const {
@@ -18430,15 +18430,15 @@
                             }
                         }
                         this.layerManager && (this.layerManager.context.mousePosition = {
                             x: e.x,
                             y: e.y
                         }), e.event = t
                     })), wo(this, "_onEvent", (t => {
-                        const e = Lh[t.type],
+                        const e = Oh[t.type],
                             n = t.offsetCenter;
                         if (!e || !n || !this.layerManager) return;
                         const i = this.layerManager.getLayers(),
                             r = this.deckPicker.getLastPickedObject({
                                 x: n.x,
                                 y: n.y,
                                 layers: i,
@@ -18491,15 +18491,15 @@
                     }, this._metricsCounter = 0, this.setProps(t), t._typedArrayManagerProps && nc.setOptions(t._typedArrayManagerProps), this.animationLoop.start()
                 }
                 finalize() {
                     var t, e, n, i, r, s, o, a;
                     this.animationLoop.stop(), this.animationLoop = null, this._lastPointerDownInfo = null, null === (t = this.layerManager) || void 0 === t || t.finalize(), this.layerManager = null, null === (e = this.viewManager) || void 0 === e || e.finalize(), this.viewManager = null, null === (n = this.effectManager) || void 0 === n || n.finalize(), this.effectManager = null, null === (i = this.deckRenderer) || void 0 === i || i.finalize(), this.deckRenderer = null, null === (r = this.deckPicker) || void 0 === r || r.finalize(), this.deckPicker = null, null === (s = this.eventManager) || void 0 === s || s.destroy(), this.eventManager = null, null === (o = this.tooltip) || void 0 === o || o.remove(), this.tooltip = null, this.props.canvas || this.props.gl || !this.canvas || (null === (a = this.canvas.parentElement) || void 0 === a || a.removeChild(this.canvas), this.canvas = null)
                 }
                 setProps(t) {
-                    this.stats.get("setProps Time").timeStart(), "onLayerHover" in t && ta.removed("onLayerHover", "onHover")(), "onLayerClick" in t && ta.removed("onLayerClick", "onClick")(), t.initialViewState && !Pf(this.props.initialViewState, t.initialViewState) && (this.viewState = t.initialViewState), Object.assign(this.props, t), this._setCanvasSize(this.props);
+                    this.stats.get("setProps Time").timeStart(), "onLayerHover" in t && ta.removed("onLayerHover", "onHover")(), "onLayerClick" in t && ta.removed("onLayerClick", "onClick")(), t.initialViewState && !Sf(this.props.initialViewState, t.initialViewState) && (this.viewState = t.initialViewState), Object.assign(this.props, t), this._setCanvasSize(this.props);
                     const e = Object.create(this.props);
                     Object.assign(e, {
                         views: this._getViews(),
                         width: this.width,
                         height: this.height,
                         viewState: this._getViewState()
                     }), this.animationLoop.setProps(e), this.layerManager && (this.viewManager.setProps(e), this.layerManager.activateViewport(this.getViewports()[0]), this.layerManager.setProps(e), this.effectManager.setProps(e), this.deckRenderer.setProps(e), this.deckPicker.setProps(e)), this.stats.get("setProps Time").timeEnd()
@@ -18680,33 +18680,33 @@
                     t && (t.style.cursor = this.props.getCursor(this.cursorState))
                 }
                 _setGLContext(t) {
                     if (this.layerManager) return;
                     this.canvas || (this.canvas = t.canvas, bd(t, {
                         enable: !0,
                         copyState: !0
-                    })), this.tooltip = new qg(this.canvas), ld(t, {
+                    })), this.tooltip = new Xg(this.canvas), ld(t, {
                         blend: !0,
                         blendFunc: [770, 771, 1, 771],
                         polygonOffsetFill: !0,
                         depthTest: !0,
                         depthFunc: 515
                     }), this.props.onWebGLInitialized(t);
-                    const e = new So;
+                    const e = new Po;
                     e.play(), this.animationLoop.attachTimeline(e), this.eventManager = new av(this.props.parent || t.canvas, {
                         touchAction: this.props.touchAction,
                         recognizerOptions: this.props.eventRecognizerOptions,
                         events: {
                             pointerdown: this._onPointerDown,
                             pointermove: this._onPointerMove,
                             pointerleave: this._onPointerMove
                         }
                     });
-                    for (const t in Lh) this.eventManager.on(t, this._onEvent);
-                    this.viewManager = new Sf({
+                    for (const t in Oh) this.eventManager.on(t, this._onEvent);
+                    this.viewManager = new Pf({
                         timeline: e,
                         eventManager: this.eventManager,
                         onViewStateChange: this._onViewStateChange.bind(this),
                         onInteractionStateChange: this._onInteractionStateChange.bind(this),
                         views: this._getViews(),
                         viewState: this._getViewState(),
                         width: this.width,
@@ -18714,15 +18714,15 @@
                     });
                     const n = this.viewManager.getViewports()[0];
                     this.layerManager = new Ef(t, {
                         deck: this,
                         stats: this.stats,
                         viewport: n,
                         timeline: e
-                    }), this.effectManager = new Ig, this.deckRenderer = new Dg(t), this.deckPicker = new Hg(t), this.setProps(this.props), this._updateCanvasSize(), this.props.onLoad()
+                    }), this.effectManager = new Rg, this.deckRenderer = new Ng(t), this.deckPicker = new Hg(t), this.setProps(this.props), this._updateCanvasSize(), this.props.onLoad()
                 }
                 _drawLayers(t, e) {
                     const {
                         gl: n
                     } = this.layerManager.context;
                     ld(n, this.props.parameters), this.props.onBeforeRender({
                         gl: n
@@ -19002,15 +19002,15 @@
                         this._checkExternalBuffer(n);
                         let t = n.value;
                         e.externalBuffer = null, e.constant = !1, this.value = t, i.bytesPerElement = t.BYTES_PER_ELEMENT, i.stride = fv(i);
                         const {
                             buffer: r,
                             byteOffset: s
                         } = this;
-                        this.doublePrecision && t instanceof Float64Array && (t = Ic(t, i));
+                        this.doublePrecision && t instanceof Float64Array && (t = Rc(t, i));
                         const o = t.byteLength + s + 2 * i.stride;
                         r.byteLength < o && r.reallocate(o), r.setAccessor(null), r.subData({
                             data: t,
                             offset: s
                         }), i.type = n.type || r.accessor.type
                     }
                     return !0
@@ -19019,15 +19019,15 @@
                     this.state.bounds = null;
                     const e = this.value,
                         {
                             startOffset: n = 0,
                             endOffset: i
                         } = t;
                     this.buffer.subData({
-                        data: this.doublePrecision && e instanceof Float64Array ? Ic(e, {
+                        data: this.doublePrecision && e instanceof Float64Array ? Rc(e, {
                             size: this.size,
                             startIndex: n,
                             endIndex: i
                         }) : e.subarray(n, i),
                         offset: n * e.BYTES_PER_ELEMENT + this.byteOffset
                     })
                 }
@@ -19041,15 +19041,15 @@
                     });
                     this.value = r;
                     const {
                         buffer: s,
                         byteOffset: o
                     } = this;
                     return s.byteLength < r.byteLength + o && (s.reallocate(r.byteLength + o), e && i && s.subData({
-                        data: i instanceof Float64Array ? Ic(i, this) : i,
+                        data: i instanceof Float64Array ? Rc(i, this) : i,
                         offset: o
                     })), n.allocatedValue = r, n.constant = !1, n.externalBuffer = null, n.bufferAccessor = this.settings, !0
                 }
                 _checkExternalBuffer(t) {
                     const {
                         value: e
                     } = t;
@@ -19167,15 +19167,15 @@
                 }
             }
             const wv = [],
                 Ev = [
                     [0, 1 / 0]
                 ];
 
-            function Pv(t) {
+            function Sv(t) {
                 const {
                     source: e,
                     target: n,
                     start: i = 0,
                     size: r,
                     getData: s
                 } = t, o = t.end || n.length, a = e.length, l = o - i;
@@ -19183,15 +19183,15 @@
                 if (n.set(e, i), !s) return;
                 let c = a;
                 for (; c < l;) {
                     const t = s(c, e);
                     for (let e = 0; e < r; e++) n[i + c] = t[e] || 0, c++
                 }
             }
-            const Sv = {
+            const Pv = {
                 interpolation: {
                     duration: 0,
                     easing: t => t
                 },
                 spring: {
                     stiffness: .05,
                     damping: .5
@@ -19202,15 +19202,15 @@
                 if (!t) return null;
                 Number.isFinite(t) && (t = {
                     type: "interpolation",
                     duration: t
                 });
                 const n = t.type || "interpolation";
                 return {
-                    ...Sv[n],
+                    ...Pv[n],
                     ...e,
                     ...t,
                     type: n
                 }
             }
 
             function Tv(t, e) {
@@ -19237,38 +19237,38 @@
                 }
             }
 
             function Mv(t) {
                 t.push(t.shift())
             }
 
-            function Lv(t, e) {
+            function Ov(t, e) {
                 const {
                     doublePrecision: n,
                     settings: i,
                     value: r,
                     size: s
                 } = t, o = n && r instanceof Float64Array ? 2 : 1;
                 return (i.noAlloc ? r.length : e * s) * o
             }
 
-            function Ov({
+            function Lv({
                 buffer: t,
                 numInstances: e,
                 attribute: n,
                 fromLength: i,
                 fromStartIndices: r,
                 getData: s = (t => t)
             }) {
                 const o = n.doublePrecision && n.value instanceof Float64Array ? 2 : 1,
                     a = n.size * o,
                     l = n.byteOffset,
                     c = n.startIndices,
                     h = r && c,
-                    u = Lv(n, e),
+                    u = Ov(n, e),
                     d = n.isConstant;
                 if (!h && i >= u) return;
                 const p = d ? n.value : n.getBuffer().getData({
                     srcByteOffset: l
                 });
                 if (n.settings.normalized && !d) {
                     const t = s;
@@ -19283,37 +19283,37 @@
                     source: t,
                     target: e,
                     size: n,
                     getData: i,
                     sourceStartIndices: r,
                     targetStartIndices: s
                 }) {
-                    if (!Array.isArray(s)) return Pv({
+                    if (!Array.isArray(s)) return Sv({
                         source: t,
                         target: e,
                         size: n,
                         getData: i
                     }), e;
                     let o = 0,
                         a = 0;
                     const l = i && ((t, e) => i(t + a, e)),
                         c = Math.min(r.length, s.length);
                     for (let i = 1; i < c; i++) {
                         const c = r[i] * n,
                             h = s[i] * n;
-                        Pv({
+                        Sv({
                             source: t.subarray(o, c),
                             target: e,
                             start: a,
                             end: h,
                             size: n,
                             getData: l
                         }), o = c, a = h
                     }
-                    a < e.length && Pv({
+                    a < e.length && Sv({
                         source: [],
                         target: e,
                         start: a,
                         size: n,
                         getData: l
                     })
                 }({
@@ -19324,15 +19324,15 @@
                     size: a,
                     getData: f
                 }), t.byteLength < m.byteLength + l && t.reallocate(m.byteLength + l), t.subData({
                     data: m,
                     offset: l
                 })
             }
-            class Rv extends mv {
+            class Iv extends mv {
                 constructor(t, e) {
                     super(t, e, {
                         startIndices: null,
                         lastExternalBuffer: null,
                         binaryValue: null,
                         binaryAccessor: null,
                         needsUpdate: !0,
@@ -19566,15 +19566,15 @@
                                 n = !1
                         }
                         if (!n) throw new Error("Illegal attribute generated for ".concat(this.id))
                     }
                 }
             }
             const kv = "out vec4 transform_output;\nvoid main() {\n  transform_output = vec4(0);\n}",
-                Iv = "#version 300 es\n".concat(kv);
+                Rv = "#version 300 es\n".concat(kv);
 
             function jv(t, e) {
                 e = Array.isArray(e) ? e : [e];
                 const n = t.replace(/^\s+/, "").split(/\s+/),
                     [i, r, s] = n;
                 return e.includes(i) && r && s ? {
                     qualifier: i,
@@ -19587,41 +19587,41 @@
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                 const {
                     version: e = 100,
                     input: n,
                     inputType: i,
                     output: r
                 } = t;
-                if (!n) return 300 === e ? Iv : e > 300 ? "#version ".concat(e, "\n").concat(kv) : "void main() {gl_FragColor = vec4(0);}";
+                if (!n) return 300 === e ? Rv : e > 300 ? "#version ".concat(e, "\n").concat(kv) : "void main() {gl_FragColor = vec4(0);}";
                 const s = function(t, e) {
                     switch (e) {
                         case "float":
                             return "vec4(".concat(t, ", 0.0, 0.0, 1.0)");
                         case "vec2":
                             return "vec4(".concat(t, ", 0.0, 1.0)");
                         case "vec3":
                             return "vec4(".concat(t, ", 1.0)");
                         case "vec4":
                             return t;
                         default:
-                            return Nh(!1), null
+                            return Dh(!1), null
                     }
                 }(n, i);
                 return e >= 300 ? "#version ".concat(e, " ").concat(300 === e ? "es" : "", "\nin ").concat(i, " ").concat(n, ";\nout vec4 ").concat(r, ";\nvoid main() {\n  ").concat(r, " = ").concat(s, ";\n}") : "varying ".concat(i, " ").concat(n, ";\nvoid main() {\n  gl_FragColor = ").concat(s, ";\n}")
             }
-            class Fv extends Od {
+            class Fv extends Ld {
                 get[Symbol.toStringTag]() {
                     return "TransformFeedback"
                 }
                 static isSupported(t) {
                     return Mu(t)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    Ou(t), super(t, e), this.initialize(e), this.stubRemovedMethods("TransformFeedback", "v6.0", ["pause", "resume"]), Object.seal(this)
+                    Lu(t), super(t, e), this.initialize(e), this.stubRemovedMethods("TransformFeedback", "v6.0", ["pause", "resume"]), Object.seal(this)
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this.buffers = {}, this.unused = {}, this.configuration = null, this.bindOnUse = !0, Ad(this.buffers) || this.bind((() => this._unbindBuffers())), this.setProps(t), this
                 }
                 setProps(t) {
                     "program" in t && (this.configuration = t.program && t.program.configuration), "configuration" in t && (this.configuration = t.configuration), "bindOnUse" in t && (t = t.bindOnUse), "buffers" in t && this.setBuffers(t.buffers)
@@ -19635,15 +19635,15 @@
                 setBuffer(t, e) {
                     const n = this._getVaryingIndex(t),
                         {
                             buffer: i,
                             byteSize: r,
                             byteOffset: s
                         } = this._getBufferParams(e);
-                    return n < 0 ? (this.unused[t] = i, Su.warn("".concat(this.id, " unused varying buffer ").concat(t))(), this) : (this.buffers[n] = e, this.bindOnUse || this._bindBuffer(n, i, s, r), this)
+                    return n < 0 ? (this.unused[t] = i, Pu.warn("".concat(this.id, " unused varying buffer ").concat(t))(), this) : (this.buffers[n] = e, this.bindOnUse || this._bindBuffer(n, i, s, r), this)
                 }
                 begin() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 0;
                     return this.gl.bindTransformFeedback(36386, this.handle), this._bindBuffers(), this.gl.beginTransformFeedback(t), this
                 }
                 end() {
                     return this.gl.endTransformFeedback(), this._unbindBuffers(), this.gl.bindTransformFeedback(36386, null), this
@@ -19839,24 +19839,24 @@
                     return this.resources[t] && this.resources[t].delete(), this.resources[t] = n, n
                 }
                 _getNextIndex() {
                     return (this.currentIndex + 1) % 2
                 }
             }
 
-            function Dv(t) {
+            function Nv(t) {
                 let e = 100;
                 const n = t.match(/[^\s]+/g);
                 if (n.length >= 2 && "#version" === n[0]) {
                     const t = parseInt(n[1], 10);
                     Number.isFinite(t) && (e = t)
                 }
                 return e
             }
-            const Nv = {
+            const Dv = {
                     name: "transform",
                     vs: "attribute float transform_elementID;\nvec2 transform_getPixelSizeHalf(vec2 size) {\n  return vec2(1.) / (2. * size);\n}\n\nvec2 transform_getPixelIndices(vec2 texSize, vec2 pixelSizeHalf) {\n  float yIndex = floor((transform_elementID / texSize[0]) + pixelSizeHalf[1]);\n  float xIndex = transform_elementID - (yIndex * texSize[0]);\n  return vec2(xIndex, yIndex);\n}\nvec2 transform_getTexCoord(vec2 size) {\n  vec2 pixelSizeHalf = transform_getPixelSizeHalf(size);\n  vec2 indices = transform_getPixelIndices(size, pixelSizeHalf);\n  vec2 coord = indices / size + pixelSizeHalf;\n  return coord;\n}\nvec2 transform_getPos(vec2 size) {\n  vec2 texCoord = transform_getTexCoord(size);\n  vec2 pos = (texCoord * (2.0, 2.0)) - (1., 1.);\n  return pos;\n}\nvec4 transform_getInput(sampler2D texSampler, vec2 size) {\n  vec2 texCoord = transform_getTexCoord(size);\n  vec4 textureColor = texture2D(texSampler, texCoord);\n  return textureColor;\n}\n",
                     fs: null
                 },
                 Vv = "transform_uSize_",
                 Uv = "transform_position";
             const Gv = {
@@ -19952,15 +19952,15 @@
                                 case "vec2":
                                     return 2;
                                 case "vec3":
                                     return 3;
                                 case "vec4":
                                     return 4;
                                 default:
-                                    return Nh(!1), null
+                                    return Dh(!1), null
                             }
                         }(this.targetTextureType),
                         s = new i(n.length * r / 4);
                     let o = 0;
                     for (let t = 0; t < n.length; t += 4)
                         for (let e = 0; e < r; e++) s[o++] = n[t + e];
                     return s
@@ -20179,15 +20179,15 @@
                                                             case "vec2":
                                                                 return "xy";
                                                             case "vec3":
                                                                 return "xyz";
                                                             case "vec4":
                                                                 return "xyzw";
                                                             default:
-                                                                return Nh(!1), null
+                                                                return Dh(!1), null
                                                         }
                                                     }(r),
                                                     c = "  ".concat(r, " ").concat(s, " = transform_getInput(").concat(i, ", ").concat(o, ").").concat(l, ";\n");
                                                 return n[i] = s, {
                                                     updatedLine: e,
                                                     inject: {
                                                         "vs:#decl": a,
@@ -20233,27 +20233,27 @@
                         sourceTextureMap: e,
                         targetTextureVarying: this.targetTextureVarying,
                         targetTexture: n
                     }), l = cu([t.inject || {}, o]);
                     return this.targetTextureType = s, this.samplerTextureMap = a, {
                         vs: i,
                         fs: t._fs || zv({
-                            version: Dv(i),
+                            version: Nv(i),
                             input: this.targetTextureVarying,
                             inputType: s,
                             output: "transform_output"
                         }),
-                        modules: this.hasSourceTextures || this.targetTextureVarying ? [Nv].concat(t.modules || []) : t.modules,
+                        modules: this.hasSourceTextures || this.targetTextureVarying ? [Dv].concat(t.modules || []) : t.modules,
                         uniforms: r,
                         inject: l
                     }
                 }
             }
             let Hv = null;
-            class Zv extends Od {
+            class Zv extends Ld {
                 get[Symbol.toStringTag]() {
                     return "VertexArrayObject"
                 }
                 static isSupported(t) {
                     return !(arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {}).constantAttributeZero || Mu(t) || "Chrome" === vm()
                 }
                 static getDefaultArray(t) {
@@ -20436,21 +20436,21 @@
                 _getParameter(t, e) {
                     let {
                         location: n
                     } = e;
                     return wd(Number.isFinite(n)), this.bind((() => 34373 === t ? this.gl.getVertexAttribOffset(n, t) : this.gl.getVertexAttrib(n, t)))
                 }
             }
-            const qv = /^(.+)__LOCATION_([0-9]+)$/,
-                Xv = ["setBuffers", "setGeneric", "clearBindings", "setLocations", "setGenericValues", "setDivisor", "enable", "disable"];
+            const Xv = /^(.+)__LOCATION_([0-9]+)$/,
+                qv = ["setBuffers", "setGeneric", "clearBindings", "setLocations", "setGenericValues", "setDivisor", "enable", "disable"];
             class Yv {
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const n = e.id || e.program && e.program.id;
-                    this.id = n, this.gl = t, this.configuration = null, this.elements = null, this.elementsAccessor = null, this.values = null, this.accessors = null, this.unused = null, this.drawParams = null, this.buffer = null, this.attributes = {}, this.vertexArrayObject = new Zv(t), Md(this, "VertexArray", "v6.0", Xv), this.initialize(e), Object.seal(this)
+                    this.id = n, this.gl = t, this.configuration = null, this.elements = null, this.elementsAccessor = null, this.values = null, this.accessors = null, this.unused = null, this.drawParams = null, this.buffer = null, this.attributes = {}, this.vertexArrayObject = new Zv(t), Md(this, "VertexArray", "v6.0", qv), this.initialize(e), Object.seal(this)
                 }
                 delete() {
                     this.buffer && this.buffer.delete(), this.vertexArrayObject.delete()
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this.reset(), this.configuration = null, this.bindOnUse = !1, this.setProps(t)
@@ -20534,19 +20534,19 @@
                             location: -1,
                             accessor: null
                         },
                         {
                             location: s,
                             name: o
                         } = this._getAttributeIndex(t);
-                    if (!Number.isFinite(s) || s < 0) return this.unused[t] = e, Su.once(3, (() => "unused value ".concat(t, " in ").concat(this.id)))(), r;
+                    if (!Number.isFinite(s) || s < 0) return this.unused[t] = e, Pu.once(3, (() => "unused value ".concat(t, " in ").concat(this.id)))(), r;
                     const a = this._getAttributeInfo(o || s);
                     if (!a) return r;
                     const l = this.accessors[s] || {},
-                        c = Dd.resolve(a.accessor, l, n, i),
+                        c = Nd.resolve(a.accessor, l, n, i),
                         {
                             size: h,
                             type: u
                         } = c;
                     return wd(Number.isFinite(h) && Number.isFinite(u)), {
                         location: s,
                         accessor: c
@@ -20556,15 +20556,15 @@
                     return this.configuration && this.configuration.getAttributeInfo(t)
                 }
                 _getAttributeIndex(t) {
                     const e = Number(t);
                     if (Number.isFinite(e)) return {
                         location: e
                     };
-                    const n = qv.exec(t),
+                    const n = Xv.exec(t),
                         i = n ? n[1] : t,
                         r = n ? Number(n[2]) : 0;
                     return this.configuration ? {
                         location: this.configuration.getAttributeLocation(i) + r,
                         name: i
                     } : {
                         location: -1
@@ -20630,15 +20630,15 @@
                             t.vertexCount = Math.min(t.vertexCount, n)
                         }
                     }
                 }
                 setElements() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null,
                         e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    return Su.deprecated("setElements", "setElementBuffer")(), this.setElementBuffer(t, e)
+                    return Pu.deprecated("setElements", "setElementBuffer")(), this.setElementBuffer(t, e)
                 }
             }
 
             function Kv(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 const {
                     isInteger: n = !1
@@ -20678,15 +20678,15 @@
                         {
                             data: d,
                             changed: p
                         } = t.getDebugData();
                     let f;
                     if (o = p ? "*" : "", a = d, u = t.byteLength, h = u / d.BYTES_PER_ELEMENT / c, n) {
                         const t = n.divisor > 0;
-                        f = "".concat(t ? "I " : "P ", " ").concat(h, " (x").concat(c, "=").concat(u, " bytes ").concat(Pd(r, l), ")")
+                        f = "".concat(t ? "I " : "P ", " ").concat(h, " (x").concat(c, "=").concat(u, " bytes ").concat(Sd(r, l), ")")
                     } else s = !0, f = "".concat(u, " bytes");
                     return {
                         [i]: "".concat(o).concat(Kv(a, {
                             size: c,
                             isInteger: s
                         })),
                         "Format ": f
@@ -20986,23 +20986,23 @@
                         uniforms: i = {},
                         attributes: r = {},
                         transformFeedback: s = this.transformFeedback,
                         parameters: o = {},
                         vertexArray: a = this.vertexArray
                     } = t;
                     let l;
-                    this.setAttributes(r), this.updateModuleSettings(e), this.setUniforms(i), Su.priority >= 2 && (l = this._logDrawCallStart(2));
+                    this.setAttributes(r), this.updateModuleSettings(e), this.setUniforms(i), Pu.priority >= 2 && (l = this._logDrawCallStart(2));
                     const c = this.vertexArray.getDrawParams(),
                         {
                             isIndexed: h = c.isIndexed,
                             indexType: u = c.indexType,
                             indexOffset: d = c.indexOffset,
                             vertexArrayInstanced: p = c.isInstanced
                         } = this.props;
-                    p && !this.isInstanced && Su.warn("Found instanced attributes on non-instanced model", this.id)();
+                    p && !this.isInstanced && Pu.warn("Found instanced attributes on non-instanced model", this.id)();
                     const {
                         isInstanced: f,
                         instanceCount: g
                     } = this, {
                         onBeforeRender: m = sb,
                         onAfterRender: v = sb
                     } = this.props;
@@ -21018,15 +21018,15 @@
                         transformFeedback: s,
                         isIndexed: h,
                         indexType: u,
                         isInstanced: f,
                         instanceCount: g,
                         offset: h ? d : 0
                     }));
-                    return v(), Su.priority >= 2 && this._logDrawCallEnd(l, a, n), b
+                    return v(), Pu.priority >= 2 && this._logDrawCallEnd(l, a, n), b
                 }
                 transform() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         discard: e = !0,
                         feedbackBuffers: n,
                         unbindModels: i = []
@@ -21044,15 +21044,15 @@
                     } finally {
                         i.forEach((t => t.vertexArray.bindBuffers()))
                     }
                     return this
                 }
                 render() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    return Su.warn("Model.render() is deprecated. Use Model.setUniforms() and Model.draw()")(), this.setUniforms(t).draw()
+                    return Pu.warn("Model.render() is deprecated. Use Model.setUniforms() and Model.draw()")(), this.setUniforms(t).draw()
                 }
                 _setModelProps(t) {
                     Object.assign(this.props, t), "uniforms" in t && this.setUniforms(t.uniforms), "pickable" in t && (this.pickable = t.pickable), "instanceCount" in t && (this.instanceCount = t.instanceCount), "geometry" in t && this.setGeometry(t.geometry), "attributes" in t && this.setAttributes(t.attributes), "_feedbackBuffers" in t && this._setFeedbackBuffers(t._feedbackBuffers)
                 }
                 _checkProgram() {
                     if (!this._programDirty && this.programManager.stateHash === this._programManagerState) return;
                     let {
@@ -21105,16 +21105,16 @@
                     } = this.program;
                     return this.transformFeedback = this.transformFeedback || new Fv(e, {
                         program: this.program
                     }), this.transformFeedback.setBuffers(t), this
                 }
                 _logDrawCallStart(t) {
                     const e = t > 3 ? 0 : 1e4;
-                    if (!(Date.now() - this.lastLogTime < e)) return this.lastLogTime = Date.now(), Su.group(2, ">>> DRAWING MODEL ".concat(this.id), {
-                        collapsed: Su.level <= 2
+                    if (!(Date.now() - this.lastLogTime < e)) return this.lastLogTime = Date.now(), Pu.group(2, ">>> DRAWING MODEL ".concat(this.id), {
+                        collapsed: Pu.level <= 2
                     })(), t
                 }
                 _logDrawCallEnd(t, e, n, i) {
                     if (void 0 === t) return;
                     const r = function(t) {
                             let {
                                 vertexArray: e,
@@ -21152,15 +21152,15 @@
                             count: c
                         } = Qv({
                             header: "".concat(this.id, " uniforms"),
                             program: this.program,
                             uniforms: Object.assign({}, this.program.uniforms, n),
                             undefinedOnly: !0
                         });
-                    c > 0 && Su.log("MISSING UNIFORMS", Object.keys(l))(), a > 0 && Su.log("UNUSED UNIFORMS", Object.keys(o))();
+                    c > 0 && Pu.log("MISSING UNIFORMS", Object.keys(l))(), a > 0 && Pu.log("UNUSED UNIFORMS", Object.keys(o))();
                     const h = function(t) {
                         const e = {},
                             n = "Accessors for ".concat(t.id);
                         for (const i of t.attributeInfos)
                             if (i) {
                                 const t = eb(i);
                                 e["in ".concat(t)] = {
@@ -21170,18 +21170,18 @@
                             if (i) {
                                 const t = eb(i);
                                 e["out ".concat(t)] = {
                                     [n]: JSON.stringify(i.accessor)
                                 }
                             } return e
                     }(this.vertexArray.configuration);
-                    Su.table(t, r)(), Su.table(t, s)(), Su.table(t + 1, h)(), i && i.log({
+                    Pu.table(t, r)(), Pu.table(t, s)(), Pu.table(t + 1, h)(), i && i.log({
                         logLevel: 2,
                         message: "Rendered to ".concat(i.id)
-                    }), Su.groupEnd(2)()
+                    }), Pu.groupEnd(2)()
                 }
             }
             class lb {
                 static isSupported(t) {
                     return Mu(t)
                 }
                 constructor(t) {
@@ -21236,15 +21236,15 @@
                 _initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         gl: e
                     } = this;
                     this._buildResourceTransforms(e, t), t = this._updateModelProps(t), this.model = new ab(e, Object.assign({}, t, {
                         fs: t.fs || zv({
-                            version: Dv(t.vs)
+                            version: Nv(t.vs)
                         }),
                         id: t.id || "transform-model",
                         drawMode: t.drawMode || 0,
                         vertexCount: t.elementCount
                     })), this.bufferTransform && this.bufferTransform.setupResources({
                         model: this.model
                     })
@@ -21273,15 +21273,15 @@
             const cb = {
                 interpolation: class {
                     constructor({
                         gl: t,
                         attribute: e,
                         timeline: n
                     }) {
-                        wo(this, "gl", void 0), wo(this, "type", "interpolation"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.transition = new If(n), this.attribute = e, this.attributeInTransition = new Rv(t, e.settings), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.transform = function(t, e) {
+                        wo(this, "gl", void 0), wo(this, "type", "interpolation"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.transition = new Rf(n), this.attribute = e, this.attributeInTransition = new Iv(t, e.settings), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.transform = function(t, e) {
                             const n = Av(e.size);
                             return new lb(t, {
                                 vs: "\n#define SHADER_NAME interpolation-transition-vertex-shader\n\nuniform float time;\nattribute ATTRIBUTE_TYPE aFrom;\nattribute ATTRIBUTE_TYPE aTo;\nvarying ATTRIBUTE_TYPE vCurrent;\n\nvoid main(void) {\n  vCurrent = mix(aFrom, aTo, time);\n  gl_Position = vec4(0.0);\n}\n",
                                 defines: {
                                     ATTRIBUTE_TYPE: n
                                 },
                                 varyings: ["vCurrent"]
@@ -21308,19 +21308,19 @@
                         const s = {
                             numInstances: e,
                             attribute: r,
                             fromLength: this.currentLength,
                             fromStartIndices: this.currentStartIndices,
                             getData: t.enter
                         };
-                        for (const t of i) Ov({
+                        for (const t of i) Lv({
                             buffer: t,
                             ...s
                         });
-                        this.currentStartIndices = r.startIndices, this.currentLength = Lv(r, e), this.attributeInTransition.setData({
+                        this.currentStartIndices = r.startIndices, this.currentLength = Ov(r, e), this.attributeInTransition.setData({
                             buffer: i[1],
                             value: r.value
                         }), this.transition.start(t), this.transform.update({
                             elementCount: Math.floor(this.currentLength / r.size),
                             sourceBuffers: {
                                 aFrom: i[0],
                                 aTo: Tv(0, r)
@@ -21356,15 +21356,15 @@
                 },
                 spring: class {
                     constructor({
                         gl: t,
                         attribute: e,
                         timeline: n
                     }) {
-                        wo(this, "gl", void 0), wo(this, "type", "spring"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "texture", void 0), wo(this, "framebuffer", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.type = "spring", this.transition = new If(n), this.attribute = e, this.attributeInTransition = new Rv(t, {
+                        wo(this, "gl", void 0), wo(this, "type", "spring"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "texture", void 0), wo(this, "framebuffer", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.type = "spring", this.transition = new Rf(n), this.attribute = e, this.attributeInTransition = new Iv(t, {
                             ...e.settings,
                             normalized: !1
                         }), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.texture = function(t) {
                             return new Kd(t, {
                                 data: new Uint8Array(4),
                                 format: 6408,
                                 type: 5121,
@@ -21412,19 +21412,19 @@
                         } = this, s = {
                             numInstances: e,
                             attribute: r,
                             fromLength: this.currentLength,
                             fromStartIndices: this.currentStartIndices,
                             getData: t.enter
                         };
-                        for (const t of i) Ov({
+                        for (const t of i) Lv({
                             buffer: t,
                             ...s
                         });
-                        this.settings = t, this.currentStartIndices = r.startIndices, this.currentLength = Lv(r, e), this.attributeInTransition.setData({
+                        this.settings = t, this.currentStartIndices = r.startIndices, this.currentLength = Ov(r, e), this.attributeInTransition.setData({
                             buffer: i[1],
                             value: r.value
                         }), this.transition.start({
                             ...t,
                             duration: 1 / 0
                         }), this.transform.update({
                             elementCount: Math.floor(this.currentLength / r.size),
@@ -21651,15 +21651,15 @@
                 _createAttribute(t, e, n) {
                     const i = {
                         ...e,
                         id: t,
                         size: (e.isIndexed ? 1 : e.size) || 1,
                         divisor: n.instanced ? 1 : e.divisor || 0
                     };
-                    return new Rv(this.gl, i)
+                    return new Iv(this.gl, i)
                 }
                 _mapUpdateTriggersToAttributes() {
                     const t = {};
                     for (const e in this.attributes) this.attributes[e].getUpdateTriggers().forEach((n => {
                         t[n] || (t[n] = []), t[n].push(e)
                     }));
                     this.updateTriggers = t
@@ -21697,15 +21697,15 @@
                         n += r * r
                     }
                     return Math.sqrt(n)
                 }
                 return Math.abs(t - e)
             }
             const mb = {
-                interpolation: class extends If {
+                interpolation: class extends Rf {
                     get value() {
                         return this._value
                     }
                     _onUpdate() {
                         const {
                             time: t,
                             settings: {
@@ -21714,15 +21714,15 @@
                                 duration: i,
                                 easing: r
                             }
                         } = this, s = r(t / i);
                         this._value = ac(e, n, s)
                     }
                 },
-                spring: class extends If {
+                spring: class extends Rf {
                     get value() {
                         return this._currValue
                     }
                     _onUpdate() {
                         const {
                             fromValue: t,
                             toValue: e,
@@ -21860,15 +21860,15 @@
 
             function Eb(t) {
                 const e = t[Co],
                     n = e && e.constructor;
                 return n ? n._propTypes : {}
             }
 
-            function Pb(t, e) {
+            function Sb(t, e) {
                 if (!e) return t;
                 const n = {
                     ...t,
                     ...e
                 };
                 if ("defines" in e && (n.defines = {
                         ...t.defines,
@@ -21884,15 +21884,15 @@
                         };
                         for (const t in e.inject) i[t] = (i[t] || "") + e.inject[t];
                         n.inject = i
                     } else n.inject = e.inject;
                 return n
             }
 
-            function Sb(t, e, n = !1) {
+            function Pb(t, e, n = !1) {
                 const i = e.projectPosition(t);
                 if (n && e instanceof kf) {
                     const [n, r, s = 0] = t, o = e.getDistanceScales([n, r]);
                     i[2] = s * o.unitsPerMeter[2]
                 }
                 return i
             }
@@ -21901,21 +21901,21 @@
                 viewport: e,
                 modelMatrix: n,
                 coordinateSystem: i,
                 coordinateOrigin: r,
                 offsetMode: s
             }) {
                 let [o, a, l = 0] = t;
-                switch (n && ([o, a, l] = qc([], [o, a, l, 1], n)), i) {
+                switch (n && ([o, a, l] = Xc([], [o, a, l, 1], n)), i) {
                     case Th.LNGLAT:
-                        return Sb([o, a, l], e, s);
+                        return Pb([o, a, l], e, s);
                     case Th.LNGLAT_OFFSETS:
-                        return Sb([o + r[0], a + r[1], l + (r[2] || 0)], e, s);
+                        return Pb([o + r[0], a + r[1], l + (r[2] || 0)], e, s);
                     case Th.METER_OFFSETS:
-                        return Sb(yh(r, [o, a, l]), e, s);
+                        return Pb(yh(r, [o, a, l]), e, s);
                     case Th.CARTESIAN:
                     default:
                         return e.isGeospatial ? [o + r[0], a + r[1], l + r[2]] : e.projectPosition([o, a, l])
                 }
             }
             const Tb = {
                     10241: 9987,
@@ -21930,29 +21930,29 @@
                         equal: (t, e, n) => Boolean(t) === Boolean(e)
                     },
                     number: {
                         validate: (t, e) => Number.isFinite(t) && (!("max" in e) || t <= e.max) && (!("min" in e) || t >= e.min)
                     },
                     color: {
                         validate: (t, e) => e.optional && !t || kb(t) && (3 === t.length || 4 === t.length),
-                        equal: (t, e, n) => Lb(t, e)
+                        equal: (t, e, n) => Ob(t, e)
                     },
                     accessor: {
                         validate(t, e) {
-                            const n = Ib(t);
-                            return "function" === n || n === Ib(e.value)
+                            const n = Rb(t);
+                            return "function" === n || n === Rb(e.value)
                         },
-                        equal: (t, e, n) => "function" == typeof e || Lb(t, e)
+                        equal: (t, e, n) => "function" == typeof e || Ob(t, e)
                     },
                     array: {
                         validate: (t, e) => e.optional && !t || kb(t),
-                        equal: (t, e, n) => n.compare ? Lb(t, e) : t === e
+                        equal: (t, e, n) => n.compare ? Ob(t, e) : t === e
                     },
                     object: {
-                        equal: (t, e, n) => n.compare ? Pf(t, e) : t === e
+                        equal: (t, e, n) => n.compare ? Sf(t, e) : t === e
                     },
                     function: {
                         validate: (t, e) => e.optional && !t || "function" == typeof t,
                         equal: (t, e, n) => !n.compare || t === e
                     },
                     data: {
                         transform: (t, e, n) => {
@@ -21987,78 +21987,78 @@
                         release: t => {
                             var e;
                             (e = t) && e instanceof Kd && Ab[e.id] && (e.delete(), delete Ab[e.id])
                         }
                     }
                 };
 
-            function Lb(t, e) {
+            function Ob(t, e) {
                 if (t === e) return !0;
                 if (!kb(t) || !kb(e)) return !1;
                 const n = t.length;
                 if (n !== e.length) return !1;
                 for (let i = 0; i < n; i++)
                     if (t[i] !== e[i]) return !1;
                 return !0
             }
 
-            function Ob(t, e) {
-                switch (Ib(e)) {
+            function Lb(t, e) {
+                switch (Rb(e)) {
                     case "object":
-                        return Rb(t, e);
+                        return Ib(t, e);
                     case "array":
-                        return Rb(t, {
+                        return Ib(t, {
                             type: "array",
                             value: e,
                             compare: !1
                         });
                     case "boolean":
-                        return Rb(t, {
+                        return Ib(t, {
                             type: "boolean",
                             value: e
                         });
                     case "number":
-                        return Rb(t, {
+                        return Ib(t, {
                             type: "number",
                             value: e
                         });
                     case "function":
-                        return Rb(t, {
+                        return Ib(t, {
                             type: "function",
                             value: e,
                             compare: !0
                         });
                     default:
                         return {
                             name: t, type: "unknown", value: e
                         }
                 }
             }
 
-            function Rb(t, e) {
+            function Ib(t, e) {
                 return "type" in e ? {
                     name: t,
                     ...Mb[e.type],
                     ...e
                 } : "value" in e ? {
                     name: t,
-                    type: Ib(e.value),
+                    type: Rb(e.value),
                     ...e
                 } : {
                     name: t,
                     type: "object",
                     value: e
                 }
             }
 
             function kb(t) {
                 return Array.isArray(t) || ArrayBuffer.isView(t)
             }
 
-            function Ib(t) {
+            function Rb(t) {
                 return kb(t) ? "array" : null === t ? "null" : typeof t
             }
 
             function jb(t) {
                 return Bb(t, "_mergedDefaultProps") || (function(t) {
                     if (!t.prototype) return;
                     const e = Object.getPrototypeOf(t),
@@ -22067,15 +22067,15 @@
                             const e = {},
                                 n = {},
                                 i = {};
                             for (const [r, s] of Object.entries(t)) {
                                 const t = null == s ? void 0 : s.deprecatedFor;
                                 if (t) i[r] = Array.isArray(t) ? t : [t];
                                 else {
-                                    const t = Ob(r, s);
+                                    const t = Lb(r, s);
                                     e[r] = t, n[r] = t.value
                                 }
                             }
                             return {
                                 propTypes: e,
                                 defaultProps: n,
                                 deprecatedProps: i
@@ -22151,41 +22151,41 @@
             function Fb(t, e) {
                 return Object.prototype.hasOwnProperty.call(t, e)
             }
 
             function Bb(t, e) {
                 return Fb(t, e) && t[e]
             }
-            let Db = 0;
-            class Nb {
+            let Nb = 0;
+            class Db {
                 constructor(...t) {
                     wo(this, "id", void 0), wo(this, "props", void 0), wo(this, "count", void 0), this.props = function(t, e) {
                         const n = jb(t.constructor),
                             i = Object.create(n);
                         i[Co] = t, i[Ao] = {}, i[Mo] = {};
                         for (let t = 0; t < e.length; ++t) {
                             const n = e[t];
                             for (const t in n) i[t] = n[t]
                         }
                         return Object.freeze(i), i
-                    }(this, t), this.id = this.props.id, this.count = Db++
+                    }(this, t), this.id = this.props.id, this.count = Nb++
                 }
                 clone(t) {
                     const {
                         props: e
                     } = this, n = {};
                     for (const t in e[To]) t in e[Mo] ? n[t] = e[Mo][t] : t in e[Ao] && (n[t] = e[Ao][t]);
                     return new this.constructor({
                         ...e,
                         ...n,
                         ...t
                     })
                 }
             }
-            wo(Nb, "componentName", "Component"), wo(Nb, "defaultProps", {});
+            wo(Db, "componentName", "Component"), wo(Db, "defaultProps", {});
             const Vb = Object.freeze({});
             class Ub {
                 constructor(t) {
                     wo(this, "component", void 0), wo(this, "onAsyncPropUpdated", void 0), wo(this, "asyncProps", void 0), wo(this, "oldProps", void 0), wo(this, "oldAsyncProps", void 0), this.component = t, this.asyncProps = {}, this.onAsyncPropUpdated = () => {}, this.oldProps = null, this.oldAsyncProps = null
                 }
                 finalize() {
                     for (const t in this.asyncProps) {
@@ -22345,16 +22345,16 @@
             }
             const Wb = 2 ** 24 - 1,
                 Hb = Object.freeze([]),
                 Zb = hf((({
                     oldViewport: t,
                     viewport: e
                 }) => t.equals(e)));
-            let qb = new Uint8ClampedArray(0);
-            const Xb = {
+            let Xb = new Uint8ClampedArray(0);
+            const qb = {
                 data: {
                     type: "data",
                     value: Hb,
                     async: !0
                 },
                 dataComparator: {
                     type: "function",
@@ -22428,15 +22428,15 @@
                 pickable: !1,
                 opacity: {
                     type: "number",
                     min: 0,
                     max: 1,
                     value: 1
                 },
-                operation: Oh,
+                operation: Lh,
                 onHover: {
                     type: "function",
                     value: null,
                     compare: !1,
                     optional: !0
                 },
                 onClick: {
@@ -22502,15 +22502,15 @@
                 highlightedObjectIndex: null,
                 autoHighlight: !1,
                 highlightColor: {
                     type: "accessor",
                     value: [0, 0, 128, 128]
                 }
             };
-            class Yb extends Nb {
+            class Yb extends Db {
                 constructor(...t) {
                     super(...t), wo(this, "internalState", null), wo(this, "lifecycle", "Awaiting state"), wo(this, "context", void 0), wo(this, "state", void 0), wo(this, "parent", null)
                 }
                 get root() {
                     let t = this;
                     for (; t.parent;) t = t.parent;
                     return t
@@ -22671,15 +22671,15 @@
                     const {
                         positions: n,
                         instancePositions: i
                     } = e.attributes;
                     return null === (t = n || i) || void 0 === t ? void 0 : t.getBounds()
                 }
                 getShaders(t) {
-                    for (const e of this.props.extensions) t = Pb(t, e.getShaders.call(this, e));
+                    for (const e of this.props.extensions) t = Sb(t, e.getShaders.call(this, e));
                     return t
                 }
                 shouldUpdateState(t) {
                     return t.changeFlags.propsOrDataChanged
                 }
                 updateState(t) {
                     const e = this.getAttributeManager(),
@@ -22793,26 +22793,26 @@
                     }
                     return this.props
                 }
                 calculateInstancePickingColors(t, {
                     numInstances: e
                 }) {
                     if (t.constant) return;
-                    const n = Math.floor(qb.length / 3);
+                    const n = Math.floor(Xb.length / 3);
                     if (this.internalState.usesPickingColorCache = !0, n < e) {
-                        e > Wb && ta.warn("Layer has too many data objects. Picking might not be able to distinguish all objects.")(), qb = nc.allocate(qb, e, {
+                        e > Wb && ta.warn("Layer has too many data objects. Picking might not be able to distinguish all objects.")(), Xb = nc.allocate(Xb, e, {
                             size: 3,
                             copy: !0,
                             maxCount: Math.max(e, Wb)
                         });
-                        const t = Math.floor(qb.length / 3),
+                        const t = Math.floor(Xb.length / 3),
                             i = [];
-                        for (let e = n; e < t; e++) this.encodePickingColor(e, i), qb[3 * e + 0] = i[0], qb[3 * e + 1] = i[1], qb[3 * e + 2] = i[2]
+                        for (let e = n; e < t; e++) this.encodePickingColor(e, i), Xb[3 * e + 0] = i[0], Xb[3 * e + 1] = i[1], Xb[3 * e + 2] = i[2]
                     }
-                    t.value = qb.subarray(0, 3 * e)
+                    t.value = Xb.subarray(0, 3 * e)
                 }
                 _setModelAttributes(t, e) {
                     const n = this.getAttributeManager(),
                         i = t.userData.excludeAttributes || {},
                         r = n.getShaderAttributes(e, i);
                     t.setAttributes(r)
                 }
@@ -22833,15 +22833,15 @@
                     })
                 }
                 restorePickingColors() {
                     const {
                         pickingColors: t,
                         instancePickingColors: e
                     } = this.getAttributeManager().attributes, n = t || e;
-                    n && (this.internalState.usesPickingColorCache && n.value.buffer !== qb.buffer && (n.value = qb.subarray(0, n.value.length)), n.updateSubBuffer({
+                    n && (this.internalState.usesPickingColorCache && n.value.buffer !== Xb.buffer && (n.value = Xb.subarray(0, n.value.length)), n.updateSubBuffer({
                         startOffset: 0
                     }))
                 }
                 _initialize() {
                     Mf(!this.internalState), Mf(Number.isFinite(this.props.coordinateSystem)), na("layer.initialize", this);
                     const t = this._getAttributeManager();
                     t && t.addInstanced({
@@ -23084,15 +23084,15 @@
                         i = !!n && n.getNeedsRedraw(t);
                     return e = e || i, e
                 }
                 _onAsyncPropUpdated() {
                     this._diffProps(this.props, this.internalState.getOldProps()), this.setNeedsUpdate()
                 }
             }
-            wo(Yb, "defaultProps", Xb), wo(Yb, "layerName", "Layer");
+            wo(Yb, "defaultProps", qb), wo(Yb, "layerName", "Layer");
             const Kb = {
                 position: "absolute",
                 zIndex: -1
             };
 
             function $b(t, e) {
                 if ("function" == typeof t) return t(e);
@@ -23112,19 +23112,19 @@
             }
 
             function Jb(t) {
                 return t && "object" == typeof t && "type" in t || !1
             }
 
             function Qb(t) {
-                if ("function" == typeof t) return (0, c.createElement)(Lf, {}, t);
+                if ("function" == typeof t) return (0, c.createElement)(Of, {}, t);
                 if (Array.isArray(t)) return t.map(Qb);
                 if (Jb(t)) {
                     if (t.type === c.Fragment) return Qb(t.props.children);
-                    if (dv(t.type, Lf)) return t
+                    if (dv(t.type, Of)) return t
                 }
                 return t
             }
             const ty = {
                 mixBlendMode: null
             };
 
@@ -23152,15 +23152,15 @@
                                     const n = {},
                                         i = t.defaultProps || {};
                                     for (const t in e) i[t] !== e[t] && (n[t] = e[t]);
                                     return new t(n)
                                 }(e, t.props);
                                 r.push(n)
                             } else i.push(t);
-                            if (dv(e, Lf) && e !== Lf && t.props.id) {
+                            if (dv(e, Of) && e !== Of && t.props.id) {
                                 const n = new e(t.props);
                                 s[n.id] = n
                             }
                         } else t && i.push(t)
                     })), Object.keys(s).length > 0 && (Array.isArray(n) ? n.forEach((t => {
                         s[t.id] = t
                     })) : n && (s[n.id] = n), n = Object.values(s)), {
@@ -23281,15 +23281,15 @@
                             } = e || {};
                             if (!i || !i.views.length) return [];
                             const r = {},
                                 s = i.views[0].id;
                             for (const e of t) {
                                 let t = s,
                                     n = e;
-                                Jb(e) && dv(e.type, Lf) && (t = e.props.id || s, n = e.props.children);
+                                Jb(e) && dv(e.type, Of) && (t = e.props.id || s, n = e.props.children);
                                 const o = i.getViewport(t),
                                     a = i.getViewState(t);
                                 if (o) {
                                     const {
                                         x: e,
                                         y: i,
                                         width: s,
@@ -23797,17 +23797,17 @@
                         const t = yy(g, f);
                         t && (by(u, g, t, f, g), p = t), _y(c, g), xy(u, g), My(f, r, p), i && c.length > n && (c = [], h.push(c), _y(c, u)), p = yy(d, f)
                     }
                     _y(c, d), xy(u, d)
                 }
                 return i ? h : h[0]
             }
-            const Py = 0;
+            const Sy = 0;
 
-            function Sy(t, e) {
+            function Py(t, e) {
                 for (let n = 0; n < e.length; n++) t.push(e[n]);
                 return t
             }
 
             function Cy(t, e = null, n) {
                 if (!t.length) return [];
                 const {
@@ -23826,30 +23826,30 @@
                 let h = [];
                 for (; l.length;) {
                     const {
                         pos: t,
                         types: e,
                         holes: n
                     } = l.shift();
-                    Ly(t, i, n[0] || t.length, c), h = Ay(c[0], r, s, h);
+                    Oy(t, i, n[0] || t.length, c), h = Ay(c[0], r, s, h);
                     const u = yy(c[1], h);
                     if (u) {
                         let r = Ty(t, e, i, 0, n[0] || t.length, h, u);
                         const s = {
                                 pos: r[0].pos,
                                 types: r[0].types,
                                 holes: []
                             },
                             a = {
                                 pos: r[1].pos,
                                 types: r[1].types,
                                 holes: []
                             };
                         l.push(s, a);
-                        for (let l = 0; l < n.length; l++) r = Ty(t, e, i, n[l], n[l + 1] || t.length, h, u), r[0] && (s.holes.push(s.pos.length), s.pos = Sy(s.pos, r[0].pos), o && (s.types = Sy(s.types, r[0].types))), r[1] && (a.holes.push(a.pos.length), a.pos = Sy(a.pos, r[1].pos), o && (a.types = Sy(a.types, r[1].types)))
+                        for (let l = 0; l < n.length; l++) r = Ty(t, e, i, n[l], n[l + 1] || t.length, h, u), r[0] && (s.holes.push(s.pos.length), s.pos = Py(s.pos, r[0].pos), o && (s.types = Py(s.types, r[0].types))), r[1] && (a.holes.push(a.pos.length), a.pos = Py(a.pos, r[1].pos), o && (a.types = Py(a.types, r[1].types)))
                     } else {
                         const i = {
                             positions: t
                         };
                         o && (i.edgeTypes = e), n.length && (i.holeIndices = n), a.push(i)
                     }
                 }
@@ -23865,15 +23865,15 @@
                     d = [];
                 let p, f, g;
                 const m = wy(t, a - 1, n, i);
                 let v = Math.sign(8 & o ? m[1] - s[3] : m[0] - s[2]),
                     b = e && e[a - 1],
                     y = 0,
                     _ = 0;
-                for (let r = 0; r < a; r++) p = wy(t, r, n, i, p), f = Math.sign(8 & o ? p[1] - s[3] : p[0] - s[2]), g = e && e[i / n + r], f && v && v !== f && (by(m, p, o, s, d), _y(l, d) && h.push(b), _y(c, d) && u.push(b)), f <= 0 ? (_y(l, p) && h.push(g), y -= f) : h.length && (h[h.length - 1] = Py), f >= 0 ? (_y(c, p) && u.push(g), _ += f) : u.length && (u[u.length - 1] = Py), xy(m, p), v = f, b = g;
+                for (let r = 0; r < a; r++) p = wy(t, r, n, i, p), f = Math.sign(8 & o ? p[1] - s[3] : p[0] - s[2]), g = e && e[i / n + r], f && v && v !== f && (by(m, p, o, s, d), _y(l, d) && h.push(b), _y(c, d) && u.push(b)), f <= 0 ? (_y(l, p) && h.push(g), y -= f) : h.length && (h[h.length - 1] = Sy), f >= 0 ? (_y(c, p) && u.push(g), _ += f) : u.length && (u[u.length - 1] = Sy), xy(m, p), v = f, b = g;
                 return [y ? {
                     pos: l,
                     types: e && h
                 } : null, _ ? {
                     pos: c,
                     types: e && u
                 } : null]
@@ -23885,38 +23885,38 @@
                 return i[0] = r, i[1] = s, i[2] = r + e, i[3] = s + e, i
             }
 
             function My(t, e, n) {
                 8 & n ? (t[1] += e, t[3] += e) : 4 & n ? (t[1] -= e, t[3] -= e) : 2 & n ? (t[0] += e, t[2] += e) : 1 & n && (t[0] -= e, t[2] -= e)
             }
 
-            function Ly(t, e, n, i) {
+            function Oy(t, e, n, i) {
                 let r = 1 / 0,
                     s = -1 / 0,
                     o = 1 / 0,
                     a = -1 / 0;
                 for (let i = 0; i < n; i += e) {
                     const e = t[i],
                         n = t[i + 1];
                     r = e < r ? e : r, s = e > s ? e : s, o = n < o ? n : o, a = n > a ? n : a
                 }
                 return i[0][0] = r, i[0][1] = o, i[1][0] = s, i[1][1] = a, i
             }
 
-            function Oy(t, e, n, i) {
+            function Ly(t, e, n, i) {
                 let r = -1,
                     s = -1;
                 for (let o = n + 1; o < i; o += e) {
                     const e = Math.abs(t[o]);
                     e > r && (r = e, s = o - 1)
                 }
                 return s
             }
 
-            function Ry(t, e, n, i, r = 85.051129) {
+            function Iy(t, e, n, i, r = 85.051129) {
                 const s = t[n],
                     o = t[i - e];
                 if (Math.abs(s - o) > 180) {
                     const i = wy(t, 0, e, n);
                     i[0] += 360 * Math.round((o - s) / 360), _y(t, i), i[1] = Math.sign(i[1]) * r, _y(t, i), i[0] = s, _y(t, i)
                 }
             }
@@ -23926,15 +23926,15 @@
                 for (let o = n; o < i; o += e) {
                     r = t[o];
                     const e = r - s;
                     (e > 180 || e < -180) && (r -= 360 * Math.round(e / 360)), t[o] = s = r
                 }
             }
 
-            function Iy(t, e) {
+            function Ry(t, e) {
                 let n;
                 const i = t.length / e;
                 for (let r = 0; r < i && (n = t[r * e], (n + 180) % 360 == 0); r++);
                 const r = 360 * -Math.round(n / 360);
                 if (0 !== r)
                     for (let n = 0; n < i; n++) t[n * e] += r
             }
@@ -23960,52 +23960,52 @@
                             n = t[t.length - 1];
                         return e[0] === n[0] && e[1] === n[1] && e[2] === n[2]
                     }(n))
                     for (let e = 0; e < i; e++) t[s++] = n[0][e] || 0;
                 return jy.start = e, jy.end = s, jy.size = i, vy(t, r, jy), s
             }
 
-            function Dy(t, e, n, i, r = 0, s, o) {
+            function Ny(t, e, n, i, r = 0, s, o) {
                 const a = (s = s || n.length) - r;
                 if (a <= 0) return e;
                 let l = e;
                 for (let e = 0; e < a; e++) t[l++] = n[r + e];
                 if (! function(t, e, n, i) {
                         for (let r = 0; r < e; r++)
                             if (t[n + r] !== t[i - e + r]) return !1;
                         return !0
                     }(n, i, r, s))
                     for (let e = 0; e < i; e++) t[l++] = n[r + e];
                 return jy.start = e, jy.end = l, jy.size = i, vy(t, o, jy), l
             }
 
-            function Ny(t, e) {
+            function Dy(t, e) {
                 ! function(t) {
                     if (t = t && t.positions || t, !Array.isArray(t) && !ArrayBuffer.isView(t)) throw new Error("invalid polygon")
                 }(t);
                 const n = [],
                     i = [];
                 if ("positions" in t) {
                     const {
                         positions: r,
                         holeIndices: s
                     } = t;
                     if (s) {
                         let t = 0;
-                        for (let o = 0; o <= s.length; o++) t = Dy(n, t, r, e, s[o - 1], s[o], 0 === o ? 1 : -1), i.push(t);
+                        for (let o = 0; o <= s.length; o++) t = Ny(n, t, r, e, s[o - 1], s[o], 0 === o ? 1 : -1), i.push(t);
                         return i.pop(), {
                             positions: n,
                             holeIndices: i
                         }
                     }
                     t = r
                 }
                 if (! function(t) {
                         return Array.isArray(t[0])
-                    }(t)) return Dy(n, 0, t, e, 0, n.length, 1), n;
+                    }(t)) return Ny(n, 0, t, e, 0, n.length, 1), n;
                 if (! function(t) {
                         return t.length >= 1 && t[0].length >= 2 && Number.isFinite(t[0][0])
                     }(t)) {
                     let r = 0;
                     for (const [s, o] of t.entries()) r = By(n, r, o, e, 0 === s ? 1 : -1), i.push(r);
                     return i.pop(), {
                         positions: n,
@@ -24153,15 +24153,15 @@
                     super.updateGeometry(t);
                     const e = this.buffers.indices;
                     if (e) this.vertexCount = (e.value || e).length;
                     else if (this.data && !this.getGeometry) throw new Error("missing indices buffer")
                 }
                 normalizeGeometry(t) {
                     if (this.normalize) {
-                        const e = Ny(t, this.positionSize);
+                        const e = Dy(t, this.positionSize);
                         return this.opts.resolution ? Cy(zy(e), Fy(e), {
                             size: this.positionSize,
                             gridResolution: this.opts.resolution,
                             edgeTypes: !0
                         }) : this.opts.wrapLongitude ? function(t, e = null, n) {
                             const {
                                 size: i = 2,
@@ -24172,28 +24172,28 @@
                             const o = [],
                                 a = [];
                             let l = 0,
                                 c = 0;
                             for (let r = 0; r <= e.length; r++) {
                                 const s = e[r] || t.length,
                                     h = c,
-                                    u = Oy(t, i, l, s);
+                                    u = Ly(t, i, l, s);
                                 for (let e = u; e < s; e++) o[c++] = t[e];
                                 for (let e = l; e < u; e++) o[c++] = t[e];
-                                ky(o, i, h, c), Ry(o, i, h, c, null == n ? void 0 : n.maxLatitude), l = s, a[r] = c
+                                ky(o, i, h, c), Iy(o, i, h, c, null == n ? void 0 : n.maxLatitude), l = s, a[r] = c
                             }
                             a.pop();
                             const h = Cy(o, a, {
                                 size: i,
                                 gridResolution: 360,
                                 gridOffset: [-180, -180],
                                 edgeTypes: s
                             });
                             if (r)
-                                for (const t of h) Iy(t.positions, i);
+                                for (const t of h) Ry(t.positions, i);
                             return h
                         }(zy(e), Fy(e), {
                             size: this.positionSize,
                             maxLatitude: 86,
                             edgeTypes: !0
                         }) : e
                     }
@@ -24286,16 +24286,16 @@
 
             function Gy(t) {
                 return Array.isArray(t) && t.length > 0 && !Number.isFinite(t[0])
             }
             const Wy = "\nattribute vec2 vertexPositions;\nattribute float vertexValid;\n\nuniform bool extruded;\nuniform bool isWireframe;\nuniform float elevationScale;\nuniform float opacity;\n\nvarying vec4 vColor;\n\nstruct PolygonProps {\n  vec4 fillColors;\n  vec4 lineColors;\n  vec3 positions;\n  vec3 nextPositions;\n  vec3 pickingColors;\n  vec3 positions64Low;\n  vec3 nextPositions64Low;\n  float elevations;\n};\n\nvec3 project_offset_normal(vec3 vector) {\n  if (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT ||\n    project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT_OFFSETS) {\n    // normals generated by the polygon tesselator are in lnglat offsets instead of meters\n    return normalize(vector * project_uCommonUnitsPerWorldUnit);\n  }\n  return project_normal(vector);\n}\n\nvoid calculatePosition(PolygonProps props) {\n#ifdef IS_SIDE_VERTEX\n  if(vertexValid < 0.5){\n    gl_Position = vec4(0.);\n    return;\n  }\n#endif\n\n  vec3 pos;\n  vec3 pos64Low;\n  vec3 normal;\n  vec4 colors = isWireframe ? props.lineColors : props.fillColors;\n\n  geometry.worldPosition = props.positions;\n  geometry.worldPositionAlt = props.nextPositions;\n  geometry.pickingColor = props.pickingColors;\n\n#ifdef IS_SIDE_VERTEX\n  pos = mix(props.positions, props.nextPositions, vertexPositions.x);\n  pos64Low = mix(props.positions64Low, props.nextPositions64Low, vertexPositions.x);\n#else\n  pos = props.positions;\n  pos64Low = props.positions64Low;\n#endif\n\n  if (extruded) {\n    pos.z += props.elevations * vertexPositions.y * elevationScale;\n  }\n  gl_Position = project_position_to_clipspace(pos, pos64Low, vec3(0.), geometry.position);\n\n  DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n\n  if (extruded) {\n  #ifdef IS_SIDE_VERTEX\n    normal = vec3(\n      props.positions.y - props.nextPositions.y + (props.positions64Low.y - props.nextPositions64Low.y),\n      props.nextPositions.x - props.positions.x + (props.nextPositions64Low.x - props.positions64Low.x),\n      0.0);\n    normal = project_offset_normal(normal);\n  #else\n    normal = project_normal(vec3(0.0, 0.0, 1.0));\n  #endif\n    geometry.normal = normal;\n    vec3 lightColor = lighting_getLightColor(colors.rgb, project_uCameraPosition, geometry.position.xyz, normal);\n    vColor = vec4(lightColor, colors.a * opacity);\n  } else {\n    vColor = vec4(colors.rgb, colors.a * opacity);\n  }\n  DECKGL_FILTER_COLOR(vColor, geometry);\n}\n",
                 Hy = "#define SHADER_NAME solid-polygon-layer-vertex-shader\n\nattribute vec3 positions;\nattribute vec3 positions64Low;\nattribute float elevations;\nattribute vec4 fillColors;\nattribute vec4 lineColors;\nattribute vec3 pickingColors;\n\n".concat(Wy, "\n\nvoid main(void) {\n  PolygonProps props;\n\n  props.positions = positions;\n  props.positions64Low = positions64Low;\n  props.elevations = elevations;\n  props.fillColors = fillColors;\n  props.lineColors = lineColors;\n  props.pickingColors = pickingColors;\n\n  calculatePosition(props);\n}\n"),
                 Zy = "#define SHADER_NAME solid-polygon-layer-vertex-shader-side\n#define IS_SIDE_VERTEX\n\n\nattribute vec3 instancePositions;\nattribute vec3 nextPositions;\nattribute vec3 instancePositions64Low;\nattribute vec3 nextPositions64Low;\nattribute float instanceElevations;\nattribute vec4 instanceFillColors;\nattribute vec4 instanceLineColors;\nattribute vec3 instancePickingColors;\n\n".concat(Wy, "\n\nvoid main(void) {\n  PolygonProps props;\n\n  #if RING_WINDING_ORDER_CW == 1\n    props.positions = instancePositions;\n    props.positions64Low = instancePositions64Low;\n    props.nextPositions = nextPositions;\n    props.nextPositions64Low = nextPositions64Low;\n  #else\n    props.positions = nextPositions;\n    props.positions64Low = nextPositions64Low;\n    props.nextPositions = instancePositions;\n    props.nextPositions64Low = instancePositions64Low;\n  #endif\n  props.elevations = instanceElevations;\n  props.fillColors = instanceFillColors;\n  props.lineColors = instanceLineColors;\n  props.pickingColors = instancePickingColors;\n\n  calculatePosition(props);\n}\n"),
-                qy = [0, 0, 0, 255],
-                Xy = {
+                Xy = [0, 0, 0, 255],
+                qy = {
                     filled: !0,
                     extruded: !1,
                     wireframe: !1,
                     _normalize: !0,
                     _windingOrder: "CW",
                     elevationScale: {
                         type: "number",
@@ -24308,19 +24308,19 @@
                     },
                     getElevation: {
                         type: "accessor",
                         value: 1e3
                     },
                     getFillColor: {
                         type: "accessor",
-                        value: qy
+                        value: Xy
                     },
                     getLineColor: {
                         type: "accessor",
-                        value: qy
+                        value: Xy
                     },
                     material: !0
                 },
                 Yy = {
                     enter: (t, e) => e.length ? e.subarray(e.length - t.length) : t
                 };
             class Ky extends Yb {
@@ -24410,15 +24410,15 @@
                         },
                         fillColors: {
                             size: this.props.colorFormat.length,
                             type: 5121,
                             normalized: !0,
                             transition: Yy,
                             accessor: "getFillColor",
-                            defaultValue: qy,
+                            defaultValue: Xy,
                             shaderAttributes: {
                                 fillColors: {
                                     divisor: 0
                                 },
                                 instanceFillColors: {
                                     divisor: 1
                                 }
@@ -24426,15 +24426,15 @@
                         },
                         lineColors: {
                             size: this.props.colorFormat.length,
                             type: 5121,
                             normalized: !0,
                             transition: Yy,
                             accessor: "getLineColor",
-                            defaultValue: qy,
+                            defaultValue: Xy,
                             shaderAttributes: {
                                 lineColors: {
                                     divisor: 0
                                 },
                                 instanceLineColors: {
                                     divisor: 1
                                 }
@@ -24594,15 +24594,15 @@
                     } = this.state;
                     t.startIndices = e.vertexStarts, t.value = e.get("positions")
                 }
                 calculateVertexValid(t) {
                     t.value = this.state.polygonTesselator.get("vertexValid")
                 }
             }
-            wo(Ky, "defaultProps", Xy), wo(Ky, "layerName", "SolidPolygonLayer");
+            wo(Ky, "defaultProps", qy), wo(Ky, "layerName", "SolidPolygonLayer");
             class $y extends Vy {
                 constructor(t) {
                     super({
                         ...t,
                         attributes: {
                             positions: {
                                 size: 3,
@@ -24646,15 +24646,15 @@
                             const a = Ey(o, {
                                 size: n,
                                 broken: !0,
                                 gridResolution: 360,
                                 gridOffset: [-180, -180]
                             });
                             if (s)
-                                for (const t of a) Iy(t, n);
+                                for (const t of a) Ry(t, n);
                             return a
                         }(r, {
                             size: e
                         }) : r
                     }(t, this.positionSize, this.opts.resolution, this.opts.wrapLongitude) : t
                 }
                 getGeometrySize(t) {
@@ -25052,15 +25052,15 @@
                     } = t, {
                         iterable: c,
                         objectInfo: h
                     } = yv(e, a, l);
                     for (const t of c) {
                         h.index++;
                         let e = n(t, h);
-                        r && (e = Ny(e, o));
+                        r && (e = Dy(e, o));
                         const {
                             holeIndices: i
                         } = e, a = e.positions || e;
                         if (i)
                             for (let e = 0; e <= i.length; e++) {
                                 const n = a.slice(i[e - 1] || 0, i[e] || a.length);
                                 s.push(this.getSubLayerRow({
@@ -25096,47 +25096,47 @@
                     } = this.props, {
                         getFillColor: b,
                         getLineColor: y,
                         getLineWidth: _,
                         getLineDashArray: x,
                         getElevation: w,
                         getPolygon: E,
-                        updateTriggers: P,
-                        material: S
+                        updateTriggers: S,
+                        material: P
                     } = this.props, {
                         paths: C,
                         pathsDiff: T
-                    } = this.state, A = this.getSubLayerClass("fill", Ky), M = this.getSubLayerClass("stroke", n_), L = this.shouldRenderSubLayer("fill", C) && new A({
+                    } = this.state, A = this.getSubLayerClass("fill", Ky), M = this.getSubLayerClass("stroke", n_), O = this.shouldRenderSubLayer("fill", C) && new A({
                         _dataDiff: e,
                         extruded: r,
                         elevationScale: l,
                         filled: i,
                         wireframe: s,
                         _normalize: o,
                         _windingOrder: a,
                         getElevation: w,
                         getFillColor: b,
                         getLineColor: r && s ? y : r_,
-                        material: S,
+                        material: P,
                         transitions: c
                     }, this.getSubLayerProps({
                         id: "fill",
-                        updateTriggers: P && {
-                            getPolygon: P.getPolygon,
-                            getElevation: P.getElevation,
-                            getFillColor: P.getFillColor,
+                        updateTriggers: S && {
+                            getPolygon: S.getPolygon,
+                            getElevation: S.getElevation,
+                            getFillColor: S.getFillColor,
                             lineColors: r && s,
-                            getLineColor: P.getLineColor
+                            getLineColor: S.getLineColor
                         }
                     }), {
                         data: t,
                         positionFormat: h,
                         getPolygon: E
                     });
-                    return [!r && L, !r && n && this.shouldRenderSubLayer("stroke", C) && new M({
+                    return [!r && O, !r && n && this.shouldRenderSubLayer("stroke", C) && new M({
                         _dataDiff: T && (() => T),
                         widthUnits: u,
                         widthScale: d,
                         widthMinPixels: p,
                         widthMaxPixels: f,
                         jointRounded: g,
                         miterLimit: m,
@@ -25148,24 +25148,24 @@
                             getPath: c.getPolygon
                         },
                         getColor: this.getSubLayerAccessor(y),
                         getWidth: this.getSubLayerAccessor(_),
                         getDashArray: this.getSubLayerAccessor(x)
                     }, this.getSubLayerProps({
                         id: "stroke",
-                        updateTriggers: P && {
-                            getWidth: P.getLineWidth,
-                            getColor: P.getLineColor,
-                            getDashArray: P.getLineDashArray
+                        updateTriggers: S && {
+                            getWidth: S.getLineWidth,
+                            getColor: S.getLineColor,
+                            getDashArray: S.getLineDashArray
                         }
                     }), {
                         data: C,
                         positionFormat: h,
                         getPath: t => t.path
-                    }), r && L]
+                    }), r && O]
                 }
             }
             wo(o_, "layerName", "PolygonLayer"), wo(o_, "defaultProps", s_);
             const a_ = () => {},
                 l_ = {
                     10241: 9987,
                     10240: 9729,
@@ -25340,15 +25340,15 @@
                                 if (e instanceof Yd && (b = e, h = Number.isFinite(h) ? h : b.width, u = Number.isFinite(u) ? u : b.height, b.bind(0), e = b.target), m) switch (e) {
                                     case 3553:
                                     case 34067:
                                         f.copyTexSubImage2D(e, s, a, l, i, r, h, u);
                                         break;
                                     case 35866:
                                     case 32879:
-                                        Ou(f).copyTexSubImage3D(e, s, a, l, c, i, r, h, u)
+                                        Lu(f).copyTexSubImage3D(e, s, a, l, c, i, r, h, u)
                                 } else f.copyTexImage2D(e, s, o, i, r, h, u, 0);
                                 b && b.unbind(), f.bindFramebuffer(36160, v || null), p && d.delete()
                             }(t, o, {
                                 targetY: 0,
                                 width: r,
                                 height: s
                             }), t.delete(), o
@@ -25879,30 +25879,30 @@
                     type: "color",
                     value: [0, 0, 0, 255]
                 }
             }), wo(__, "layerName", "MultiIconLayer");
             var x_ = n(9296),
                 w_ = n.n(x_);
             const E_ = 32,
-                P_ = [];
+                S_ = [];
 
-            function S_(t, e, n, i) {
+            function P_(t, e, n, i) {
                 let r = 0;
                 for (let o = e; o < n; o++) {
                     var s;
                     r += (null === (s = i[t[o]]) || void 0 === s ? void 0 : s.width) || 0
                 }
                 return r
             }
 
             function C_(t, e, n, i, r, s) {
                 let o = e,
                     a = 0;
                 for (let l = e; l < n; l++) {
-                    const e = S_(t, l, l + 1, r);
+                    const e = P_(t, l, l + 1, r);
                     a + e > i && (o < l && s.push(l), o = l, a = 0), a += e
                 }
                 return a
             }
 
             function T_(t, e, n, i, r = 0, s) {
                 void 0 === s && (s = t.length);
@@ -25910,15 +25910,15 @@
                 return "break-all" === e ? C_(t, r, s, n, i, o) : function(t, e, n, i, r, s) {
                     let o = e,
                         a = e,
                         l = e,
                         c = 0;
                     for (let h = e; h < n; h++)
                         if (" " === t[h] ? l = h + 1 : " " !== t[h + 1] && h + 1 !== n || (l = h + 1), l > a) {
-                            let e = S_(t, a, l, r);
+                            let e = P_(t, a, l, r);
                             c + e > i && (o < a && (s.push(a), o = a, c = 0), e > i && (e = C_(t, a, l, i, r, s), o = s[s.length - 1])), a = l, c += e
                         }
                 }(t, r, s, n, i, o), o
             }
 
             function A_(t, e, n, i, r, s) {
                 let o = 0,
@@ -25942,15 +25942,15 @@
                     d = [0, 0];
                 let p = 0,
                     f = 0,
                     g = 0;
                 for (let t = 0; t <= o; t++) {
                     const m = s[t];
                     if ("\n" !== m && t !== o || (g = t), g > f) {
-                        const t = h ? T_(s, n, i, r, f, g) : P_;
+                        const t = h ? T_(s, n, i, r, f, g) : S_;
                         for (let n = 0; n <= t.length; n++) {
                             const i = 0 === n ? f : t[n - 1],
                                 o = n < t.length ? t[n] : g;
                             A_(s, i, o, r, a, d);
                             for (let t = i; t < o; t++) l[t] = p + d[1] / 2, c[t] = d[0];
                             p += d[1] * e, u[0] = Math.max(u[0], d[0])
                         }
@@ -25961,15 +25961,15 @@
                 return u[1] = p, {
                     x: a,
                     y: l,
                     rowWidth: c,
                     size: u
                 }
             }
-            class L_ {
+            class O_ {
                 constructor(t = 5) {
                     wo(this, "limit", void 0), wo(this, "_cache", {}), wo(this, "_order", []), this.limit = t
                 }
                 get(t) {
                     const e = this._cache[t];
                     return e && (this._deleteOrder(t), this._appendOrder(t)), e
                 }
@@ -25983,42 +25983,42 @@
                     const e = this._order.indexOf(t);
                     e >= 0 && this._order.splice(e, 1)
                 }
                 _appendOrder(t) {
                     this._order.push(t)
                 }
             }
-            const O_ = {
+            const L_ = {
                 fontFamily: "Monaco, monospace",
                 fontWeight: "normal",
                 characterSet: function() {
                     const t = [];
                     for (let e = 32; e < 128; e++) t.push(String.fromCharCode(e));
                     return t
                 }(),
                 fontSize: 64,
                 buffer: 4,
                 sdf: !1,
                 cutoff: .25,
                 radius: 12,
                 smoothing: .1
             };
-            let R_ = new L_(3);
+            let I_ = new O_(3);
 
             function k_(t, e) {
                 for (let n = 0; n < t.length; n++) e.data[4 * n + 3] = t[n]
             }
 
-            function I_(t, e, n, i) {
+            function R_(t, e, n, i) {
                 t.font = "".concat(i, " ").concat(n, "px ").concat(e), t.fillStyle = "#000", t.textBaseline = "alphabetic", t.textAlign = "left"
             }
             class j_ {
                 constructor() {
                     wo(this, "props", {
-                        ...O_
+                        ...L_
                     }), wo(this, "_key", void 0), wo(this, "_atlas", void 0)
                 }
                 get texture() {
                     return this._atlas
                 }
                 get mapping() {
                     return this._atlas && this._atlas.mapping
@@ -26029,38 +26029,38 @@
                 setProps(t = {}) {
                     Object.assign(this.props, t);
                     const e = this._key;
                     this._key = this._getKey();
                     const n = function(t, e) {
                             let n;
                             n = "string" == typeof e ? new Set(Array.from(e)) : new Set(e);
-                            const i = R_.get(t);
+                            const i = I_.get(t);
                             if (!i) return n;
                             for (const t in i.mapping) n.has(t) && n.delete(t);
                             return n
                         }(this._key, this.props.characterSet),
-                        i = R_.get(this._key);
+                        i = I_.get(this._key);
                     if (i && 0 === n.size) return void(this._key !== e && (this._atlas = i));
                     const r = this._generateFontAtlas(this._key, n, i);
-                    this._atlas = r, R_.set(this._key, r)
+                    this._atlas = r, I_.set(this._key, r)
                 }
                 _generateFontAtlas(t, e, n) {
                     const {
                         fontFamily: i,
                         fontWeight: r,
                         fontSize: s,
                         buffer: o,
                         sdf: a,
                         radius: l,
                         cutoff: c
                     } = this.props;
                     let h = n && n.data;
                     h || (h = document.createElement("canvas"), h.width = 1024);
                     const u = h.getContext("2d");
-                    I_(u, i, s, r);
+                    R_(u, i, s, r);
                     const {
                         mapping: d,
                         canvasHeight: p,
                         xOffset: f,
                         yOffset: g
                     } = function({
                         characterSet: t,
@@ -26103,15 +26103,15 @@
                             yOffset: n.yOffset
                         }
                     });
                     if (h.height !== p) {
                         const t = u.getImageData(0, 0, h.width, h.height);
                         h.height = p, u.putImageData(t, 0, 0)
                     }
-                    if (I_(u, i, s, r), a) {
+                    if (R_(u, i, s, r), a) {
                         const t = new(w_())(s, o, l, c, i, r),
                             n = u.getImageData(0, 0, t.size, t.size);
                         for (const i of e) k_(t.draw(i), n), u.putImageData(n, d[i].x - o, d[i].y + o)
                     } else
                         for (const t of e) u.fillText(t, d[t].x, d[t].y + .9 * s);
                     return {
                         xOffset: f,
@@ -26299,58 +26299,58 @@
             }
             wo(F_, "defaultProps", z_), wo(F_, "layerName", "TextBackgroundLayer");
             const B_ = {
                     start: 1,
                     middle: 0,
                     end: -1
                 },
-                D_ = {
+                N_ = {
                     top: 1,
                     center: 0,
                     bottom: -1
                 },
-                N_ = [0, 0, 0, 255],
+                D_ = [0, 0, 0, 255],
                 V_ = {
                     billboard: !0,
                     sizeScale: 1,
                     sizeUnits: "pixels",
                     sizeMinPixels: 0,
                     sizeMaxPixels: Number.MAX_SAFE_INTEGER,
                     background: !1,
                     getBackgroundColor: {
                         type: "accessor",
                         value: [255, 255, 255, 255]
                     },
                     getBorderColor: {
                         type: "accessor",
-                        value: N_
+                        value: D_
                     },
                     getBorderWidth: {
                         type: "accessor",
                         value: 0
                     },
                     backgroundPadding: {
                         type: "array",
                         value: [0, 0, 0, 0]
                     },
                     characterSet: {
                         type: "object",
-                        value: O_.characterSet
+                        value: L_.characterSet
                     },
-                    fontFamily: O_.fontFamily,
-                    fontWeight: O_.fontWeight,
+                    fontFamily: L_.fontFamily,
+                    fontWeight: L_.fontWeight,
                     lineHeight: 1,
                     outlineWidth: {
                         type: "number",
                         value: 0,
                         min: 0
                     },
                     outlineColor: {
                         type: "color",
-                        value: N_
+                        value: D_
                     },
                     fontSettings: {},
                     wordBreak: "break-word",
                     maxWidth: {
                         type: "number",
                         value: -1
                     },
@@ -26360,15 +26360,15 @@
                     },
                     getPosition: {
                         type: "accessor",
                         value: t => t.position
                     },
                     getColor: {
                         type: "accessor",
-                        value: N_
+                        value: D_
                     },
                     getSize: {
                         type: "accessor",
                         value: 32
                     },
                     getAngle: {
                         type: "accessor",
@@ -26402,15 +26402,15 @@
                                 getTextAnchor: a,
                                 getAlignmentBaseline: l
                             } = this.props,
                             c = i(t, e) || "",
                             {
                                 size: [h, u]
                             } = M_(c, o, r, s, n);
-                        return [(B_["function" == typeof a ? a(t, e) : a] - 1) * h / 2, (D_["function" == typeof l ? l(t, e) : l] - 1) * u / 2, h, u]
+                        return [(B_["function" == typeof a ? a(t, e) : a] - 1) * h / 2, (N_["function" == typeof l ? l(t, e) : l] - 1) * u / 2, h, u]
                     })), wo(this, "getIconOffsets", ((t, e) => {
                         const n = this.state.fontAtlasManager.mapping,
                             i = this.state.getText,
                             {
                                 wordBreak: r,
                                 maxWidth: s,
                                 lineHeight: o,
@@ -26421,15 +26421,15 @@
                             {
                                 x: h,
                                 y: u,
                                 rowWidth: d,
                                 size: [p, f]
                             } = M_(c, o, r, s, n),
                             g = B_["function" == typeof a ? a(t, e) : a],
-                            m = D_["function" == typeof l ? l(t, e) : l],
+                            m = N_["function" == typeof l ? l(t, e) : l],
                             v = h.length,
                             b = new Array(2 * v);
                         let y = 0;
                         for (let t = 0; t < v; t++) {
                             const e = (1 - g) * (p - d[t]) / 2;
                             b[y++] = (g - 1) * p / 2 + e + h[t], b[y++] = (m - 1) * f / 2 + u[t]
                         }
@@ -26577,33 +26577,33 @@
                         backgroundPadding: v,
                         background: b,
                         billboard: y,
                         fontSettings: _,
                         outlineWidth: x,
                         outlineColor: w,
                         sizeScale: E,
-                        sizeUnits: P,
-                        sizeMinPixels: S,
+                        sizeUnits: S,
+                        sizeMinPixels: P,
                         sizeMaxPixels: C,
                         transitions: T,
                         updateTriggers: A
-                    } = this.props, M = this.getSubLayerClass("characters", __), L = this.getSubLayerClass("background", F_);
-                    return [b && new L({
+                    } = this.props, M = this.getSubLayerClass("characters", __), O = this.getSubLayerClass("background", F_);
+                    return [b && new O({
                         getFillColor: f,
                         getLineColor: g,
                         getLineWidth: m,
                         padding: v,
                         getPosition: c,
                         getSize: u,
                         getAngle: d,
                         getPixelOffset: p,
                         billboard: y,
                         sizeScale: E / this.state.fontAtlasManager.props.fontSize,
-                        sizeUnits: P,
-                        sizeMinPixels: S,
+                        sizeUnits: S,
+                        sizeMinPixels: P,
                         sizeMaxPixels: C,
                         transitions: T && {
                             getPosition: T.getPosition,
                             getAngle: T.getAngle,
                             getSize: T.getSize,
                             getFillColor: T.getBackgroundColor,
                             getLineColor: T.getBorderColor,
@@ -26633,28 +26633,28 @@
                             attributes: a.attributes.background
                         } : a,
                         _dataDiff: l,
                         autoHighlight: !1,
                         getBoundingRect: this.getBoundingRect
                     }), new M({
                         sdf: _.sdf,
-                        smoothing: Number.isFinite(_.smoothing) ? _.smoothing : O_.smoothing,
+                        smoothing: Number.isFinite(_.smoothing) ? _.smoothing : L_.smoothing,
                         outlineWidth: x,
                         outlineColor: w,
                         iconAtlas: r,
                         iconMapping: s,
                         getPosition: c,
                         getColor: h,
                         getSize: u,
                         getAngle: d,
                         getPixelOffset: p,
                         billboard: y,
                         sizeScale: E * i,
-                        sizeUnits: P,
-                        sizeMinPixels: S * i,
+                        sizeUnits: S,
+                        sizeMinPixels: P * i,
                         sizeMaxPixels: C * i,
                         transitions: T && {
                             getPosition: T.getPosition,
                             getAngle: T.getAngle,
                             getColor: T.getColor,
                             getSize: T.getSize,
                             getPixelOffset: T.getPixelOffset
@@ -26682,15 +26682,15 @@
                         numInstances: e,
                         getIconOffsets: this.getIconOffsets,
                         getIcon: n
                     })]
                 }
                 static set fontAtlasCacheLimit(t) {
                     ! function(t) {
-                        ta.assert(Number.isFinite(t) && t >= 3, "Invalid cache limit"), R_ = new L_(t)
+                        ta.assert(Number.isFinite(t) && t >= 3, "Invalid cache limit"), I_ = new O_(t)
                     }(t)
                 }
             }
             wo(U_, "defaultProps", V_), wo(U_, "layerName", "TextLayer");
             const G_ = {
                     circle: {
                         type: b_,
@@ -26797,15 +26797,15 @@
                 props: e
             }) {
                 const n = {};
                 for (const i in e) n[i] = t.defaultProps[e[i]];
                 return n
             }
 
-            function q_(t, e) {
+            function X_(t, e) {
                 const {
                     transitions: n,
                     updateTriggers: i
                 } = t.props, r = {
                     updateTriggers: {},
                     transitions: n && {
                         getPosition: n.geometry
@@ -26815,15 +26815,15 @@
                     const o = e[s];
                     let a = t.props[s];
                     s.startsWith("get") && (a = t.getSubLayerAccessor(a), r.updateTriggers[o] = i[s], n && (r.transitions[o] = n[s])), r[o] = a
                 }
                 return r
             }
 
-            function X_(t, e, n = {}) {
+            function q_(t, e, n = {}) {
                 const i = {
                         pointFeatures: [],
                         lineFeatures: [],
                         polygonFeatures: [],
                         polygonOutlineFeatures: []
                     },
                     {
@@ -27102,23 +27102,23 @@
                         i = this.getSubLayerRow.bind(this);
                     let r = {};
                     const s = {};
                     if (Array.isArray(e.dataChanged)) {
                         const t = this.state.features;
                         for (const e in t) r[e] = t[e].slice(), s[e] = [];
                         for (const o of e.dataChanged) {
-                            const e = X_(n, i, o);
+                            const e = q_(n, i, o);
                             for (const n in t) s[n].push(i_({
                                 data: r[n],
                                 getIndex: t => t.__source.index,
                                 dataRange: o,
                                 replace: e[n]
                             }))
                         }
-                    } else r = X_(n, i);
+                    } else r = q_(n, i);
                     const o = function(t, e) {
                         const n = {
                                 points: {},
                                 lines: {},
                                 polygons: {},
                                 polygonsOutline: {}
                             },
@@ -27153,15 +27153,15 @@
                     const {
                         extruded: t,
                         wireframe: e
                     } = this.props, {
                         layerProps: n
                     } = this.state, i = "polygons-fill", r = this.shouldRenderSubLayer(i, n.polygons.data) && this.getSubLayerClass(i, H_.type);
                     if (r) {
-                        const s = q_(this, H_.props),
+                        const s = X_(this, H_.props),
                             o = t && e;
                         return o || delete s.getLineColor, s.updateTriggers.lineColors = o, new r(s, this.getSubLayerProps({
                             id: i,
                             updateTriggers: s.updateTriggers
                         }), n.polygons)
                     }
                     return null
@@ -27170,15 +27170,15 @@
                     const {
                         extruded: t,
                         stroked: e
                     } = this.props, {
                         layerProps: n
                     } = this.state, i = "polygons-stroke", r = "linestrings", s = !t && e && this.shouldRenderSubLayer(i, n.polygonsOutline.data) && this.getSubLayerClass(i, W_.type), o = this.shouldRenderSubLayer(r, n.lines.data) && this.getSubLayerClass(r, W_.type);
                     if (s || o) {
-                        const t = q_(this, W_.props);
+                        const t = X_(this, W_.props);
                         return [s && new s(t, this.getSubLayerProps({
                             id: i,
                             updateTriggers: t.updateTriggers
                         }), n.polygonsOutline), o && new o(t, this.getSubLayerProps({
                             id: r,
                             updateTriggers: t.updateTriggers
                         }), n.lines)]
@@ -27199,15 +27199,15 @@
                     const r = new Set(t.split("+")),
                         s = [];
                     for (const t of r) {
                         const r = "points-".concat(t),
                             o = G_[t],
                             a = o && this.shouldRenderSubLayer(r, e.points.data) && this.getSubLayerClass(r, o.type);
                         if (a) {
-                            const l = q_(this, o.props);
+                            const l = X_(this, o.props);
                             let c = e.points;
                             if ("text" === t && n) {
                                 const {
                                     instancePickingColors: t,
                                     ...e
                                 } = c.data.attributes;
                                 c = {
@@ -27406,17 +27406,17 @@
                     } = this;
                     let l;
                     if (Number.isFinite(s)) l = lx(a, [i, o, s, 1]);
                     else {
                         const t = lx(a, [i, o, -1, 1]),
                             e = lx(a, [i, o, 1, 1]),
                             r = ((n || 0) / rx + 1) * sx,
-                            s = Sc(Ec([], t, e)),
-                            c = Sc(t),
-                            h = Sc(e),
+                            s = Pc(Ec([], t, e)),
+                            c = Pc(t),
+                            h = Pc(e),
                             u = (4 * c * h - (s - c - h) ** 2) / 16 * 4 / s;
                         l = function(t, e, n, i) {
                             var r = e[0],
                                 s = e[1],
                                 o = e[2];
                             return t[0] = r + i * (n[0] - r), t[1] = s + i * (n[1] - s), t[2] = o + i * (n[2] - o), t
                         }([], t, e, (Math.sqrt(c - u) - Math.sqrt(Math.max(0, r * r - u))) / Math.sqrt(s))
@@ -27425,15 +27425,15 @@
                     return Number.isFinite(s) ? [c, h, u] : Number.isFinite(n) ? [c, h, n] : [c, h]
                 }
                 projectPosition(t) {
                     const [e, n, i = 0] = t, r = e * nx, s = n * nx, o = Math.cos(s), a = (i / rx + 1) * sx;
                     return [Math.sin(r) * o * a, -Math.cos(r) * o * a, Math.sin(s) * a]
                 }
                 unprojectPosition(t) {
-                    const [e, n, i] = t, r = Pc(t), s = Math.asin(i / r);
+                    const [e, n, i] = t, r = Sc(t), s = Math.asin(i / r);
                     return [Math.atan2(e, -n) * ix, s * ix, (r / sx - 1) * rx]
                 }
                 projectFlat(t) {
                     return t
                 }
                 unprojectFlat(t) {
                     return t
@@ -27444,23 +27444,23 @@
                         longitude: t[0] - n[0] + this.longitude,
                         latitude: t[1] - n[1] + this.latitude
                     }
                 }
             }
 
             function lx(t, e) {
-                const n = qc([], e, t);
+                const n = Xc([], e, t);
                 return Zc(n, n, 1 / n[3]), n
             }
             const cx = -1,
-                hx = new Lc,
-                ux = new Lc;
+                hx = new Oc,
+                ux = new Oc;
             class dx {
                 constructor(t = [0, 0, 0], e = [0, 0, 0], n) {
-                    wo(this, "center", void 0), wo(this, "halfDiagonal", void 0), wo(this, "minimum", void 0), wo(this, "maximum", void 0), n = n || hx.copy(t).add(e).scale(.5), this.center = new Lc(n), this.halfDiagonal = new Lc(e).subtract(this.center), this.minimum = new Lc(t), this.maximum = new Lc(e)
+                    wo(this, "center", void 0), wo(this, "halfDiagonal", void 0), wo(this, "minimum", void 0), wo(this, "maximum", void 0), n = n || hx.copy(t).add(e).scale(.5), this.center = new Oc(n), this.halfDiagonal = new Oc(e).subtract(this.center), this.minimum = new Oc(t), this.maximum = new Oc(e)
                 }
                 clone() {
                     return new dx(this.minimum, this.maximum, this.center)
                 }
                 equals(t) {
                     return this === t || Boolean(t) && this.minimum.equals(t.minimum) && this.maximum.equals(t.maximum)
                 }
@@ -27481,25 +27481,25 @@
                         {
                             halfDiagonal: n
                         } = this;
                     let i, r = 0;
                     return i = Math.abs(e.x) - n.x, i > 0 && (r += i * i), i = Math.abs(e.y) - n.y, i > 0 && (r += i * i), i = Math.abs(e.z) - n.z, i > 0 && (r += i * i), r
                 }
             }
-            const px = new Lc,
-                fx = new Lc;
+            const px = new Oc,
+                fx = new Oc;
             class gx {
                 constructor(t = [0, 0, 0], e = 0) {
-                    wo(this, "center", void 0), wo(this, "radius", void 0), this.radius = -0, this.center = new Lc, this.fromCenterRadius(t, e)
+                    wo(this, "center", void 0), wo(this, "radius", void 0), this.radius = -0, this.center = new Oc, this.fromCenterRadius(t, e)
                 }
                 fromCenterRadius(t, e) {
                     return this.center.from(t), this.radius = e, this
                 }
                 fromCornerPoints(t, e) {
-                    return e = px.from(e), this.center = (new Lc).from(t).add(e).scale(.5), this.radius = this.center.distance(e), this
+                    return e = px.from(e), this.center = (new Oc).from(t).add(e).scale(.5), this.radius = this.center.distance(e), this
                 }
                 equals(t) {
                     return this === t || Boolean(t) && this.center.equals(t.center) && this.radius === t.radius
                 }
                 clone() {
                     return new gx(this.center, this.radius)
                 }
@@ -27701,17 +27701,17 @@
                     return this.transform(t, e)
                 }
                 transformVector3(t, e) {
                     return this.transform(t, e)
                 }
             }
             let xx, wx, Ex;
-            class Px extends pc {
+            class Sx extends pc {
                 static get ZERO() {
-                    return Ex || (Ex = new Px(0, 0, 0, 0), Object.freeze(Ex)), Ex
+                    return Ex || (Ex = new Sx(0, 0, 0, 0), Object.freeze(Ex)), Ex
                 }
                 constructor(t = 0, e = 0, n = 0, i = 0) {
                     super(-0, -0, -0, -0), sc(t) && 1 === arguments.length ? this.copy(t) : (ic.debug && (hc(t), hc(e), hc(n), hc(i)), this[0] = t, this[1] = e, this[2] = n, this[3] = i)
                 }
                 set(t, e, n, i) {
                     return this[0] = t, this[1] = e, this[2] = n, this[3] = i, this.check()
                 }
@@ -27756,15 +27756,15 @@
                     return wc(this, this, t), this.check()
                 }
                 applyMatrix4(t) {
                     return t.transform(this, this), this
                 }
             }
 
-            function Sx() {
+            function Px() {
                 var t = new gc(4);
                 return gc != Float32Array && (t[0] = 0, t[1] = 0, t[2] = 0), t[3] = 1, t
             }
 
             function Cx(t, e, n) {
                 n *= .5;
                 var i = Math.sin(n);
@@ -27778,47 +27778,47 @@
                     o = e[3],
                     a = n[0],
                     l = n[1],
                     c = n[2],
                     h = n[3];
                 return t[0] = i * h + o * a + r * c - s * l, t[1] = r * h + o * l + s * a - i * c, t[2] = s * h + o * c + i * l - r * a, t[3] = o * h - i * a - r * l - s * c, t
             }
-            var Ax, Mx, Lx, Ox, Rx = Zc,
+            var Ax, Mx, Ox, Lx, Ix = Zc,
                 kx = function(t) {
                     var e = t[0],
                         n = t[1],
                         i = t[2],
                         r = t[3];
                     return Math.hypot(e, n, i, r)
                 },
-                Ix = function(t) {
+                Rx = function(t) {
                     var e = t[0],
                         n = t[1],
                         i = t[2],
                         r = t[3];
                     return e * e + n * n + i * i + r * r
                 },
-                jx = (Ax = mc(), Mx = vc(1, 0, 0), Lx = vc(0, 1, 0), function(t, e, n) {
+                jx = (Ax = mc(), Mx = vc(1, 0, 0), Ox = vc(0, 1, 0), function(t, e, n) {
                     var i = bc(e, n);
-                    return i < -.999999 ? (yc(Ax, Mx, e), Pc(Ax) < 1e-6 && yc(Ax, Lx, e), function(t, e) {
+                    return i < -.999999 ? (yc(Ax, Mx, e), Sc(Ax) < 1e-6 && yc(Ax, Ox, e), function(t, e) {
                         var n = e[0],
                             i = e[1],
                             r = e[2],
                             s = n * n + i * i + r * r;
                         s > 0 && (s = 1 / Math.sqrt(s)), t[0] = e[0] * s, t[1] = e[1] * s, t[2] = e[2] * s
                     }(Ax, Ax), Cx(t, Ax, Math.PI), t) : i > .999999 ? (t[0] = 0, t[1] = 0, t[2] = 0, t[3] = 1, t) : (yc(Ax, e, n), t[0] = Ax[0], t[1] = Ax[1], t[2] = Ax[2], t[3] = 1 + i, function(t, e) {
                         var n = e[0],
                             i = e[1],
                             r = e[2],
                             s = e[3],
                             o = n * n + i * i + r * r + s * s;
                         return o > 0 && (o = 1 / Math.sqrt(o)), t[0] = n * o, t[1] = i * o, t[2] = r * o, t[3] = s * o, t
                     }(t, t))
                 });
-            Sx(), Sx(), Ox = new gc(9), gc != Float32Array && (Ox[1] = 0, Ox[2] = 0, Ox[3] = 0, Ox[5] = 0, Ox[6] = 0, Ox[7] = 0), Ox[0] = 1, Ox[4] = 1, Ox[8] = 1;
+            Px(), Px(), Lx = new gc(9), gc != Float32Array && (Lx[1] = 0, Lx[2] = 0, Lx[3] = 0, Lx[5] = 0, Lx[6] = 0, Lx[7] = 0), Lx[0] = 1, Lx[4] = 1, Lx[8] = 1;
             const zx = [0, 0, 0, 1];
             class Fx extends cc {
                 constructor(t = 0, e = 0, n = 0, i = 1) {
                     super(-0, -0, -0, -0), Array.isArray(t) && 1 === arguments.length ? this.copy(t) : this.set(t, e, n, i)
                 }
                 copy(t) {
                     return this[0] = t[0], this[1] = t[1], this[2] = t[2], this[3] = t[3], this.check()
@@ -27880,15 +27880,15 @@
                 set w(t) {
                     this[3] = hc(t)
                 }
                 len() {
                     return kx(this)
                 }
                 lengthSquared() {
-                    return Ix(this)
+                    return Rx(this)
                 }
                 dot(t) {
                     return function(t, e) {
                         return t[0] * e[0] + t[1] * e[1] + t[2] * e[2] + t[3] * e[3]
                     }(this, t)
                 }
                 rotationTo(t, e) {
@@ -27976,15 +27976,15 @@
                             o = e[3],
                             a = Math.sin(n),
                             l = Math.cos(n);
                         t[0] = i * l + r * a, t[1] = r * l - i * a, t[2] = s * l + o * a, t[3] = o * l - s * a
                     }(this, this, t), this.check()
                 }
                 scale(t) {
-                    return Rx(this, this, t), this.check()
+                    return Ix(this, this, t), this.check()
                 }
                 slerp(t, e, n) {
                     let i, r, s;
                     switch (arguments.length) {
                         case 1:
                             ({
                                 start: i = zx,
@@ -28006,15 +28006,15 @@
                             p = n[0],
                             f = n[1],
                             g = n[2],
                             m = n[3];
                         (s = c * p + h * f + u * g + d * m) < 0 && (s = -s, p = -p, f = -f, g = -g, m = -m), 1 - s > fc ? (r = Math.acos(s), o = Math.sin(r), a = Math.sin((1 - i) * r) / o, l = Math.sin(i * r) / o) : (a = 1 - i, l = i), t[0] = a * c + l * p, t[1] = a * h + l * f, t[2] = a * u + l * g, t[3] = a * d + l * m
                     }(this, i, r, s), this.check()
                 }
-                transformVector4(t, e = new Px) {
+                transformVector4(t, e = new Sx) {
                     return function(t, e, n) {
                         var i = e[0],
                             r = e[1],
                             s = e[2],
                             o = n[0],
                             a = n[1],
                             l = n[2],
@@ -28035,54 +28035,54 @@
                 premultiply(t) {
                     return this.multiplyLeft(t)
                 }
                 multiply(t) {
                     return this.multiplyRight(t)
                 }
             }
-            const Bx = new Lc,
-                Dx = new Lc,
-                Nx = new Lc,
-                Vx = new Lc,
-                Ux = new Lc,
-                Gx = new Lc,
-                Wx = new Lc;
+            const Bx = new Oc,
+                Nx = new Oc,
+                Dx = new Oc,
+                Vx = new Oc,
+                Ux = new Oc,
+                Gx = new Oc,
+                Wx = new Oc;
             class Hx {
                 constructor(t = [0, 0, 0], e = [0, 0, 0, 0, 0, 0, 0, 0, 0]) {
-                    wo(this, "center", void 0), wo(this, "halfAxes", void 0), this.center = (new Lc).from(t), this.halfAxes = new _x(e)
+                    wo(this, "center", void 0), wo(this, "halfAxes", void 0), this.center = (new Oc).from(t), this.halfAxes = new _x(e)
                 }
                 get halfSize() {
                     const t = this.halfAxes.getColumn(0),
                         e = this.halfAxes.getColumn(1),
                         n = this.halfAxes.getColumn(2);
-                    return [new Lc(t).len(), new Lc(e).len(), new Lc(n).len()]
+                    return [new Oc(t).len(), new Oc(e).len(), new Oc(n).len()]
                 }
                 get quaternion() {
                     const t = this.halfAxes.getColumn(0),
                         e = this.halfAxes.getColumn(1),
                         n = this.halfAxes.getColumn(2),
-                        i = new Lc(t).normalize(),
-                        r = new Lc(e).normalize(),
-                        s = new Lc(n).normalize();
+                        i = new Oc(t).normalize(),
+                        r = new Oc(e).normalize(),
+                        s = new Oc(n).normalize();
                     return (new Fx).fromMatrix3(new _x([...i, ...r, ...s]))
                 }
                 fromCenterHalfSizeQuaternion(t, e, n) {
                     const i = new Fx(n),
                         r = (new _x).fromQuaternion(i);
-                    return r[0] = r[0] * e[0], r[1] = r[1] * e[0], r[2] = r[2] * e[0], r[3] = r[3] * e[1], r[4] = r[4] * e[1], r[5] = r[5] * e[1], r[6] = r[6] * e[2], r[7] = r[7] * e[2], r[8] = r[8] * e[2], this.center = (new Lc).from(t), this.halfAxes = r, this
+                    return r[0] = r[0] * e[0], r[1] = r[1] * e[0], r[2] = r[2] * e[0], r[3] = r[3] * e[1], r[4] = r[4] * e[1], r[5] = r[5] * e[1], r[6] = r[6] * e[2], r[7] = r[7] * e[2], r[8] = r[8] * e[2], this.center = (new Oc).from(t), this.halfAxes = r, this
                 }
                 clone() {
                     return new Hx(this.center, this.halfAxes)
                 }
                 equals(t) {
                     return this === t || Boolean(t) && this.center.equals(t.center) && this.halfAxes.equals(t.halfAxes)
                 }
                 getBoundingSphere(t = new gx) {
                     const e = this.halfAxes,
-                        n = e.getColumn(0, Nx),
+                        n = e.getColumn(0, Dx),
                         i = e.getColumn(1, Vx),
                         r = e.getColumn(2, Ux),
                         s = Bx.copy(n).add(i).add(r);
                     return t.center.copy(this.center), t.radius = s.magnitude(), t
                 }
                 intersectPlane(t) {
                     const e = this.center,
@@ -28095,107 +28095,107 @@
                         l = n.dot(e) + t.distance;
                     return l <= -a ? cx : l >= a ? 1 : 0
                 }
                 distanceTo(t) {
                     return Math.sqrt(this.distanceSquaredTo(t))
                 }
                 distanceSquaredTo(t) {
-                    const e = Dx.from(t).subtract(this.center),
+                    const e = Nx.from(t).subtract(this.center),
                         n = this.halfAxes,
-                        i = n.getColumn(0, Nx),
+                        i = n.getColumn(0, Dx),
                         r = n.getColumn(1, Vx),
                         s = n.getColumn(2, Ux),
                         o = i.magnitude(),
                         a = r.magnitude(),
                         l = s.magnitude();
                     i.normalize(), r.normalize(), s.normalize();
                     let c, h = 0;
                     return c = Math.abs(e.dot(i)) - o, c > 0 && (h += c * c), c = Math.abs(e.dot(r)) - a, c > 0 && (h += c * c), c = Math.abs(e.dot(s)) - l, c > 0 && (h += c * c), h
                 }
                 computePlaneDistances(t, e, n = [-0, -0]) {
                     let i = Number.POSITIVE_INFINITY,
                         r = Number.NEGATIVE_INFINITY;
                     const s = this.center,
                         o = this.halfAxes,
-                        a = o.getColumn(0, Nx),
+                        a = o.getColumn(0, Dx),
                         l = o.getColumn(1, Vx),
                         c = o.getColumn(2, Ux),
                         h = Gx.copy(a).add(l).add(c).add(s),
                         u = Wx.copy(h).subtract(t);
                     let d = e.dot(u);
                     return i = Math.min(d, i), r = Math.max(d, r), h.copy(s).add(a).add(l).subtract(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), h.copy(s).add(a).subtract(l).add(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), h.copy(s).add(a).subtract(l).subtract(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), s.copy(h).subtract(a).add(l).add(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), s.copy(h).subtract(a).add(l).subtract(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), s.copy(h).subtract(a).subtract(l).add(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), s.copy(h).subtract(a).subtract(l).subtract(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), n[0] = i, n[1] = r, n
                 }
                 transform(t) {
                     this.center.transformAsPoint(t);
-                    const e = this.halfAxes.getColumn(0, Nx);
+                    const e = this.halfAxes.getColumn(0, Dx);
                     e.transformAsPoint(t);
                     const n = this.halfAxes.getColumn(1, Vx);
                     n.transformAsPoint(t);
                     const i = this.halfAxes.getColumn(2, Ux);
                     return i.transformAsPoint(t), this.halfAxes = new _x([...e, ...n, ...i]), this
                 }
                 getTransform() {
                     throw new Error("not implemented")
                 }
             }
-            const Zx = new Lc,
-                qx = new Lc;
-            class Xx {
+            const Zx = new Oc,
+                Xx = new Oc;
+            class qx {
                 constructor(t = [0, 0, 1], e = 0) {
-                    wo(this, "normal", void 0), wo(this, "distance", void 0), this.normal = new Lc, this.distance = -0, this.fromNormalDistance(t, e)
+                    wo(this, "normal", void 0), wo(this, "distance", void 0), this.normal = new Oc, this.distance = -0, this.fromNormalDistance(t, e)
                 }
                 fromNormalDistance(t, e) {
                     return dc(Number.isFinite(e)), this.normal.from(t).normalize(), this.distance = e, this
                 }
                 fromPointNormal(t, e) {
                     t = Zx.from(t), this.normal.from(e).normalize();
                     const n = -this.normal.dot(t);
                     return this.distance = n, this
                 }
                 fromCoefficients(t, e, n, i) {
                     return this.normal.set(t, e, n), dc(lc(this.normal.len(), 1)), this.distance = i, this
                 }
                 clone() {
-                    return new Xx(this.normal, this.distance)
+                    return new qx(this.normal, this.distance)
                 }
                 equals(t) {
                     return lc(this.distance, t.distance) && lc(this.normal, t.normal)
                 }
                 getPointDistance(t) {
                     return this.normal.dot(t) + this.distance
                 }
                 transform(t) {
-                    const e = qx.copy(this.normal).transformAsVector(t).normalize(),
+                    const e = Xx.copy(this.normal).transformAsVector(t).normalize(),
                         n = this.normal.scale(-this.distance).transform(t);
                     return this.fromPointNormal(n, e)
                 }
                 projectPointOntoPlane(t, e = [0, 0, 0]) {
                     t = Zx.from(t);
                     const n = this.getPointDistance(t),
-                        i = qx.copy(this.normal).scale(n);
+                        i = Xx.copy(this.normal).scale(n);
                     return t.subtract(i).to(e)
                 }
             }
-            const Yx = [new Lc([1, 0, 0]), new Lc([0, 1, 0]), new Lc([0, 0, 1])],
-                Kx = new Lc,
-                $x = new Lc;
-            new Xx(new Lc(1, 0, 0), 0);
+            const Yx = [new Oc([1, 0, 0]), new Oc([0, 1, 0]), new Oc([0, 0, 1])],
+                Kx = new Oc,
+                $x = new Oc;
+            new qx(new Oc(1, 0, 0), 0);
             class Jx {
                 constructor(t = []) {
                     wo(this, "planes", void 0), this.planes = t
                 }
                 fromBoundingSphere(t) {
                     this.planes.length = 2 * Yx.length;
                     const e = t.center,
                         n = t.radius;
                     let i = 0;
                     for (const t of Yx) {
                         let r = this.planes[i],
                             s = this.planes[i + 1];
-                        r || (r = this.planes[i] = new Xx), s || (s = this.planes[i + 1] = new Xx);
+                        r || (r = this.planes[i] = new qx), s || (s = this.planes[i + 1] = new qx);
                         const o = Kx.copy(t).scale(-n).add(e);
                         t.dot(o), r.fromPointNormal(o, t);
                         const a = Kx.copy(t).scale(n).add(e),
                             l = $x.copy(t).negate();
                         l.dot(a), s.fromPointNormal(a, l), i += 2
                     }
                     return this
@@ -28221,15 +28221,15 @@
                             a = t.intersectPlane(o);
                         if (a === cx) return Jx.MASK_OUTSIDE;
                         0 === a && (n |= s)
                     }
                     return n
                 }
             }
-            wo(Jx, "MASK_OUTSIDE", 4294967295), wo(Jx, "MASK_INSIDE", 0), wo(Jx, "MASK_INDETERMINATE", 2147483647), new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, Math.PI;
+            wo(Jx, "MASK_OUTSIDE", 4294967295), wo(Jx, "MASK_INSIDE", 0), wo(Jx, "MASK_INDETERMINATE", 2147483647), new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, Math.PI;
             const Qx = {
                     EPSILON1: .1,
                     EPSILON2: .01,
                     EPSILON3: .001,
                     EPSILON4: 1e-4,
                     EPSILON5: 1e-5,
                     EPSILON6: 1e-6,
@@ -28284,19 +28284,19 @@
                 if (Math.abs(t[tw.getElementIndex(o, s)]) > n) {
                     const e = (t[tw.getElementIndex(o, o)] - t[tw.getElementIndex(s, s)]) / 2 / t[tw.getElementIndex(o, s)];
                     let n;
                     n = e < 0 ? -1 / (-e + Math.sqrt(1 + e * e)) : 1 / (e + Math.sqrt(1 + e * e)), a = 1 / Math.sqrt(1 + n * n), l = n * a
                 }
                 return _x.IDENTITY.to(e), e[tw.getElementIndex(s, s)] = e[tw.getElementIndex(o, o)] = a, e[tw.getElementIndex(o, s)] = l, e[tw.getElementIndex(s, o)] = -l, e
             }
-            const cw = new Lc,
-                hw = new Lc,
-                uw = new Lc,
-                dw = new Lc,
-                pw = new Lc,
+            const cw = new Oc,
+                hw = new Oc,
+                uw = new Oc,
+                dw = new Oc,
+                pw = new Oc,
                 fw = new _x,
                 gw = {
                     diagonal: new _x,
                     unitary: new _x
                 },
                 mw = 512,
                 vw = [
@@ -28371,17 +28371,17 @@
                         const e = this.z < 1 ? yw : this.z < 2 ? bw : vw,
                             i = [];
                         for (const r of e) {
                             const e = Tw(this.x + r[0], this.y + r[1], this.z);
                             e[2] = t[0], i.push(n(e)), t[0] !== t[1] && (e[2] = t[1], i.push(n(e)))
                         }
                         return function(t, e = new Hx) {
-                            if (!t || 0 === t.length) return e.halfAxes = new _x([0, 0, 0, 0, 0, 0, 0, 0, 0]), e.center = new Lc, e;
+                            if (!t || 0 === t.length) return e.halfAxes = new _x([0, 0, 0, 0, 0, 0, 0, 0, 0]), e.center = new Oc, e;
                             const n = t.length,
-                                i = new Lc(0, 0, 0);
+                                i = new Oc(0, 0, 0);
                             for (const e of t) i.add(e);
                             const r = 1 / n;
                             i.multiplyByScalar(r);
                             let s = 0,
                                 o = 0,
                                 a = 0,
                                 l = 0,
@@ -28422,16 +28422,16 @@
                                 y = -Number.MAX_VALUE,
                                 _ = Number.MAX_VALUE,
                                 x = Number.MAX_VALUE,
                                 w = Number.MAX_VALUE;
                             for (const e of t) cw.copy(e), v = Math.max(cw.dot(f), v), b = Math.max(cw.dot(g), b), y = Math.max(cw.dot(m), y), _ = Math.min(cw.dot(f), _), x = Math.min(cw.dot(g), x), w = Math.min(cw.dot(m), w);
                             f = f.multiplyByScalar(.5 * (_ + v)), g = g.multiplyByScalar(.5 * (x + b)), m = m.multiplyByScalar(.5 * (w + y)), e.center.copy(f).add(g).add(m);
                             const E = hw.set(v - _, b - x, y - w).multiplyByScalar(.5),
-                                P = new _x([E[0], 0, 0, 0, E[1], 0, 0, 0, E[2]]);
-                            return e.halfAxes.multiplyRight(P), e
+                                S = new _x([E[0], 0, 0, 0, E[1], 0, 0, 0, E[2]]);
+                            return e.halfAxes.multiplyRight(S), e
                         }(i)
                     }
                     const i = Math.pow(2, this.z),
                         r = mw / i,
                         s = this.x * r + e * mw,
                         o = mw - (this.y + 1) * r;
                     return new dx([s, o, t[0]], [s + r, o + r, t[1]])
@@ -28450,20 +28450,20 @@
                         if (n !== e.length) return !1;
                         for (let i = 0; i < n; i++)
                             if (t[i] !== e[i]) return !1;
                         return !0
                     }
                 };
 
-            function Pw(t, e) {
+            function Sw(t, e) {
                 const n = [e.transformAsPoint([t[0], t[1]]), e.transformAsPoint([t[2], t[1]]), e.transformAsPoint([t[0], t[3]]), e.transformAsPoint([t[2], t[3]])];
                 return [Math.min(...n.map((t => t[0]))), Math.min(...n.map((t => t[1]))), Math.max(...n.map((t => t[0]))), Math.max(...n.map((t => t[1])))]
             }
 
-            function Sw({
+            function Pw({
                 viewport: t,
                 z: e,
                 cullRect: n
             }) {
                 const i = n.x - t.x,
                     r = n.y - t.y,
                     {
@@ -28476,20 +28476,20 @@
                         },
                         a = t.unproject([i, r], n),
                         l = t.unproject([i + s, r], n),
                         c = t.unproject([i, r + o], n),
                         h = t.unproject([i + s, r + o], n);
                     return [Math.min(a[0], l[0], c[0], h[0]), Math.min(a[1], l[1], c[1], h[1]), Math.max(a[0], l[0], c[0], h[0]), Math.max(a[1], l[1], c[1], h[1])]
                 }
-                const a = Sw({
+                const a = Pw({
                         viewport: t,
                         z: e[0],
                         cullRect: n
                     }),
-                    l = Sw({
+                    l = Pw({
                         viewport: t,
                         z: e[1],
                         cullRect: n
                     });
                 return [Math.min(a[0], l[0]), Math.min(a[1], l[1]), Math.max(a[2], l[2]), Math.max(a[3], l[3])]
             }
 
@@ -28524,15 +28524,15 @@
                     left: s,
                     top: o,
                     right: a,
                     bottom: l
                 }
             }
 
-            function Lw({
+            function Ow({
                 viewport: t,
                 maxZoom: e,
                 minZoom: n,
                 zRange: i,
                 extent: r,
                 tileSize: s = xw,
                 modelMatrix: o,
@@ -28542,20 +28542,20 @@
                 let c = t.isGeospatial ? Math.round(t.zoom + Math.log2(xw / s)) + l : Math.ceil(t.zoom) + l;
                 if ("number" == typeof n && Number.isFinite(n) && c < n) {
                     if (!r) return [];
                     c = n
                 }
                 "number" == typeof e && Number.isFinite(e) && c > e && (c = e);
                 let h = r;
-                return o && a && r && !t.isGeospatial && (h = Pw(r, o)), t.isGeospatial ? function(t, e, n, i) {
+                return o && a && r && !t.isGeospatial && (h = Sw(r, o)), t.isGeospatial ? function(t, e, n, i) {
                     const r = t instanceof ax && t.resolution ? t.projectPosition : null,
                         s = Object.values(t.getFrustumPlanes()).map((({
                             normal: t,
                             distance: e
-                        }) => new Xx(t.clone().negate(), e))),
+                        }) => new qx(t.clone().negate(), e))),
                         o = new Jx(s),
                         a = t.distanceScales.unitsPerMeter[2],
                         l = n && n[0] * a || 0,
                         c = n && n[1] * a || 0,
                         h = t instanceof kf && t.pitch <= 60 ? e : 0;
                     if (i) {
                         const [t, e, n, r] = i, s = mh([t, r]), o = mh([n, e]);
@@ -28580,33 +28580,33 @@
                 }(t, c, i, r) : function(t, e, n, i, r) {
                     const s = function(t, e, n) {
                             let i;
                             return i = t.getBounds(), t.isGeospatial ? [Math.max(i[0], n[0]), Math.max(i[1], n[1]), Math.min(i[2], n[2]), Math.min(i[3], n[3])] : [Math.max(Math.min(i[0], n[2]), n[0]), Math.max(Math.min(i[1], n[3]), n[1]), Math.min(Math.max(i[2], n[0]), n[2]), Math.min(Math.max(i[3], n[1]), n[3])]
                         }(t, 0, i),
                         o = Cw(e, n),
                         [a, l, c, h] = function(t, e, n) {
-                            return n ? Pw(t, n).map((t => t * e / xw)) : t.map((t => t * e / xw))
+                            return n ? Sw(t, n).map((t => t * e / xw)) : t.map((t => t * e / xw))
                         }(s, o, r),
                         u = [];
                     for (let t = Math.floor(a); t < c; t++)
                         for (let n = Math.floor(l); n < h; n++) u.push({
                             x: t,
                             y: n,
                             z: e
                         });
                     return u
                 }(t, c, s, h || ww, a)
             }
-            var Ow = n(4155);
+            var Lw = n(4155);
 
-            function Rw() {
+            function Iw() {
                 let t;
                 if ("undefined" != typeof window && window.performance) t = window.performance.now();
-                else if (void 0 !== Ow && Ow.hrtime) {
-                    const e = Ow.hrtime();
+                else if (void 0 !== Lw && Lw.hrtime) {
+                    const e = Lw.hrtime();
                     t = 1e3 * e[0] + e[1] / 1e6
                 } else t = Date.now();
                 return t
             }
             class kw {
                 constructor(t, e) {
                     this.name = void 0, this.type = void 0, this.sampleSize = 1, this.time = 0, this.count = 0, this.samples = 0, this.lastTiming = 0, this.lastSampleTime = 0, this.lastSampleCount = 0, this._count = 0, this._time = 0, this._samples = 0, this._startTime = 0, this._timerPending = !1, this.name = t, this.type = e, this.reset()
@@ -28629,18 +28629,18 @@
                 subtractCount(t) {
                     return this._count -= t, this._samples++, this._checkSampling(), this
                 }
                 addTime(t) {
                     return this._time += t, this.lastTiming = t, this._samples++, this._checkSampling(), this
                 }
                 timeStart() {
-                    return this._startTime = Rw(), this._timerPending = !0, this
+                    return this._startTime = Iw(), this._timerPending = !0, this
                 }
                 timeEnd() {
-                    return this._timerPending ? (this.addTime(Rw() - this._startTime), this._timerPending = !1, this._checkSampling(), this) : this
+                    return this._timerPending ? (this.addTime(Iw() - this._startTime), this._timerPending = !1, this._checkSampling(), this) : this
                 }
                 getSampleAverageCount() {
                     return this.sampleSize > 0 ? this.lastSampleCount / this.sampleSize : 0
                 }
                 getSampleAverageTime() {
                     return this.sampleSize > 0 ? this.lastSampleTime / this.sampleSize : 0
                 }
@@ -28656,15 +28656,15 @@
                 getHz() {
                     return this.time > 0 ? this.samples / (this.time / 1e3) : 0
                 }
                 _checkSampling() {
                     this._samples === this.sampleSize && (this.lastSampleTime = this._time, this.lastSampleCount = this._count, this.count += this._count, this.time += this._time, this.samples += this._samples, this._time = 0, this._count = 0, this._samples = 0)
                 }
             }
-            class Iw {
+            class Rw {
                 constructor(t) {
                     this.id = void 0, this.stats = {}, this.id = t.id, this.stats = {}, this._initializeStats(t.stats), Object.seal(this)
                 }
                 get(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "count";
                     return this._getOrCreate({
                         name: t,
@@ -28711,15 +28711,15 @@
             };
             class zw {
                 constructor() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     wo(this, "props", void 0), wo(this, "stats", void 0), wo(this, "activeRequestCount", 0), wo(this, "requestQueue", []), wo(this, "requestMap", new Map), wo(this, "deferredUpdate", null), this.props = {
                         ...jw,
                         ...t
-                    }, this.stats = new Iw({
+                    }, this.stats = new Rw({
                         id: this.props.id
                     }), this.stats.get("Queued Requests"), this.stats.get("Active Requests"), this.stats.get("Cancelled Requests"), this.stats.get("Queued Requests Ever"), this.stats.get("Active Requests Ever")
                 }
                 scheduleRequest(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : () => 0;
                     if (!this.props.throttleRequests) return Promise.resolve({
                         done: () => {}
@@ -28774,45 +28774,45 @@
                     return t.priority = t.getPriority(t.handle), !(t.priority < 0 && (t.resolve(null), 1))
                 }
             }
             const Fw = "best-available",
                 Bw = {
                     [Fw]: function(t) {
                         for (const e of t) e.state = 0;
-                        for (const e of t) e.isSelected && !Dw(e) && Nw(e);
+                        for (const e of t) e.isSelected && !Nw(e) && Dw(e);
                         for (const e of t) e.isVisible = Boolean(2 & e.state)
                     },
                     "no-overlap": function(t) {
                         for (const e of t) e.state = 0;
-                        for (const e of t) e.isSelected && Dw(e);
+                        for (const e of t) e.isSelected && Nw(e);
                         const e = Array.from(t).sort(((t, e) => t.zoom - e.zoom));
                         for (const t of e)
                             if (t.isVisible = Boolean(2 & t.state), t.children && (t.isVisible || 1 & t.state))
                                 for (const e of t.children) e.state = 1;
-                            else t.isSelected && Nw(t)
+                            else t.isSelected && Dw(t)
                     },
                     never: () => {}
                 };
 
-            function Dw(t) {
+            function Nw(t) {
                 let e = t;
                 for (; e;) {
                     if (e.isLoaded || e.content) return e.state |= 2, !0;
                     e = e.parent
                 }
                 return !1
             }
 
-            function Nw(t) {
-                for (const e of t.children) e.isLoaded || e.content ? e.state |= 2 : Nw(e)
+            function Dw(t) {
+                for (const e of t.children) e.isLoaded || e.content ? e.state |= 2 : Dw(e)
             }
             const Vw = {
                 TilesetClass: class {
                     constructor(t) {
-                        wo(this, "opts", void 0), wo(this, "_requestScheduler", void 0), wo(this, "_cache", void 0), wo(this, "_dirty", void 0), wo(this, "_tiles", void 0), wo(this, "_cacheByteSize", void 0), wo(this, "_viewport", void 0), wo(this, "_zRange", void 0), wo(this, "_selectedTiles", void 0), wo(this, "_frameNumber", void 0), wo(this, "_modelMatrix", void 0), wo(this, "_modelMatrixInverse", void 0), wo(this, "_maxZoom", void 0), wo(this, "_minZoom", void 0), wo(this, "onTileLoad", void 0), wo(this, "_getCullBounds", hf(Sw)), this.opts = t, this.onTileLoad = t => {
+                        wo(this, "opts", void 0), wo(this, "_requestScheduler", void 0), wo(this, "_cache", void 0), wo(this, "_dirty", void 0), wo(this, "_tiles", void 0), wo(this, "_cacheByteSize", void 0), wo(this, "_viewport", void 0), wo(this, "_zRange", void 0), wo(this, "_selectedTiles", void 0), wo(this, "_frameNumber", void 0), wo(this, "_modelMatrix", void 0), wo(this, "_modelMatrixInverse", void 0), wo(this, "_maxZoom", void 0), wo(this, "_minZoom", void 0), wo(this, "onTileLoad", void 0), wo(this, "_getCullBounds", hf(Pw)), this.opts = t, this.onTileLoad = t => {
                             this.opts.onTileLoad(t), this.opts.maxCacheByteSize && (this._cacheByteSize += t.byteLength, this._resizeCache())
                         }, this._requestScheduler = new zw({
                             maxRequests: t.maxRequests,
                             throttleRequests: t.maxRequests > 0
                         }), this._cache = new Map, this._tiles = [], this._dirty = !1, this._cacheByteSize = 0, this._viewport = null, this._selectedTiles = null, this._frameNumber = 0, this._modelMatrix = new Qc, this._modelMatrixInverse = new Qc, this.setOptions(t)
                     }
                     get tiles() {
@@ -28861,15 +28861,15 @@
                         }
                         const s = this.updateTileStates();
                         return this._pruneRequests(), this._dirty && this._resizeCache(), s && this._frameNumber++, this._frameNumber
                     }
                     isTileVisible(t, e) {
                         if (!t.isVisible) return !1;
                         if (e && this._viewport) {
-                            const [n, i, r, s] = Sw({
+                            const [n, i, r, s] = Pw({
                                 viewport: this._viewport,
                                 z: this._zRange,
                                 cullRect: e
                             }), {
                                 bbox: o
                             } = t;
                             if ("west" in o) return o.west < r && o.east > n && o.south < s && o.north > i;
@@ -28888,15 +28888,15 @@
                         modelMatrixInverse: s
                     }) {
                         const {
                             tileSize: o,
                             extent: a,
                             zoomOffset: l
                         } = this.opts;
-                        return Lw({
+                        return Ow({
                             viewport: t,
                             maxZoom: e,
                             minZoom: n,
                             zRange: i,
                             tileSize: o,
                             extent: a,
                             modelMatrix: r,
@@ -29212,15 +29212,16 @@
                         tile: n
                     } = t.props;
                     return this.state.tileset.isTileVisible(n, e)
                 }
             }
             wo(Uw, "defaultProps", Vw), wo(Uw, "layerName", "TileLayer");
             var Gw = n(9757),
-                Ww = t => {
+                Ww = n(8399),
+                Hw = t => {
                     const [e, n] = (0, c.useState)({
                         displayColorPicker: !1
                     }), [i, r, s] = t.channel.color;
                     return (0, o.jsxs)("div", {
                         className: "BioImageViewer-Slider",
                         children: [(0, o.jsxs)("div", {
                             className: "BioImageViewer-Slider__main",
@@ -29307,15 +29308,15 @@
                                 t.onChannelUpdate(Number((e?.target)?.value), t.channel.color, t.channel.visible, t.channel.id)
                             },
                             min: t.channel.min,
                             max: t.channel.max
                         })]
                     })
                 },
-                Hw = t => {
+                Zw = t => {
                     const e = (0, c.useRef)(null),
                         [n, i] = (0, c.useState)({
                             isOpen: !1
                         });
                     return (0, o.jsxs)("div", {
                         className: "BioImageViewer-ControlPanel",
                         children: [(0, o.jsxs)("h6", {
@@ -29382,24 +29383,24 @@
                             ref: e,
                             className: "BioImageViewer-ControlPanel__list",
                             style: {
                                 maxHeight: n.isOpen ? e.current?.scrollHeight : 0
                             },
                             children: t.channels.map(((e, n) => (0, o.jsx)("li", {
                                 className: "BioImageViewer-ControlPanel__item",
-                                children: (0, o.jsx)(Ww, {
+                                children: (0, o.jsx)(Hw, {
                                     channel: e,
                                     id: n,
                                     onChannelUpdate: t.onChannelUpdate
                                 })
                             }, e.id)))
                         })]
                     })
                 },
-                Zw = t => {
+                Xw = t => {
                     const e = e => {
                         t.onAttributeUpdate((e?.target)?.value)
                     };
                     return (0, o.jsxs)("div", {
                         className: "BioImageViewer-AttributePanel",
                         children: [(0, o.jsx)("h6", {
                             className: "BioImageViewer-AttributePanel__title",
@@ -29426,15 +29427,15 @@
                     })
                 };
             const qw = [
                     [255, 0, 0, 255],
                     [0, 255, 0, 255],
                     [0, 0, 255, 255]
                 ],
-                Xw = {
+                Yw = {
                     uint8: {
                         bytes: Uint8Array.BYTES_PER_ELEMENT,
                         format: Gw.Z.RED_INTEGER,
                         internalFormat: Gw.Z.R8UI,
                         type: Gw.Z.UNSIGNED_BYTE,
                         filtering: Gw.Z.NEAREST,
                         samplerType: "usampler2DArray",
@@ -29472,36 +29473,36 @@
                         filtering: Gw.Z.NEAREST,
                         samplerType: "sampler2DArray",
                         create: function(t) {
                             return new Float32Array(t)
                         }
                     }
                 },
-                Yw = {
+                Kw = {
                     fs: "#version 300 es\n#define SHADER_NAME image-layer-fragment-shader\n#define num_channels CHANNEL_NUMBER\n#define sampler_type SAMPLER_TYPE\n\nprecision highp sampler_type;\nprecision highp float;\nprecision highp int;\n\nuniform sampler_type texture_arr;\nuniform int channelMapping[num_channels];\nuniform vec4 colors[num_channels];\nuniform vec2 ranges[num_channels];\n\nin vec2 vTexCoord;\n\nvoid main() {\n  vec4 color = vec4(0);\n\n  for (int i = 0; i < num_channels; ++i)\n  {\n    if (channelMapping[i] == -1) continue;\n    float intensity = float(texture(texture_arr, vec3(vTexCoord.xy, channelMapping[i])).r);\n    color += colors[i] * clamp((intensity - ranges[i].x) / (ranges[i].y - ranges[i].x + 0.01), 0.0, 1.0);\n  }\n\n  gl_FragColor = vec4(color.rgb, 1.0);\n  \n  geometry.uv = vTexCoord;\n  DECKGL_FILTER_COLOR(gl_FragColor, geometry);\n}\n",
                     vs: "#version 300 es\n#define SHADER_NAME image-layer-vertex-shader\n\nattribute vec2 texCoords;\nattribute vec3 positions;\nattribute vec3 positions64Low;\nattribute vec3 instancePickingColors;\nvarying vec2 vTexCoord;\n\nvoid main(void) {\n  geometry.worldPosition = positions;\n  geometry.uv = texCoords;\n  geometry.pickingColor = instancePickingColors;\n  gl_Position = project_position_to_clipspace(positions, positions64Low, vec3(0.), geometry.position);\n  DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n  vTexCoord = texCoords;\n  vec4 color = vec4(0.);\n  DECKGL_FILTER_COLOR(color, geometry);\n}\n"
                 };
-            class Kw extends Yb {
+            class $w extends Yb {
                 constructor(t) {
                     super(t), this.state = {
                         texture: null
                     }
                 }
                 getShaders() {
                     const t = {
-                        ...Yw
+                        ...Kw
                     };
-                    return t.fs = t.fs.replace("CHANNEL_NUMBER", `${this.props.channels.length}`), t.fs = t.fs.replace("SAMPLER_TYPE", Xw[this.props.format].samplerType), super.getShaders({
+                    return t.fs = t.fs.replace("CHANNEL_NUMBER", `${this.props.channels.length}`), t.fs = t.fs.replace("SAMPLER_TYPE", Yw[this.props.format].samplerType), super.getShaders({
                         ...t,
                         modules: [sy, dy]
                     })
                 }
                 generateTexture(t) {
                     const e = t.createTexture();
-                    return t.activeTexture(t.TEXTURE0), t.bindTexture(t.TEXTURE_2D_ARRAY, e), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_MAG_FILTER, Xw[this.props.format].filtering), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_MIN_FILTER, Xw[this.props.format].filtering), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_WRAP_S, t.CLAMP_TO_EDGE), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_WRAP_T, t.CLAMP_TO_EDGE), t.texImage3D(t.TEXTURE_2D_ARRAY, 0, Xw[this.props.format].internalFormat, this.props.width, this.props.height, this.props.activeChannels, 0, Xw[this.props.format].format, Xw[this.props.format].type, this.props.data), e
+                    return t.activeTexture(t.TEXTURE0), t.bindTexture(t.TEXTURE_2D_ARRAY, e), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_MAG_FILTER, Yw[this.props.format].filtering), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_MIN_FILTER, Yw[this.props.format].filtering), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_WRAP_S, t.CLAMP_TO_EDGE), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_WRAP_T, t.CLAMP_TO_EDGE), t.texImage3D(t.TEXTURE_2D_ARRAY, 0, Yw[this.props.format].internalFormat, this.props.width, this.props.height, this.props.activeChannels, 0, Yw[this.props.format].format, Yw[this.props.format].type, this.props.data), e
                 }
                 initializeState() {
                     const {
                         gl: t
                     } = this.context;
                     t.pixelStorei(Gw.Z.UNPACK_ALIGNMENT, 1), t.pixelStorei(Gw.Z.PACK_ALIGNMENT, 1);
                     const e = this.getAttributeManager();
@@ -29590,28 +29591,28 @@
                             channelMapping: this.state.channelMapping,
                             colors: this.props.channels.map((t => t.color)).flat().map((t => t / 255)),
                             ranges: this.props.channels.map((t => [t.min, t.intensity])).flat()
                         }).draw()
                     }
                 }
             }
-            Kw.layerName = "ImageLayer", Kw.defaultProps = {
+            $w.layerName = "ImageLayer", $w.defaultProps = {
                 bounds: [],
                 pickable: !1,
                 coordinateSystem: Th.CARTESIAN,
                 data: null,
                 width: 0,
                 height: 0,
                 format: "uint8",
                 channels: [],
                 channelMapping: [],
                 activeChannels: 0
             };
-            var $w = Kw;
-            class Jw extends Uw {
+            var Jw = $w;
+            class Qw extends Uw {
                 constructor(t) {
                     super(t)
                 }
                 shouldUpdateState({
                     props: t,
                     oldProps: e,
                     context: n,
@@ -29635,15 +29636,15 @@
                         channelRanges: this.props.channelRanges,
                         channelMapping: this.props.channelMapping,
                         token: this.props.api,
                         basePath: this.props.basePath
                     };
                     return new Promise(((i, r) => {
                         if ("undefined" != typeof Worker) {
-                            const r = new Worker(new URL(n.p + n.u(241), n.b), {
+                            const r = new Worker(new URL(n.p + n.u(79), n.b), {
                                 type: void 0
                             });
                             r.onmessage = function(t) {
                                 r.terminate(), i({
                                     data: t.data.data,
                                     width: t.data.width,
                                     height: t.data.height,
@@ -29658,51 +29659,51 @@
                 renderSubLayers(t) {
                     const {
                         left: e,
                         bottom: n,
                         right: i,
                         top: r
                     } = t.tile.bbox;
-                    return new $w({
+                    return new Jw({
                         id: t.id,
                         data: t.data?.data,
                         width: t.data?.width,
                         height: t.data?.height,
                         format: this.props.attribute.type.toLowerCase(),
                         channels: this.props.channels,
                         activeChannels: t.data.channels,
                         channelMapping: this.props.channelMapping,
                         bounds: [oc(e, 0, t.extent[2]), oc(n, 0, t.extent[3]), oc(i, 0, t.extent[2]), oc(r, 0, t.extent[3])]
                     })
                 }
             }
-            Jw.defaultProps = {
+            Qw.defaultProps = {
                 api: "",
                 namespace: "",
                 metadata: [],
                 channels: [],
                 channelRanges: [],
                 channelMapping: [],
                 visible: !0
             };
-            var Qw = Jw,
-                tE = t => {
+            var tE = Qw,
+                eE = t => {
                     const {
                         tooltipText: e,
                         children: n
                     } = t;
                     return (0, o.jsxs)("div", {
                         className: "BIV-Tooltip",
                         children: [n, (0, o.jsx)("div", {
                             className: "BIV-Tooltip__content",
                             children: e
                         })]
                     })
                 },
-                eE = t => {
+                nE = t => {
                     const {
                         setZoom: e,
                         zoom: n,
                         resetControls: i
                     } = t, r = (0, c.useCallback)((() => {
                         e(n + .1)
                     }), [e]), s = (0, c.useCallback)((() => {
@@ -29710,15 +29711,15 @@
                     }), [e]), a = (0, c.useMemo)((() => (t => {
                         if (void 0 === t) return "-";
                         const e = 100 * Math.pow(2, t);
                         return `${Math.floor(e)}%`
                     })(n)), [n]);
                     return (0, o.jsxs)("div", {
                         className: "BIV-ZoomControls",
-                        children: [(0, o.jsx)(tE, {
+                        children: [(0, o.jsx)(eE, {
                             tooltipText: "Zoom in +",
                             children: (0, o.jsx)("button", {
                                 className: "BIV-ZoomControls__button",
                                 onClick: r,
                                 children: (0, o.jsx)("svg", {
                                     width: "20",
                                     height: "20",
@@ -29728,15 +29729,15 @@
                                     children: (0, o.jsx)("path", {
                                         d: "M10.0261 18.3333C10.2671 18.3333 10.4851 18.2732 10.6803 18.1529C10.8754 18.0325 11.034 17.8776 11.156 17.6881C11.2749 17.4986 11.3344 17.2941 11.3344 17.0745V11.2949H17.0524C17.2811 11.2949 17.493 11.2362 17.6882 11.1189C17.8834 11.0016 18.0404 10.8452 18.1593 10.6497C18.2752 10.4542 18.3332 10.2376 18.3332 9.99999C18.3332 9.76538 18.2737 9.55182 18.1548 9.35931C18.0358 9.1638 17.8773 9.00589 17.679 8.88557C17.4808 8.76526 17.2673 8.7051 17.0386 8.7051H11.3161V2.93448C11.3161 2.70588 11.2551 2.49683 11.1331 2.30734C11.0112 2.11483 10.851 1.95992 10.6528 1.84262C10.4546 1.72531 10.235 1.66666 9.99412 1.66666C9.76235 1.66666 9.54736 1.72381 9.34914 1.83811C9.14786 1.95241 8.98776 2.10581 8.86883 2.29831C8.7499 2.48781 8.69043 2.69535 8.69043 2.92095V8.68705H2.95876C2.73309 8.68705 2.52343 8.74571 2.32979 8.86301C2.13156 8.98032 1.97146 9.13673 1.84948 9.33224C1.7275 9.52475 1.6665 9.7368 1.6665 9.96841C1.6665 10.206 1.72597 10.4211 1.8449 10.6136C1.96384 10.8061 2.12241 10.961 2.32064 11.0783C2.51581 11.1926 2.72547 11.2498 2.94961 11.2498H8.67671V17.0249C8.67671 17.2445 8.73465 17.4475 8.85053 17.634C8.96641 17.8205 9.12499 17.9739 9.32626 18.0942C9.52449 18.2115 9.73796 18.2702 9.96667 18.2702L10.0261 18.3333Z",
                                         fill: "black",
                                         fillOpacity: "0.7"
                                     })
                                 })
                             })
-                        }), (0, o.jsx)(tE, {
+                        }), (0, o.jsx)(eE, {
                             tooltipText: "Zoom out -",
                             children: (0, o.jsx)("button", {
                                 className: "BIV-ZoomControls__button",
                                 onClick: s,
                                 children: (0, o.jsxs)("svg", {
                                     width: "20",
                                     height: "20",
@@ -29762,15 +29763,15 @@
                                         })
                                     })]
                                 })
                             })
                         }), (0, o.jsx)("p", {
                             className: "BIV-ZoomControls__label",
                             children: a
-                        }), (0, o.jsx)(tE, {
+                        }), (0, o.jsx)(eE, {
                             tooltipText: "Reset zoom level",
                             children: (0, o.jsx)("button", {
                                 className: "BIV-ZoomControls__button",
                                 onClick: i,
                                 children: (0, o.jsx)("svg", {
                                     width: "20",
                                     height: "20",
@@ -29783,55 +29784,129 @@
                                         fillOpacity: "0.7"
                                     })
                                 })
                             })
                         })]
                     })
                 },
-                nE = (t, e, n = !1) => {
+                iE = (t, e, n = !1) => {
                     let i;
                     return (...r) => {
                         const s = n && !i;
                         clearTimeout(i), i = setTimeout((function() {
                             i = null, n || t(...r)
                         }), e), s && t(...r)
                     }
                 };
-            const iE = new Map([
+            const rE = new Map([
                     ["m", 0],
                     ["dm", -1],
                     ["cm", -2],
                     ["mm", -3],
                     ["μm", -6],
                     ["nm", -9],
                     ["pm", -12]
                 ]),
-                rE = ["m", "mm", "μm", "nm", "pm"];
+                sE = ["m", "mm", "μm", "nm", "pm"];
 
-            function sE(t, e = "μm") {
+            function oE(t, e = "μm") {
                 if (t < 1) {
-                    let n = rE.indexOf(e) + 1;
-                    for (; n < rE.length && t < 1;) {
-                        const i = rE[n];
-                        t *= Math.pow(10, iE.get(e) - iE.get(i)), e = i, ++n
+                    let n = sE.indexOf(e) + 1;
+                    for (; n < sE.length && t < 1;) {
+                        const i = sE[n];
+                        t *= Math.pow(10, rE.get(e) - rE.get(i)), e = i, ++n
                     }
                 } else {
-                    let n = rE.indexOf(e) - 1;
+                    let n = sE.indexOf(e) - 1;
                     for (; n > -1 && t > 1e3;) {
-                        const i = rE[n];
-                        t *= Math.pow(10, iE.get(e) - iE.get(i)), e = i, --n
+                        const i = sE[n];
+                        t *= Math.pow(10, rE.get(e) - rE.get(i)), e = i, --n
                     }
                 }
                 return [t, e]
             }
 
-            function oE(t, e) {
+            function aE(t, e) {
                 return `${t.toFixed(2)} ${e}`
             }
-            var aE = t => {
+            const lE = "TILEDB_BIOIMAGE_CACHE";
+            let cE = 1;
+            const hE = async t => {
+                let e = await (0, Ww.X3)(lE);
+                const n = [];
+                for (const i of t) e.objectStoreNames.contains(i + "_1") || n.push(i);
+                e.close(), 0 !== n.length && (cE = e.version + 1, e = await (0, Ww.X3)(lE, cE, {
+                    upgrade(t) {
+                        for (const e of n) {
+                            for (let n = 0; n < 1; ++n) t.objectStoreNames.contains(e + "_" + n) && t.deleteObjectStore(e + "_" + n);
+                            t.createObjectStore(e + "_1", {
+                                autoIncrement: !0
+                            }).createIndex("timestamp", "__timestamp")
+                        }
+                    }
+                }), e.close())
+            }, uE = t => {
+                const [e, n] = (0, c.useState)({
+                    tileCount: 0,
+                    size: 0
+                });
+                return (0, c.useEffect)((() => {
+                    const e = setInterval((() => {
+                        (async () => {
+                            const e = await (async t => {
+                                    const e = await (0, Ww.X3)(lE),
+                                        n = t.map((t => `${t}_1`)),
+                                        i = await Promise.all(Array.from(e.objectStoreNames).filter((t => n.includes(t))).map((t => e.count(t))));
+                                    return e.close(), i.reduce(((t, e) => t + e), 0)
+                                })(t.levels.map((e => `${e.id}_${t.tileSize}`))),
+                                i = e * Yw[t.attribute.type.toLowerCase()].bytes * t.tileSize ** 2 / 2 ** 30;
+                            n((t => ({
+                                ...t,
+                                tileCount: e,
+                                size: i
+                            })))
+                        })()
+                    }), 6e4);
+                    return () => clearInterval(e)
+                }), [t.levels, t.attribute]), (0, o.jsxs)("div", {
+                    className: "BIV-CacheControls",
+                    children: [(0, o.jsx)(eE, {
+                        tooltipText: "Clear cache",
+                        children: (0, o.jsx)("button", {
+                            className: "BIV-CacheControls__button",
+                            onClick: async () => {
+                                await (async t => {
+                                    const e = await (0, Ww.X3)(lE),
+                                        n = t.map((t => `${t}_1`));
+                                    await Promise.all(Array.from(e.objectStoreNames).filter((t => n.includes(t))).map((t => e.clear(t)))), e.close()
+                                })(t.levels.map((e => `${e.id}_${t.tileSize}`)))
+                            },
+                            children: (0, o.jsx)("svg", {
+                                width: "20",
+                                height: "20",
+                                viewBox: "0 0 16 16",
+                                fill: "none",
+                                xmlns: "http://www.w3.org/2000/svg",
+                                children: (0, o.jsx)("path", {
+                                    d: "M11 1.5v1h3.5a.5.5 0 0 1 0 1h-.538l-.853 10.66A2 2 0 0 1 11.115 16h-6.23a2 2 0 0 1-1.994-1.84L2.038 3.5H1.5a.5.5 0 0 1 0-1H5v-1A1.5 1.5 0 0 1 6.5 0h3A1.5 1.5 0 0 1 11 1.5Zm-5 0v1h4v-1a.5.5 0 0 0-.5-.5h-3a.5.5 0 0 0-.5.5ZM4.5 5.029l.5 8.5a.5.5 0 1 0 .998-.06l-.5-8.5a.5.5 0 1 0-.998.06Zm6.53-.528a.5.5 0 0 0-.528.47l-.5 8.5a.5.5 0 0 0 .998.058l.5-8.5a.5.5 0 0 0-.47-.528ZM8 4.5a.5.5 0 0 0-.5.5v8.5a.5.5 0 0 0 1 0V5a.5.5 0 0 0-.5-.5Z",
+                                    fill: "black",
+                                    fillOpacity: "0.7"
+                                })
+                            })
+                        })
+                    }), (0, o.jsxs)("p", {
+                        className: "BIV-CacheControls__label",
+                        children: ["Cached tiles: ", e.tileCount]
+                    }), (0, o.jsxs)("p", {
+                        className: "BIV-CacheControls__label",
+                        children: [e.size.toFixed(3), " GBs Approx."]
+                    })]
+                })
+            };
+            var dE = t => {
                 const {
                     groupNamespace: e,
                     groupID: n,
                     client: i,
                     onLoad: r
                 } = t, s = (0, c.useRef)(null), [a, l] = (0, c.useState)({
                     loaded: !1,
@@ -29923,15 +29998,15 @@
                                 dimensions: t.originalShape,
                                 axes: t.originalAxes,
                                 arrayExtends: t.storedShape,
                                 arrayAxes: t.storedAxes,
                                 axesMapping: t.axesMapping
                             }), ++h
                         }
-                        return i(a, o), l
+                        return i(a, o), await hE([`${l[0].id}_4096`]), await hE(l.map((t => `${t.id}_1024`)).filter(((t, e, n) => n.indexOf(t) === e))), l
                     })(i, e, n, t.onGroupLoaded).then((t => {
                         l((e => ({
                             ...e,
                             metadata: t,
                             target: [t[0].dimensions[t[0].axes.indexOf("X")] / 2, t[0].dimensions[t[0].axes.indexOf("Y")] / 2, 0],
                             loaded: !0
                         }))), r?.(), s.current = a
@@ -29954,30 +30029,30 @@
                     return {
                         imageWidth: n,
                         imageHeight: i,
                         minimapZoom: r,
                         minimapWidth: Math.pow(2, r) * n - 2,
                         minimapHeight: Math.pow(2, r) * i - 2
                     }
-                }), [a.metadata]), g = (0, c.useMemo)((() => new Og({
+                }), [a.metadata]), g = (0, c.useMemo)((() => new Lg({
                     id: "main",
                     controller: {
                         scrollZoom: {
                             speed: .01,
                             smooth: !0
                         },
                         inertia: !0,
                         doubleClickZoom: !1
                     }
-                })), [Og]), m = (0, c.useMemo)((() => nE((t => {
+                })), [Lg]), m = (0, c.useMemo)((() => iE((t => {
                     l((e => ({
                         ...e,
                         ...t.viewState
                     })))
-                }), 200)), [nE]);
+                }), 200)), [iE]);
                 (0, c.useEffect)((() => {
                     a.loaded && v(a.target, a.width, a.height, a.zoom)
                 }), [a.target, a.width, a.height, a.zoom]);
                 const v = (t, e, n, i) => {
                     const r = e / 2 * Math.pow(2, -i),
                         s = n / 2 * Math.pow(2, -i),
                         o = [
@@ -29991,58 +30066,65 @@
                         viewArea: {
                             shape: o
                         }
                     })))
                 };
                 return (0, o.jsxs)("div", {
                     className: "BioImageViewer__main",
-                    children: [(0, o.jsx)(eE, {
-                        resetControls: () => {
-                            s.current && l((t => ({
-                                ...t,
-                                zoom: s.current?.zoom
-                            })))
-                        },
-                        orthographicView: g,
-                        zoom: a.zoom,
-                        setZoom: t => {
-                            l((e => ({
-                                ...e,
-                                zoom: t
-                            })))
-                        }
+                    children: [(0, o.jsxs)("div", {
+                        className: "BioImageViewer-Viewer__controls",
+                        children: [(0, o.jsx)(uE, {
+                            levels: a.metadata,
+                            tileSize: 1024,
+                            attribute: t.attributes[0]
+                        }), (0, o.jsx)(nE, {
+                            resetControls: () => {
+                                s.current && l((t => ({
+                                    ...t,
+                                    zoom: s.current?.zoom
+                                })))
+                            },
+                            orthographicView: g,
+                            zoom: a.zoom,
+                            setZoom: t => {
+                                l((e => ({
+                                    ...e,
+                                    zoom: t
+                                })))
+                            }
+                        })]
                     }), a.loaded && (0, o.jsxs)(iy, {
-                        views: [g, new Og({
+                        views: [g, new Lg({
                             id: "mini-map",
                             x: "60px",
                             y: "30px",
                             height: `${f}px`,
                             width: `${p}px`,
                             controller: !1,
                             viewState: {
                                 target: [h / 2, u / 2, 0],
                                 zoom: d
                             }
                         })],
-                        layers: [new Qw({
+                        layers: [new tE({
                             id: "tiles-for-main",
                             tileSize: 1024,
                             minZoom: a.metadata[0].zoomLevel,
                             maxZoom: a.metadata.at(-1)?.zoomLevel,
                             coordinateSystem: Th.CARTESIAN,
                             extent: [0, 0, h, u],
                             metadata: a.metadata,
                             namespace: t.groupNamespace,
                             attribute: t.attributes.filter((t => !0 === t.visible))[0],
                             channels: t.channels,
                             channelRanges: t.channelRanges,
                             channelMapping: t.channelMapping,
                             api: t.client.config.apiKey,
                             basePath: t.basePath
-                        }), new Qw({
+                        }), new tE({
                             id: "tiles-for-mini-map",
                             tileSize: 4096,
                             minZoom: a.metadata[0].zoomLevel,
                             maxZoom: a.metadata[0].zoomLevel,
                             coordinateSystem: Th.CARTESIAN,
                             extent: [0, 0, h, u],
                             metadata: a.metadata,
@@ -30075,44 +30157,44 @@
                         onViewStateChange: m,
                         initialViewState: {
                             target: a.target,
                             zoom: a.zoom,
                             minZoom: -2,
                             maxZoom: a.metadata.at(-1)?.zoomLevel ?? 0
                         },
-                        children: [(0, o.jsx)(Og, {
+                        children: [(0, o.jsx)(Lg, {
                             id: "main"
-                        }), (0, o.jsx)(Og, {
+                        }), (0, o.jsx)(Lg, {
                             id: "mini-map",
                             children: (0, o.jsx)("div", {
                                 className: "BioImageViewer-Viewer__minimap",
                                 style: {
                                     width: a.minimapVisible ? "100%" : 0
                                 },
                                 children: (0, o.jsx)("div", {
                                     className: "BioImageViewer-Viewer__minimap__controls",
                                     onClick: () => l({
                                         ...a,
                                         minimapVisible: !a.minimapVisible
                                     }),
-                                    children: a.minimapVisible ? (0, o.jsx)(tE, {
+                                    children: a.minimapVisible ? (0, o.jsx)(eE, {
                                         tooltipText: "Hide minimap",
                                         children: (0, o.jsx)("svg", {
                                             className: "BioImageViewer-Slider__icon",
                                             width: "48",
                                             height: "48",
                                             viewBox: "0 0 48 48",
                                             fill: "none",
                                             xmlns: "http://www.w3.org/2000/svg",
                                             children: (0, o.jsx)("path", {
                                                 d: "M24 8C29.908 8 35.054 11.054 39 15C41.922 17.922 44 22.044 44 24C44 25.956 41.922 30.078 39 33C35.054 36.946 29.908 40 24 40C18.092 40 12.946 36.946 9 33C5.054 29.054 4 25.956 4 24C4 22.044 6.078 17.922 9 15C12.946 11.054 18.092 8 24 8ZM24 14C21.3478 14 18.8043 15.0536 16.9289 16.9289C15.0536 18.8043 14 21.3478 14 24C14 26.6522 15.0536 29.1957 16.9289 31.0711C18.8043 32.9464 21.3478 34 24 34C26.6522 34 29.1957 32.9464 31.0711 31.0711C32.9464 29.1957 34 26.6522 34 24C34 21.3478 32.9464 18.8043 31.0711 16.9289C29.1957 15.0536 26.6522 14 24 14ZM24 18.5C25.4587 18.5 26.8576 19.0795 27.8891 20.1109C28.9205 21.1424 29.5 22.5413 29.5 24C29.5 25.4587 28.9205 26.8576 27.8891 27.8891C26.8576 28.9205 25.4587 29.5 24 29.5C22.5413 29.5 21.1424 28.9205 20.1109 27.8891C19.0795 26.8576 18.5 25.4587 18.5 24C18.5 22.5413 19.0795 21.1424 20.1109 20.1109C21.1424 19.0795 22.5413 18.5 24 18.5Z",
                                                 fill: "#0000007d"
                                             })
                                         })
-                                    }) : (0, o.jsx)(tE, {
+                                    }) : (0, o.jsx)(eE, {
                                         tooltipText: "Show minimap",
                                         children: (0, o.jsx)("svg", {
                                             className: "BioImageViewer-Slider__icon",
                                             width: "48",
                                             height: "48",
                                             viewBox: "0 0 48 48",
                                             fill: "none",
@@ -30129,20 +30211,20 @@
                     }), (0, o.jsx)("div", {
                         style: {
                             "--scalebar-length": t.scalebarLength
                         },
                         className: "BioImageViewer__scalebar",
                         children: (0, o.jsx)("p", {
                             className: "BioImageViewer__scalebar__text",
-                            children: oE(...sE(t.basePhysicalSize * Math.pow(2, 5 - a.zoom) * t.scalebarLength, t.basePhysicalSizeUnit))
+                            children: aE(...oE(t.basePhysicalSize * Math.pow(2, 5 - a.zoom) * t.scalebarLength, t.basePhysicalSizeUnit))
                         })
                     })]
                 })
             };
-            const lE = t => {
+            const pE = t => {
                     const {
                         groupNamespace: e,
                         baseGroup: n,
                         client: i
                     } = t, [r, s] = (0, c.useState)({
                         groups: [],
                         filteredGroups: [],
@@ -30225,19 +30307,19 @@
                                 onClick: () => l(),
                                 children: "Next"
                             })]
                         })]
                     });
                     var u, d, p
                 },
-                cE = "https://api.tiledb.com";
-            var hE = t => {
+                fE = "https://api.tiledb.com";
+            var gE = t => {
                 const {
                     apiKey: e,
-                    basePath: n = cE,
+                    basePath: n = fE,
                     baseGroup: i,
                     namespace: r,
                     onLoad: s,
                     onError: a
                 } = t, [l, h] = (0, c.useState)({
                     channels: new Map,
                     attributes: [],
@@ -30250,26 +30332,26 @@
                     apiKey: e,
                     basePath: n
                 }, p = new(d())(u);
                 return (0, o.jsxs)("div", {
                     className: "BioImageViewer__container",
                     children: [(0, o.jsxs)("div", {
                         className: "BioImageViewer__controls",
-                        children: [i && (0, o.jsx)(lE, {
+                        children: [i && (0, o.jsx)(pE, {
                             client: p,
                             groupNamespace: r,
                             baseGroup: i,
                             itemsPerPage: 2,
                             onGroupSelect: t => {
                                 h((e => ({
                                     ...e,
                                     groupID: t
                                 })))
                             }
-                        }), (0, o.jsx)(Hw, {
+                        }), (0, o.jsx)(Zw, {
                             channels: l.channels.get(l.attributes.filter((t => t.visible))[0]?.name) ?? [],
                             onChannelUpdate: (t, e, n, i) => {
                                 let r = !1;
                                 const s = l.attributes.filter((t => !0 === t.visible))[0].name,
                                     o = new Map(l.channels);
                                 if (o.get(s)?.map((s => s.id === i ? (s.visible !== n && (r = !0), s.intensity = t, s.color = e, s.visible = n, s) : s)), r) {
                                     const t = [],
@@ -30284,25 +30366,25 @@
                                     })))
                                 }
                                 h((t => ({
                                     ...t,
                                     channels: o
                                 })))
                             }
-                        }), l.attributes.length > 1 && (0, o.jsx)(Zw, {
+                        }), l.attributes.length > 1 && (0, o.jsx)(Xw, {
                             attributes: l.attributes,
                             onAttributeUpdate: t => {
                                 const e = l.attributes.map((e => (e.name === t ? e.visible = !0 : e.visible = !1, e)));
                                 h((t => ({
                                     ...t,
                                     attributes: e
                                 })))
                             }
                         })]
-                    }), (0, o.jsx)(aE, {
+                    }), (0, o.jsx)(dE, {
                         onLoad: s,
                         client: p,
                         groupNamespace: r,
                         groupID: l.groupID,
                         basePath: n,
                         attributes: l.attributes,
                         channels: l.channels.get(l.attributes.filter((t => t.visible))[0]?.name) ?? [],
@@ -30329,15 +30411,15 @@
                                 var r
                             }))
                         },
                         errorHandler: a
                     })]
                 })
             };
-            class uE extends h().Component {
+            class mE extends h().Component {
                 constructor(t) {
                     super(t), this.state = {
                         error: void 0
                     }
                 }
                 static getDerivedStateFromError(t) {
                     return {
@@ -30347,31 +30429,31 @@
                 componentDidCatch(t, e) {
                     this.props.errorHandler?.(t)
                 }
                 render() {
                     return this.state.error && this.props.errorState ? this.props.errorState(this.state.error) : this.props.children
                 }
             }
-            var dE = uE,
-                pE = t => {
+            var vE = mE,
+                bE = t => {
                     let e;
-                    e = "string" == typeof t.rootElement ? document.getElementById(t.rootElement) : t.rootElement, l.version.startsWith("18.") ? a.createRoot(e).render((0, o.jsx)(dE, {
+                    e = "string" == typeof t.rootElement ? document.getElementById(t.rootElement) : t.rootElement, l.version.startsWith("18.") ? a.createRoot(e).render((0, o.jsx)(vE, {
                         errorHandler: t.onError,
-                        children: (0, o.jsx)(hE, {
+                        children: (0, o.jsx)(gE, {
                             apiKey: t.apiKey,
                             groupID: t.groupID,
                             baseGroup: t.baseGroup,
                             namespace: t.namespace,
                             onError: t.onError,
                             basePath: t.basePath,
                             onLoad: t.onLoad
                         })
-                    })) : (0, l.render)((0, o.jsx)(dE, {
+                    })) : (0, l.render)((0, o.jsx)(vE, {
                         errorHandler: t.onError,
-                        children: (0, o.jsx)(hE, {
+                        children: (0, o.jsx)(gE, {
                             apiKey: t.apiKey,
                             groupID: t.groupID,
                             baseGroup: t.baseGroup,
                             namespace: t.namespace,
                             onError: t.onError,
                             basePath: t.basePath,
                             onLoad: t.onLoad
@@ -30506,15 +30588,15 @@
                 o = n.n(s),
                 a = n(6362),
                 l = n.n(a),
                 c = r()((function(t) {
                     return t[1]
                 })),
                 h = o()(l());
-            c.push([t.id, '.BioImageViewer-Slider {\n  width: 320px;\n  background: #f8fafb;\n  border-radius: 12px;\n  padding: 12px 12px 20px;\n  font-family: Inter, Arial, "sans-serif";\n}\n\n.BioImageViewer-Slider__text {\n  color: #000;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 14px;\n  font-weight: 600;\n  line-height: 20px;\n}\n\n.BioImageViewer-Slider__text--light {\n  color: #000000b3;\n}\n\n.BioImageViewer-Slider__icon {\n  width: 16px;\n}\n\n.BioImageViewer-Slider__colorpicker {\n  width: 16px;\n  height: 16px;\n  border: 2px solid #fff;\n  border-radius: 50%;\n  margin-right: 12px;\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-Slider__colorpicker-backdrop {\n  position: fixed;\n  inset: 0;\n}\n\n.BioImageViewer-Slider__colorpicker-container {\n  z-index: 2;\n  position: absolute;\n}\n\n.BioImageViewer-Slider__main {\n  justify-content: space-between;\n  display: flex;\n}\n\n.BioImageViewer-Slider__left, .BioImageViewer-Slider__info {\n  align-items: center;\n  display: flex;\n}\n\n.BioImageViewer-Slider__icon-wrapper {\n  margin-left: 6px;\n  margin-right: 14px;\n}\n\n.BioImageViewer-Slider__value {\n  color: #000000de;\n  background: #fff;\n  border: 1px solid #cfd6de;\n  border-radius: 6px;\n  padding: 6px 16px;\n  font-size: 14px;\n  font-style: normal;\n  font-weight: 400;\n  line-height: 20px;\n}\n\n.BioImageViewer-Slider__range {\n  width: 100%;\n}\n\n.BioImageViewer-ControlPanel {\n  background: #fff;\n  border-radius: 12px;\n  margin-bottom: 16px;\n  padding: 20px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-ControlPanel__title {\n  justify-content: space-between;\n  align-items: center;\n  margin: 0;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-ControlPanel__title svg {\n  margin-right: 10px;\n}\n\n.BioImageViewer-ControlPanel__title div {\n  align-items: center;\n  display: flex;\n}\n\n.BioImageViewer-ControlPanel__toggle {\n  cursor: pointer;\n}\n\n.BioImageViewer-ControlPanel__toggle svg {\n  margin: 0;\n}\n\n.BioImageViewer-ControlPanel__list {\n  margin: 0;\n  padding-left: 0;\n  list-style: none;\n  transition: max-height .8s;\n  overflow: hidden;\n}\n\n.BioImageViewer-ControlPanel__item {\n  margin-bottom: 8px;\n}\n\n.BioImageViewer-ControlPanel__item:first-child {\n  margin-top: 26px;\n}\n\n.BioImageViewer-ControlPanel__item:last-child {\n  margin-bottom: 0;\n}\n\n.BioImageViewer-AttributePanel {\n  background: #fff;\n  border-radius: 12px;\n  margin-bottom: 16px;\n  padding: 26px 16px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-AttributePanel__title {\n  align-items: center;\n  margin: 0 0 16px;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-AttributePanel__item {\n  flex-direction: row;\n  align-items: center;\n  display: flex;\n}\n\n.BioImageViewer-AttributePanel__radio {\n  margin: 0;\n}\n\n.BioImageViewer-AttributePanel__label {\n  margin: 6px;\n}\n\n.BIV-ZoomControls {\n  z-index: 1;\n  background-color: #fff;\n  border-radius: 8px;\n  align-items: center;\n  gap: 8px;\n  padding: 4px;\n  display: flex;\n  position: absolute;\n  top: 16px;\n  right: 16px;\n  box-shadow: 0 1px 3px #d1d5d7;\n}\n\n.BIV-ZoomControls__label {\n  color: #000000b3;\n  width: 56px;\n  text-align: center;\n  margin: 0;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 12px;\n  font-weight: 600;\n  line-height: 20px;\n}\n\n.BIV-ZoomControls__button {\n  width: 28px;\n  height: 28px;\n  background: no-repeat;\n  border: none;\n  padding: 0;\n}\n\n.BIV-ZoomControls__button:hover {\n  cursor: pointer;\n}\n\n.BIV-Tooltip {\n  position: relative;\n}\n\n.BIV-Tooltip:hover .BIV-Tooltip__content {\n  opacity: 1;\n}\n\n.BIV-Tooltip__content {\n  color: #fff;\n  opacity: 0;\n  white-space: nowrap;\n  background-color: #333f55;\n  border-radius: 4px;\n  padding: 8px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 12px;\n  font-weight: 600;\n  line-height: 20px;\n  transition: opacity .2s ease-in-out;\n  position: absolute;\n  bottom: -54px;\n  left: 50%;\n  transform: translateX(-50%);\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BIV-Tooltip__content:before {\n  content: "";\n  width: 0;\n  height: 0;\n  border: 10px solid #0000;\n  border-top: 0;\n  border-bottom-color: #333f55;\n  position: absolute;\n  top: -10px;\n  left: 50%;\n  transform: translateX(-50%);\n}\n\n.BioImageViewer-Viewer__minimap {\n  width: 100%;\n  height: 100%;\n  position: absolute;\n  box-shadow: 0 2px 10px #00000029;\n}\n\n.BioImageViewer-Viewer__minimap__controls {\n  width: 24px;\n  height: 100%;\n  background-color: #fff;\n  border-top-left-radius: 6px;\n  border-bottom-left-radius: 6px;\n  margin-left: -24px;\n  box-shadow: 0 2px 10px #00000029;\n}\n\n.BioImageViewer-Viewer__minimap__controls svg {\n  width: 16px;\n  height: 16px;\n  cursor: pointer;\n  margin: 6px 2px 4px 4px;\n}\n\n.BioImageViewer__container {\n  width: 100%;\n  height: 100%;\n  position: relative;\n}\n\n.BioImageViewer__container #deckgl-wrapper {\n  background-image: url(' + h + ');\n  background-size: 50px;\n}\n\n.BioImageViewer__controls {\n  z-index: 1;\n  max-height: 80vh;\n  overflow-y: overlay;\n  padding: 6px;\n  position: absolute;\n  top: 68px;\n  right: 16px;\n}\n\n.BioImageViewer__minimap {\n  width: 160px;\n  height: 90px;\n  border: 1px solid gray;\n  position: absolute;\n  top: 20px;\n  left: 20px;\n}\n\n.BioImageViewer__scalebar {\n  width: calc(var(--scalebar-length) * 1px);\n  height: 10px;\n  box-sizing: border-box;\n  background: linear-gradient(to right, #fff 50%, #000 50%);\n  border: 1px solid #000;\n  position: absolute;\n  bottom: 60px;\n  left: 20px;\n}\n\n.BioImageViewer__scalebar__text {\n  width: calc(var(--scalebar-length) * 1px);\n  height: 15px;\n  box-sizing: border-box;\n  text-align: center;\n  color: #fff;\n  text-shadow: 0 1px 3px #000000f5;\n  margin: 0;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 14px;\n  font-weight: 500;\n  position: absolute;\n  top: 10px;\n  left: -1px;\n}\n\n.BioImageViewer-GroupSelector {\n  background: #fff;\n  border-radius: 12px;\n  flex-direction: column;\n  margin-bottom: 16px;\n  padding: 26px 16px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  display: flex;\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-GroupSelector__title {\n  align-items: center;\n  margin: 0 0 26px;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-GroupSelector__title svg {\n  margin-right: 10px;\n}\n\n.BioImageViewer-GroupSelector__controls {\n  justify-content: space-between;\n  align-items: center;\n  margin: 6px;\n  display: flex;\n}\n\n.BioImageViewer-GroupSelector__list {\n  padding-left: 0;\n  list-style: none;\n}\n\n.BioImageViewer-GroupSelector__value {\n  color: #000000de;\n  background: #fff;\n  border: 1px solid #cfd6de;\n  border-radius: 6px;\n  padding: 6px 16px;\n  font-size: 14px;\n  font-style: normal;\n  font-weight: 400;\n  line-height: 20px;\n}\n\n.BioImageViewer-GroupSelector__item {\n  cursor: pointer;\n  background-color: #aeaeae;\n  border-radius: 12px;\n  margin-bottom: 12px;\n  padding: 8px;\n  font-size: 14px;\n}\n\n.BioImageViewer-GroupSelector__item:hover {\n  background-color: #0000ff26;\n}\n\n.BioImageViewer-GroupSelector__item p {\n  margin: 0;\n}\n\n.BioImageViewer-GroupSelector__item em {\n  font-size: 12px;\n}\n', ""]);
+            c.push([t.id, '.BioImageViewer-Slider {\n  width: 320px;\n  background: #f8fafb;\n  border-radius: 12px;\n  padding: 12px 12px 20px;\n  font-family: Inter, Arial, "sans-serif";\n}\n\n.BioImageViewer-Slider__text {\n  color: #000;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 14px;\n  font-weight: 600;\n  line-height: 20px;\n}\n\n.BioImageViewer-Slider__text--light {\n  color: #000000b3;\n}\n\n.BioImageViewer-Slider__icon {\n  width: 16px;\n}\n\n.BioImageViewer-Slider__colorpicker {\n  width: 16px;\n  height: 16px;\n  border: 2px solid #fff;\n  border-radius: 50%;\n  margin-right: 12px;\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-Slider__colorpicker-backdrop {\n  position: fixed;\n  inset: 0;\n}\n\n.BioImageViewer-Slider__colorpicker-container {\n  z-index: 2;\n  position: absolute;\n}\n\n.BioImageViewer-Slider__main {\n  justify-content: space-between;\n  display: flex;\n}\n\n.BioImageViewer-Slider__left, .BioImageViewer-Slider__info {\n  align-items: center;\n  display: flex;\n}\n\n.BioImageViewer-Slider__icon-wrapper {\n  margin-left: 6px;\n  margin-right: 14px;\n}\n\n.BioImageViewer-Slider__value {\n  color: #000000de;\n  background: #fff;\n  border: 1px solid #cfd6de;\n  border-radius: 6px;\n  padding: 6px 16px;\n  font-size: 14px;\n  font-style: normal;\n  font-weight: 400;\n  line-height: 20px;\n}\n\n.BioImageViewer-Slider__range {\n  width: 100%;\n}\n\n.BioImageViewer-ControlPanel {\n  background: #fff;\n  border-radius: 12px;\n  margin-bottom: 16px;\n  padding: 20px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-ControlPanel__title {\n  justify-content: space-between;\n  align-items: center;\n  margin: 0;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-ControlPanel__title svg {\n  margin-right: 10px;\n}\n\n.BioImageViewer-ControlPanel__title div {\n  align-items: center;\n  display: flex;\n}\n\n.BioImageViewer-ControlPanel__toggle {\n  cursor: pointer;\n}\n\n.BioImageViewer-ControlPanel__toggle svg {\n  margin: 0;\n}\n\n.BioImageViewer-ControlPanel__list {\n  margin: 0;\n  padding-left: 0;\n  list-style: none;\n  transition: max-height .8s;\n  overflow: hidden;\n}\n\n.BioImageViewer-ControlPanel__item {\n  margin-bottom: 8px;\n}\n\n.BioImageViewer-ControlPanel__item:first-child {\n  margin-top: 26px;\n}\n\n.BioImageViewer-ControlPanel__item:last-child {\n  margin-bottom: 0;\n}\n\n.BioImageViewer-AttributePanel {\n  background: #fff;\n  border-radius: 12px;\n  margin-bottom: 16px;\n  padding: 26px 16px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-AttributePanel__title {\n  align-items: center;\n  margin: 0 0 16px;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-AttributePanel__item {\n  flex-direction: row;\n  align-items: center;\n  display: flex;\n}\n\n.BioImageViewer-AttributePanel__radio {\n  margin: 0;\n}\n\n.BioImageViewer-AttributePanel__label {\n  margin: 6px;\n}\n\n.BIV-ZoomControls {\n  background-color: #fff;\n  border-radius: 8px;\n  align-items: center;\n  gap: 8px;\n  padding: 4px;\n  display: flex;\n  box-shadow: 0 1px 3px #d1d5d7;\n}\n\n.BIV-ZoomControls__label {\n  color: #000000b3;\n  width: 56px;\n  text-align: center;\n  margin: 0;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 12px;\n  font-weight: 600;\n  line-height: 20px;\n}\n\n.BIV-ZoomControls__button {\n  width: 28px;\n  height: 28px;\n  background: no-repeat;\n  border: none;\n  padding: 0;\n}\n\n.BIV-ZoomControls__button:hover {\n  cursor: pointer;\n}\n\n.BIV-Tooltip {\n  position: relative;\n}\n\n.BIV-Tooltip:hover .BIV-Tooltip__content {\n  opacity: 1;\n}\n\n.BIV-Tooltip__content {\n  color: #fff;\n  opacity: 0;\n  white-space: nowrap;\n  pointer-events: none;\n  background-color: #333f55;\n  border-radius: 4px;\n  padding: 8px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 12px;\n  font-weight: 600;\n  line-height: 20px;\n  transition: opacity .2s ease-in-out;\n  position: absolute;\n  bottom: -50px;\n  left: 50%;\n  transform: translateX(-50%);\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BIV-Tooltip__content:before {\n  content: "";\n  width: 0;\n  height: 0;\n  border: 10px solid #0000;\n  border-top: 0;\n  border-bottom-color: #333f55;\n  position: absolute;\n  top: -10px;\n  left: 50%;\n  transform: translateX(-50%);\n}\n\n.BioImageViewer-Viewer__controls {\n  z-index: 1;\n  flex-direction: row;\n  justify-content: flex-end;\n  gap: 12px;\n  display: flex;\n  position: absolute;\n  top: 16px;\n  right: 16px;\n}\n\n.BioImageViewer-Viewer__minimap {\n  width: 100%;\n  height: 100%;\n  position: absolute;\n  box-shadow: 0 2px 10px #00000029;\n}\n\n.BioImageViewer-Viewer__minimap__controls {\n  width: 24px;\n  height: 100%;\n  background-color: #fff;\n  border-top-left-radius: 6px;\n  border-bottom-left-radius: 6px;\n  margin-left: -24px;\n  box-shadow: 0 2px 10px #00000029;\n}\n\n.BioImageViewer-Viewer__minimap__controls svg {\n  width: 16px;\n  height: 16px;\n  cursor: pointer;\n  margin: 6px 2px 4px 4px;\n}\n\n.BIV-CacheControls {\n  z-index: 1;\n  background-color: #fff;\n  border-radius: 8px;\n  align-items: center;\n  gap: 8px;\n  padding: 4px;\n  display: flex;\n  box-shadow: 0 1px 3px #d1d5d7;\n}\n\n.BIV-CacheControls__label {\n  color: #000000b3;\n  width: 90px;\n  text-align: center;\n  margin: 0;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 12px;\n  font-weight: 600;\n  line-height: 20px;\n}\n\n.BIV-CacheControls__button {\n  width: 28px;\n  height: 28px;\n  background: no-repeat;\n  border: none;\n  padding: 0;\n}\n\n.BIV-CacheControls__button:hover {\n  cursor: pointer;\n}\n\n.BioImageViewer__container {\n  width: 100%;\n  height: 100%;\n  position: relative;\n}\n\n.BioImageViewer__container #deckgl-wrapper {\n  background-image: url(' + h + ');\n  background-size: 50px;\n}\n\n.BioImageViewer__controls {\n  z-index: 1;\n  max-height: 80vh;\n  overflow-y: overlay;\n  padding: 6px 0 6px 6px;\n  position: absolute;\n  top: 70px;\n  right: 16px;\n}\n\n.BioImageViewer__minimap {\n  width: 160px;\n  height: 90px;\n  border: 1px solid gray;\n  position: absolute;\n  top: 20px;\n  left: 20px;\n}\n\n.BioImageViewer__scalebar {\n  width: calc(var(--scalebar-length) * 1px);\n  height: 10px;\n  box-sizing: border-box;\n  background: linear-gradient(to right, #fff 50%, #000 50%);\n  border: 1px solid #000;\n  position: absolute;\n  bottom: 60px;\n  left: 20px;\n}\n\n.BioImageViewer__scalebar__text {\n  width: calc(var(--scalebar-length) * 1px);\n  height: 15px;\n  box-sizing: border-box;\n  text-align: center;\n  color: #fff;\n  text-shadow: 0 1px 3px #000000f5;\n  margin: 0;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 14px;\n  font-weight: 500;\n  position: absolute;\n  top: 10px;\n  left: -1px;\n}\n\n.BioImageViewer-GroupSelector {\n  background: #fff;\n  border-radius: 12px;\n  flex-direction: column;\n  margin-bottom: 16px;\n  padding: 26px 16px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  display: flex;\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-GroupSelector__title {\n  align-items: center;\n  margin: 0 0 26px;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-GroupSelector__title svg {\n  margin-right: 10px;\n}\n\n.BioImageViewer-GroupSelector__controls {\n  justify-content: space-between;\n  align-items: center;\n  margin: 6px;\n  display: flex;\n}\n\n.BioImageViewer-GroupSelector__list {\n  padding-left: 0;\n  list-style: none;\n}\n\n.BioImageViewer-GroupSelector__value {\n  color: #000000de;\n  background: #fff;\n  border: 1px solid #cfd6de;\n  border-radius: 6px;\n  padding: 6px 16px;\n  font-size: 14px;\n  font-style: normal;\n  font-weight: 400;\n  line-height: 20px;\n}\n\n.BioImageViewer-GroupSelector__item {\n  cursor: pointer;\n  background-color: #aeaeae;\n  border-radius: 12px;\n  margin-bottom: 12px;\n  padding: 8px;\n  font-size: 14px;\n}\n\n.BioImageViewer-GroupSelector__item:hover {\n  background-color: #0000ff26;\n}\n\n.BioImageViewer-GroupSelector__item p {\n  margin: 0;\n}\n\n.BioImageViewer-GroupSelector__item em {\n  font-size: 12px;\n}\n', ""]);
             const u = c
         },
         3645: t => {
             "use strict";
             t.exports = function(t) {
                 var e = [];
                 return e.toString = function() {
@@ -30570,25 +30652,25 @@
 
             function n(t, e, n, i, r) {
                 var s, o;
                 if (r === C(t, e, n, i) > 0)
                     for (s = e; s < n; s += i) o = E(s, t[s], t[s + 1], o);
                 else
                     for (s = n - i; s >= e; s -= i) o = E(s, t[s], t[s + 1], o);
-                return o && v(o, o.next) && (P(o), o = o.next), o
+                return o && v(o, o.next) && (S(o), o = o.next), o
             }
 
             function i(t, e) {
                 if (!t) return t;
                 e || (e = t);
                 var n, i = t;
                 do {
                     if (n = !1, i.steiner || !v(i, i.next) && 0 !== m(i.prev, i, i.next)) i = i.next;
                     else {
-                        if (P(i), (i = e = i.prev) === i.next) break;
+                        if (S(i), (i = e = i.prev) === i.next) break;
                         n = !0
                     }
                 } while (n || i !== e);
                 return e
             }
 
             function r(t, e, n, c, h, u, p) {
@@ -30608,15 +30690,15 @@
                                         n = i
                                     }
                                     s.nextZ = null, c *= 2
                                 } while (o > 1)
                             }(r)
                     }(t, c, h, u);
                     for (var f, g, m = t; t.prev !== t.next;)
-                        if (f = t.prev, g = t.next, u ? o(t, c, h, u) : s(t)) e.push(f.i / n | 0), e.push(t.i / n | 0), e.push(g.i / n | 0), P(t), t = g.next, m = g.next;
+                        if (f = t.prev, g = t.next, u ? o(t, c, h, u) : s(t)) e.push(f.i / n | 0), e.push(t.i / n | 0), e.push(g.i / n | 0), S(t), t = g.next, m = g.next;
                         else if ((t = g) === m) {
                         p ? 1 === p ? r(t = a(i(t), e, n), e, n, c, h, u, 2) : 2 === p && l(t, e, n, c, h, u) : r(i(t), e, n, c, h, u, 1);
                         break
                     }
                 }
             }
 
@@ -30654,15 +30736,15 @@
             }
 
             function a(t, e, n) {
                 var r = t;
                 do {
                     var s = r.prev,
                         o = r.next.next;
-                    !v(s, o) && b(s, r, r.next, o) && x(s, o) && x(o, s) && (e.push(s.i / n | 0), e.push(r.i / n | 0), e.push(o.i / n | 0), P(r), P(r.next), r = t = o), r = r.next
+                    !v(s, o) && b(s, r, r.next, o) && x(s, o) && x(o, s) && (e.push(s.i / n | 0), e.push(r.i / n | 0), e.push(o.i / n | 0), S(r), S(r.next), r = t = o), r = r.next
                 } while (r !== t);
                 return i(r)
             }
 
             function l(t, e, n, s, o, a) {
                 var l = t;
                 do {
@@ -30776,31 +30858,31 @@
             }
 
             function x(t, e) {
                 return m(t.prev, t, t.next) < 0 ? m(t, e, t.next) >= 0 && m(t, t.prev, e) >= 0 : m(t, e, t.prev) < 0 || m(t, t.next, e) < 0
             }
 
             function w(t, e) {
-                var n = new S(t.i, t.x, t.y),
-                    i = new S(e.i, e.x, e.y),
+                var n = new P(t.i, t.x, t.y),
+                    i = new P(e.i, e.x, e.y),
                     r = t.next,
                     s = e.prev;
                 return t.next = e, e.prev = t, n.next = r, r.prev = n, i.next = n, n.prev = i, s.next = i, i.prev = s, i
             }
 
             function E(t, e, n, i) {
-                var r = new S(t, e, n);
+                var r = new P(t, e, n);
                 return i ? (r.next = i.next, r.prev = i, i.next.prev = r, i.next = r) : (r.prev = r, r.next = r), r
             }
 
-            function P(t) {
+            function S(t) {
                 t.next.prev = t.prev, t.prev.next = t.next, t.prevZ && (t.prevZ.nextZ = t.nextZ), t.nextZ && (t.nextZ.prevZ = t.prevZ)
             }
 
-            function S(t, e, n) {
+            function P(t, e, n) {
                 this.i = t, this.x = e, this.y = n, this.prev = null, this.next = null, this.z = 0, this.prevZ = null, this.nextZ = null, this.steiner = !1
             }
 
             function C(t, e, n, i) {
                 for (var r = 0, s = e, o = n - i; s < n; s += i) r += (t[o] - t[s]) * (t[s + 1] + t[o + 1]), o = s;
                 return r
             }
@@ -30901,19 +30983,19 @@
                     }
                 }
 
                 function E(t, e) {
                     return typeof t == u ? t.apply(e && e[0] || a, e) : t
                 }
 
-                function P(t, e) {
+                function S(t, e) {
                     return t === a ? e : t
                 }
 
-                function S(t, e, n) {
+                function P(t, e, n) {
                     v(M(e), (function(e) {
                         t.addEventListener(e, n, !1)
                     }))
                 }
 
                 function C(t, e, n) {
                     v(M(e), (function(e) {
@@ -30933,66 +31015,66 @@
                     return t.indexOf(e) > -1
                 }
 
                 function M(t) {
                     return t.trim().split(/\s+/g)
                 }
 
-                function L(t, e, n) {
+                function O(t, e, n) {
                     if (t.indexOf && !n) return t.indexOf(e);
                     for (var i = 0; i < t.length;) {
                         if (n && t[i][n] == e || !n && t[i] === e) return i;
                         i++
                     }
                     return -1
                 }
 
-                function O(t) {
+                function L(t) {
                     return Array.prototype.slice.call(t, 0)
                 }
 
-                function R(t, e, n) {
+                function I(t, e, n) {
                     for (var i = [], r = [], s = 0; s < t.length;) {
                         var o = e ? t[s][e] : t[s];
-                        L(r, o) < 0 && i.push(t[s]), r[s] = o, s++
+                        O(r, o) < 0 && i.push(t[s]), r[s] = o, s++
                     }
                     return n && (i = e ? i.sort((function(t, n) {
                         return t[e] > n[e]
                     })) : i.sort()), i
                 }
 
                 function k(t, e) {
                     for (var n, i, r = e[0].toUpperCase() + e.slice(1), s = 0; s < c.length;) {
                         if ((i = (n = c[s]) ? n + r : e) in t) return i;
                         s++
                     }
                     return a
                 }
-                var I = 1;
+                var R = 1;
 
                 function j(t) {
                     var e = t.ownerDocument || t;
                     return e.defaultView || e.parentWindow || r
                 }
                 var z = "ontouchstart" in r,
                     F = k(r, "PointerEvent") !== a,
                     B = z && /mobile|tablet|ip(ad|hone|od)|android/i.test(navigator.userAgent),
-                    D = "touch",
-                    N = "mouse",
+                    N = "touch",
+                    D = "mouse",
                     V = 25,
                     U = 1,
                     G = 4,
                     W = 8,
                     H = 1,
                     Z = 2,
-                    q = 4,
-                    X = 8,
+                    X = 4,
+                    q = 8,
                     Y = 16,
-                    K = Z | q,
-                    $ = X | Y,
+                    K = Z | X,
+                    $ = q | Y,
                     J = K | $,
                     Q = ["x", "y"],
                     tt = ["clientX", "clientY"];
 
                 function et(t, e) {
                     var n = this;
                     this.manager = t, this.callback = e, this.element = t.element, this.target = t.options.inputTarget, this.domHandler = function(e) {
@@ -31080,15 +31162,15 @@
                     return {
                         x: e / t || 0,
                         y: n / t || 0
                     }
                 }
 
                 function ot(t, e) {
-                    return t === e ? H : p(t) >= p(e) ? t < 0 ? Z : q : e < 0 ? X : Y
+                    return t === e ? H : p(t) >= p(e) ? t < 0 ? Z : X : e < 0 ? q : Y
                 }
 
                 function at(t, e, n) {
                     n || (n = Q);
                     var i = e[n[0]] - t[n[0]],
                         r = e[n[1]] - t[n[1]];
                     return Math.sqrt(i * i + r * r)
@@ -31099,15 +31181,15 @@
                     var i = e[n[0]] - t[n[0]],
                         r = e[n[1]] - t[n[1]];
                     return 180 * Math.atan2(r, i) / Math.PI
                 }
                 et.prototype = {
                     handler: function() {},
                     init: function() {
-                        this.evEl && S(this.element, this.evEl, this.domHandler), this.evTarget && S(this.target, this.evTarget, this.domHandler), this.evWin && S(j(this.element), this.evWin, this.domHandler)
+                        this.evEl && P(this.element, this.evEl, this.domHandler), this.evTarget && P(this.target, this.evTarget, this.domHandler), this.evWin && P(j(this.element), this.evWin, this.domHandler)
                     },
                     destroy: function() {
                         this.evEl && C(this.element, this.evEl, this.domHandler), this.evTarget && C(this.target, this.evTarget, this.domHandler), this.evWin && C(j(this.element), this.evWin, this.domHandler)
                     }
                 };
                 var ct = {
                         mousedown: U,
@@ -31122,30 +31204,30 @@
                 }
                 x(dt, et, {
                     handler: function(t) {
                         var e = ct[t.type];
                         e & U && 0 === t.button && (this.pressed = !0), 2 & e && 1 !== t.which && (e = G), this.pressed && (e & G && (this.pressed = !1), this.callback(this.manager, e, {
                             pointers: [t],
                             changedPointers: [t],
-                            pointerType: N,
+                            pointerType: D,
                             srcEvent: t
                         }))
                     }
                 });
                 var pt = {
                         pointerdown: U,
                         pointermove: 2,
                         pointerup: G,
                         pointercancel: W,
                         pointerout: W
                     },
                     ft = {
-                        2: D,
+                        2: N,
                         3: "pen",
-                        4: N,
+                        4: D,
                         5: "kinect"
                     },
                     gt = "pointerdown",
                     mt = "pointermove pointerup pointercancel";
 
                 function vt() {
                     this.evEl = gt, this.evWin = mt, et.apply(this, arguments), this.store = this.manager.session.pointerEvents = []
@@ -31153,16 +31235,16 @@
                 r.MSPointerEvent && !r.PointerEvent && (gt = "MSPointerDown", mt = "MSPointerMove MSPointerUp MSPointerCancel"), x(vt, et, {
                     handler: function(t) {
                         var e = this.store,
                             n = !1,
                             i = t.type.toLowerCase().replace("ms", ""),
                             r = pt[i],
                             s = ft[t.pointerType] || t.pointerType,
-                            o = s == D,
-                            a = L(e, t.pointerId, "pointerId");
+                            o = s == N,
+                            a = O(e, t.pointerId, "pointerId");
                         r & U && (0 === t.button || o) ? a < 0 && (e.push(t), a = e.length - 1) : r & (G | W) && (n = !0), a < 0 || (e[a] = t, this.callback(this.manager, r, {
                             pointers: e,
                             changedPointers: [t],
                             pointerType: s,
                             srcEvent: t
                         }), n && e.splice(a, 1))
                     }
@@ -31175,27 +31257,27 @@
                 };
 
                 function yt() {
                     this.evTarget = "touchstart", this.evWin = "touchstart touchmove touchend touchcancel", this.started = !1, et.apply(this, arguments)
                 }
 
                 function _t(t, e) {
-                    var n = O(t.touches),
-                        i = O(t.changedTouches);
-                    return e & (G | W) && (n = R(n.concat(i), "identifier", !0)), [n, i]
+                    var n = L(t.touches),
+                        i = L(t.changedTouches);
+                    return e & (G | W) && (n = I(n.concat(i), "identifier", !0)), [n, i]
                 }
                 x(yt, et, {
                     handler: function(t) {
                         var e = bt[t.type];
                         if (e === U && (this.started = !0), this.started) {
                             var n = _t.call(this, t, e);
                             e & (G | W) && n[0].length - n[1].length == 0 && (this.started = !1), this.callback(this.manager, e, {
                                 pointers: n[0],
                                 changedPointers: n[1],
-                                pointerType: D,
+                                pointerType: N,
                                 srcEvent: t
                             })
                         }
                     }
                 });
                 var xt = {
                         touchstart: U,
@@ -31205,41 +31287,41 @@
                     },
                     wt = "touchstart touchmove touchend touchcancel";
 
                 function Et() {
                     this.evTarget = wt, this.targetIds = {}, et.apply(this, arguments)
                 }
 
-                function Pt(t, e) {
-                    var n = O(t.touches),
+                function St(t, e) {
+                    var n = L(t.touches),
                         i = this.targetIds;
                     if (e & (2 | U) && 1 === n.length) return i[n[0].identifier] = !0, [n, n];
-                    var r, s, o = O(t.changedTouches),
+                    var r, s, o = L(t.changedTouches),
                         a = [],
                         l = this.target;
                     if (s = n.filter((function(t) {
                             return T(t.target, l)
                         })), e === U)
                         for (r = 0; r < s.length;) i[s[r].identifier] = !0, r++;
                     for (r = 0; r < o.length;) i[o[r].identifier] && a.push(o[r]), e & (G | W) && delete i[o[r].identifier], r++;
-                    return a.length ? [R(s.concat(a), "identifier", !0), a] : void 0
+                    return a.length ? [I(s.concat(a), "identifier", !0), a] : void 0
                 }
                 x(Et, et, {
                     handler: function(t) {
                         var e = xt[t.type],
-                            n = Pt.call(this, t, e);
+                            n = St.call(this, t, e);
                         n && this.callback(this.manager, e, {
                             pointers: n[0],
                             changedPointers: n[1],
-                            pointerType: D,
+                            pointerType: N,
                             srcEvent: t
                         })
                     }
                 });
-                var St = 2500;
+                var Pt = 2500;
 
                 function Ct() {
                     et.apply(this, arguments);
                     var t = w(this.handler, this);
                     this.touch = new Et(this.manager, t), this.mouse = new dt(this.manager, t), this.primaryTouch = null, this.lastTouches = []
                 }
 
@@ -31255,78 +31337,78 @@
                             y: e.clientY
                         };
                         this.lastTouches.push(n);
                         var i = this.lastTouches;
                         setTimeout((function() {
                             var t = i.indexOf(n);
                             t > -1 && i.splice(t, 1)
-                        }), St)
+                        }), Pt)
                     }
                 }
 
                 function Mt(t) {
                     for (var e = t.srcEvent.clientX, n = t.srcEvent.clientY, i = 0; i < this.lastTouches.length; i++) {
                         var r = this.lastTouches[i],
                             s = Math.abs(e - r.x),
                             o = Math.abs(n - r.y);
                         if (s <= 25 && o <= 25) return !0
                     }
                     return !1
                 }
                 x(Ct, et, {
                     handler: function(t, e, n) {
-                        var i = n.pointerType == D,
-                            r = n.pointerType == N;
+                        var i = n.pointerType == N,
+                            r = n.pointerType == D;
                         if (!(r && n.sourceCapabilities && n.sourceCapabilities.firesTouchEvents)) {
                             if (i) Tt.call(this, e, n);
                             else if (r && Mt.call(this, n)) return;
                             this.callback(t, e, n)
                         }
                     },
                     destroy: function() {
                         this.touch.destroy(), this.mouse.destroy()
                     }
                 });
-                var Lt = k(h.style, "touchAction"),
-                    Ot = Lt !== a,
-                    Rt = "compute",
+                var Ot = k(h.style, "touchAction"),
+                    Lt = Ot !== a,
+                    It = "compute",
                     kt = "auto",
-                    It = "manipulation",
+                    Rt = "manipulation",
                     jt = "none",
                     zt = "pan-x",
                     Ft = "pan-y",
                     Bt = function() {
-                        if (!Ot) return !1;
+                        if (!Lt) return !1;
                         var t = {},
                             e = r.CSS && r.CSS.supports;
                         return ["auto", "manipulation", "pan-y", "pan-x", "pan-x pan-y", "none"].forEach((function(n) {
                             t[n] = !e || r.CSS.supports("touch-action", n)
                         })), t
                     }();
 
-                function Dt(t, e) {
+                function Nt(t, e) {
                     this.manager = t, this.set(e)
                 }
-                Dt.prototype = {
+                Nt.prototype = {
                     set: function(t) {
-                        t == Rt && (t = this.compute()), Ot && this.manager.element.style && Bt[t] && (this.manager.element.style[Lt] = t), this.actions = t.toLowerCase().trim()
+                        t == It && (t = this.compute()), Lt && this.manager.element.style && Bt[t] && (this.manager.element.style[Ot] = t), this.actions = t.toLowerCase().trim()
                     },
                     update: function() {
                         this.set(this.manager.options.touchAction)
                     },
                     compute: function() {
                         var t = [];
                         return v(this.manager.recognizers, (function(e) {
                                 E(e.options.enable, [e]) && (t = t.concat(e.getTouchAction()))
                             })),
                             function(t) {
                                 if (A(t, jt)) return jt;
                                 var e = A(t, zt),
                                     n = A(t, Ft);
-                                return e && n ? jt : e || n ? e ? zt : Ft : A(t, It) ? It : kt
+                                return e && n ? jt : e || n ? e ? zt : Ft : A(t, Rt) ? Rt : kt
                             }(t.join(" "))
                     },
                     preventDefaults: function(t) {
                         var e = t.srcEvent,
                             n = t.offsetDirection;
                         if (this.manager.session.prevented) e.preventDefault();
                         else {
@@ -31343,43 +31425,43 @@
                             if (!o || !s) return r || s && n & K || o && n & $ ? this.preventSrc(e) : void 0
                         }
                     },
                     preventSrc: function(t) {
                         this.manager.session.prevented = !0, t.preventDefault()
                     }
                 };
-                var Nt = 1,
+                var Dt = 1,
                     Vt = 32;
 
                 function Ut(t) {
-                    this.options = l({}, this.defaults, t || {}), this.id = I++, this.manager = null, this.options.enable = P(this.options.enable, !0), this.state = Nt, this.simultaneous = {}, this.requireFail = []
+                    this.options = l({}, this.defaults, t || {}), this.id = R++, this.manager = null, this.options.enable = S(this.options.enable, !0), this.state = Dt, this.simultaneous = {}, this.requireFail = []
                 }
 
                 function Gt(t) {
                     return 16 & t ? "cancel" : 8 & t ? "end" : 4 & t ? "move" : 2 & t ? "start" : ""
                 }
 
                 function Wt(t) {
-                    return t == Y ? "down" : t == X ? "up" : t == Z ? "left" : t == q ? "right" : ""
+                    return t == Y ? "down" : t == q ? "up" : t == Z ? "left" : t == X ? "right" : ""
                 }
 
                 function Ht(t, e) {
                     var n = e.manager;
                     return n ? n.get(t) : t
                 }
 
                 function Zt() {
                     Ut.apply(this, arguments)
                 }
 
-                function qt() {
+                function Xt() {
                     Zt.apply(this, arguments), this.pX = null, this.pY = null
                 }
 
-                function Xt() {
+                function qt() {
                     Zt.apply(this, arguments)
                 }
 
                 function Yt() {
                     Ut.apply(this, arguments), this._timer = null, this._input = null
                 }
 
@@ -31392,19 +31474,19 @@
                 }
 
                 function Jt() {
                     Ut.apply(this, arguments), this.pTime = !1, this.pCenter = !1, this._timer = null, this._input = null, this.count = 0
                 }
 
                 function Qt(t, e) {
-                    return (e = e || {}).recognizers = P(e.recognizers, Qt.defaults.preset), new te(t, e)
+                    return (e = e || {}).recognizers = S(e.recognizers, Qt.defaults.preset), new te(t, e)
                 }
 
                 function te(t, e) {
-                    this.options = l({}, Qt.defaults, e || {}), this.options.inputTarget = this.options.inputTarget || t, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = t, this.input = new(this.options.inputClass || (F ? vt : B ? Et : z ? Ct : dt))(this, nt), this.touchAction = new Dt(this, this.options.touchAction), ee(this, !0), v(this.options.recognizers, (function(t) {
+                    this.options = l({}, Qt.defaults, e || {}), this.options.inputTarget = this.options.inputTarget || t, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = t, this.input = new(this.options.inputClass || (F ? vt : B ? Et : z ? Ct : dt))(this, nt), this.touchAction = new Nt(this, this.options.touchAction), ee(this, !0), v(this.options.recognizers, (function(t) {
                         var e = this.add(new t[0](t[1]));
                         t[2] && e.recognizeWith(t[2]), t[3] && e.requireFailure(t[3])
                     }), this)
                 }
 
                 function ee(t, e) {
                     var n, i = t.element;
@@ -31424,20 +31506,20 @@
                     },
                     dropRecognizeWith: function(t) {
                         return m(t, "dropRecognizeWith", this) || (t = Ht(t, this), delete this.simultaneous[t.id]), this
                     },
                     requireFailure: function(t) {
                         if (m(t, "requireFailure", this)) return this;
                         var e = this.requireFail;
-                        return -1 === L(e, t = Ht(t, this)) && (e.push(t), t.requireFailure(this)), this
+                        return -1 === O(e, t = Ht(t, this)) && (e.push(t), t.requireFailure(this)), this
                     },
                     dropRequireFailure: function(t) {
                         if (m(t, "dropRequireFailure", this)) return this;
                         t = Ht(t, this);
-                        var e = L(this.requireFail, t);
+                        var e = O(this.requireFail, t);
                         return e > -1 && this.requireFail.splice(e, 1), this
                     },
                     hasRequireFailures: function() {
                         return this.requireFail.length > 0
                     },
                     canRecognizeWith: function(t) {
                         return !!this.simultaneous[t.id]
@@ -31453,23 +31535,23 @@
                     },
                     tryEmit: function(t) {
                         if (this.canEmit()) return this.emit(t);
                         this.state = Vt
                     },
                     canEmit: function() {
                         for (var t = 0; t < this.requireFail.length;) {
-                            if (!(this.requireFail[t].state & (Vt | Nt))) return !1;
+                            if (!(this.requireFail[t].state & (Vt | Dt))) return !1;
                             t++
                         }
                         return !0
                     },
                     recognize: function(t) {
                         var e = l({}, t);
                         if (!E(this.options.enable, [this, e])) return this.reset(), void(this.state = Vt);
-                        56 & this.state && (this.state = Nt), this.state = this.process(e), 30 & this.state && this.tryEmit(e)
+                        56 & this.state && (this.state = Dt), this.state = this.process(e), 30 & this.state && this.tryEmit(e)
                     },
                     process: function(t) {},
                     getTouchAction: function() {},
                     reset: function() {}
                 }, x(Zt, Ut, {
                     defaults: {
                         pointers: 1
@@ -31481,15 +31563,15 @@
                     process: function(t) {
                         var e = this.state,
                             n = t.eventType,
                             i = 6 & e,
                             r = this.attrTest(t);
                         return i && (n & W || !r) ? 16 | e : i || r ? n & G ? 8 | e : 2 & e ? 4 | e : 2 : Vt
                     }
-                }), x(qt, Zt, {
+                }), x(Xt, Zt, {
                     defaults: {
                         event: "pan",
                         threshold: 10,
                         pointers: 1,
                         direction: J
                     },
                     getTouchAction: function() {
@@ -31500,25 +31582,25 @@
                     directionTest: function(t) {
                         var e = this.options,
                             n = !0,
                             i = t.distance,
                             r = t.direction,
                             s = t.deltaX,
                             o = t.deltaY;
-                        return r & e.direction || (e.direction & K ? (r = 0 === s ? H : s < 0 ? Z : q, n = s != this.pX, i = Math.abs(t.deltaX)) : (r = 0 === o ? H : o < 0 ? X : Y, n = o != this.pY, i = Math.abs(t.deltaY))), t.direction = r, n && i > e.threshold && r & e.direction
+                        return r & e.direction || (e.direction & K ? (r = 0 === s ? H : s < 0 ? Z : X, n = s != this.pX, i = Math.abs(t.deltaX)) : (r = 0 === o ? H : o < 0 ? q : Y, n = o != this.pY, i = Math.abs(t.deltaY))), t.direction = r, n && i > e.threshold && r & e.direction
                     },
                     attrTest: function(t) {
                         return Zt.prototype.attrTest.call(this, t) && (2 & this.state || !(2 & this.state) && this.directionTest(t))
                     },
                     emit: function(t) {
                         this.pX = t.deltaX, this.pY = t.deltaY;
                         var e = Wt(t.direction);
                         e && (t.additionalEvent = this.options.event + e), this._super.emit.call(this, t)
                     }
-                }), x(Xt, Zt, {
+                }), x(qt, Zt, {
                     defaults: {
                         event: "pinch",
                         threshold: 0,
                         pointers: 2
                     },
                     getTouchAction: function() {
                         return [jt]
@@ -31578,15 +31660,15 @@
                         event: "swipe",
                         threshold: 10,
                         velocity: .3,
                         direction: K | $,
                         pointers: 1
                     },
                     getTouchAction: function() {
-                        return qt.prototype.getTouchAction.call(this)
+                        return Xt.prototype.getTouchAction.call(this)
                     },
                     attrTest: function(t) {
                         var e, n = this.options.direction;
                         return n & (K | $) ? e = t.overallVelocity : n & K ? e = t.overallVelocityX : n & $ && (e = t.overallVelocityY), this._super.attrTest.call(this, t) && n & t.offsetDirection && t.distance > this.options.threshold && t.maxPointers == this.options.pointers && p(e) > this.options.velocity && t.eventType & G
                     },
                     emit: function(t) {
                         var e = Wt(t.offsetDirection);
@@ -31599,15 +31681,15 @@
                         taps: 1,
                         interval: 300,
                         time: 250,
                         threshold: 9,
                         posThreshold: 10
                     },
                     getTouchAction: function() {
-                        return [It]
+                        return [Rt]
                     },
                     process: function(t) {
                         var e = this.options,
                             n = t.pointers.length === e.pointers,
                             i = t.distance < e.threshold,
                             r = t.deltaTime < e.time;
                         if (this.reset(), t.eventType & U && 0 === this.count) return this.failTimeout();
@@ -31630,31 +31712,31 @@
                         clearTimeout(this._timer)
                     },
                     emit: function() {
                         8 == this.state && (this._input.tapCount = this.count, this.manager.emit(this.options.event, this._input))
                     }
                 }), Qt.VERSION = "2.0.7", Qt.defaults = {
                     domEvents: !1,
-                    touchAction: Rt,
+                    touchAction: It,
                     enable: !0,
                     inputTarget: null,
                     inputClass: null,
                     preset: [
                         [Kt, {
                             enable: !1
                         }],
-                        [Xt, {
+                        [qt, {
                                 enable: !1
                             },
                             ["rotate"]
                         ],
                         [$t, {
                             direction: K
                         }],
-                        [qt, {
+                        [Xt, {
                                 direction: K
                             },
                             ["swipe"]
                         ],
                         [Jt],
                         [Jt, {
                                 event: "doubletap",
@@ -31701,15 +31783,15 @@
                         var e = this.get(t.options.event);
                         return e && this.remove(e), this.recognizers.push(t), t.manager = this, this.touchAction.update(), t
                     },
                     remove: function(t) {
                         if (m(t, "remove", this)) return this;
                         if (t = this.get(t)) {
                             var e = this.recognizers,
-                                n = L(e, t); - 1 !== n && (e.splice(n, 1), this.touchAction.update())
+                                n = O(e, t); - 1 !== n && (e.splice(n, 1), this.touchAction.update())
                         }
                         return this
                     },
                     on: function(t, e) {
                         if (t !== a && e !== a) {
                             var n = this.handlers;
                             return v(M(t), (function(t) {
@@ -31717,15 +31799,15 @@
                             })), this
                         }
                     },
                     off: function(t, e) {
                         if (t !== a) {
                             var n = this.handlers;
                             return v(M(t), (function(t) {
-                                e ? n[t] && n[t].splice(L(n[t], e), 1) : delete n[t]
+                                e ? n[t] && n[t].splice(O(n[t], e), 1) : delete n[t]
                             })), this
                         }
                     },
                     emit: function(t, e) {
                         this.options.domEvents && function(t, e) {
                             var n = s.createEvent("Event");
                             n.initEvent(t, !0, !0), n.gesture = e, e.target.dispatchEvent(n)
@@ -31742,46 +31824,46 @@
                         this.element && ee(this, !1), this.handlers = {}, this.session = {}, this.input.destroy(), this.element = null
                     }
                 }, l(Qt, {
                     INPUT_START: U,
                     INPUT_MOVE: 2,
                     INPUT_END: G,
                     INPUT_CANCEL: W,
-                    STATE_POSSIBLE: Nt,
+                    STATE_POSSIBLE: Dt,
                     STATE_BEGAN: 2,
                     STATE_CHANGED: 4,
                     STATE_ENDED: 8,
                     STATE_RECOGNIZED: 8,
                     STATE_CANCELLED: 16,
                     STATE_FAILED: Vt,
                     DIRECTION_NONE: H,
                     DIRECTION_LEFT: Z,
-                    DIRECTION_RIGHT: q,
-                    DIRECTION_UP: X,
+                    DIRECTION_RIGHT: X,
+                    DIRECTION_UP: q,
                     DIRECTION_DOWN: Y,
                     DIRECTION_HORIZONTAL: K,
                     DIRECTION_VERTICAL: $,
                     DIRECTION_ALL: J,
                     Manager: te,
                     Input: et,
-                    TouchAction: Dt,
+                    TouchAction: Nt,
                     TouchInput: Et,
                     MouseInput: dt,
                     PointerEventInput: vt,
                     TouchMouseInput: Ct,
                     SingleTouchInput: yt,
                     Recognizer: Ut,
                     AttrRecognizer: Zt,
                     Tap: Jt,
-                    Pan: qt,
+                    Pan: Xt,
                     Swipe: $t,
-                    Pinch: Xt,
+                    Pinch: qt,
                     Rotate: Kt,
                     Press: Yt,
-                    on: S,
+                    on: P,
                     off: C,
                     each: v,
                     merge: _,
                     extend: y,
                     assign: l,
                     inherit: x,
                     bindFn: w,
@@ -32074,50 +32156,50 @@
                 v = n(8517),
                 b = n(1469),
                 y = n(4144),
                 _ = n(6688),
                 x = n(3218),
                 w = n(2928),
                 E = n(3674),
-                P = n(1704),
-                S = "[object Arguments]",
+                S = n(1704),
+                P = "[object Arguments]",
                 C = "[object Function]",
                 T = "[object Object]",
                 A = {};
-            A[S] = A["[object Array]"] = A["[object ArrayBuffer]"] = A["[object DataView]"] = A["[object Boolean]"] = A["[object Date]"] = A["[object Float32Array]"] = A["[object Float64Array]"] = A["[object Int8Array]"] = A["[object Int16Array]"] = A["[object Int32Array]"] = A["[object Map]"] = A["[object Number]"] = A[T] = A["[object RegExp]"] = A["[object Set]"] = A["[object String]"] = A["[object Symbol]"] = A["[object Uint8Array]"] = A["[object Uint8ClampedArray]"] = A["[object Uint16Array]"] = A["[object Uint32Array]"] = !0, A["[object Error]"] = A[C] = A["[object WeakMap]"] = !1, t.exports = function t(e, n, M, L, O, R) {
-                var k, I = 1 & n,
+            A[P] = A["[object Array]"] = A["[object ArrayBuffer]"] = A["[object DataView]"] = A["[object Boolean]"] = A["[object Date]"] = A["[object Float32Array]"] = A["[object Float64Array]"] = A["[object Int8Array]"] = A["[object Int16Array]"] = A["[object Int32Array]"] = A["[object Map]"] = A["[object Number]"] = A[T] = A["[object RegExp]"] = A["[object Set]"] = A["[object String]"] = A["[object Symbol]"] = A["[object Uint8Array]"] = A["[object Uint8ClampedArray]"] = A["[object Uint16Array]"] = A["[object Uint32Array]"] = !0, A["[object Error]"] = A[C] = A["[object WeakMap]"] = !1, t.exports = function t(e, n, M, O, L, I) {
+                var k, R = 1 & n,
                     j = 2 & n,
                     z = 4 & n;
-                if (M && (k = O ? M(e, L, O, R) : M(e)), void 0 !== k) return k;
+                if (M && (k = L ? M(e, O, L, I) : M(e)), void 0 !== k) return k;
                 if (!x(e)) return e;
                 var F = b(e);
                 if (F) {
-                    if (k = g(e), !I) return c(e, k)
+                    if (k = g(e), !R) return c(e, k)
                 } else {
                     var B = f(e),
-                        D = B == C || "[object GeneratorFunction]" == B;
-                    if (y(e)) return l(e, I);
-                    if (B == T || B == S || D && !O) {
-                        if (k = j || D ? {} : v(e), !I) return j ? u(e, a(k, e)) : h(e, o(k, e))
+                        N = B == C || "[object GeneratorFunction]" == B;
+                    if (y(e)) return l(e, R);
+                    if (B == T || B == P || N && !L) {
+                        if (k = j || N ? {} : v(e), !R) return j ? u(e, a(k, e)) : h(e, o(k, e))
                     } else {
-                        if (!A[B]) return O ? e : {};
-                        k = m(e, B, I)
+                        if (!A[B]) return L ? e : {};
+                        k = m(e, B, R)
                     }
                 }
-                R || (R = new i);
-                var N = R.get(e);
-                if (N) return N;
-                R.set(e, k), w(e) ? e.forEach((function(i) {
-                    k.add(t(i, n, M, i, e, R))
+                I || (I = new i);
+                var D = I.get(e);
+                if (D) return D;
+                I.set(e, k), w(e) ? e.forEach((function(i) {
+                    k.add(t(i, n, M, i, e, I))
                 })) : _(e) && e.forEach((function(i, r) {
-                    k.set(r, t(i, n, M, r, e, R))
+                    k.set(r, t(i, n, M, r, e, I))
                 }));
-                var V = F ? void 0 : (z ? j ? p : d : j ? P : E)(e);
+                var V = F ? void 0 : (z ? j ? p : d : j ? S : E)(e);
                 return r(V || e, (function(i, r) {
-                    V && (i = e[r = i]), s(k, r, t(i, n, M, r, e, R))
+                    V && (i = e[r = i]), s(k, r, t(i, n, M, r, e, I))
                 })), k
             }
         },
         3118: (t, e, n) => {
             var i = n(3218),
                 r = Object.create,
                 s = function() {
@@ -32208,30 +32290,30 @@
             t.exports = function(t, e, n, g, m, v) {
                 var b = l(t),
                     y = l(e),
                     _ = b ? d : a(t),
                     x = y ? d : a(e),
                     w = (_ = _ == u ? p : _) == p,
                     E = (x = x == u ? p : x) == p,
-                    P = _ == x;
-                if (P && c(t)) {
+                    S = _ == x;
+                if (S && c(t)) {
                     if (!c(e)) return !1;
                     b = !0, w = !1
                 }
-                if (P && !w) return v || (v = new i), b || h(t) ? r(t, e, n, g, m, v) : s(t, e, _, n, g, m, v);
+                if (S && !w) return v || (v = new i), b || h(t) ? r(t, e, n, g, m, v) : s(t, e, _, n, g, m, v);
                 if (!(1 & n)) {
-                    var S = w && f.call(t, "__wrapped__"),
+                    var P = w && f.call(t, "__wrapped__"),
                         C = E && f.call(e, "__wrapped__");
-                    if (S || C) {
-                        var T = S ? t.value() : t,
+                    if (P || C) {
+                        var T = P ? t.value() : t,
                             A = C ? e.value() : e;
                         return v || (v = new i), m(T, A, n, g, v)
                     }
                 }
-                return !!P && (v || (v = new i), o(t, e, n, g, m, v))
+                return !!S && (v || (v = new i), o(t, e, n, g, m, v))
             }
         },
         5588: (t, e, n) => {
             var i = n(4160),
                 r = n(7005);
             t.exports = function(t) {
                 return r(t) && "[object Map]" == i(t)
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/995.ed09fb94a4cde32b3298.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
-/*! For license information please see 635.b2bedc962bcd82714540.js.LICENSE.txt */
+/*! For license information please see 995.ed09fb94a4cde32b3298.js.LICENSE.txt */
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
-    [635], {
+    [995], {
         9757: (t, e, r) => {
             "use strict";
             r.d(e, {
                 Z: () => i
             });
             const i = {
                 DEPTH_BUFFER_BIT: 256,
@@ -15679,14 +15679,160 @@
                     if (Array.isArray(t) || "array" === e)
                         for (s = 0, a = r, o = (e = new d(t.length + r)).length; a < o; a++, s++) e[a] = null === t[s] ? NaN : t[s];
                     else 0 === r ? e = new d(t) : (e = new d(t.length + r)).set(t, r)
                 }
                 return e
             }
         },
+        8399: (t, e, r) => {
+            "use strict";
+            r.d(e, {
+                X3: () => y
+            });
+            const i = (t, e) => e.some((e => t instanceof e));
+            let s, n;
+            const a = new WeakMap,
+                o = new WeakMap,
+                c = new WeakMap,
+                u = new WeakMap,
+                p = new WeakMap;
+            let d = {
+                get(t, e, r) {
+                    if (t instanceof IDBTransaction) {
+                        if ("done" === e) return o.get(t);
+                        if ("objectStoreNames" === e) return t.objectStoreNames || c.get(t);
+                        if ("store" === e) return r.objectStoreNames[1] ? void 0 : r.objectStore(r.objectStoreNames[0])
+                    }
+                    return g(t[e])
+                },
+                set: (t, e, r) => (t[e] = r, !0),
+                has: (t, e) => t instanceof IDBTransaction && ("done" === e || "store" === e) || e in t
+            };
+
+            function l(t) {
+                d = t(d)
+            }
+
+            function h(t) {
+                return "function" == typeof t ? (e = t) !== IDBDatabase.prototype.transaction || "objectStoreNames" in IDBTransaction.prototype ? (n || (n = [IDBCursor.prototype.advance, IDBCursor.prototype.continue, IDBCursor.prototype.continuePrimaryKey])).includes(e) ? function(...t) {
+                    return e.apply(f(this), t), g(a.get(this))
+                } : function(...t) {
+                    return g(e.apply(f(this), t))
+                } : function(t, ...r) {
+                    const i = e.call(f(this), t, ...r);
+                    return c.set(i, t.sort ? t.sort() : [t]), g(i)
+                } : (t instanceof IDBTransaction && function(t) {
+                    if (o.has(t)) return;
+                    const e = new Promise(((e, r) => {
+                        const i = () => {
+                                t.removeEventListener("complete", s), t.removeEventListener("error", n), t.removeEventListener("abort", n)
+                            },
+                            s = () => {
+                                e(), i()
+                            },
+                            n = () => {
+                                r(t.error || new DOMException("AbortError", "AbortError")), i()
+                            };
+                        t.addEventListener("complete", s), t.addEventListener("error", n), t.addEventListener("abort", n)
+                    }));
+                    o.set(t, e)
+                }(t), i(t, s || (s = [IDBDatabase, IDBObjectStore, IDBIndex, IDBCursor, IDBTransaction])) ? new Proxy(t, d) : t);
+                var e
+            }
+
+            function g(t) {
+                if (t instanceof IDBRequest) return function(t) {
+                    const e = new Promise(((e, r) => {
+                        const i = () => {
+                                t.removeEventListener("success", s), t.removeEventListener("error", n)
+                            },
+                            s = () => {
+                                e(g(t.result)), i()
+                            },
+                            n = () => {
+                                r(t.error), i()
+                            };
+                        t.addEventListener("success", s), t.addEventListener("error", n)
+                    }));
+                    return e.then((e => {
+                        e instanceof IDBCursor && a.set(e, t)
+                    })).catch((() => {})), p.set(e, t), e
+                }(t);
+                if (u.has(t)) return u.get(t);
+                const e = h(t);
+                return e !== t && (u.set(t, e), p.set(e, t)), e
+            }
+            const f = t => p.get(t);
+
+            function y(t, e, {
+                blocked: r,
+                upgrade: i,
+                blocking: s,
+                terminated: n
+            } = {}) {
+                const a = indexedDB.open(t, e),
+                    o = g(a);
+                return i && a.addEventListener("upgradeneeded", (t => {
+                    i(g(a.result), t.oldVersion, t.newVersion, g(a.transaction), t)
+                })), r && a.addEventListener("blocked", (t => r(t.oldVersion, t.newVersion, t))), o.then((t => {
+                    n && t.addEventListener("close", (() => n())), s && t.addEventListener("versionchange", (t => s(t.oldVersion, t.newVersion, t)))
+                })).catch((() => {})), o
+            }
+            const S = ["get", "getKey", "getAll", "getAllKeys", "count"],
+                m = ["put", "add", "delete", "clear"],
+                A = new Map;
+
+            function T(t, e) {
+                if (!(t instanceof IDBDatabase) || e in t || "string" != typeof e) return;
+                if (A.get(e)) return A.get(e);
+                const r = e.replace(/FromIndex$/, ""),
+                    i = e !== r,
+                    s = m.includes(r);
+                if (!(r in (i ? IDBIndex : IDBObjectStore).prototype) || !s && !S.includes(r)) return;
+                const n = async function(t, ...e) {
+                    const n = this.transaction(t, s ? "readwrite" : "readonly");
+                    let a = n.store;
+                    return i && (a = a.index(e.shift())), (await Promise.all([a[r](...e), s && n.done]))[0]
+                };
+                return A.set(e, n), n
+            }
+            l((t => ({
+                ...t,
+                get: (e, r, i) => T(e, r) || t.get(e, r, i),
+                has: (e, r) => !!T(e, r) || t.has(e, r)
+            })));
+            const E = ["continue", "continuePrimaryKey", "advance"],
+                b = {},
+                _ = new WeakMap,
+                O = new WeakMap,
+                P = {
+                    get(t, e) {
+                        if (!E.includes(e)) return t[e];
+                        let r = b[e];
+                        return r || (r = b[e] = function(...t) {
+                            _.set(this, O.get(this)[e](...t))
+                        }), r
+                    }
+                };
+            async function* U(...t) {
+                let e = this;
+                if (e instanceof IDBCursor || (e = await e.openCursor(...t)), !e) return;
+                const r = new Proxy(e, P);
+                for (O.set(r, e), p.set(r, f(e)); e;) yield r, e = await (_.get(r) || e.continue()), _.delete(r)
+            }
+
+            function v(t, e) {
+                return e === Symbol.asyncIterator && i(t, [IDBIndex, IDBObjectStore, IDBCursor]) || "iterate" === e && i(t, [IDBIndex, IDBObjectStore])
+            }
+            l((t => ({
+                ...t,
+                get: (e, r, i) => v(e, r) ? U : t.get(e, r, i),
+                has: (e, r) => v(e, r) || t.has(e, r)
+            })))
+        },
         8648: function(t, e) {
             ! function(r) {
                 "use strict";
 
                 function i(t, e) {
                     if (t instanceof Boolean || "boolean" == typeof t) return !1;
                     if (e instanceof Object || (e = {}), e.hasOwnProperty("allowBlank") && !e.allowBlank && "" === t) return !1;
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/995.ed09fb94a4cde32b3298.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/744.cd9879bb199b94dec1b9.js` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/744.189af4ed2998fcfe7556.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -12,15 +12,15 @@
                 BioImageViewerModel: () => d,
                 BioImageViewerView: () => p
             });
             var s = l(1395);
             const n = l(4147),
                 a = n.version,
                 r = n.name;
-            var o = l(5742),
+            var o = l(4614),
                 u = l.n(o);
             class d extends s.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: d.model_name,
                         _model_module: d.model_module,
                         _model_module_version: d.model_module_version,
@@ -57,11 +57,11 @@
                         version: a,
                         exports: t
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.3-alpha.3","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","tiledb","bioimaging","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js","dist/*.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension && jlpm run build:dist","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:dist":"NODE_OPTIONS=--max-old-space-size=4096 webpack --mode=production","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.3"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.lab.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.3-alpha.4","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","tiledb","bioimaging","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js","dist/*.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension && jlpm run build:dist","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:dist":"NODE_OPTIONS=--max-old-space-size=4096 webpack --mode=production","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.4"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","ts-loader":"^9.2.5","typescript":"~4.1.3"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.lab.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/remoteEntry.2fd765b4b184cbb0da17.js` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/remoteEntry.a7cbc27a79641454b2f4.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, i, o, a, l, d, u, f, s, c, p, h, b, v, m, g, y = {
+    var e, r, t, n, i, o, a, d, l, u, f, c, s, p, h, v, b, m, g, y = {
             5290: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -44,27 +44,27 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        241: "7a42393c28911f92f6c6",
+        79: "06e38572ee0f6236bd5c",
         446: "3bf34f45c93ace9c0f28",
-        556: "2c70ba3b8c5599c82503",
-        635: "b2bedc962bcd82714540",
-        744: "cd9879bb199b94dec1b9",
-        747: "433530952542f03ebc71"
+        556: "06e35fefdb145d6110cd",
+        744: "189af4ed2998fcfe7556",
+        747: "433530952542f03ebc71",
+        995: "ed09fb94a4cde32b3298"
     } [e] + ".js?v=" + {
-        241: "7a42393c28911f92f6c6",
+        79: "06e38572ee0f6236bd5c",
         446: "3bf34f45c93ace9c0f28",
-        556: "2c70ba3b8c5599c82503",
-        635: "b2bedc962bcd82714540",
-        744: "cd9879bb199b94dec1b9",
-        747: "433530952542f03ebc71"
+        556: "06e35fefdb145d6110cd",
+        744: "189af4ed2998fcfe7556",
+        747: "433530952542f03ebc71",
+        995: "ed09fb94a4cde32b3298"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -72,34 +72,34 @@
         enumerable: !0,
         set: () => {
             throw new Error("ES Modules may not assign module.exports or exports.*, Use ESM export syntax, instead: " + e.id)
         }
     }), e), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", S.l = (t, n, i, o) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, l;
+            var a, d;
             if (void 0 !== i)
-                for (var d = document.getElementsByTagName("script"), u = 0; u < d.length; u++) {
-                    var f = d[u];
+                for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
+                    var f = l[u];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + i) {
                         a = f;
                         break
                     }
                 }
-            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
-            var s = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(c);
+            a || (d = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
+            var c = (r, n) => {
+                    a.onerror = a.onload = null, clearTimeout(s);
                     var i = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), i && i.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(s.bind(null, void 0, {
+                s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = s.bind(null, a.onerror), a.onload = s.bind(null, a.onload), l && document.head.appendChild(a)
+            a.onerror = c.bind(null, a.onerror), a.onload = c.bind(null, a.onload), d && document.head.appendChild(a)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -111,25 +111,25 @@
             n || (n = []);
             var i = r[t];
             if (i || (i = r[t] = {}), !(n.indexOf(i) >= 0)) {
                 if (n.push(i), e[t]) return e[t];
                 S.o(S.S, t) || (S.S[t] = {});
                 var o = S.S[t],
                     a = "@tiledb-inc/jupyter-bioimage-viewer",
-                    l = (e, r, t, n) => {
+                    d = (e, r, t, n) => {
                         var i = o[e] = o[e] || {},
-                            l = i[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : a > l.from)) && (i[r] = {
+                            d = i[r];
+                        (!d || !d.loaded && (!n != !d.eager ? n : a > d.from)) && (i[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
-                    d = [];
-                return "default" === t && (l("@tiledb-inc/bioimage-viewer", "0.1.3", (() => Promise.all([S.e(635), S.e(556), S.e(446)]).then((() => () => S(1556))))), l("@tiledb-inc/jupyter-bioimage-viewer", "0.1.3-alpha.3", (() => S.e(744).then((() => () => S(1744)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                    l = [];
+                return "default" === t && (d("@tiledb-inc/bioimage-viewer", "0.1.4", (() => Promise.all([S.e(995), S.e(556), S.e(446)]).then((() => () => S(1556))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.3-alpha.4", (() => S.e(744).then((() => () => S(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -148,123 +148,123 @@
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var i = e[n],
                 o = (typeof i)[0];
             if (n >= r.length) return "u" == o;
             var a = r[n],
-                l = (typeof a)[0];
-            if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
+                d = (typeof a)[0];
+            if (o != d) return "o" == o && "n" == d || "s" == d || "u" == o;
             if ("o" != o && "u" != o && i != a) return i < a;
             n++
         }
     }, i = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
             return t
         }
         var a = [];
         for (o = 1; o < e.length; o++) {
-            var l = e[o];
-            a.push(0 === l ? "not(" + d() + ")" : 1 === l ? "(" + d() + " || " + d() + ")" : 2 === l ? a.pop() + " " + a.pop() : i(l))
+            var d = e[o];
+            a.push(0 === d ? "not(" + l() + ")" : 1 === d ? "(" + l() + " || " + l() + ")" : 2 === d ? a.pop() + " " + a.pop() : i(d))
         }
-        return d();
+        return l();
 
-        function d() {
+        function l() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 i = n < 0;
             i && (n = -n - 1);
-            for (var a = 0, l = 1, d = !0;; l++, a++) {
-                var u, f, s = l < e.length ? (typeof e[l])[0] : "";
-                if (a >= r.length || "o" == (f = (typeof(u = r[a]))[0])) return !d || ("u" == s ? l > n && !i : "" == s != i);
+            for (var a = 0, d = 1, l = !0;; d++, a++) {
+                var u, f, c = d < e.length ? (typeof e[d])[0] : "";
+                if (a >= r.length || "o" == (f = (typeof(u = r[a]))[0])) return !l || ("u" == c ? d > n && !i : "" == c != i);
                 if ("u" == f) {
-                    if (!d || "u" != s) return !1
-                } else if (d)
-                    if (s == f)
-                        if (l <= n) {
-                            if (u != e[l]) return !1
+                    if (!l || "u" != c) return !1
+                } else if (l)
+                    if (c == f)
+                        if (d <= n) {
+                            if (u != e[d]) return !1
                         } else {
-                            if (i ? u > e[l] : u < e[l]) return !1;
-                            u != e[l] && (d = !1)
+                            if (i ? u > e[d] : u < e[d]) return !1;
+                            u != e[d] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
-                    if (i || l <= n) return !1;
-                    d = !1, l--
+                else if ("s" != c && "n" != c) {
+                    if (i || d <= n) return !1;
+                    l = !1, d--
                 } else {
-                    if (l <= n || f < s != i) return !1;
-                    d = !1
-                } else "s" != s && "n" != s && (d = !1, l--)
+                    if (d <= n || f < c != i) return !1;
+                    l = !1
+                } else "s" != c && "n" != c && (l = !1, d--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var s = [],
+            p = s.pop.bind(s);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
         return !!p()
     }, a = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, l = (e, r) => {
+    }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
-        var i = l(e, t);
-        return o(n, i) || s(d(e, t, i, n)), c(e[t][i])
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
+        var i = d(e, t);
+        return o(n, i) || c(l(e, t, i, n)), s(e[t][i])
     }, f = (e, r, t) => {
         var i = e[r];
         return (r = Object.keys(i).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && i[r]
-    }, s = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, i) {
+    }, s = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, i) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, n, i)) : e(r, S.S[r], t, n, i)
-    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), b = p(((e, r, t, n, i) => {
+    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), v = p(((e, r, t, n, i) => {
         var o = r && S.o(r, t) && f(r, t, n);
-        return o ? c(o) : i()
-    })), v = {}, m = {
+        return o ? s(o) : i()
+    })), b = {}, m = {
         1395: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ]),
-        5742: () => b("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 3], (() => Promise.all([S.e(635), S.e(556), S.e(446)]).then((() => () => S(1556))))),
+        4614: () => v("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 4], (() => Promise.all([S.e(995), S.e(556), S.e(446)]).then((() => () => S(1556))))),
         4456: () => h("default", "react-dom", [1, 17, 0, 1]),
         6271: () => h("default", "react", [1, 17, 0, 1])
     }, g = {
         446: [4456, 6271],
-        744: [1395, 5742]
+        744: [1395, 4614]
     }, S.f.consumes = (e, r) => {
         S.o(g, e) && g[e].forEach((e => {
-            if (S.o(v, e)) return r.push(v[e]);
+            if (S.o(b, e)) return r.push(b[e]);
             var t = r => {
-                    v[e] = 0, S.m[e] = t => {
+                    b[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete v[e], S.m[e] = t => {
+                    delete b[e], S.m[e] = t => {
                         throw delete S.c[e], r
                     }
                 };
             try {
                 var i = m[e]();
-                i.then ? r.push(v[e] = i.then(t).catch(n)) : t(i)
+                i.then ? r.push(b[e] = i.then(t).catch(n)) : t(i)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         S.b = document.baseURI || self.location.href;
         var e = {
@@ -285,21 +285,21 @@
                                 o = t && t.target && t.target.src;
                             a.message = "Loading chunk " + r + " failed.\n(" + i + ": " + o + ")", a.name = "ChunkLoadError", a.type = i, a.request = o, n[1](a)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, i, [o, a, l] = t,
-                    d = 0;
+                var n, i, [o, a, d] = t,
+                    l = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (n in a) S.o(a, n) && (S.m[n] = a[n]);
-                    l && l(S)
+                    d && d(S)
                 }
-                for (r && r(t); d < o.length; d++) i = o[d], S.o(e, i) && e[i] && e[i][0](), e[i] = 0
+                for (r && r(t); l < o.length; l++) i = o[l], S.o(e, i) && e[i] && e[i][0](), e[i] = 0
             },
             t = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
     var j = S(5290);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@tiledb-inc/jupyter-bioimage-viewer"] = j
 })();
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.990301724137931%*

 * *Differences: {"'packages'": "{23: {'versionInfo': '0.1.4'}, insert: [(36, OrderedDict([('name', 'idb'), "*

 * *               "('versionInfo', '7.1.1'), ('licenseId', 'ISC'), ('extractedText', 'ISC License "*

 * *               '(ISC)\\nCopyright (c) 2016, Jake Archibald '*

 * *               '<jaffathecake@gmail.com>\\n\\nPermission to use, copy, modify, and/or distribute '*

 * *               'this software for any purpose with or without fee is hereby granted, provided that '*

 * *               'the above copyright notice and this permissio […]*

```diff
@@ -138,15 +138,15 @@
             "name": "@probe.gl/stats",
             "versionInfo": "3.6.0"
         },
         {
             "extractedText": "",
             "licenseId": "MIT",
             "name": "@tiledb-inc/bioimage-viewer",
-            "versionInfo": "0.1.3"
+            "versionInfo": "0.1.4"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2020 TileDB, Inc.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@tiledb-inc/tiledb-cloud",
             "versionInfo": "1.0.13-alpha.0"
         },
@@ -213,14 +213,20 @@
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (C) 2011-2014 by Jorik Tangelder (Eight Media)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "hammerjs",
             "versionInfo": "2.0.8"
         },
         {
+            "extractedText": "ISC License (ISC)\nCopyright (c) 2016, Jake Archibald <jaffathecake@gmail.com>\n\nPermission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.\n",
+            "licenseId": "ISC",
+            "name": "idb",
+            "versionInfo": "7.1.1"
+        },
+        {
             "extractedText": "MIT license\n\nCopyright (C) 2015 Miguel Mota\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of\nthis software and associated documentation files (the \"Software\"), to deal in\nthe Software without restriction, including without limitation the rights to\nuse, copy, modify, merge, publish, distribute, sublicense, and/or sell copies\nof the Software, and to permit persons to whom the Software is furnished to do\nso, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "is-base64",
             "versionInfo": "0.1.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) Sindre Sorhus <sindresorhus@gmail.com> (sindresorhus.com)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.3a3
+Version: 0.1.3a4
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.3a4/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 tiledb_jupyter_bioimg.egg-info/SOURCES.txt
 tiledb_jupyter_bioimg.egg-info/dependency_links.txt
 tiledb_jupyter_bioimg.egg-info/not-zip-safe
 tiledb_jupyter_bioimg.egg-info/requires.txt
 tiledb_jupyter_bioimg.egg-info/top_level.txt
 tiledb_jupyter_bioimg/labextension/package.json
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
-tiledb_jupyter_bioimg/labextension/static/241.7a42393c28911f92f6c6.js
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
-tiledb_jupyter_bioimg/labextension/static/556.2c70ba3b8c5599c82503.js
-tiledb_jupyter_bioimg/labextension/static/556.2c70ba3b8c5599c82503.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js
-tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/744.cd9879bb199b94dec1b9.js
+tiledb_jupyter_bioimg/labextension/static/556.06e35fefdb145d6110cd.js
+tiledb_jupyter_bioimg/labextension/static/556.06e35fefdb145d6110cd.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/744.189af4ed2998fcfe7556.js
 tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.2fd765b4b184cbb0da17.js
+tiledb_jupyter_bioimg/labextension/static/79.06e38572ee0f6236bd5c.js
+tiledb_jupyter_bioimg/labextension/static/995.ed09fb94a4cde32b3298.js
+tiledb_jupyter_bioimg/labextension/static/995.ed09fb94a4cde32b3298.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.a7cbc27a79641454b2f4.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a3/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.3a4/tsconfig.json`

 * *Files identical despite different names*

