# Comparing `tmp/datasette-render-images-0.3.2.tar.gz` & `tmp/datasette-render-images-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datasette-render-images-0.3.2.tar", last modified: Sun Aug 23 18:37:13 2020, max compression
+gzip compressed data, was "datasette-render-images-0.4.tar", last modified: Wed Jun 14 21:37:00 2023, max compression
```

## Comparing `datasette-render-images-0.3.2.tar` & `datasette-render-images-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-23 18:37:13.747914 datasette-render-images-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (116)     2888 2020-08-23 18:37:13.747914 datasette-render-images-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2189 2020-08-23 18:37:06.000000 datasette-render-images-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-23 18:37:13.747914 datasette-render-images-0.3.2/datasette_render_images.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2888 2020-08-23 18:37:13.000000 datasette-render-images-0.3.2/datasette_render_images.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      329 2020-08-23 18:37:13.000000 datasette-render-images-0.3.2/datasette_render_images.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-23 18:37:13.000000 datasette-render-images-0.3.2/datasette_render_images.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       53 2020-08-23 18:37:13.000000 datasette-render-images-0.3.2/datasette_render_images.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       25 2020-08-23 18:37:13.000000 datasette-render-images-0.3.2/datasette_render_images.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       24 2020-08-23 18:37:13.000000 datasette-render-images-0.3.2/datasette_render_images.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      887 2020-08-23 18:37:06.000000 datasette-render-images-0.3.2/datasette_render_images.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-23 18:37:13.747914 datasette-render-images-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      875 2020-08-23 18:37:06.000000 datasette-render-images-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:37:00.632800 datasette-render-images-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-14 21:37:00.632800 datasette-render-images-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-14 21:36:46.000000 datasette-render-images-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:37:00.632800 datasette-render-images-0.4/datasette_render_images.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-14 21:37:00.000000 datasette-render-images-0.4/datasette_render_images.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-14 21:37:00.000000 datasette-render-images-0.4/datasette_render_images.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:37:00.000000 datasette-render-images-0.4/datasette_render_images.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 21:37:00.000000 datasette-render-images-0.4/datasette_render_images.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 21:37:00.000000 datasette-render-images-0.4/datasette_render_images.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-14 21:37:00.000000 datasette-render-images-0.4/datasette_render_images.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-14 21:36:46.000000 datasette-render-images-0.4/datasette_render_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:37:00.632800 datasette-render-images-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-14 21:36:46.000000 datasette-render-images-0.4/setup.py
```

### Comparing `datasette-render-images-0.3.2/PKG-INFO` & `datasette-render-images-0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 Metadata-Version: 2.1
 Name: datasette-render-images
-Version: 0.3.2
+Version: 0.4
 Summary: Datasette plugin that renders binary blob images using data-uris
 Home-page: https://github.com/simonw/datasette-render-images
 Author: Simon Willison
 License: Apache License, Version 2.0
-Description: # datasette-render-images
-        
-        [![PyPI](https://img.shields.io/pypi/v/datasette-render-images.svg)](https://pypi.org/project/datasette-render-images/)
-        [![Changelog](https://img.shields.io/github/v/release/simonw/datasette-render-images?include_prereleases&label=changelog)](https://github.com/simonw/datasette-render-images/releases)
-        [![Tests](https://github.com/simonw/datasette-render-images/workflows/Test/badge.svg)](https://github.com/simonw/datasette-render-images/actions?query=workflow%3ATest)
-        [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/datasette-render-images/blob/main/LICENSE)
-        
-        A Datasette plugin that renders binary blob images with data-uris, using the [render_cell() plugin hook](https://datasette.readthedocs.io/en/stable/plugins.html#render-cell-value-column-table-database-datasette).
-        
-        ## Installation
-        
-        Install this plugin in the same environment as Datasette.
-        
-            $ pip install datasette-render-images
-        
-        ## Usage
-        
-        If a database row contains binary image data (PNG, GIF or JPEG), this plugin will detect that it is an image (using the [imghdr module](https://docs.python.org/3/library/imghdr.html) and render that cell using an `<img src="data:image/png;base64,...">` element.
-        
-        Here's a [demo of the plugin in action](https://datasette-render-images-demo.datasette.io/favicons/favicons).
-        
-        ## Creating a compatible database table
-        
-        You can use the [sqlite-utils insert-files](https://sqlite-utils.readthedocs.io/en/stable/cli.html#inserting-binary-data-from-files) command to insert image files into a database table:
-        
-            $ pip install sqlite-utils
-            $ sqlite-utils insert-files gifs.db images *.gif
-        
-        See [Fun with binary data and SQLite](https://simonwillison.net/2020/Jul/30/fun-binary-data-and-sqlite/) for more on this tool.
-        
-        ## Configuration
-        
-        By default the plugin will only render images that are smaller than 100KB. You can adjust this limit using the `size_limit` plugin configuration option - for example, to increase the limit to 1MB (1000000 bytes) use the following in `metadata.json`:
-        
-        ```json
-        {
-            "plugins": {
-                "datasette-render-images": {
-                    "size_limit": 1000000
-                }
-            }
-        }
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
+
+# datasette-render-images
+
+[![PyPI](https://img.shields.io/pypi/v/datasette-render-images.svg)](https://pypi.org/project/datasette-render-images/)
+[![Changelog](https://img.shields.io/github/v/release/simonw/datasette-render-images?include_prereleases&label=changelog)](https://github.com/simonw/datasette-render-images/releases)
+[![Tests](https://github.com/simonw/datasette-render-images/workflows/Test/badge.svg)](https://github.com/simonw/datasette-render-images/actions?query=workflow%3ATest)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/datasette-render-images/blob/main/LICENSE)
+
+A Datasette plugin that renders binary blob images with data-uris, using the [render_cell() plugin hook](https://docs.datasette.io/en/stable/plugins.html#render-cell-value-column-table-database-datasette).
+
+## Installation
+
+Install this plugin in the same environment as Datasette.
+
+    $ pip install datasette-render-images
+
+## Usage
+
+If a database row contains binary image data (PNG, GIF or JPEG), this plugin will detect that it is an image (using the [imghdr module](https://docs.python.org/3/library/imghdr.html) and render that cell using an `<img src="data:image/png;base64,...">` element.
+
+Here's a [demo of the plugin in action](https://datasette-render-images-demo.datasette.io/favicons/favicons).
+
+## Creating a compatible database table
+
+You can use the [sqlite-utils insert-files](https://sqlite-utils.datasette.io/en/stable/cli.html#inserting-data-from-files) command to insert image files into a database table:
+
+    $ pip install sqlite-utils
+    $ sqlite-utils insert-files gifs.db images *.gif
+
+See [Fun with binary data and SQLite](https://simonwillison.net/2020/Jul/30/fun-binary-data-and-sqlite/) for more on this tool.
+
+## Configuration
+
+By default the plugin will only render images that are smaller than 100KB. You can adjust this limit using the `size_limit` plugin configuration option - for example, to increase the limit to 1MB (1000000 bytes) use the following in `metadata.json`:
+
+```json
+{
+    "plugins": {
+        "datasette-render-images": {
+            "size_limit": 1000000
+        }
+    }
+}
+```
```

### Comparing `datasette-render-images-0.3.2/README.md` & `datasette-render-images-0.4/datasette_render_images.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+Metadata-Version: 2.1
+Name: datasette-render-images
+Version: 0.4
+Summary: Datasette plugin that renders binary blob images using data-uris
+Home-page: https://github.com/simonw/datasette-render-images
+Author: Simon Willison
+License: Apache License, Version 2.0
+Description-Content-Type: text/markdown
+Provides-Extra: test
+
 # datasette-render-images
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-render-images.svg)](https://pypi.org/project/datasette-render-images/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/datasette-render-images?include_prereleases&label=changelog)](https://github.com/simonw/datasette-render-images/releases)
 [![Tests](https://github.com/simonw/datasette-render-images/workflows/Test/badge.svg)](https://github.com/simonw/datasette-render-images/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/datasette-render-images/blob/main/LICENSE)
 
-A Datasette plugin that renders binary blob images with data-uris, using the [render_cell() plugin hook](https://datasette.readthedocs.io/en/stable/plugins.html#render-cell-value-column-table-database-datasette).
+A Datasette plugin that renders binary blob images with data-uris, using the [render_cell() plugin hook](https://docs.datasette.io/en/stable/plugins.html#render-cell-value-column-table-database-datasette).
 
 ## Installation
 
 Install this plugin in the same environment as Datasette.
 
     $ pip install datasette-render-images
 
@@ -17,15 +27,15 @@
 
 If a database row contains binary image data (PNG, GIF or JPEG), this plugin will detect that it is an image (using the [imghdr module](https://docs.python.org/3/library/imghdr.html) and render that cell using an `<img src="data:image/png;base64,...">` element.
 
 Here's a [demo of the plugin in action](https://datasette-render-images-demo.datasette.io/favicons/favicons).
 
 ## Creating a compatible database table
 
-You can use the [sqlite-utils insert-files](https://sqlite-utils.readthedocs.io/en/stable/cli.html#inserting-binary-data-from-files) command to insert image files into a database table:
+You can use the [sqlite-utils insert-files](https://sqlite-utils.datasette.io/en/stable/cli.html#inserting-data-from-files) command to insert image files into a database table:
 
     $ pip install sqlite-utils
     $ sqlite-utils insert-files gifs.db images *.gif
 
 See [Fun with binary data and SQLite](https://simonwillison.net/2020/Jul/30/fun-binary-data-and-sqlite/) for more on this tool.
 
 ## Configuration
```

### Comparing `datasette-render-images-0.3.2/datasette_render_images.egg-info/PKG-INFO` & `datasette-render-images-0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,43 @@
-Metadata-Version: 2.1
-Name: datasette-render-images
-Version: 0.3.2
-Summary: Datasette plugin that renders binary blob images using data-uris
-Home-page: https://github.com/simonw/datasette-render-images
-Author: Simon Willison
-License: Apache License, Version 2.0
-Description: # datasette-render-images
-        
-        [![PyPI](https://img.shields.io/pypi/v/datasette-render-images.svg)](https://pypi.org/project/datasette-render-images/)
-        [![Changelog](https://img.shields.io/github/v/release/simonw/datasette-render-images?include_prereleases&label=changelog)](https://github.com/simonw/datasette-render-images/releases)
-        [![Tests](https://github.com/simonw/datasette-render-images/workflows/Test/badge.svg)](https://github.com/simonw/datasette-render-images/actions?query=workflow%3ATest)
-        [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/datasette-render-images/blob/main/LICENSE)
-        
-        A Datasette plugin that renders binary blob images with data-uris, using the [render_cell() plugin hook](https://datasette.readthedocs.io/en/stable/plugins.html#render-cell-value-column-table-database-datasette).
-        
-        ## Installation
-        
-        Install this plugin in the same environment as Datasette.
-        
-            $ pip install datasette-render-images
-        
-        ## Usage
-        
-        If a database row contains binary image data (PNG, GIF or JPEG), this plugin will detect that it is an image (using the [imghdr module](https://docs.python.org/3/library/imghdr.html) and render that cell using an `<img src="data:image/png;base64,...">` element.
-        
-        Here's a [demo of the plugin in action](https://datasette-render-images-demo.datasette.io/favicons/favicons).
-        
-        ## Creating a compatible database table
-        
-        You can use the [sqlite-utils insert-files](https://sqlite-utils.readthedocs.io/en/stable/cli.html#inserting-binary-data-from-files) command to insert image files into a database table:
-        
-            $ pip install sqlite-utils
-            $ sqlite-utils insert-files gifs.db images *.gif
-        
-        See [Fun with binary data and SQLite](https://simonwillison.net/2020/Jul/30/fun-binary-data-and-sqlite/) for more on this tool.
-        
-        ## Configuration
-        
-        By default the plugin will only render images that are smaller than 100KB. You can adjust this limit using the `size_limit` plugin configuration option - for example, to increase the limit to 1MB (1000000 bytes) use the following in `metadata.json`:
-        
-        ```json
-        {
-            "plugins": {
-                "datasette-render-images": {
-                    "size_limit": 1000000
-                }
-            }
+# datasette-render-images
+
+[![PyPI](https://img.shields.io/pypi/v/datasette-render-images.svg)](https://pypi.org/project/datasette-render-images/)
+[![Changelog](https://img.shields.io/github/v/release/simonw/datasette-render-images?include_prereleases&label=changelog)](https://github.com/simonw/datasette-render-images/releases)
+[![Tests](https://github.com/simonw/datasette-render-images/workflows/Test/badge.svg)](https://github.com/simonw/datasette-render-images/actions?query=workflow%3ATest)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/datasette-render-images/blob/main/LICENSE)
+
+A Datasette plugin that renders binary blob images with data-uris, using the [render_cell() plugin hook](https://docs.datasette.io/en/stable/plugins.html#render-cell-value-column-table-database-datasette).
+
+## Installation
+
+Install this plugin in the same environment as Datasette.
+
+    $ pip install datasette-render-images
+
+## Usage
+
+If a database row contains binary image data (PNG, GIF or JPEG), this plugin will detect that it is an image (using the [imghdr module](https://docs.python.org/3/library/imghdr.html) and render that cell using an `<img src="data:image/png;base64,...">` element.
+
+Here's a [demo of the plugin in action](https://datasette-render-images-demo.datasette.io/favicons/favicons).
+
+## Creating a compatible database table
+
+You can use the [sqlite-utils insert-files](https://sqlite-utils.datasette.io/en/stable/cli.html#inserting-data-from-files) command to insert image files into a database table:
+
+    $ pip install sqlite-utils
+    $ sqlite-utils insert-files gifs.db images *.gif
+
+See [Fun with binary data and SQLite](https://simonwillison.net/2020/Jul/30/fun-binary-data-and-sqlite/) for more on this tool.
+
+## Configuration
+
+By default the plugin will only render images that are smaller than 100KB. You can adjust this limit using the `size_limit` plugin configuration option - for example, to increase the limit to 1MB (1000000 bytes) use the following in `metadata.json`:
+
+```json
+{
+    "plugins": {
+        "datasette-render-images": {
+            "size_limit": 1000000
         }
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: test
+    }
+}
+```
```

### Comparing `datasette-render-images-0.3.2/setup.py` & `datasette-render-images-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3.2"
+VERSION = "0.4"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

