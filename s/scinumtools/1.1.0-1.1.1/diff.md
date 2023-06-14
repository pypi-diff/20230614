# Comparing `tmp/scinumtools-1.1.0.tar.gz` & `tmp/scinumtools-1.1.1.tar.gz`

## Comparing `scinumtools-1.1.0.tar` & `scinumtools-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,28 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.1.0/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.1.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.1.0/tests/cached_data.npy
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scinumtools-1.1.0/tests/test_data.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.1.0/tests/test_stats.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.1.0/tests/test_struct.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.1.0/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.1.0/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.1.1/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.1.1/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/phys/units/DIP_Solver_Units.py
+-rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0    10693 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.1.1/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.1.1/tests/cached_data.npy
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 scinumtools-1.1.1/tests/test_data.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scinumtools-1.1.1/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.1.1/tests/test_stats.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.1.1/tests/test_struct.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 scinumtools-1.1.1/tests/test_units.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.1.1/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.1.1/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.1.1/PKG-INFO
```

### Comparing `scinumtools-1.1.0/.github/workflows/python-publish.yml` & `scinumtools-1.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.0/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.1.1/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.0/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.1.1/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.0/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.1.1/src/scinumtools/structs/ParameterClass.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,44 +52,47 @@
     def items(self):
         return [(key,value) for key,value in enumerate(self._data)]
 
 @dataclass
 class ParameterDict:
     """ ParameterDict class collects parameters in a concise form and create a dictionary
     """
-    _items: list
+    _keys: list
     _settings: list
     _data: dict
 
     def __init__(self, settings: list, parameters: dict=None):
         self._settings = settings
         self._data = {}
-        self._items = []
+        self._keys = []
         if parameters:
             for key,values in parameters.items():
                 self.append(key, values)            
 
     def __enter__(self):
         return self
     
     def __exit__(self, type, value, tb):
         pass
     
     def __getitem__(self, key):
         if isinstance(key,int):
-            return self._data[self._items[key]]
+            return self._data[self._keys[key]]
         else:
             return self._data[key]
 
     def __setitem__(self, key, values):
         self.append(key, values)
 
+    def keys(self):
+        return self._keys
+        
     def items(self):
         return self._data.items()
 
     def append(self, key, values):
         if self._data is None:
             self._data = {}
         settings = ParameterSettings(dict(zip(self._settings, values)))
-        self._items.append(key)
+        self._keys.append(key)
         self._data[key] = settings
```

### Comparing `scinumtools-1.1.0/tests/test_data.py` & `scinumtools-1.1.1/tests/test_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,28 +25,60 @@
     data = read_data('foo2','bar2')
 
     assert data == dict(a='foo', b='bar')
 
 def test_normalizing():
 
     xlen = 10
-    ylen = 10
+    ylen = 20
     data = np.linspace(1,xlen*ylen,xlen*ylen).reshape(xlen,ylen) - 10
 
+    # Test only data
     with NormalizeData() as n:
         for row in data:
             n.append(row)
         linnorm = n.linnorm()
         lognorm = n.lognorm()
+        zranges = n.zranges()
 
     assert linnorm.vmin == -9.
-    assert linnorm.vmax == 90.0
+    assert linnorm.vmax == 190.0
     assert lognorm.vmin == 0
-    assert lognorm.vmax == 1.954242509439325
-
+    assert lognorm.vmax == 2.278753600952829
+    assert zranges.minpos == 1
+    assert zranges.min == -9
+    assert zranges.max == 190.0
+    
+    # Test data and x-axis
+    with NormalizeData(xaxis=True) as n:
+        for r,row in enumerate(data):
+            xdata = np.linspace(-r,r,xlen)
+            n.append(row, xdata)
+        xranges = n.xranges()
+
+    assert xranges.minpos == 0.11111111111111116
+    assert xranges.min == -9
+    assert xranges.max == 9
+
+    # Test data and both axes
+    with NormalizeData(xaxis=True, yaxis=True) as n:
+        for r,row in enumerate(data):
+            xdata = np.linspace(-r,r,xlen)
+            ydata = np.linspace(-r*2,r*2,ylen)
+            n.append(row, xdata, ydata)
+        xranges = n.xranges()
+        yranges = n.yranges()
+
+    assert xranges.minpos == 0.11111111111111116
+    assert xranges.min == -9
+    assert xranges.max == 9
+    assert yranges.minpos == 0.10526315789473673
+    assert yranges.min == -18
+    assert yranges.max == 18
+    
 def test_list_to_grid():
 
     data = range(7)
     ncols = 2
     grid = []
     for row in ListToGrid(data,ncols):
         grid.append(row)
```

### Comparing `scinumtools-1.1.0/tests/test_stats.py` & `scinumtools-1.1.1/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.0/tests/test_struct.py` & `scinumtools-1.1.1/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.0/.gitignore` & `scinumtools-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.1.0/pyproject.toml` & `scinumtools-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.1.0/PKG-INFO` & `scinumtools-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

