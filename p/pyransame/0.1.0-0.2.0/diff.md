# Comparing `tmp/pyransame-0.1.0.tar.gz` & `tmp/pyransame-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyransame-0.1.0.tar", last modified: Thu May 25 12:03:39 2023, max compression
+gzip compressed data, was "pyransame-0.2.0.tar", last modified: Wed Jun 14 20:27:25 2023, max compression
```

## Comparing `pyransame-0.1.0.tar` & `pyransame-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.397144 pyransame-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 12:03:28.000000 pyransame-0.1.0/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-05-25 12:03:28.000000 pyransame-0.1.0/.devcontainer/oncreatecommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-25 12:03:28.000000 pyransame-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-25 12:03:28.000000 pyransame-0.1.0/.github/workflows/pages_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-25 12:03:28.000000 pyransame-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-25 12:03:28.000000 pyransame-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-25 12:03:28.000000 pyransame-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-25 12:03:28.000000 pyransame-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 12:03:28.000000 pyransame-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 12:03:39.393144 pyransame-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-25 12:03:28.000000 pyransame-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   146735 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/_static/surface_sampling.png
--rw-r--r--   0 runner    (1001) docker     (123)   183927 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/_static/volume_sampling.png
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 12:03:28.000000 pyransame-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 12:03:28.000000 pyransame-0.1.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 12:03:28.000000 pyransame-0.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:03:39.397144 pyransame-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.389144 pyransame-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/src/pyransame/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-25 12:03:28.000000 pyransame-0.1.0/src/pyransame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:28.000000 pyransame-0.1.0/src/pyransame/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-25 12:03:28.000000 pyransame-0.1.0/src/pyransame/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-25 12:03:28.000000 pyransame-0.1.0/src/pyransame/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-25 12:03:28.000000 pyransame-0.1.0/src/pyransame/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/src/pyransame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 12:03:28.000000 pyransame-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-25 12:03:28.000000 pyransame-0.1.0/tests/test_random_surface_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-25 12:03:28.000000 pyransame-0.1.0/tests/test_random_volume_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-25 12:03:28.000000 pyransame-0.1.0/tests/test_rng.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-25 12:03:28.000000 pyransame-0.1.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:25.155938 pyransame-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:25.143938 pyransame-0.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-14 20:27:09.000000 pyransame-0.2.0/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-06-14 20:27:09.000000 pyransame-0.2.0/.devcontainer/oncreatecommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:25.143938 pyransame-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-14 20:27:09.000000 pyransame-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:25.143938 pyransame-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-14 20:27:09.000000 pyransame-0.2.0/.github/workflows/build_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-14 20:27:09.000000 pyransame-0.2.0/.github/workflows/pages_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-14 20:27:09.000000 pyransame-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-14 20:27:09.000000 pyransame-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-14 20:27:09.000000 pyransame-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-14 20:27:09.000000 pyransame-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-14 20:27:09.000000 pyransame-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-14 20:27:25.155938 pyransame-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-14 20:27:09.000000 pyransame-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:25.147938 pyransame-0.2.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-14 20:27:09.000000 pyransame-0.2.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:25.147938 pyransame-0.2.0/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   146735 2023-06-14 20:27:09.000000 pyransame-0.2.0/doc/_static/surface_sampling.png
+-rw-r--r--   0 runner    (1001) docker     (123)   183927 2023-06-14 20:27:09.000000 pyransame-0.2.0/doc/_static/volume_sampling.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-14 20:27:09.000000 pyransame-0.2.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-14 20:27:09.000000 pyransame-0.2.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-14 20:27:09.000000 pyransame-0.2.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-14 20:27:09.000000 pyransame-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 20:27:09.000000 pyransame-0.2.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 20:27:09.000000 pyransame-0.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 20:27:25.155938 pyransame-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:25.139937 pyransame-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:25.151938 pyransame-0.2.0/src/pyransame/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 20:27:09.000000 pyransame-0.2.0/src/pyransame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 20:27:25.000000 pyransame-0.2.0/src/pyransame/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:09.000000 pyransame-0.2.0/src/pyransame/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-14 20:27:09.000000 pyransame-0.2.0/src/pyransame/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-06-14 20:27:09.000000 pyransame-0.2.0/src/pyransame/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-14 20:27:09.000000 pyransame-0.2.0/src/pyransame/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:25.151938 pyransame-0.2.0/src/pyransame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-14 20:27:25.000000 pyransame-0.2.0/src/pyransame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-14 20:27:25.000000 pyransame-0.2.0/src/pyransame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:27:25.000000 pyransame-0.2.0/src/pyransame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 20:27:25.000000 pyransame-0.2.0/src/pyransame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 20:27:25.000000 pyransame-0.2.0/src/pyransame.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:27:25.155938 pyransame-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 20:27:09.000000 pyransame-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-14 20:27:09.000000 pyransame-0.2.0/tests/test_random_surface_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-14 20:27:09.000000 pyransame-0.2.0/tests/test_random_volume_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-14 20:27:09.000000 pyransame-0.2.0/tests/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-06-14 20:27:09.000000 pyransame-0.2.0/tests/test_util.py
```

### Comparing `pyransame-0.1.0/.github/workflows/pages_publish.yml` & `pyransame-0.2.0/.github/workflows/pages_publish.yml`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/.github/workflows/python-publish.yml` & `pyransame-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/.github/workflows/test.yml` & `pyransame-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/.gitignore` & `pyransame-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/LICENSE` & `pyransame-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/PKG-INFO` & `pyransame-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyransame
-Version: 0.1.0
+Version: 0.2.0
 Summary: PYthon RAndom SAmpling for MEshes
 Author-email: Matthew Flamm <matthewhflamm0@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/MatthewFlamm/pyransame
 Project-URL: Bug Tracker, https://github.com/MatthewFlamm/pyransame/issues
 Project-URL: Documentation, https://matthewflamm.github.io/pyransame/
 Keywords: pyvista,vtk,numpy,mesh,sample
```

### Comparing `pyransame-0.1.0/README.md` & `pyransame-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/doc/Makefile` & `pyransame-0.2.0/doc/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
-SPHINXOPTS    ?=
+SPHINXOPTS    ?= -W
 SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = .
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `pyransame-0.1.0/doc/_static/surface_sampling.png` & `pyransame-0.2.0/doc/_static/surface_sampling.png`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/doc/_static/volume_sampling.png` & `pyransame-0.2.0/doc/_static/volume_sampling.png`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/doc/index.rst` & `pyransame-0.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/doc/make.bat` & `pyransame-0.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/pyproject.toml` & `pyransame-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/src/pyransame/surface.py` & `pyransame-0.2.0/src/pyransame/surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 
 def random_surface_points(
     mesh: pv.DataSet,
     n: int = 1,
     weights: Optional[Union[str, npt.ArrayLike]] = None,
 ) -> np.ndarray:
-    """Generate random points on surface.
+    """
+    Generate random points on surface.
 
     Supported cell types:
 
     - Triangle
     - Triangle Strip
     - Pixel
     - Polygon
@@ -29,15 +30,15 @@
 
     Parameters
     ----------
     mesh : pyvista.DataSet
         The mesh for which to generate random points.  Must have cells.
 
     n : int, default: 1
-        Number of random points to generate
+        Number of random points to generate.
 
     weights : str, or array_like, optional
         Weights to use for probability of choosing points inside each cell.
 
         If a ``str`` is supplied, it will use the existing cell data on ``mesh``.
 
     Returns
@@ -57,16 +58,16 @@
 
     >>> cpos = [
     ...     (-0.07, 0.2, 0.5),
     ...     (-0.02, 0.1, -0.0),
     ...     (0.04, 1.0, -0.2),
     ... ]
     >>> pl = pv.Plotter()
-    >>> pl.add_mesh(mesh, color='tan')
-    >>> pl.add_points(points, render_points_as_spheres=True, point_size=10.0, color='red')
+    >>> _ = pl.add_mesh(mesh, color='tan')
+    >>> _ = pl.add_points(points, render_points_as_spheres=True, point_size=10.0, color='red')
     >>> pl.show(cpos=cpos)
     """
     if weights is None:
         weights = np.ones(mesh.n_cells)
 
     if isinstance(weights, str):
         weights = mesh.cell_data[weights]
```

### Comparing `pyransame-0.1.0/src/pyransame/volume.py` & `pyransame-0.2.0/src/pyransame/volume.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,31 +12,37 @@
 
 
 def random_volume_points(
     mesh: pv.DataSet,
     n: int = 1,
     weights: Optional[Union[str, npt.ArrayLike]] = None,
 ) -> np.ndarray:
-    """Generate random points in a volume.
+    """
+    Generate random points in a volume.
 
     Supported cell types:
 
+    - Hexagonal Prism
+    - Hexahedron
+    - Pentagonal Prism
+    - Polyhedron
     - Pyramid
     - Tetrahedron
     - Voxel
+    - Wedge
 
     All cells must be convex.
 
     Parameters
     ----------
     mesh : pyvista.DataSet
         The mesh for which to generate random points.  Must have cells.
 
     n : int, default: 1
-        Number of random points to generate
+        Number of random points to generate.
 
     weights : str, or array_like, optional
         Weights to use for probability of choosing points inside each cell.
 
         If a ``str`` is supplied, it will use the existing cell data on ``mesh``.
 
     Returns
@@ -50,17 +56,17 @@
     >>> import pyvista as pv
     >>> mesh = pv.UniformGrid(dimensions=(11, 11, 11))
     >>> points = pyransame.random_volume_points(mesh, n=500)
 
     Now plot result.
 
     >>> pl = pv.Plotter()
-    >>> pl.add_mesh(mesh, style='wireframe')
-    >>> pl.add_points(points, render_points_as_spheres=True, point_size=10.0, color='red')
-    >>> pl.show(cpos=cpos)
+    >>> _ = pl.add_mesh(mesh, style='wireframe')
+    >>> _ = pl.add_points(points, render_points_as_spheres=True, point_size=10.0, color='red')
+    >>> pl.show()
     """
     if weights is None:
         weights = np.ones(mesh.n_cells)
 
     if isinstance(weights, str):
         weights = mesh.cell_data[weights]
 
@@ -95,13 +101,32 @@
             points[
                 point_indices[i] : point_indices[i + 1], :
             ] = util._generate_points_in_voxel(c.points, count)
         elif c.type == CellType.PYRAMID:
             points[
                 point_indices[i] : point_indices[i + 1], :
             ] = util._generate_points_in_pyramid(c.points, count)
+        elif c.type == CellType.WEDGE:
+            points[
+                point_indices[i] : point_indices[i + 1], :
+            ] = util._generate_points_in_wedge(c.points, count)
+        elif c.type == CellType.HEXAHEDRON:
+            points[
+                point_indices[i] : point_indices[i + 1], :
+            ] = util._generate_points_in_hexahedron(c.points, count)
+        elif c.type == CellType.PENTAGONAL_PRISM:
+            points[
+                point_indices[i] : point_indices[i + 1], :
+            ] = util._generate_points_in_pentagonal_prism(c.points, count)
+        elif c.type == CellType.HEXAGONAL_PRISM:
+            points[
+                point_indices[i] : point_indices[i + 1], :
+            ] = util._generate_points_in_hexagonal_prism(c.points, count)
+        elif c.type == CellType.POLYHEDRON:
+            points[
+                point_indices[i] : point_indices[i + 1], :
+            ] = util._generate_points_in_polyhedron(c, count)
         else:
             raise NotImplementedError(
                 f"Random generation for {c.type.name} not yet supported"
             )
-
     return points
```

### Comparing `pyransame-0.1.0/src/pyransame.egg-info/PKG-INFO` & `pyransame-0.2.0/src/pyransame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyransame
-Version: 0.1.0
+Version: 0.2.0
 Summary: PYthon RAndom SAmpling for MEshes
 Author-email: Matthew Flamm <matthewhflamm0@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/MatthewFlamm/pyransame
 Project-URL: Bug Tracker, https://github.com/MatthewFlamm/pyransame/issues
 Project-URL: Documentation, https://matthewflamm.github.io/pyransame/
 Keywords: pyvista,vtk,numpy,mesh,sample
```

### Comparing `pyransame-0.1.0/src/pyransame.egg-info/SOURCES.txt` & `pyransame-0.2.0/src/pyransame.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.md
 pyproject.toml
 requirements-doc.txt
 requirements-test.txt
 .devcontainer/devcontainer.json
 .devcontainer/oncreatecommand.sh
 .github/dependabot.yml
+.github/workflows/build_docs.yml
 .github/workflows/pages_publish.yml
 .github/workflows/python-publish.yml
 .github/workflows/test.yml
 doc/Makefile
 doc/conf.py
 doc/index.rst
 doc/make.bat
```

### Comparing `pyransame-0.1.0/tests/test_random_surface_points.py` & `pyransame-0.2.0/tests/test_random_surface_points.py`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/tests/test_rng.py` & `pyransame-0.2.0/tests/test_rng.py`

 * *Files identical despite different names*

### Comparing `pyransame-0.1.0/tests/test_util.py` & `pyransame-0.2.0/tests/test_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,30 @@
 
 import numpy as np
 import pytest
 import pyvista as pv
 from hypothesis import assume, given, settings
 from hypothesis import strategies as st
 from hypothesis.extra.numpy import arrays
+from vtk import VTK_POLYHEDRON, vtkIdList, vtkPoints, vtkUnstructuredGrid
 
 from pyransame.util import (
+    _generate_points_in_hexagonal_prism,
+    _generate_points_in_hexahedron,
+    _generate_points_in_pentagonal_prism,
     _generate_points_in_pixel,
     _generate_points_in_polygon,
+    _generate_points_in_polyhedron,
     _generate_points_in_pyramid,
     _generate_points_in_quad,
     _generate_points_in_tetra,
     _generate_points_in_tri,
     _generate_points_in_tri_strip,
     _generate_points_in_voxel,
+    _generate_points_in_wedge,
 )
 
 
 @settings(deadline=timedelta(milliseconds=500))
 # Use min_value and max_value to avoid numerical imprecision artifacts, but still span a large space
 @given(
     arrays(float, 3, elements=st.floats(min_value=-1000.0, max_value=1000.0)),
@@ -227,7 +233,98 @@
     )
 
     center = np.array([0.0, 0.0, 0.25])
 
     points = _generate_points_in_pyramid(mesh.points, 2000000)
 
     assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
+
+
+def test_uniformity_wedge():
+    a = np.array((0.0, 0.0, 0.0))
+    b = np.array((1.0, 0.0, 0.0))
+    c = np.array((0.5, np.sqrt(3.0) / 2.0, 0.0))
+    d = np.array((0.0, 0.0, 1.0))
+    e = np.array((1.0, 0.0, 1.0))
+    f = np.array((0.5, np.sqrt(3.0) / 2.0, 1.0))
+
+    center = np.array((0.5, np.sqrt(3.0) / 6.0, 0.5))
+
+    # needs a lot of points to converge
+    points = _generate_points_in_wedge(np.array([a, b, c, d, e, f]), 2000000)
+
+    assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
+
+
+def test_uniformity_hexahedra():
+    p = np.array(
+        [
+            [0.0, 0.0, 0.0],
+            [1.0, 0.0, 0.0],
+            [1.0, 0.0, 1.0],
+            [0.0, 0.0, 1.0],
+            [0.0, 1.0, 0.0],
+            [1.0, 1.0, 0.0],
+            [1.0, 1.0, 1.0],
+            [0.0, 1.0, 1.0],
+        ]
+    )
+
+    center = np.array([0.5, 0.5, 0.5])
+
+    points = _generate_points_in_hexahedron(p, 2000000)
+    assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
+
+
+def test_uniformity_pentagonal_prism():
+    angles = np.arange(5) * 2 * np.pi / 5  # angles of regular pentagon in radians
+    p = np.zeros(shape=(10, 3))
+    np.sin(angles, out=p[0:5, 0])
+    np.cos(angles, out=p[0:5, 1])
+
+    np.sin(angles, out=p[5:, 0])
+    np.cos(angles, out=p[5:, 1])
+    p[5:, 2] = 1.0
+
+    center = np.array([0.0, 0.0, 0.5])
+    points = _generate_points_in_pentagonal_prism(p, 2000000)
+    assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
+
+
+def test_uniformity_hexagonal_prism():
+    angles = np.arange(6) * 2 * np.pi / 6  # angles of regular hexagon in radians
+    p = np.zeros(shape=(12, 3))
+    np.sin(angles, out=p[0:6, 0])
+    np.cos(angles, out=p[0:6, 1])
+
+    np.sin(angles, out=p[6:, 0])
+    np.cos(angles, out=p[6:, 1])
+    p[6:, 2] = 1.0
+
+    center = np.array([0.0, 0.0, 0.5])
+    points = _generate_points_in_hexagonal_prism(p, 2000000)
+    assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
+
+
+def test_uniformity_polyhedron():
+    dodecahedron_poly = pv.Dodecahedron()
+
+    faces = []
+    for cell in dodecahedron_poly.cell:
+        faces.append(cell.point_ids)
+
+    faces = []
+    faces.append(dodecahedron_poly.n_cells)
+    for cell in dodecahedron_poly.cell:
+        point_ids = cell.point_ids
+        faces.append(len(point_ids))
+        [faces.append(id) for id in point_ids]
+
+    faces.insert(0, len(faces))
+
+    mesh = pv.UnstructuredGrid(
+        faces, [pv.CellType.POLYHEDRON], dodecahedron_poly.points
+    )
+
+    points = _generate_points_in_polyhedron(mesh.get_cell(0), 2000000)
+
+    assert np.allclose(points.mean(axis=0), np.array(mesh.center), rtol=1e-3, atol=1e-3)
```

