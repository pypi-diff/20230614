# Comparing `tmp/scinumtools-1.1.2.tar.gz` & `tmp/scinumtools-1.2.0.tar.gz`

## Comparing `scinumtools-1.1.2.tar` & `scinumtools-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.1.2/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.1.2/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/phys/units/DIP_Solver_Units.py
--rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0    10693 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.1.2/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.1.2/tests/cached_data.npy
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 scinumtools-1.1.2/tests/test_data.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scinumtools-1.1.2/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.1.2/tests/test_stats.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.1.2/tests/test_struct.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 scinumtools-1.1.2/tests/test_units.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.1.2/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.1.2/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.2.0/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.2.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/phys/units/DIP_Solver_Units.py
+-rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0    10693 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.2.0/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.2.0/tests/cached_data.npy
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 scinumtools-1.2.0/tests/test_data.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scinumtools-1.2.0/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.2.0/tests/test_stats.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.2.0/tests/test_struct.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 scinumtools-1.2.0/tests/test_units.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.2.0/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.2.0/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.2.0/PKG-INFO
```

### Comparing `scinumtools-1.1.2/.github/workflows/python-publish.yml` & `scinumtools-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/src/scinumtools/data/ImageClass.py` & `scinumtools-1.2.0/src/scinumtools/data/ImageClass.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,14 @@
         if res and extent:
             layer.im = layer.im.resize(res)
             return layer
         else:
             self.im = self.im.resize(res)
             return self
         
-    def draw(self, ax=None):
+    def draw(self, ax=None, **kwargs):
         """ Draw current image on an axis
 
         :param ax: Matplotlib axis
         """
         if not ax: ax=plt
-        ax.imshow(np.asarray(self.im), extent=self.extent, origin='lower')
+        ax.imshow(np.asarray(self.im), extent=self.extent, origin='lower', **kwargs)
```

### Comparing `scinumtools-1.1.2/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.2.0/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.2.0/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/src/scinumtools/phys/units/DIP_Solver_Units.py` & `scinumtools-1.2.0/src/scinumtools/phys/units/DIP_Solver_Units.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.2.0/src/scinumtools/phys/units/QuantityClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.2.0/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.2.0/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.2.0/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.2.0/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/tests/test_data.py` & `scinumtools-1.2.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/tests/test_stats.py` & `scinumtools-1.2.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/tests/test_struct.py` & `scinumtools-1.2.0/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/tests/test_units.py` & `scinumtools-1.2.0/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/.gitignore` & `scinumtools-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.2/pyproject.toml` & `scinumtools-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.1.2"
+version = "1.2.0"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.1.2/PKG-INFO` & `scinumtools-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.1.2
+Version: 1.2.0
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

