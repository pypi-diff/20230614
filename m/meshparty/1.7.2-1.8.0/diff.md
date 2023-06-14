# Comparing `tmp/meshparty-1.7.2.tar.gz` & `tmp/meshparty-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meshparty-1.7.2.tar", last modified: Fri Oct 18 02:32:56 2019, max compression
+gzip compressed data, was "dist/meshparty-1.8.0.tar", last modified: Tue Dec  3 23:22:22 2019, max compression
```

## Comparing `meshparty-1.7.2.tar` & `meshparty-1.8.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 forrestc (1223548560) 1457291929        0 2019-10-18 02:32:56.000000 meshparty-1.7.2/
--rw-r--r--   0 forrestc (1223548560) 1457291929       67 2019-10-14 20:44:32.000000 meshparty-1.7.2/test_requirements.txt
--rw-r--r--   0 forrestc (1223548560) 1457291929      260 2019-10-18 02:32:56.000000 meshparty-1.7.2/PKG-INFO
-drwxr-xr-x   0 forrestc (1223548560) 1457291929        0 2019-10-18 02:32:56.000000 meshparty-1.7.2/meshlabscripts/
--rw-r--r--   0 forrestc (1223548560) 1457291929      210 2018-11-13 00:22:21.000000 meshparty-1.7.2/meshlabscripts/mergeclosevertices.mlb
--rw-r--r--   0 forrestc (1223548560) 1457291929    11357 2019-03-18 20:54:12.000000 meshparty-1.7.2/LICENSE
--rw-r--r--   0 forrestc (1223548560) 1457291929      151 2019-10-18 02:32:28.000000 meshparty-1.7.2/requirements.txt
--rw-r--r--   0 forrestc (1223548560) 1457291929      145 2019-09-26 00:06:12.000000 meshparty-1.7.2/environment.yml
--rw-r--r--   0 forrestc (1223548560) 1457291929      106 2019-10-18 02:32:40.000000 meshparty-1.7.2/.bumpversion.cfg
--rw-r--r--   0 forrestc (1223548560) 1457291929      134 2019-09-26 00:06:12.000000 meshparty-1.7.2/MANIFEST.in
--rw-r--r--   0 forrestc (1223548560) 1457291929      420 2019-03-31 15:04:01.000000 meshparty-1.7.2/.coveragerc
-drwxr-xr-x   0 forrestc (1223548560) 1457291929        0 2019-10-18 02:32:56.000000 meshparty-1.7.2/docs/
-drwxr-xr-x   0 forrestc (1223548560) 1457291929        0 2019-10-18 02:32:56.000000 meshparty-1.7.2/docs/guide/
--rw-r--r--   0 forrestc (1223548560) 1457291929     1838 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/guide/filtering.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929     8468 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/guide/skeletons.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929     1694 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/guide/loading.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929     1660 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/guide/repair.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929     3404 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/guide/analysis.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929     4100 2019-10-14 20:44:32.000000 meshparty-1.7.2/docs/guide/visualization.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929      649 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/index.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929       40 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/includeme.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929      634 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/Makefile
--rw-r--r--   0 forrestc (1223548560) 1457291929     2386 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/conf.py
-drwxr-xr-x   0 forrestc (1223548560) 1457291929        0 2019-10-18 02:32:56.000000 meshparty-1.7.2/docs/source/
--rw-r--r--   0 forrestc (1223548560) 1457291929     2144 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/source/meshparty.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929       64 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/source/modules.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929      795 2019-09-26 00:06:12.000000 meshparty-1.7.2/docs/make.bat
--rw-r--r--   0 forrestc (1223548560) 1457291929      645 2019-09-26 00:06:12.000000 meshparty-1.7.2/.readthedocs.yml
--rw-r--r--   0 forrestc (1223548560) 1457291929     1725 2019-09-24 23:28:20.000000 meshparty-1.7.2/setup.py
--rw-r--r--   0 forrestc (1223548560) 1457291929      972 2019-01-24 02:33:09.000000 meshparty-1.7.2/example.py
--rw-r--r--   0 forrestc (1223548560) 1457291929      166 2019-10-14 20:44:32.000000 meshparty-1.7.2/.gitignore
--rw-r--r--   0 forrestc (1223548560) 1457291929       59 2019-10-18 02:32:56.000000 meshparty-1.7.2/setup.cfg
-drwxr-xr-x   0 forrestc (1223548560) 1457291929        0 2019-10-18 02:32:56.000000 meshparty-1.7.2/meshparty.egg-info/
--rw-r--r--   0 forrestc (1223548560) 1457291929      260 2019-10-18 02:32:55.000000 meshparty-1.7.2/meshparty.egg-info/PKG-INFO
--rw-r--r--   0 forrestc (1223548560) 1457291929      977 2019-10-18 02:32:56.000000 meshparty-1.7.2/meshparty.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc (1223548560) 1457291929      210 2019-10-18 02:32:55.000000 meshparty-1.7.2/meshparty.egg-info/requires.txt
--rw-r--r--   0 forrestc (1223548560) 1457291929       10 2019-10-18 02:32:55.000000 meshparty-1.7.2/meshparty.egg-info/top_level.txt
--rw-r--r--   0 forrestc (1223548560) 1457291929        1 2019-10-18 02:32:55.000000 meshparty-1.7.2/meshparty.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc (1223548560) 1457291929     2151 2019-09-26 00:06:12.000000 meshparty-1.7.2/README.rst
--rw-r--r--   0 forrestc (1223548560) 1457291929       41 2019-09-24 23:28:20.000000 meshparty-1.7.2/optional_requirements.txt
--rw-r--r--   0 forrestc (1223548560) 1457291929       62 2018-12-19 20:11:13.000000 meshparty-1.7.2/.pypirc
--rw-r--r--   0 forrestc (1223548560) 1457291929     1182 2019-09-26 00:06:12.000000 meshparty-1.7.2/.travis.yml
-drwxr-xr-x   0 forrestc (1223548560) 1457291929        0 2019-10-18 02:32:56.000000 meshparty-1.7.2/meshparty/
--rw-r--r--   0 forrestc (1223548560) 1457291929    52078 2019-10-18 02:32:28.000000 meshparty-1.7.2/meshparty/trimesh_io.py
--rw-r--r--   0 forrestc (1223548560) 1457291929     5912 2019-09-26 00:06:12.000000 meshparty-1.7.2/meshparty/mesh_filters.py
--rw-r--r--   0 forrestc (1223548560) 1457291929     2103 2018-11-13 00:22:21.000000 meshparty-1.7.2/meshparty/meshlabserver.py
--rw-r--r--   0 forrestc (1223548560) 1457291929    17100 2019-09-26 00:06:12.000000 meshparty-1.7.2/meshparty/skeleton.py
--rw-r--r--   0 forrestc (1223548560) 1457291929    16813 2019-09-26 00:06:12.000000 meshparty-1.7.2/meshparty/trimesh_repair.py
--rw-r--r--   0 forrestc (1223548560) 1457291929       21 2019-10-18 02:32:40.000000 meshparty-1.7.2/meshparty/__init__.py
--rw-r--r--   0 forrestc (1223548560) 1457291929    35961 2019-10-14 21:20:00.000000 meshparty-1.7.2/meshparty/trimesh_vtk.py
--rw-r--r--   0 forrestc (1223548560) 1457291929     3480 2018-12-25 17:56:03.000000 meshparty-1.7.2/meshparty/iterator.py
--rw-r--r--   0 forrestc (1223548560) 1457291929     9041 2019-09-26 00:06:12.000000 meshparty-1.7.2/meshparty/utils.py
--rw-r--r--   0 forrestc (1223548560) 1457291929    29667 2019-10-18 02:32:28.000000 meshparty-1.7.2/meshparty/skeletonize.py
--rw-r--r--   0 forrestc (1223548560) 1457291929     2028 2019-09-26 00:06:12.000000 meshparty-1.7.2/meshparty/mesh_skel_utils.py
--rw-r--r--   0 forrestc (1223548560) 1457291929     8497 2019-09-26 00:06:12.000000 meshparty-1.7.2/meshparty/skeleton_io.py
+drwxr-xr-x   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)        0 2019-12-03 23:22:22.000000 meshparty-1.8.0/
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      106 2019-12-03 23:22:09.000000 meshparty-1.8.0/.bumpversion.cfg
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      420 2019-03-31 15:04:01.000000 meshparty-1.8.0/.coveragerc
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      166 2019-12-03 23:21:38.000000 meshparty-1.8.0/.gitignore
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)       62 2018-12-19 20:11:13.000000 meshparty-1.8.0/.pypirc
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      660 2019-12-03 23:21:43.000000 meshparty-1.8.0/.readthedocs.yml
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     1182 2019-12-03 23:21:38.000000 meshparty-1.8.0/.travis.yml
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)    11357 2019-03-18 20:54:12.000000 meshparty-1.8.0/LICENSE
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      134 2019-12-03 23:21:38.000000 meshparty-1.8.0/MANIFEST.in
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      303 2019-12-03 23:22:22.000000 meshparty-1.8.0/PKG-INFO
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     2151 2019-12-03 23:21:38.000000 meshparty-1.8.0/README.rst
+drwxr-xr-x   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)        0 2019-12-03 23:22:22.000000 meshparty-1.8.0/docs/
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      634 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/Makefile
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     2405 2019-12-03 23:21:43.000000 meshparty-1.8.0/docs/conf.py
+drwxr-xr-x   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)        0 2019-12-03 23:22:22.000000 meshparty-1.8.0/docs/guide/
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     3404 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/guide/analysis.rst
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     1838 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/guide/filtering.rst
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     1694 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/guide/loading.rst
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     1660 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/guide/repair.rst
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     8468 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/guide/skeletons.rst
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)    11537 2019-12-03 23:21:43.000000 meshparty-1.8.0/docs/guide/visualization.rst
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)       40 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/includeme.rst
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      649 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/index.rst
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      795 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/make.bat
+drwxr-xr-x   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)        0 2019-12-03 23:22:22.000000 meshparty-1.8.0/docs/source/
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     2144 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/source/meshparty.rst
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)       64 2019-12-03 23:21:38.000000 meshparty-1.8.0/docs/source/modules.rst
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      197 2019-12-03 23:21:43.000000 meshparty-1.8.0/environment.yml
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      972 2019-01-24 02:33:09.000000 meshparty-1.8.0/example.py
+drwxr-xr-x   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)        0 2019-12-03 23:22:22.000000 meshparty-1.8.0/meshlabscripts/
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      210 2018-11-13 00:22:21.000000 meshparty-1.8.0/meshlabscripts/mergeclosevertices.mlb
+drwxr-xr-x   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)        0 2019-12-03 23:22:22.000000 meshparty-1.8.0/meshparty/
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)       21 2019-12-03 23:22:09.000000 meshparty-1.8.0/meshparty/__init__.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     3480 2018-12-25 17:56:03.000000 meshparty-1.8.0/meshparty/iterator.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     5912 2019-12-03 23:21:38.000000 meshparty-1.8.0/meshparty/mesh_filters.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     2028 2019-12-03 23:21:38.000000 meshparty-1.8.0/meshparty/mesh_skel_utils.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     2103 2018-11-13 00:22:21.000000 meshparty-1.8.0/meshparty/meshlabserver.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)    17100 2019-12-03 23:21:38.000000 meshparty-1.8.0/meshparty/skeleton.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     8497 2019-12-03 23:21:38.000000 meshparty-1.8.0/meshparty/skeleton_io.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)    29667 2019-12-03 23:21:38.000000 meshparty-1.8.0/meshparty/skeletonize.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)    52078 2019-12-03 23:21:38.000000 meshparty-1.8.0/meshparty/trimesh_io.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)    16813 2019-12-03 23:21:38.000000 meshparty-1.8.0/meshparty/trimesh_repair.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)    39980 2019-12-03 23:21:43.000000 meshparty-1.8.0/meshparty/trimesh_vtk.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     9041 2019-12-03 23:21:38.000000 meshparty-1.8.0/meshparty/utils.py
+drwxr-xr-x   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)        0 2019-12-03 23:22:22.000000 meshparty-1.8.0/meshparty.egg-info/
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      303 2019-12-03 23:22:21.000000 meshparty-1.8.0/meshparty.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      977 2019-12-03 23:22:21.000000 meshparty-1.8.0/meshparty.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)        1 2019-12-03 23:22:21.000000 meshparty-1.8.0/meshparty.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      212 2019-12-03 23:22:21.000000 meshparty-1.8.0/meshparty.egg-info/requires.txt
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)       10 2019-12-03 23:22:21.000000 meshparty-1.8.0/meshparty.egg-info/top_level.txt
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)       41 2019-11-25 15:44:26.000000 meshparty-1.8.0/optional_requirements.txt
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)      153 2019-12-03 23:21:38.000000 meshparty-1.8.0/requirements.txt
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)       38 2019-12-03 23:22:22.000000 meshparty-1.8.0/setup.cfg
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)     1725 2019-11-25 15:46:02.000000 meshparty-1.8.0/setup.py
+-rw-r--r--   0 forrestc (1223548560) ALLENINST\Domain Users (1457291929)       67 2019-12-03 23:21:38.000000 meshparty-1.8.0/test_requirements.txt
```

### Comparing `meshparty-1.7.2/LICENSE` & `meshparty-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/docs/guide/filtering.rst` & `meshparty-1.8.0/docs/guide/filtering.rst`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/docs/guide/skeletons.rst` & `meshparty-1.8.0/docs/guide/skeletons.rst`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/docs/guide/loading.rst` & `meshparty-1.8.0/docs/guide/loading.rst`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/docs/guide/repair.rst` & `meshparty-1.8.0/docs/guide/repair.rst`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/docs/guide/analysis.rst` & `meshparty-1.8.0/docs/guide/analysis.rst`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/docs/index.rst` & `meshparty-1.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/docs/Makefile` & `meshparty-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/docs/conf.py` & `meshparty-1.8.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 html_theme = 'alabaster'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.coverage', 'sphinx.ext.napoleon', 'sphinx.ext.viewcode',
-    'sphinx.ext.githubpages', 'sphinx.ext.intersphinx']
+    'sphinx.ext.githubpages', 'sphinx.ext.intersphinx','sphinxcontrib.yt']
 autodoc_inherit_docstrings = False
 
 intersphinx_mapping = {'trimesh':('https://trimsh.org/', None),
                        'networkx':('https://networkx.github.io/documentation/stable', None),
                        'scipy':('https://docs.scipy.org/doc/scipy/reference/', None)}
```

### Comparing `meshparty-1.7.2/docs/source/meshparty.rst` & `meshparty-1.8.0/docs/source/meshparty.rst`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/docs/make.bat` & `meshparty-1.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/.readthedocs.yml` & `meshparty-1.8.0/.readthedocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 # Required
 version: 2
 
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   configuration: docs/conf.py
+  builder: html
 
 # Build documentation with MkDocs
 #mkdocs:
 #  configuration: mkdocs.yml
 
 # Optionally build your docs in additional formats such as PDF and ePub
-formats: all
+formats: []
 
 # Optionally set the version of Python and requirements required to build your docs
 python:
   version: 3.7
   install:
     - requirements: docs/requirements.txt
     - method: setuptools
```

### Comparing `meshparty-1.7.2/setup.py` & `meshparty-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/example.py` & `meshparty-1.8.0/example.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty.egg-info/SOURCES.txt` & `meshparty-1.8.0/meshparty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/README.rst` & `meshparty-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/.travis.yml` & `meshparty-1.8.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty/trimesh_io.py` & `meshparty-1.8.0/meshparty/trimesh_io.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty/mesh_filters.py` & `meshparty-1.8.0/meshparty/mesh_filters.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty/meshlabserver.py` & `meshparty-1.8.0/meshparty/meshlabserver.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty/skeleton.py` & `meshparty-1.8.0/meshparty/skeleton.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty/trimesh_repair.py` & `meshparty-1.8.0/meshparty/trimesh_repair.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty/trimesh_vtk.py` & `meshparty-1.8.0/meshparty/trimesh_vtk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import vtk
 from vtk.util.numpy_support import numpy_to_vtk, numpy_to_vtkIdTypeArray, vtk_to_numpy
 import numpy as np
 import os
-
+import logging
 
 def numpy_to_vtk_cells(mat):
     """function to convert a numpy array of integers to a vtkCellArray
 
     Parameters
     ----------
     mat : np.array
@@ -255,15 +255,16 @@
     else:
         edges = None
     return points, tris, edges
 
 
 def render_actors(actors, camera=None, do_save=False, filename=None,
                   scale=4, back_color=(1, 1, 1),
-                  VIDEO_WIDTH=1080, VIDEO_HEIGHT=720,
+                  VIDEO_WIDTH=None, VIDEO_HEIGHT=None,
+                  video_width=1080, video_height=720,
                   return_keyframes=False):
     """
     Visualize a set of actors in a 3d scene, optionally saving a snapshot. 
     Creates a window, renderer, interactor, add the actors and starts the visualization
     (can save images and close render window)
 
     Parameters
@@ -290,17 +291,24 @@
         (useful for retrieving user input camera position ren.GetActiveCamera())
     (list[vtk.vtkCamera])
         list of vtk cameras when user pressed 'k' (only if return_keyframes=True)
 
     """
     if do_save:
         assert(filename is not None)
+    if VIDEO_HEIGHT is not None:
+        logging.warning('VIDEO_HEIGHT deprecated, please use video_height')
+        video_height=VIDEO_HEIGHT
+    if VIDEO_WIDTH is not None:
+        logging.warning('VIDEO_WIDTH is deprecated, please use VIDEO_WIDTH')
+        video_width=VIDEO_WIDTH
+        
     # create a rendering window and renderer
     ren, renWin, iren = _setup_renderer(
-        VIDEO_WIDTH, VIDEO_HEIGHT, back_color, camera=camera)
+        video_width, video_height, back_color, camera=camera)
 
     for a in actors:
         # assign actor to the renderer
         ren.AddActor(a)
 
     # render
     if camera is None:
@@ -452,15 +460,15 @@
         map_colors, whether the colors should be mapped through a colormap
         or used as is
 
     """
     map_colors = False
     if not isinstance(color, np.ndarray):
         color = np.array(color)
-    if color.shape == (len(xyz), 3):
+    if ((color.shape == (len(xyz), 3)) | (color.shape == (len(xyz), 4))):
         # then we have explicit colors
         if color.dtype != np.uint8:
             # if not passing uint8 assume 0-1 mapping
             assert(np.max(color) <= 1.0)
             assert(np.min(color) >= 0)
             color = np.uint8(color*255)
     elif color.shape == (len(xyz),):
@@ -903,14 +911,20 @@
 
     # create a renderwindowinteractor
     iren = vtk.vtkRenderWindowInteractor()
     iren.SetRenderWindow(renWin)
 
     return ren, renWin, iren
 
+def make_camera_interpolator(times, cameras):
+    assert(len(times) == len(cameras))
+    camera_interp = vtk.vtkCameraInterpolator()
+    for t, cam in zip(times, cameras):
+        camera_interp.AddCamera(t, cam)
+    return camera_interp
 
 def render_movie(actors, directory, times, cameras, start_frame=0,
                  video_width=1280, video_height=720, scale=4,
                  do_save=True, back_color=(1, 1, 1)):
     """
     Function to create a series of png frames based upon a defining 
     a set of cameras at a set of times.
@@ -964,21 +978,105 @@
         times = np.array([0, 90, 180])
         cameras = [camera_start, camera_180, camera_start]
         render_movie([mesh_actor],
                 'movie',
                 times,
                 cameras)
     """
+    camera_interp=make_camera_interpolator(times, cameras)
 
-    camera_interp = vtk.vtkCameraInterpolator()
-    assert(len(times) == len(cameras))
-    for t, cam in zip(times, cameras):
-        camera_interp.AddCamera(t, cam)
+    def interpolate_camera(actors, camera, t):
+        camera_interp.InterpolateCamera(t, camera)
+    
+    renWin, end_frame = render_movie_flexible(actors, directory, times,
+                                          interpolate_camera,
+                                          start_frame=start_frame,
+                                          video_width=video_width,
+                                          video_height=video_height,
+                                          scale=scale,
+                                          do_save=do_save,
+                                          back_color=back_color)
+    return renWin, end_frame
+
+    
+def render_movie_flexible(actors, directory, times, frame_change_function, start_frame=0,
+                 video_width=1280, video_height=720, scale=4, camera=None,
+                 do_save=True, back_color=(1, 1, 1)):
+    """
+    Function to create a series of png frames based upon a defining 
+    a frame change function that will alter actors and camera at
+    each time point
+    This will save images as a series of png images in the directory
+    specified.
+    The movie will start at time 0 and will go to frame np.max(times)
+    Reccomend to make times start at 0 and the length of the movie
+    you want.  Keep in mind that typical movies are encoded at 15-30
+    frames per second and times is units of frames.
 
-    camera = vtk.vtkCamera()
+    This is the most general of the movie making functions,
+    and can be used to custom change coloring of actors or their positions
+    over time using tranformations. 
+
+    Parameters
+    ----------
+    actors :  list of vtkActor's
+        list of vtkActors to render
+    directory : str
+        folder to save images into
+    times : np.array
+        array of K frame times to set the camera to
+    frame_change_function : func
+        a function that takes (actors, camera, t) as arguments.
+        where actors are the list of actors passed here,
+        camera is the camera for the rendering,
+        and t is the current frame number.
+        This function may alter the actors and camera as a function
+        of time in some user defined manner.
+    start_frame : int
+        number to save the first frame number as... (default 0)
+        i.e. frames will start_frame = 5, first file would be 005.png
+    video_width : int
+        size of video in pixels
+    video_height : int
+        size of the video in pixels
+    scale : int
+        how much to expand the image
+    do_save : bool
+        whether to save the images to disk or just play interactively
+    Returns
+    -------
+    vtkRenderer
+        the renderer used to render
+    endframe
+        the last frame written
+    Example
+    -------
+    ::
+
+        from meshparty import trimesh_io, trimesh_vtk
+        mm = trimesh_io.MeshMeta(disk_cache_path = 'meshes')
+        mesh = mm.mesh(filename='mymesh.obj')
+        mesh_actor = trimesh_vtk.mesh_actor(mesh)
+        mesh_center = np.mean(mesh.vertices, axis=0)
+
+        camera_start = trimesh_vtk.oriented_camera(mesh_center, backoff = 10000, backoff_vector=(0, 0, 1))
+        camera_180 = trimesh_vtk.oriented_camera(mesh_center, backoff = 10000, backoff_vector=(0, 0, -1))
+        times = np.array([0, 90, 180])
+        cameras = [camera_start, camera_180, camera_start]
+        render_movie([mesh_actor],
+                'movie',
+                times,
+                cameras)
+    """
+    if not os.path.isdir(directory):
+        os.makedirs(directory)
+
+
+    if camera is None:
+        camera = vtk.vtkCamera()
     # create a rendering window and renderer
     ren, renWin, iren = _setup_renderer(
         video_width, video_height, back_color, camera=camera)
 
     for a in actors:
         # assign actor to the renderer
         ren.AddActor(a)
@@ -993,31 +1091,30 @@
     # Setup movie writer
     if do_save:
         moviewriter = vtk.vtkPNGWriter()
         moviewriter.SetInputConnection(imageFilter.GetOutputPort())
         renWin.OffScreenRenderingOn()
 
     for i in np.arange(0, np.max(times)+1):
-        camera_interp.InterpolateCamera(i, camera)
+        frame_change_function(actors, camera, i)  
         ren.ResetCameraClippingRange()
         camera.ViewingRaysModified()
         renWin.Render()
 
         if do_save:
             filename = os.path.join(directory, "%04d.png" % (i+start_frame))
             moviewriter.SetFileName(filename)
             # Export a current frame
             imageFilter.Update()
             imageFilter.Modified()
             moviewriter.Write()
-
+    
     renWin.Finalize()
     return renWin, i+start_frame
 
-
 def scale_bar_actor(center, camera, length=10000, color=(0, 0, 0), linewidth=5, font_size=20):
     """Creates a xyz 3d scale bar actor located at a specific location with a given size
 
     Parameters
     ----------
     center : iterable
         a length 3 iterable of xyz position
```

### Comparing `meshparty-1.7.2/meshparty/iterator.py` & `meshparty-1.8.0/meshparty/iterator.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty/utils.py` & `meshparty-1.8.0/meshparty/utils.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty/skeletonize.py` & `meshparty-1.8.0/meshparty/skeletonize.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty/mesh_skel_utils.py` & `meshparty-1.8.0/meshparty/mesh_skel_utils.py`

 * *Files identical despite different names*

### Comparing `meshparty-1.7.2/meshparty/skeleton_io.py` & `meshparty-1.8.0/meshparty/skeleton_io.py`

 * *Files identical despite different names*

