# Comparing `tmp/eudist-0.1.5.tar.gz` & `tmp/eudist-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eudist-0.1.5.tar", last modified: Wed Nov  2 12:16:21 2022, max compression
+gzip compressed data, was "eudist-0.1.6.tar", last modified: Wed Jun 14 11:54:38 2023, max compression
```

## Comparing `eudist-0.1.5.tar` & `eudist-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-02 12:16:21.652666 eudist-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     1425 2022-11-02 08:51:47.000000 eudist-0.1.5/.build-wheels.sh
--rw-rw-rw-   0 root         (0) root         (0)      117 2022-11-02 08:36:24.000000 eudist-0.1.5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2677 2022-11-02 11:07:55.000000 eudist-0.1.5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-10-10 13:02:49.000000 eudist-0.1.5/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       16 2022-10-10 13:02:49.000000 eudist-0.1.5/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      466 2022-10-10 13:02:49.000000 eudist-0.1.5/Makefile
--rw-r--r--   0 root         (0) root         (0)     1495 2022-11-02 12:16:21.652666 eudist-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      446 2022-10-10 13:02:49.000000 eudist-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-02 12:16:21.652666 eudist-0.1.5/docs/
--rw-rw-rw-   0 root         (0) root         (0)     5976 2022-11-02 08:36:24.000000 eudist-0.1.5/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2022-11-02 08:36:24.000000 eudist-0.1.5/docs/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-02 12:16:21.652666 eudist-0.1.5/eudist/
--rw-rw-rw-   0 root         (0) root         (0)     4713 2022-10-10 13:02:49.000000 eudist-0.1.5/eudist/point_plane.py
--rw-rw-rw-   0 root         (0) root         (0)     7192 2022-10-10 13:02:49.000000 eudist-0.1.5/eudist/test_point_plane.py
--rw-rw-rw-   0 root         (0) root         (0)     1909 2022-10-10 13:02:49.000000 eudist-0.1.5/eudist/test_polymesh.py
--rw-rw-rw-   0 root         (0) root         (0)     2497 2022-10-10 13:02:49.000000 eudist-0.1.5/eudist/test_seqment.py
--rw-r--r--   0 root         (0) root         (0)   506215 2022-11-02 12:16:21.000000 eudist-0.1.5/eudist.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-02 12:16:21.652666 eudist-0.1.5/eudist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1495 2022-11-02 12:16:21.000000 eudist-0.1.5/eudist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2022-11-02 12:16:21.000000 eudist-0.1.5/eudist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-02 12:16:21.000000 eudist-0.1.5/eudist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-11-02 12:16:21.000000 eudist-0.1.5/eudist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-11-02 12:16:21.000000 eudist-0.1.5/eudist.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5209 2022-11-02 08:36:24.000000 eudist-0.1.5/eudist.pyx
--rw-rw-rw-   0 root         (0) root         (0)     6782 2022-10-10 13:02:49.000000 eudist-0.1.5/eudist_cpp.cxx
--rw-rw-rw-   0 root         (0) root         (0)      835 2022-10-10 13:02:49.000000 eudist-0.1.5/eudist_cpp.hxx
--rw-rw-rw-   0 root         (0) root         (0)      527 2022-10-10 13:02:49.000000 eudist-0.1.5/eudist_cpp.pxd
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-11-02 10:26:30.000000 eudist-0.1.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       62 2022-11-02 10:27:20.000000 eudist-0.1.5/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1347 2022-11-02 12:16:21.656666 eudist-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1415 2022-11-02 10:32:13.000000 eudist-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 11:54:38.862602 eudist-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-06-14 10:03:56.000000 eudist-0.1.6/.build-wheels.sh
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-13 15:34:21.000000 eudist-0.1.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2704 2023-06-14 08:36:01.000000 eudist-0.1.6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-13 15:34:21.000000 eudist-0.1.6/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-06-13 15:34:21.000000 eudist-0.1.6/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-13 15:34:21.000000 eudist-0.1.6/Makefile
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-14 11:54:38.862602 eudist-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-06-13 15:34:21.000000 eudist-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 11:54:38.858602 eudist-0.1.6/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     5976 2023-06-13 15:34:21.000000 eudist-0.1.6/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-13 15:34:21.000000 eudist-0.1.6/docs/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 11:54:38.862602 eudist-0.1.6/eudist/
+-rw-rw-rw-   0 root         (0) root         (0)     4713 2023-06-13 15:34:21.000000 eudist-0.1.6/eudist/point_plane.py
+-rw-rw-rw-   0 root         (0) root         (0)     7192 2023-06-13 15:34:21.000000 eudist-0.1.6/eudist/test_point_plane.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-06-13 15:34:21.000000 eudist-0.1.6/eudist/test_polymesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     2497 2023-06-13 15:34:21.000000 eudist-0.1.6/eudist/test_seqment.py
+-rw-r--r--   0 root         (0) root         (0)   508777 2023-06-14 11:54:38.000000 eudist-0.1.6/eudist.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 11:54:38.862602 eudist-0.1.6/eudist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-14 11:54:38.000000 eudist-0.1.6/eudist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-06-14 11:54:38.000000 eudist-0.1.6/eudist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 11:54:38.000000 eudist-0.1.6/eudist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-14 11:54:38.000000 eudist-0.1.6/eudist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-14 11:54:38.000000 eudist-0.1.6/eudist.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5209 2023-06-13 15:34:21.000000 eudist-0.1.6/eudist.pyx
+-rw-rw-rw-   0 root         (0) root         (0)     7270 2023-06-13 15:34:21.000000 eudist-0.1.6/eudist_cpp.cxx
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-13 15:34:21.000000 eudist-0.1.6/eudist_cpp.hxx
+-rw-rw-rw-   0 root         (0) root         (0)      527 2023-06-13 15:34:21.000000 eudist-0.1.6/eudist_cpp.pxd
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-06-13 15:34:21.000000 eudist-0.1.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-13 15:34:21.000000 eudist-0.1.6/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-06-14 11:54:38.862602 eudist-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-13 15:34:21.000000 eudist-0.1.6/setup.py
```

### Comparing `eudist-0.1.5/.build-wheels.sh` & `eudist-0.1.6/.build-wheels.sh`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,23 @@
     if ! auditwheel show "$wheel"; then
         echo "Skipping non-platform wheel $wheel"
     else
         auditwheel repair "$wheel" --plat "$PLAT" -w /io/wheelhouse/
     fi
 }
 
+SKIP=3.12
+
 for PYBIN in /opt/python/cp3*/bin;
 do
     npv=1.15
     test $($PYBIN/python -V |grep 3.. -o) == 3.9 && npv=1.18
     test $($PYBIN/python -V |grep 3... -o) == 3.10 && npv=1.21
     test $($PYBIN/python -V |grep 3... -o) == 3.11 && npv=1.22
+    test $($PYBIN/python -V |grep 3... -o) == $SKIP && continue
     $PYBIN/pip install numpy==$npv cython setuptools_scm
     git checkout -- setup.cfg
     export SETUPTOOLS_SCM_PRETEND_VERSION=$($PYBIN/python3 -c 'from setuptools_scm import get_version ;print(get_version("."))')
     sed -e "s/numpy.*/numpy>=$($PYBIN/python -c 'from numpy.version import version; print(version)')/" -i setup.cfg
     grep numpy setup.cfg
     PY=$PYBIN/python make
     "${PYBIN}/pip" wheel . --no-deps -w wheelhouse/
@@ -31,14 +34,15 @@
 for whl in wheelhouse/*.whl; do
     LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$(pwd)/../../../lib/ repair_wheel "$whl"
 done
 
 ls -l /io/wheelhouse
 
 for PYBIN in /opt/python/cp3*/bin/; do
+    test $($PYBIN/python -V |grep 3... -o) == $SKIP && continue
     "${PYBIN}/pip" install $NAME --no-index -f /io/wheelhouse
     if test -e "${PYBIN}/nosetests"
     then
 	(
 	    cd "$HOME"
 	    "${PYBIN}/nosetests" $NAME
 	)
```

### Comparing `eudist-0.1.5/.gitlab-ci.yml` & `eudist-0.1.6/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     - python setup.py build_ext --inplace
     - ls -l
     - ls -l eudist/
     - python -m pytest
   parallel:
     matrix:
       - image: python:latest
+      - image: python:3.12
       - image: python:3.11
       - image: python:3.10
       - image: python:3.9
       - image: python:3.8
       - image: python:3.7
       - image: python:3.6
```

### Comparing `eudist-0.1.5/COPYING` & `eudist-0.1.6/COPYING`

 * *Files identical despite different names*

### Comparing `eudist-0.1.5/PKG-INFO` & `eudist-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eudist
-Version: 0.1.5
+Version: 0.1.6
 Summary: Calculate distances between simple shapes such as polygons.
 Home-page: https://github.com/dschwoerer/eudist
 Author: David Bold
 Author-email: dave@ipp.mpg.de
 License: GPL
 Project-URL: Bug Tracker, https://github.com/dschwoerer/eudist/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `eudist-0.1.5/docs/conf.py` & `eudist-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eudist-0.1.5/eudist/point_plane.py` & `eudist-0.1.6/eudist/point_plane.py`

 * *Files identical despite different names*

### Comparing `eudist-0.1.5/eudist/test_point_plane.py` & `eudist-0.1.6/eudist/test_point_plane.py`

 * *Files identical despite different names*

### Comparing `eudist-0.1.5/eudist/test_polymesh.py` & `eudist-0.1.6/eudist/test_polymesh.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,17 +20,15 @@
         p += self.off1[slc]
         p = np.matmul(self.rot, p)
         p += self.off2[slc]
         p = p.reshape(shp)
         return p
 
 
-def test_polymesh_1():
-    nx = 5
-    ny = 7
+def do_test_polymesh_1(nx=5, ny=7, iter=10):
     x = np.arange(nx + 1)[:, None] * np.ones((nx + 1, ny + 1))
     y = np.arange(ny + 1)[None, :] * np.ones((nx + 1, ny + 1))
     mesh = np.array([x, y])  # .flatten(), y.flatten()])
     trans = Transform(2)
     mesh = trans(mesh)
     cx, cy = np.random.randint(nx), np.random.randint(ny)
     cell0 = np.array([[cx, cy], [cx, cy + 1.0], [cx + 1, cy + 1], [cx + 1, cy]]).T
@@ -39,24 +37,34 @@
     a = cell[:, 0]
     b = cell[:, 1] - a
     c = cell[:, 3] - a
     d = cell[:, 2] - a - b - c
     meshx, meshy = mesh
     mesh = eudist.PolyMesh(meshx, meshy)
 
-    for _ in range(10):
+    for _ in range(iter):
         xx, xy = np.random.rand(2) * 1.5 - 0.25
         pos = a + b * xx + c * xy + xx * xy * d
         isin = 0 <= xx <= 1 and 0 <= xy <= 1
         try:
             assert (mesh.find_cell(pos) == cellid) == isin
         except AssertionError:
             print(mesh.find_cell(pos), cellid, cx, cy, nx, ny)
             import matplotlib.pyplot as plt
 
             print(meshx.shape)
             data = ((x == cx) & (y == cy)).astype(int)
             plt.pcolormesh(meshx, meshy, data)
-            plt.scatter(pos[0], pos[1])
-            plt.plot(cell[0], cell[1])
+            plt.scatter(*pos)
+            plt.plot(*cell)
             plt.show()
             raise
+
+
+def test_polymesh_1():
+    do_test_polymesh_1()
+
+
+def test_polymesh_2():
+    for nx in [5, 7, 13, 128]:
+        for ny in [5, 7, 14, 64]:
+            do_test_polymesh_1(nx, ny, nx * ny)
```

### Comparing `eudist-0.1.5/eudist/test_seqment.py` & `eudist-0.1.6/eudist/test_seqment.py`

 * *Files identical despite different names*

### Comparing `eudist-0.1.5/eudist.cpp` & `eudist-0.1.6/eudist.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/usr/local/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
             "/usr/local/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
@@ -36,16 +36,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -105,24 +105,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -230,15 +234,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -269,15 +273,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -593,35 +597,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1492,26 +1496,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1737,22 +1741,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -2059,15 +2071,15 @@
 /* Implementation of 'eudist' */
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_ImportError;
 static const char __pyx_k_0[] = "0";
 static const char __pyx_k_1[] = "1";
-static const char __pyx_k_5[] = "5";
+static const char __pyx_k_6[] = "6";
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_c[] = "c";
 static const char __pyx_k__3[] = ", ";
 static const char __pyx_k__4[] = ") != (";
 static const char __pyx_k__5[] = ")";
 static const char __pyx_k_np[] = "np";
@@ -2090,15 +2102,15 @@
 static const char __pyx_k_pnts[] = "pnts";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_seq0[] = "seq0";
 static const char __pyx_k_seq1[] = "seq1";
 static const char __pyx_k_sqrt[] = "sqrt";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_vlen[] = "_vlen";
-static const char __pyx_k_0_1_5[] = "0.1.5";
+static const char __pyx_k_0_1_6[] = "0.1.6";
 static const char __pyx_k_Plane[] = "Plane";
 static const char __pyx_k_datax[] = "datax";
 static const char __pyx_k_datay[] = "datay";
 static const char __pyx_k_guess[] = "guess";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_order[] = "order";
 static const char __pyx_k_range[] = "range";
@@ -2145,17 +2157,17 @@
 static const char __pyx_k_PolyMesh___reduce_cython[] = "PolyMesh.__reduce_cython__";
 static const char __pyx_k_PolyMesh__eudist_dealloc[] = "PolyMesh._eudist_dealloc";
 static const char __pyx_k_PolyMesh___setstate_cython[] = "PolyMesh.__setstate_cython__";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static PyObject *__pyx_kp_u_0;
-static PyObject *__pyx_kp_u_0_1_5;
+static PyObject *__pyx_kp_u_0_1_6;
 static PyObject *__pyx_kp_u_1;
-static PyObject *__pyx_kp_u_5;
+static PyObject *__pyx_kp_u_6;
 static PyObject *__pyx_kp_u_Data_mismatch;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_n_s_Plane;
 static PyObject *__pyx_n_s_Plane___reduce_cython;
 static PyObject *__pyx_n_s_Plane___setstate_cython;
 static PyObject *__pyx_n_s_Plane__eudist_dealloc;
 static PyObject *__pyx_n_s_Plane_dist;
@@ -7256,15 +7268,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_6eudist_PolyMesh(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -7368,15 +7380,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -7420,17 +7432,17 @@
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_u_0, __pyx_k_0, sizeof(__pyx_k_0), 0, 1, 0, 0},
-  {&__pyx_kp_u_0_1_5, __pyx_k_0_1_5, sizeof(__pyx_k_0_1_5), 0, 1, 0, 0},
+  {&__pyx_kp_u_0_1_6, __pyx_k_0_1_6, sizeof(__pyx_k_0_1_6), 0, 1, 0, 0},
   {&__pyx_kp_u_1, __pyx_k_1, sizeof(__pyx_k_1), 0, 1, 0, 0},
-  {&__pyx_kp_u_5, __pyx_k_5, sizeof(__pyx_k_5), 0, 1, 0, 0},
+  {&__pyx_kp_u_6, __pyx_k_6, sizeof(__pyx_k_6), 0, 1, 0, 0},
   {&__pyx_kp_u_Data_mismatch, __pyx_k_Data_mismatch, sizeof(__pyx_k_Data_mismatch), 0, 1, 0, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_n_s_Plane, __pyx_k_Plane, sizeof(__pyx_k_Plane), 0, 0, 1, 1},
   {&__pyx_n_s_Plane___reduce_cython, __pyx_k_Plane___reduce_cython, sizeof(__pyx_k_Plane___reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_Plane___setstate_cython, __pyx_k_Plane___setstate_cython, sizeof(__pyx_k_Plane___setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_Plane__eudist_dealloc, __pyx_k_Plane__eudist_dealloc, sizeof(__pyx_k_Plane__eudist_dealloc), 0, 0, 1, 1},
   {&__pyx_n_s_Plane_dist, __pyx_k_Plane_dist, sizeof(__pyx_k_Plane_dist), 0, 0, 1, 1},
@@ -7785,29 +7797,29 @@
   __pyx_tuple__43 = PyTuple_Pack(11, __pyx_n_s_seq0, __pyx_n_s_seq1, __pyx_n_s_eps, __pyx_n_s_v0, __pyx_n_s_v1, __pyx_n_s_p0, __pyx_n_s_p1, __pyx_n_s_dist, __pyx_n_s_det1, __pyx_n_s_t0, __pyx_n_s_t1); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
   __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_eudist_pyx, __pyx_n_s_do_seg_seg_intersect, 141, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(1, 141, __pyx_L1_error)
 
   /* "eudist/_version.py":5
  * # don't change, don't track in version control
- * __version__ = version = '0.1.5'
- * __version_tuple__ = version_tuple = ('0', '1', '5')             # <<<<<<<<<<<<<<
+ * __version__ = version = '0.1.6'
+ * __version_tuple__ = version_tuple = ('0', '1', '6')             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__45 = PyTuple_Pack(3, __pyx_kp_u_0, __pyx_kp_u_1, __pyx_kp_u_5); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(4, 5, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(3, __pyx_kp_u_0, __pyx_kp_u_1, __pyx_kp_u_6); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(4, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -7881,55 +7893,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -8113,15 +8109,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_eudist) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -8367,24 +8363,24 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_do_seg_seg_intersect, __pyx_t_1) < 0) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "eudist/_version.py":4
  * # file generated by setuptools_scm
  * # don't change, don't track in version control
- * __version__ = version = '0.1.5'             # <<<<<<<<<<<<<<
- * __version_tuple__ = version_tuple = ('0', '1', '5')
+ * __version__ = version = '0.1.6'             # <<<<<<<<<<<<<<
+ * __version_tuple__ = version_tuple = ('0', '1', '6')
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_1_5) < 0) __PYX_ERR(4, 4, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version_2, __pyx_kp_u_0_1_5) < 0) __PYX_ERR(4, 4, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_1_6) < 0) __PYX_ERR(4, 4, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version_2, __pyx_kp_u_0_1_6) < 0) __PYX_ERR(4, 4, __pyx_L1_error)
 
   /* "eudist/_version.py":5
  * # don't change, don't track in version control
- * __version__ = version = '0.1.5'
- * __version_tuple__ = version_tuple = ('0', '1', '5')             # <<<<<<<<<<<<<<
+ * __version__ = version = '0.1.6'
+ * __version_tuple__ = version_tuple = ('0', '1', '6')             # <<<<<<<<<<<<<<
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_version_tuple, __pyx_tuple__45) < 0) __PYX_ERR(4, 5, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_version_tuple_2, __pyx_tuple__45) < 0) __PYX_ERR(4, 5, __pyx_L1_error)
 
   /* "eudist.pyx":1
  * # distutils: language=c++             # <<<<<<<<<<<<<<
  * # distutils: include_dirs =
@@ -9564,17 +9560,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -9732,28 +9726,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -10255,61 +10249,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -10916,17 +10928,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -10993,15 +11010,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -11045,15 +11065,15 @@
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -11443,15 +11463,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -11597,15 +11617,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -11682,15 +11702,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -11878,15 +11898,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `eudist-0.1.5/eudist.egg-info/PKG-INFO` & `eudist-0.1.6/eudist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eudist
-Version: 0.1.5
+Version: 0.1.6
 Summary: Calculate distances between simple shapes such as polygons.
 Home-page: https://github.com/dschwoerer/eudist
 Author: David Bold
 Author-email: dave@ipp.mpg.de
 License: GPL
 Project-URL: Bug Tracker, https://github.com/dschwoerer/eudist/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `eudist-0.1.5/eudist.pyx` & `eudist-0.1.6/eudist.pyx`

 * *Files identical despite different names*

### Comparing `eudist-0.1.5/eudist_cpp.cxx` & `eudist-0.1.6/eudist_cpp.cxx`

 * *Files 2% similar despite different names*

```diff
@@ -211,54 +211,78 @@
       }
     }
     return min;
   }
   return plane.dist(dot);
 }
 
+void PolyMesh::add_to_outer(int &pos, int i, int j) {
+  int iin = i * ny + j;
+  outer[pos++] = datax[iin];
+  outer[pos++] = datay[iin];
+};
+
 PolyMesh::PolyMesh(const double *datax, const double *datay, int nx, int ny)
     : nx(nx), ny(ny), datax(datax), datay(datay),
       num_cells((nx - 1) * (ny - 1)) {
   bounds = new double[num_cells * 2 * 4];
+  outer = new double[(nx + ny) * 2 * 2];
   int pos = 0;
   for (int i = 0; i < nx - 1; ++i) {
     for (int j = 0; j < ny - 1; ++j) {
       int iin = i * ny + j;
       bounds[pos++] = datax[iin];
       bounds[pos++] = datay[iin];
       bounds[pos++] = datax[iin + 1];
       bounds[pos++] = datay[iin + 1];
-      bounds[pos++] = datax[iin + ny+1];
-      bounds[pos++] = datay[iin + ny+1];
+      bounds[pos++] = datax[iin + ny + 1];
+      bounds[pos++] = datay[iin + ny + 1];
       bounds[pos++] = datax[iin + ny];
       bounds[pos++] = datay[iin + ny];
     }
   }
-  // printf("%d %d=%d\n",num_cells, num_cells*8, pos);
-  // assert(num_cells * 8 == pos);
+  {
+    int pos = 0;
+    int i = 0;
+    int j = 0;
+    for (; i < nx - 1; ++i) {
+      add_to_outer(pos, i, j);
+    }
+    for (; j < ny - 1; ++j) {
+      add_to_outer(pos, i, j);
+    }
+    for (; i > 0; --i) {
+      add_to_outer(pos, i, j);
+    }
+    for (; j > 0; --j) {
+      add_to_outer(pos, i, j);
+    }
+  }
 }
 
-PolyMesh::~PolyMesh(){
-  delete[] bounds;
-}
+PolyMesh::~PolyMesh() { delete[] bounds; }
 
 int PolyMesh::find_cell(const double *dot, int guess) {
   if (guess >= 0) {
     for (int i = -1; i < 2; ++i) {
       for (int j = -1; j < 2; ++j) {
-        int pos = guess + i + (ny -1) * j;
+        int pos = guess + i + (ny - 1) * j;
         if (pos >= 0 and pos < num_cells) {
           if (winding_number(bounds + pos * 8, dot, 4)) {
             return pos;
           }
         }
       }
     }
   }
 
+  if (winding_number(outer, dot, (nx + ny - 2) * 2) == 0) {
+    return -1;
+  }
+
   for (int pos = 0; pos < num_cells; ++pos) {
     if (winding_number(bounds + pos * 8, dot, 4)) {
       return pos;
     }
   }
   return -1;
 }
```

### Comparing `eudist-0.1.5/eudist_cpp.hxx` & `eudist-0.1.6/eudist_cpp.hxx`

 * *Files 22% similar despite different names*

```diff
@@ -33,9 +33,11 @@
 
 private:
   const int nx;
   const int ny;
   const double *datax;
   const double *datay;
   const int num_cells;
-  double *bounds;
+  double *bounds{nullptr};
+  double *outer{nullptr};
+  void add_to_outer(int &pos, int i, int j);
 };
```

### Comparing `eudist-0.1.5/eudist_cpp.pxd` & `eudist-0.1.6/eudist_cpp.pxd`

 * *Files identical despite different names*

### Comparing `eudist-0.1.5/setup.cfg` & `eudist-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `eudist-0.1.5/setup.py` & `eudist-0.1.6/setup.py`

 * *Files identical despite different names*

