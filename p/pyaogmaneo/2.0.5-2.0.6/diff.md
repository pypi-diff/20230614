# Comparing `tmp/pyaogmaneo-2.0.5.tar.gz` & `tmp/pyaogmaneo-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.0.5.tar", last modified: Mon Jun 12 22:04:58 2023, max compression
+gzip compressed data, was "pyaogmaneo-2.0.6.tar", last modified: Wed Jun 14 18:13:00 2023, max compression
```

## Comparing `pyaogmaneo-2.0.5.tar` & `pyaogmaneo-2.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.5/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-06-12 22:02:11.000000 pyaogmaneo-2.0.5/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.5/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.5/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-05-18 17:15:10.000000 pyaogmaneo-2.0.5/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-12 22:04:58.000000 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-06-12 22:04:58.000000 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-12 22:04:58.000000 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-06-12 22:04:58.000000 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.5/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-06-12 22:01:38.000000 pyaogmaneo-2.0.5/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-12 22:04:58.814855 pyaogmaneo-2.0.5/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-09 23:28:26.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-09 23:43:55.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)    15208 2023-06-12 02:04:51.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     6938 2023-06-12 22:02:24.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8183 2023-06-12 01:45:03.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-06-12 22:02:33.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8963 2023-06-12 01:45:03.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/CMake/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.6/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-06-14 18:10:02.000000 pyaogmaneo-2.0.6/CMakeLists.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.6/LICENSE.md
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.6/MANIFEST.in
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-05-18 17:15:10.000000 pyaogmaneo-2.0.6/README.md
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-14 18:13:00.000000 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-06-14 18:13:00.000000 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-14 18:13:00.000000 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-06-14 18:13:00.000000 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.6/pyproject.toml
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/setup.cfg
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-06-14 18:10:12.000000 pyaogmaneo-2.0.6/setup.py
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/source/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/source/pyaogmaneo/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-09 23:28:26.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-09 23:43:55.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    15208 2023-06-12 02:04:51.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     6938 2023-06-12 22:02:24.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8183 2023-06-12 01:45:03.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-06-12 22:02:33.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8963 2023-06-12 01:45:03.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.0.5/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.0.6/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.5/CMakeLists.txt` & `pyaogmaneo-2.0.6/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 39b1c24a17f0330b44b4194f084086378115f8fc
+        GIT_TAG ade5d3b08d2d2897a38dc010bb911f5f46af3929
     )
 
     FetchContent_GetProperties(AOgmaNeo)
 
     if(NOT AOgmaNeo_POPULATED)
         FetchContent_Populate(AOgmaNeo)
         add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
```

### Comparing `pyaogmaneo-2.0.5/LICENSE.md` & `pyaogmaneo-2.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.5/PKG-INFO` & `pyaogmaneo-2.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.5/README.md` & `pyaogmaneo-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.5/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.0.6/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.5/setup.py` & `pyaogmaneo-2.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.0.5",
+    version="2.0.6",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.0.5/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.0.6/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.5/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.0.6/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.5/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.0.6/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.5/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.0.6/source/pyaogmaneo/py_hierarchy.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.5/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.0.6/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.5/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.0.6/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.5/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.0.6/source/pyaogmaneo/py_module.cpp`

 * *Files identical despite different names*

