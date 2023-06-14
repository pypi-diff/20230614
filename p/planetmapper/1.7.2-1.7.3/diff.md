# Comparing `tmp/planetmapper-1.7.2.tar.gz` & `tmp/planetmapper-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.7.2.tar", last modified: Thu Jun  1 14:34:34 2023, max compression
+gzip compressed data, was "planetmapper-1.7.3.tar", last modified: Wed Jun 14 10:02:26 2023, max compression
```

## Comparing `planetmapper-1.7.2.tar` & `planetmapper-1.7.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:34:34.386503 planetmapper-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 14:34:23.000000 planetmapper-1.7.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-01 14:34:34.386503 planetmapper-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-01 14:34:23.000000 planetmapper-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:34:34.382503 planetmapper-1.7.2/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28536 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    80564 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)   112233 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:34:34.382503 planetmapper-1.7.2/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/data/ring_aliases.json
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118018 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    46500 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:34:34.382503 planetmapper-1.7.2/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-01 14:34:23.000000 planetmapper-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:34:34.386503 planetmapper-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-01 14:34:23.000000 planetmapper-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:34:34.386503 planetmapper-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    34896 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    39958 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    28477 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:02:26.047176 planetmapper-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-14 10:02:13.000000 planetmapper-1.7.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-14 10:02:26.047176 planetmapper-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-14 10:02:13.000000 planetmapper-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:02:26.043176 planetmapper-1.7.3/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28536 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81538 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112264 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:02:26.043176 planetmapper-1.7.3/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/data/ring_aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118683 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46604 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-06-14 10:02:13.000000 planetmapper-1.7.3/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:02:26.043176 planetmapper-1.7.3/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-14 10:02:26.000000 planetmapper-1.7.3/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-14 10:02:26.000000 planetmapper-1.7.3/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:02:26.000000 planetmapper-1.7.3/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-14 10:02:26.000000 planetmapper-1.7.3/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-14 10:02:26.000000 planetmapper-1.7.3/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 10:02:26.000000 planetmapper-1.7.3/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-14 10:02:13.000000 planetmapper-1.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 10:02:26.047176 planetmapper-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-14 10:02:13.000000 planetmapper-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:02:26.047176 planetmapper-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34896 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39958 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28477 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-14 10:02:13.000000 planetmapper-1.7.3/tests/test_utils.py
```

### Comparing `planetmapper-1.7.2/LICENSE.txt` & `planetmapper-1.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/PKG-INFO` & `planetmapper-1.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.2
+Version: 1.7.3
 Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
@@ -12,21 +12,21 @@
 Keywords: planetmapper,astronomy,space,science,spice,ephemeris,planetary-science
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ![PlanetMapper logo](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/logo_wide_transparent.png)
 
-[![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
+[![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPI&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
 [![Publish](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
 [![Checks](https://github.com/ortk95/planetmapper/actions/workflows/checks.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/checks.yml)
 [![Coverage Status](https://img.shields.io/coverallsCoverage/github/ortk95/planetmapper)](https://coveralls.io/github/ortk95/planetmapper)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
 
-PlanetMapper is a Python module for visualising, navigating and mapping Solar System observations.
+PlanetMapper is an open source Python module for visualising, navigating and mapping Solar System observations.
 
 ## [Documentation](https://planetmapper.readthedocs.io)
 For full documentation and [API reference](https://planetmapper.readthedocs.io/en/latest/documentation.html), visit [planetmapper.readthedocs.io](https://planetmapper.readthedocs.io/en/latest/index.html)
 
 
 ## [Installation](https://planetmapper.readthedocs.io/en/latest/installation.html)
 ```
```

### Comparing `planetmapper-1.7.2/README.md` & `planetmapper-1.7.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# ![PlanetMapper logo](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/logo_wide_transparent.png)
+# ![PlanetMapper logo](docs/images/logo_wide_transparent.png)
 
-[![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
+[![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPI&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
 [![Publish](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
 [![Checks](https://github.com/ortk95/planetmapper/actions/workflows/checks.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/checks.yml)
 [![Coverage Status](https://img.shields.io/coverallsCoverage/github/ortk95/planetmapper)](https://coveralls.io/github/ortk95/planetmapper)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
 
-PlanetMapper is a Python module for visualising, navigating and mapping Solar System observations.
+PlanetMapper is an open source Python module for visualising, navigating and mapping Solar System observations.
 
 ## [Documentation](https://planetmapper.readthedocs.io)
 For full documentation and [API reference](https://planetmapper.readthedocs.io/en/latest/documentation.html), visit [planetmapper.readthedocs.io](https://planetmapper.readthedocs.io/en/latest/index.html)
 
 
 ## [Installation](https://planetmapper.readthedocs.io/en/latest/installation.html)
 ```
 pip install planetmapper --upgrade
 ```
 
 _Requires Python 3.10+_
 
 ## Key features
 ### [Fit and map astronomical observations using a full featured user interface](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
-[![Screenshot of the PlanetMapper graphical user interface showing an observation of Europa being navigated](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/gui_fitting.png)](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
+[![Screenshot of the PlanetMapper graphical user interface showing an observation of Europa being navigated](docs/images/gui_fitting.png)](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
 
 ### [Easily visualise solar system observations with just a few lines of code](https://planetmapper.readthedocs.io/en/latest/general_python_api.html#wireframe-plots)
 
 ```python
 body = planetmapper.Body('saturn', '2020-01-01')
 body.plot_wireframe_radec()
 plt.show()
 ```
 
-[![Image of Saturn generated with PlanetMapper showing the orientation of Saturn and its rings](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/saturn_wireframe_radec.png)](https://planetmapper.readthedocs.io/en/latest/general_python_api.html#wireframe-plots)
+[![Image of Saturn generated with PlanetMapper showing the orientation of Saturn and its rings](docs/images/saturn_wireframe_radec.png)](https://planetmapper.readthedocs.io/en/latest/general_python_api.html#wireframe-plots)
 
 ### [Convert coordinates, generate backplanes and project maps of telescope observations](https://planetmapper.readthedocs.io/en/latest/general_python_api.html)
-[![Plot of a mapped Jupiter observation, generated with PlanetMapper, showing observed and mapped versions of the Jupiter data](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/jupiter_mapped.png)](https://planetmapper.readthedocs.io/en/latest/general_python_api.html)
+[![Plot of a mapped Jupiter observation, generated with PlanetMapper, showing observed and mapped versions of the Jupiter data](docs/images/jupiter_mapped.png)](https://planetmapper.readthedocs.io/en/latest/general_python_api.html)
 
 
 ## Contributing
 
 If you spot a bug, have a suggestion, or want contribute code to PlanetMapper, check out the [contributing guidelines](https://github.com/ortk95/planetmapper/blob/main/CONTRIBUTING.md)!
```

### Comparing `planetmapper-1.7.2/planetmapper/__init__.py` & `planetmapper-1.7.3/planetmapper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-A Python module for visualising, navigating and mapping Solar System observations.
+PlanetMapper: A Python module for visualising, navigating and mapping Solar System
+observations.
 
 ..
     See https://planetmapper.readthedocs.io for full documentation.
 
 The core logic of this code is based on conversion between different coordinate systems
 of interest. The `xy` and `radec` coordinate systems define positions from the point of
 view of the observer while the `lonlat` coordinate system defines locations on the
```

### Comparing `planetmapper-1.7.2/planetmapper/base.py` & `planetmapper-1.7.3/planetmapper/base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/planetmapper/basic_body.py` & `planetmapper-1.7.3/planetmapper/basic_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,33 @@
             observer=observer,
             aberration_correction=aberration_correction,
             observer_frame=observer_frame,
             **kwargs,
         )
 
         # Document instance variables
+        self.target: str
+        """
+        Name of the target body, as standardised by 
+        :func:`SpiceBase.standardise_body_name`.
+        """
+        self.utc: str
+        """
+        String representation of the time of the observation in the format
+        `'2000-01-01T00:00:00.000000'`. This time is in the UTC timezone.
+        """
+        self.observer: str
+        """
+        Name of the observer body, as standardised by 
+        :func:`SpiceBase.standardise_body_name`.
+        """
+        self.aberration_correction: str
+        """Aberration correction used to correct light travel time in SPICE."""
+        self.observer_frame: str
+        """Observer reference frame."""
         self.et: float
         """Ephemeris time of the observation corresponding to `utc`."""
         self.dtm: datetime.datetime
         """Python timezone aware datetime of the observation corresponding to `utc`."""
         self.target_body_id: int
         """SPICE numeric ID of the target body."""
         self.target_light_time: float
```

### Comparing `planetmapper-1.7.2/planetmapper/body.py` & `planetmapper-1.7.3/planetmapper/body.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,39 @@
             observer=observer,
             aberration_correction=aberration_correction,
             observer_frame=observer_frame,
             **kwargs,
         )
 
         # Document instance variables
+        self.target: str
+        """
+        Name of the target body, as standardised by 
+        :func:`SpiceBase.standardise_body_name`.
+        """
+        self.utc: str
+        """
+        String representation of the time of the observation in the format
+        `'2000-01-01T00:00:00.000000'`. This time is in the UTC timezone.
+        """
+        self.observer: str
+        """
+        Name of the observer body, as standardised by 
+        :func:`SpiceBase.standardise_body_name`.
+        """
+        self.aberration_correction: str
+        """Aberration correction used to correct light travel time in SPICE."""
+        self.observer_frame: str
+        """Observer reference frame."""
+        self.illumination_source: str
+        """Illumination source."""
+        self.subpoint_method: str
+        """Method used to calculate the sub-observer point in SPICE."""
+        self.surface_method: str
+        """Method used to calculate surface intercepts in SPICE."""
         self.et: float
         """Ephemeris time of the observation corresponding to `utc`."""
         self.dtm: datetime.datetime
         """Python timezone aware datetime of the observation corresponding to `utc`."""
         self.target_body_id: int
         """SPICE numeric ID of the target body."""
         self.r_eq: float
```

### Comparing `planetmapper-1.7.2/planetmapper/body_xy.py` & `planetmapper-1.7.3/planetmapper/body_xy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1466,15 +1466,16 @@
         ny = yy.shape[0]
 
         def plot_fn(ax: Axes):
             self.plot_map_wireframe(
                 ax=ax,
                 add_axis_labels=False,
                 add_title=False,
-                **(plot_kwargs or {}) | dict(common_formatting=dict(color='k')),
+                **(plot_kwargs or {})
+                | dict(common_formatting=dict(color='k')),  # type:ignore
                 **map_kwargs,
             )
             # Add dx/dy to the limits to ensure the wireframe covers all of each pixel
             # as the xx and yy coordinates only give the centre of each pixel
             dx = abs(xx[0][1] - xx[0][0]) / 2
             ax.set_xlim(np.nanmin(xx) - dx, np.nanmax(xx) + dx)
             dy = abs(yy[1][0] - yy[0][0]) / 2
```

### Comparing `planetmapper-1.7.2/planetmapper/data/rings.json` & `planetmapper-1.7.3/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/planetmapper/data_loader.py` & `planetmapper-1.7.3/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/planetmapper/gui.py` & `planetmapper-1.7.3/planetmapper/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tkinter.colorchooser
 import tkinter.filedialog
 import tkinter.messagebox
 import tkinter.scrolledtext
 import traceback
 from collections import defaultdict
 from tkinter import ttk
-from typing import Any, Callable, Literal, TypeVar
+from typing import Any, Callable, Literal, TypedDict, TypeVar
 
 import matplotlib as mpl
 import matplotlib.cm
 import matplotlib.colors
 import matplotlib.markers
 import matplotlib.patheffects as path_effects
 import matplotlib.pyplot as plt
@@ -1657,76 +1657,84 @@
         if self.apply_changes():
             self.close_window()
 
     def click_apply(self) -> None:
         self.apply_changes()
 
     def apply_changes(self) -> bool:
-        kwargs = {k: v.get() for k, v in self.stringvars.items()}
-        for k, v in kwargs.items():
+        ObservationKwargs = TypedDict(
+            'ObservationKwargs',
+            {'path': str, 'target': str, 'utc': str | float, 'observer': str},
+        )
+        observation_kwargs: ObservationKwargs = {
+            k: v.get() for k, v in self.stringvars.items()
+        }  #  type: ignore
+        for k, v in observation_kwargs.items():
             if isinstance(v, str) and len(v.strip()) == 0:
                 tkinter.messagebox.showwarning(
                     title=f'Error parsing {k}', message=f'{k!r} must not be empty'
                 )
                 return False
 
         string = self.kernel_txt.get('1.0', 'end')
         kernels = [k.strip() for k in string.splitlines()]
         base.load_kernels(*kernels, clear_before=True)
 
         kernel_help = '\n' + base._SPICE_ERROR_HELP_TEXT
 
         sb = base.SpiceBase(auto_load_kernels=False)
         try:
-            target = sb.standardise_body_name(kwargs['target'])
+            target = sb.standardise_body_name(observation_kwargs['target'])
         # pylint: disable-next=bare-except
         except:
             tkinter.messagebox.showwarning(
                 title='Error parsing target',
                 message='Target name {!r} not recognised\n{}'.format(
-                    kwargs['target'], kernel_help
+                    observation_kwargs['target'], kernel_help
                 ),
             )
             return False
 
         try:
-            observer = sb.standardise_body_name(kwargs['observer'])
+            observer = sb.standardise_body_name(observation_kwargs['observer'])
         # pylint: disable-next=bare-except
         except:
             tkinter.messagebox.showwarning(
                 title='Error parsing observer',
                 message='Observer name {!r} not recognised\n{}'.format(
-                    kwargs['observer'], kernel_help
+                    observation_kwargs['observer'], kernel_help
                 ),
             )
             return False
 
         if target == observer:
             tkinter.messagebox.showwarning(
                 title='Target and observer identical',
                 message='Target and observer must correspond to different bodies',
             )
             return False
 
         try:
-            kwargs['utc'] = float(kwargs['utc'])  #  type: ignore
+            observation_kwargs['utc'] = float(
+                observation_kwargs['utc']
+            )  #  type: ignore
         except ValueError:
             try:
-                spice.utc2et(kwargs['utc'])
+                spice.utc2et(observation_kwargs['utc'])  #  type: ignore
             # pylint: disable-next=bare-except
             except:
                 tkinter.messagebox.showwarning(
                     title='Error parsing utc',
                     message='Could not parse {!r}\n{}'.format(
-                        kwargs['utc'], kernel_help
+                        observation_kwargs['utc'], kernel_help
                     ),
                 )
                 return False
         try:
-            observation = Observation(**kwargs, auto_load_kernels=False)
+            observation = Observation(**observation_kwargs, auto_load_kernels=False)
         # pylint: disable-next=broad-except
         except Exception as e:
             traceback.print_exc()
             tkinter.messagebox.showwarning(
                 title='Error processing inputs',
                 message=f'Error: {e}' + '\n\nSee terminal for more details',
             )
@@ -1869,107 +1877,109 @@
 
         self.nav_widgets: list[tk.Widget] = []
         self.map_widgets: list[tk.Widget] = []
         self.map_rect_widgets: list[tk.Widget] = []
         self.map_ortho_widgets: list[tk.Widget] = []
 
         self.grid_frame.grid_columnconfigure(1, weight=1)
-        label_kw = dict(sticky='w', pady=5)
+
+        LabelKwargs = TypedDict('LabelKwargs', {'sticky': str, 'pady': int})
+        label_kwargs = LabelKwargs(sticky='w', pady=5)
 
         # Navigated
         ttk.Checkbutton(
             self.grid_frame, text='Save navigated observation', variable=self.save_nav
         ).grid(row=0, column=1, columnspan=2, sticky='ew')
 
-        ttk.Label(self.grid_frame, text='Path: ').grid(row=1, column=0, **label_kw)
+        ttk.Label(self.grid_frame, text='Path: ').grid(row=1, column=0, **label_kwargs)
         w = ttk.Entry(self.grid_frame, textvariable=self.path_nav)
         w.grid(row=1, column=1, sticky='ew')
         self.nav_widgets.append(w)
         w = ttk.Button(self.grid_frame, text='...', width=3, command=self.get_path_nav)
         w.grid(row=1, column=2)
         self.nav_widgets.append(w)
 
-        ttk.Label(self.grid_frame, text=' ').grid(row=2, column=0, **label_kw)
+        ttk.Label(self.grid_frame, text=' ').grid(row=2, column=0, **label_kwargs)
 
         # Mapped
         ttk.Checkbutton(
             self.grid_frame, text='Save mapped observation', variable=self.save_map
         ).grid(row=3, column=1, columnspan=2, sticky='ew')
 
-        ttk.Label(self.grid_frame, text='Path: ').grid(row=4, column=0, **label_kw)
+        ttk.Label(self.grid_frame, text='Path: ').grid(row=4, column=0, **label_kwargs)
         w = ttk.Entry(self.grid_frame, textvariable=self.path_map)
         w.grid(row=4, column=1, sticky='ew')
         self.map_widgets.append(w)
         w = ttk.Button(self.grid_frame, text='...', width=3, command=self.get_path_map)
         w.grid(row=4, column=2, sticky='w')
         self.map_widgets.append(w)
 
         self.map_option_grid = ttk.Frame(self.grid_frame)
         self.map_option_grid.grid(row=5, column=0, columnspan=3, sticky='nsew')
 
         for col in [1, 3, 5]:
             self.map_option_grid.grid_columnconfigure(col, weight=1)
 
-        label_kw = dict(sticky='w', pady=2)
+        label_kwargs = LabelKwargs(sticky='w', pady=2)
 
         ttk.Label(self.map_option_grid, text='Interpolation: ').grid(
-            row=0, column=0, **label_kw
+            row=0, column=0, **label_kwargs
         )
         w = ttk.Combobox(
             self.map_option_grid,
             textvariable=self.map_interpolation,
             width=15,
             values=MAP_INTERPOLATIONS,
             state='readonly',
         )
         w.grid(row=0, column=1, columnspan=5, sticky='w')
         self.map_widgets.append(w)
 
         ttk.Label(self.map_option_grid, text='Projection: ').grid(
-            row=1, column=0, **label_kw
+            row=1, column=0, **label_kwargs
         )
         w = ttk.Combobox(
             self.map_option_grid,
             textvariable=self.map_projection,
             width=15,
             values=MAP_PROJECTIONS,
             state='readonly',
         )
         w.grid(row=1, column=1, columnspan=5, sticky='w')
         self.map_widgets.append(w)
 
         # Projection options
         width = 10
         ttk.Label(self.map_option_grid, text='Degree interval: ').grid(
-            row=2, column=0, **label_kw
+            row=2, column=0, **label_kwargs
         )
         w = ttk.Entry(
             self.map_option_grid, textvariable=self.map_degree_interval, width=width
         )
         w.grid(row=2, column=1, sticky='w')
         self.map_rect_widgets.append(w)
 
         ttk.Label(self.map_option_grid, text='Output size: ').grid(
-            row=3, column=0, **label_kw
+            row=3, column=0, **label_kwargs
         )
         w = ttk.Entry(
             self.map_option_grid, textvariable=self.map_output_size, width=width
         )
         w.grid(row=3, column=1, sticky='w')
         self.map_ortho_widgets.append(w)
 
         ttk.Label(self.map_option_grid, text='Longitude: ').grid(
-            row=3, column=2, **label_kw
+            row=3, column=2, **label_kwargs
         )
         w = ttk.Entry(self.map_option_grid, textvariable=self.map_lon, width=width)
         w.grid(row=3, column=3, sticky='w')
         self.map_ortho_widgets.append(w)
 
         ttk.Label(self.map_option_grid, text='Latitude: ').grid(
-            row=3, column=4, **label_kw
+            row=3, column=4, **label_kwargs
         )
         w = ttk.Entry(self.map_option_grid, textvariable=self.map_lat, width=width)
         w.grid(row=3, column=5, sticky='w')
         self.map_ortho_widgets.append(w)
 
         message = '\n'.join(
             [
@@ -2197,15 +2207,18 @@
 
         widgets['bar'] = ttk.Progressbar(frame)
         widgets['bar'].pack(fill='x')
 
         return widgets
 
     def run_save(self) -> None:
-        save_kwargs = dict(show_progress=False, print_info=True)
+        SaveKwargs = TypedDict(
+            'SaveKwargs', {'show_progress': bool, 'print_info': bool}
+        )
+        save_kwargs = SaveKwargs(show_progress=False, print_info=True)
         observation = self.parent.gui.get_observation()
         if self.save_nav:
             observation._set_progress_hook(SaveNavProgressHookGUI(**self.nav_widgets))
             observation.save_observation(self.path_nav, **save_kwargs)
             observation._remove_progress_hook()
         if self.save_map:
             n_wavelengths = len(self.parent.gui.get_observation().data)
```

### Comparing `planetmapper-1.7.2/planetmapper/kernel_downloader.py` & `planetmapper-1.7.3/planetmapper/kernel_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,57 +32,60 @@
 
 from . import utils
 from .base import get_kernel_path
 
 URL_ROOT = 'https://naif.jpl.nasa.gov/pub/'
 
 
-def download_urls(*urls: str) -> None:
+def download_urls(*urls: str, **kwargs) -> None:
     """
     Download data from naif.jpl.nasa.gov and save locally.
 
     urls can either be a the url of a single kernel, or the index page containing
     multiple kernels.
 
     If a single kernel, download the kernel using download_kernel().
 
     If an index page, download all first-level files using
     :func:`download_kernels_from_webpage`.
 
     Args:
         urls: kernel URL on naif.jpl.nasa.gov.
+        **kwargs: passed to :func:`download_kernel` and
+            :func:`download_kernels_from_webpage`.
     """
     for url in urls:
         # look for '.' in filename part of url to identify if a file/directory
         path = urllib.parse.urlsplit(url).path
         if '.' in os.path.split(path)[1]:
-            download_kernel(url)
+            download_kernel(url, **kwargs)
         else:
-            download_kernels_from_webpage(url)
+            download_kernels_from_webpage(url, **kwargs)
 
 
-def download_kernels_from_webpage(index_url: str) -> None:
+def download_kernels_from_webpage(index_url: str, **kwargs) -> None:
     """
     Download all first-level kernels listed in the page given by index_url.
 
     URL must be on https://naif.jpl.nasa.gov/pub/. This will break if JPL changes the
     format of the webpage.
 
     .. warning ::
 
         This function will only download kernels found immediately on `index_url`.
         Kernels in nested folders must therefore be downloaded manually.
 
     Args:
         index_url: URL of index page on naif.jpl.nasa.gov.
+        **kwargs: passed to :func:`download_kernel`.
     """
     urls = get_kernel_paths_from_webpage(index_url)
     print(f'{len(urls)} to download from {index_url}')
     for idx, url in enumerate(urls):
-        download_kernel(url, note=f'[{idx+1}/{len(urls)}] ')
+        download_kernel(url, note=f'[{idx+1}/{len(urls)}] ', **kwargs)
     print(f'All kernels downloaded from {index_url}')
     print()
 
 
 def download_kernel(url: str, force_download: bool = False, note: str = '') -> None:
     """
     Download single kernel given by url.
```

### Comparing `planetmapper-1.7.2/planetmapper/observation.py` & `planetmapper-1.7.3/planetmapper/observation.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,16 @@
         **kwargs,
     ) -> None:
         self._path_arg = path
         self._data_arg = data
         self._header_arg = header
 
         # Add docstrings
+        self.path: str | None
+        """Path of input data file, or `None` if no file was provided."""
         self.data: np.ndarray
         """Observed data."""
         self.header: fits.Header
         """
         FITS header containing data about the observation. If this is not provided, then
         a basic header will be produced containing data derived from the `target` and 
         `utc` parameters.
```

### Comparing `planetmapper-1.7.2/planetmapper/progress.py` & `planetmapper-1.7.3/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/planetmapper/utils.py` & `planetmapper-1.7.3/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.7.3/planetmapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.2
+Version: 1.7.3
 Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
@@ -12,21 +12,21 @@
 Keywords: planetmapper,astronomy,space,science,spice,ephemeris,planetary-science
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ![PlanetMapper logo](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/logo_wide_transparent.png)
 
-[![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
+[![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPI&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
 [![Publish](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
 [![Checks](https://github.com/ortk95/planetmapper/actions/workflows/checks.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/checks.yml)
 [![Coverage Status](https://img.shields.io/coverallsCoverage/github/ortk95/planetmapper)](https://coveralls.io/github/ortk95/planetmapper)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
 
-PlanetMapper is a Python module for visualising, navigating and mapping Solar System observations.
+PlanetMapper is an open source Python module for visualising, navigating and mapping Solar System observations.
 
 ## [Documentation](https://planetmapper.readthedocs.io)
 For full documentation and [API reference](https://planetmapper.readthedocs.io/en/latest/documentation.html), visit [planetmapper.readthedocs.io](https://planetmapper.readthedocs.io/en/latest/index.html)
 
 
 ## [Installation](https://planetmapper.readthedocs.io/en/latest/installation.html)
 ```
```

### Comparing `planetmapper-1.7.2/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.7.3/planetmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/pyproject.toml` & `planetmapper-1.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/setup.py` & `planetmapper-1.7.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 sys.path.append(os.path.join(root, 'planetmapper'))
 # pylint: disable-next=import-error
 import common  # type: ignore
 
 with open(os.path.join(root, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
+# Replace relative image links with absolute links to GitHub hosted images so that
+# images display properly on PyPI
+long_description = long_description.replace(
+    '](docs/images/',
+    '](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/',
+)
+
 setuptools.setup(
     name='planetmapper',
     version=common.__version__,
     author=common.__author__,
     author_email='oliver.king95@gmail.com',
     description=common.__description__,
     long_description=long_description,
@@ -26,15 +33,18 @@
     package_dir={'planetmapper': 'planetmapper'},
     package_data={'planetmapper': ['data/*.json']},
     include_package_data=True,
     project_urls={
         'Documentation': 'https://planetmapper.readthedocs.io/',
         'GitHub': common.__url__,
     },
-    entry_points={'console_scripts': ['planetmapper=planetmapper:main']},
+    entry_points={
+        # Copy any changes here to the conda-forge recipe (meta.yaml)
+        'console_scripts': ['planetmapper=planetmapper:main'],
+    },
     python_requires='>=3.10.0',
     install_requires=[
         'astropy',
         'matplotlib',
         'numpy',
         'Pillow',
         'spiceypy',
```

### Comparing `planetmapper-1.7.2/tests/test_base.py` & `planetmapper-1.7.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/tests/test_basic_body.py` & `planetmapper-1.7.3/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/tests/test_body.py` & `planetmapper-1.7.3/tests/test_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/tests/test_body_xy.py` & `planetmapper-1.7.3/tests/test_body_xy.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/tests/test_common.py` & `planetmapper-1.7.3/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/tests/test_data_loader.py` & `planetmapper-1.7.3/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/tests/test_init.py` & `planetmapper-1.7.3/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/tests/test_kernel_downloader.py` & `planetmapper-1.7.3/tests/test_kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/tests/test_observation.py` & `planetmapper-1.7.3/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/tests/test_progress.py` & `planetmapper-1.7.3/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.2/tests/test_utils.py` & `planetmapper-1.7.3/tests/test_utils.py`

 * *Files identical despite different names*

