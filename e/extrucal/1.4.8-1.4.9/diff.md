# Comparing `tmp/extrucal-1.4.8.tar.gz` & `tmp/extrucal-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrucal-1.4.8.tar", max compression
+gzip compressed data, was "extrucal-1.4.9.tar", max compression
```

## Comparing `extrucal-1.4.8.tar` & `extrucal-1.4.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2022-02-23 23:24:05.549046 extrucal-1.4.8/LICENSE
--rw-r--r--   0        0        0     5208 2022-02-23 23:24:05.553046 extrucal-1.4.8/README.md
--rw-r--r--   0        0        0     1452 2022-02-23 23:24:14.865022 extrucal-1.4.8/pyproject.toml
--rw-r--r--   0        0        0      110 2022-02-23 23:24:05.553046 extrucal-1.4.8/src/extrucal/__init__.py
--rw-r--r--   0        0        0    14049 2022-02-23 23:24:05.553046 extrucal-1.4.8/src/extrucal/cable_extrusion.py
--rw-r--r--   0        0        0    17052 2022-02-23 23:24:05.553046 extrucal-1.4.8/src/extrucal/extrusion.py
--rw-r--r--   0        0        0    13543 2022-02-23 23:24:05.553046 extrucal-1.4.8/src/extrucal/rod_extrusion.py
--rw-r--r--   0        0        0    13590 2022-02-23 23:24:05.553046 extrucal-1.4.8/src/extrucal/sheet_extrusion.py
--rw-r--r--   0        0        0    13944 2022-02-23 23:24:05.553046 extrucal-1.4.8/src/extrucal/tube_extrusion.py
--rw-r--r--   0        0        0     6215 2022-02-23 23:24:21.386960 extrucal-1.4.8/setup.py
--rw-r--r--   0        0        0     6095 2022-02-23 23:24:21.387533 extrucal-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-02-23 23:29:06.331517 extrucal-1.4.9/LICENSE
+-rw-r--r--   0        0        0     5208 2022-02-23 23:29:06.335517 extrucal-1.4.9/README.md
+-rw-r--r--   0        0        0     1452 2022-02-23 23:29:16.792050 extrucal-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0      110 2022-02-23 23:29:06.339517 extrucal-1.4.9/src/extrucal/__init__.py
+-rw-r--r--   0        0        0    14049 2022-02-23 23:29:06.339517 extrucal-1.4.9/src/extrucal/cable_extrusion.py
+-rw-r--r--   0        0        0    17052 2022-02-23 23:29:06.339517 extrucal-1.4.9/src/extrucal/extrusion.py
+-rw-r--r--   0        0        0    13543 2022-02-23 23:29:06.339517 extrucal-1.4.9/src/extrucal/rod_extrusion.py
+-rw-r--r--   0        0        0    13590 2022-02-23 23:29:06.339517 extrucal-1.4.9/src/extrucal/sheet_extrusion.py
+-rw-r--r--   0        0        0    13944 2022-02-23 23:29:06.339517 extrucal-1.4.9/src/extrucal/tube_extrusion.py
+-rw-r--r--   0        0        0     6215 2022-02-23 23:29:23.311341 extrucal-1.4.9/setup.py
+-rw-r--r--   0        0        0     6095 2022-02-23 23:29:23.312034 extrucal-1.4.9/PKG-INFO
```

### Comparing `extrucal-1.4.8/LICENSE` & `extrucal-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `extrucal-1.4.8/README.md` & `extrucal-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `extrucal-1.4.8/pyproject.toml` & `extrucal-1.4.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "extrucal"
-version = "1.4.8"
+version = "1.4.9"
 description = "Provides functions for calculating various parameters in extrusion processes"
 authors = ["John W.S. Lee"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/johnwslee/extrucal"
 repository = "https://github.com/johnwslee/extrucal"
 documentation = "https://extrucal.readthedocs.io/en/latest/"
```

### Comparing `extrucal-1.4.8/src/extrucal/cable_extrusion.py` & `extrucal-1.4.9/src/extrucal/cable_extrusion.py`

 * *Files identical despite different names*

### Comparing `extrucal-1.4.8/src/extrucal/extrusion.py` & `extrucal-1.4.9/src/extrucal/extrusion.py`

 * *Files identical despite different names*

### Comparing `extrucal-1.4.8/src/extrucal/rod_extrusion.py` & `extrucal-1.4.9/src/extrucal/rod_extrusion.py`

 * *Files identical despite different names*

### Comparing `extrucal-1.4.8/src/extrucal/sheet_extrusion.py` & `extrucal-1.4.9/src/extrucal/sheet_extrusion.py`

 * *Files identical despite different names*

### Comparing `extrucal-1.4.8/src/extrucal/tube_extrusion.py` & `extrucal-1.4.9/src/extrucal/tube_extrusion.py`

 * *Files identical despite different names*

### Comparing `extrucal-1.4.8/setup.py` & `extrucal-1.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'numpy>=1.22.2,<2.0.0',
  'pandas>=1.4.1,<2.0.0',
  'sphinx-autoapi>=1.8.4,<2.0.0',
  'sphinx-rtd-theme>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'extrucal',
-    'version': '1.4.8',
+    'version': '1.4.9',
     'description': 'Provides functions for calculating various parameters in extrusion processes',
     'long_description': '[![ci-cd](https://github.com/johnwslee/extrucal/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/johnwslee/extrucal/actions/workflows/ci-cd.yml)\n[![codecov](https://codecov.io/gh/johnwslee/extrucal/branch/main/graph/badge.svg?token=YT37K0ESGF)](https://codecov.io/gh/johnwslee/extrucal)\n[![Documentation Status](https://readthedocs.org/projects/extrucal/badge/?version=latest)](https://extrucal.readthedocs.io/en/latest/index.html)\n![license status](https://img.shields.io/github/license/johnwslee/extrucal)\n\n# extrucal\n\n**Author:** John W.S. Lee\n\n`extrucal` provides functions that calculate throughputs and screw RPMs for various types of extrusion processes. Theoretical throughputs can be calculated by using the screw geometry and the processing condition, whereas the throughputs required for extruded products(cable, tube, rod, and sheet) can be calculated by using the product geometry. Based on these calculated throughputs, `extrucal` functions can generate tables and plots that show the processing windows considering extruder size, line speed, and screw RPM.\n\nA large portion of arguments for the functions are given the typical values. Some of the arguments for functions are as follows:\n screw size, channel depth, polymer melt density, screw RPM, screw pitch, flight width, number of flights, line speed, extruder size, etc.\n\n## Installation\n\n`extrucal` can be installed PyPI using the following terminal command:\n\n```bash\n$ pip install extrucal\n```\n\n## Package Functions\n\n**1. Functions in `extrucal.extrusion`**\n\n- `throughput_cal()`\n  - This function calculates the extrusion throughput (Drag Flow) given the screw size, RPM, the channel depth of metering channel, and screw pitch\n  \n- `throughput_table()`\n  - This function generates a table containing the extrusion throughput with respect to channel depth and screw RPM\n  \n- `throughput_plot()`\n  - This function generates a plot containing the extrusion throughput with respect to channel depth and screw RPM\n\n**2. Functions in `extrucal.cable_extrusion`**\n\n- `cable_cal()`\n  - This function calculates the required throughput for cables given the outer diameter, thickness, line speed, and solid polymer density\n  \n- `cable_table()`\n  - This function generate a table containing the required screw RPM with respect to line speed and extruder size\n  \n- `cable_plot()`\n  - This function generate a plot containing the required screw RPM with respect to line speed and extruder size\n\n**3. Functions in `extrucal.tube_extrusion`**\n\n- `tube_cal()`\n  - This function calculates the required throughput for tubes given the outer diameter, inner diameter, line speed, and solid polymer density\n  \n- `tube_table()`\n  - This function generate a table containing the required screw RPM with respect to line speed and extruder size\n  \n- `tube_plot()`\n  - This function generate a plot containing the required screw RPM with respect to line speed and extruder size\n\n**4. Functions in `extrucal.rod_extrusion`**\n\n- `rod_cal()`\n  - This function calculates the required throughput for rods given the outer diameter, line speed, solid polymer density, and number of die holes\n  \n- `rod_table()`\n  - This function generate a table containing the required screw RPM with respect to line speed and extruder size\n  \n- `rod_plot()`\n  - This function generate a plot containing the required screw RPM with respect to line speed and extruder size\n\n**5. Functions in `extrucal.sheet_extrusion`**\n\n- `sheet_cal()`\n  - This function calculates the required throughput for sheets given the width, thickness, line speed, solid polymer density, and number of die holes\n  \n- `sheet_table()`\n  - This function generate a table containing the required screw RPM with respect to line speed and extruder size\n  \n- `sheet_plot()`\n  - This function generate a plot containing the required screw RPM with respect to line speed and extruder size\n\n\n## Usage\n\n`extrucal` can be used to calculate extrusion throughput and to generate tables and plots of various parameters in extrusion processes\n\n```python\nfrom extrucal.extrusion import throughput_cal, throughput_table, throughput_plot\nfrom extrucal.cable_extrusion import cable_cal, cable_table, cable_plot\nfrom extrucal.tube_extrusion import tube_cal, tube_table, tube_plot\nfrom extrucal.rod_extrusion import rod_cal, rod_table, rod_plot\nfrom extrucal.sheet_extrusion import sheet_cal, sheet_table, sheet_plot\n```\n\n## Dependencies\n\n-   Python 3.9 and Python packages:\n\n    -   pandas==1.4.1\n    -   numpy==1.22.2\n    -   ipykernel==6.9.1\n    -   altair-saver==0.5.0\n\n## Documentation\n\nDocumentation `extrucal` can be found at [Read the Docs](https://extrucal.readthedocs.io/en/latest/index.html)\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`extrucal` was created by John Lee. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`extrucal` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'John W.S. Lee',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/johnwslee/extrucal',
```

### Comparing `extrucal-1.4.8/PKG-INFO` & `extrucal-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrucal
-Version: 1.4.8
+Version: 1.4.9
 Summary: Provides functions for calculating various parameters in extrusion processes
 Home-page: https://github.com/johnwslee/extrucal
 License: MIT
 Author: John W.S. Lee
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

