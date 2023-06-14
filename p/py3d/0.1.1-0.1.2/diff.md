# Comparing `tmp/py3d-0.1.1.tar.gz` & `tmp/py3d-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.1.1.tar", last modified: Sun Jun 11 15:16:41 2023, max compression
+gzip compressed data, was "py3d-0.1.2.tar", last modified: Wed Jun 14 01:21:24 2023, max compression
```

## Comparing `py3d-0.1.1.tar` & `py3d-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 15:16:41.660717 py3d-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-11 15:16:41.660717 py3d-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-11 15:16:21.000000 py3d-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 15:16:41.660717 py3d-0.1.1/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-11 15:15:38.000000 py3d-0.1.1/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28565 2023-06-11 15:15:38.000000 py3d-0.1.1/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-06-11 15:15:38.000000 py3d-0.1.1/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 15:16:41.660717 py3d-0.1.1/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-11 15:16:41.000000 py3d-0.1.1/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-11 15:16:41.000000 py3d-0.1.1/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-11 15:16:41.000000 py3d-0.1.1/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-11 15:16:41.000000 py3d-0.1.1/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-11 15:16:41.000000 py3d-0.1.1/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-11 15:16:41.660717 py3d-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-11 15:15:38.000000 py3d-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 01:21:24.702869 py3d-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-14 01:21:24.702869 py3d-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-14 01:21:03.000000 py3d-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 01:21:24.698869 py3d-0.1.2/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-14 01:20:17.000000 py3d-0.1.2/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28565 2023-06-14 01:20:17.000000 py3d-0.1.2/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22729 2023-06-14 01:20:17.000000 py3d-0.1.2/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 01:21:24.702869 py3d-0.1.2/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-14 01:21:24.000000 py3d-0.1.2/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-14 01:21:24.000000 py3d-0.1.2/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 01:21:24.000000 py3d-0.1.2/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-14 01:21:24.000000 py3d-0.1.2/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-14 01:21:24.000000 py3d-0.1.2/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 01:21:24.702869 py3d-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-14 01:20:17.000000 py3d-0.1.2/setup.py
```

### Comparing `py3d-0.1.1/PKG-INFO` & `py3d-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.1
+Version: 0.1.2
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.1/README.md` & `py3d-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.1.1/py3d/core.py` & `py3d-0.1.2/py3d/core.py`

 * *Files identical despite different names*

### Comparing `py3d-0.1.1/py3d/viewer.html` & `py3d-0.1.2/py3d/viewer.html`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,16 @@
                     }
                 }
                 this.canvas_x = ev.clientX
                 this.canvas_y = ev.clientY
             }
             this.canvas.onwheel = (ev) => {
                 ev.preventDefault()
-                this.camera.translation[2] = Math.max(0, this.camera.translation[2] - ev.deltaY / 100)
+                let step = ev.deltaY * 10 ** (Math.round(Math.log10(this.camera.translation[2])) - 3)
+                this.camera.translation[2] = Math.max(0, this.camera.translation[2] - step)
                 this.toolbar.tooltip.innerHTML = this.camera.position()
                 this.camera.update_projection()
                 this.render()
             }
             this.toolbar.btn_orth.onclick = (ev) => {
                 this.toolbar.btn_orth.innerHTML = this.toolbar.btn_orth.innerHTML == this.camera.ORTHOGRAPHIC ? this.camera.PERSPECTIVE : this.camera.ORTHOGRAPHIC
                 this.camera.type = this.toolbar.btn_orth.innerHTML
```

### Comparing `py3d-0.1.1/py3d.egg-info/PKG-INFO` & `py3d-0.1.2/py3d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.1
+Version: 0.1.2
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.1/setup.py` & `py3d-0.1.2/setup.py`

 * *Files identical despite different names*

