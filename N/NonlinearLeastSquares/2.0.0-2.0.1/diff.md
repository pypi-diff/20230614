# Comparing `tmp/NonlinearLeastSquares-2.0.0.tar.gz` & `tmp/NonlinearLeastSquares-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NonlinearLeastSquares-2.0.0.tar", last modified: Fri Nov  9 18:38:52 2018, max compression
+gzip compressed data, was "NonlinearLeastSquares-2.0.1.tar", last modified: Thu Oct  6 05:17:54 2022, max compression
```

## Comparing `NonlinearLeastSquares-2.0.0.tar` & `NonlinearLeastSquares-2.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 kak       (1000) kak       (1000)        0 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/
-drwxr-xr-x   0 kak       (1000) kak       (1000)        0 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/TestNonlinearLeastSquares/
--rw-r--r--   0 kak       (1000) kak       (1000)    16406 2018-11-09 17:45:58.000000 NonlinearLeastSquares-2.0.0/TestNonlinearLeastSquares/OptimizedSurfaceFit.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      657 2016-12-01 23:35:09.000000 NonlinearLeastSquares-2.0.0/TestNonlinearLeastSquares/Test.py
--rw-r--r--   0 kak       (1000) kak       (1000)     1568 2018-10-10 05:19:02.000000 NonlinearLeastSquares-2.0.0/TestNonlinearLeastSquares/TestNonlinearLeastSquaresCalculation.py
--rw-r--r--   0 kak       (1000) kak       (1000)   141107 2018-11-09 17:45:48.000000 NonlinearLeastSquares-2.0.0/TestNonlinearLeastSquares/NonlinearLeastSquares.py
-drwxr-xr-x   0 kak       (1000) kak       (1000)        0 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/ExamplesStructureFromCameraMotion/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    10600 2018-11-09 17:11:01.000000 NonlinearLeastSquares-2.0.0/ExamplesStructureFromCameraMotion/bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)     9393 2018-11-09 17:21:53.000000 NonlinearLeastSquares-2.0.0/ExamplesStructureFromCameraMotion/sfm_with_uncalibrated_cameras_translations_only.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)    10746 2018-11-09 17:18:38.000000 NonlinearLeastSquares-2.0.0/ExamplesStructureFromCameraMotion/sfm_with_calibrated_cameras_translations_only.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2549 2018-11-09 14:21:19.000000 NonlinearLeastSquares-2.0.0/ExamplesStructureFromCameraMotion/README
-drwxr-xr-x   0 kak       (1000) kak       (1000)        0 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/NonlinearLeastSquares/
--rw-r--r--   0 kak       (1000) kak       (1000)   140981 2018-11-09 18:31:47.000000 NonlinearLeastSquares-2.0.0/NonlinearLeastSquares/NonlinearLeastSquares.py
--rw-rw-r--   0 kak       (1000) kak       (1000)      814 2016-11-28 03:56:34.000000 NonlinearLeastSquares-2.0.0/NonlinearLeastSquares/__init__.py
--rw-r--r--   0 kak       (1000) kak       (1000)     1239 2016-12-01 23:43:52.000000 NonlinearLeastSquares-2.0.0/Makefile
--rw-r--r--   0 kak       (1000) kak       (1000)       38 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/setup.cfg
-drwxr-xr-x   0 kak       (1000) kak       (1000)        0 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/NonlinearLeastSquares.egg-info/
--rw-r--r--   0 kak       (1000) kak       (1000)       59 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/NonlinearLeastSquares.egg-info/top_level.txt
--rw-r--r--   0 kak       (1000) kak       (1000)        1 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/NonlinearLeastSquares.egg-info/dependency_links.txt
--rw-r--r--   0 kak       (1000) kak       (1000)     6051 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/NonlinearLeastSquares.egg-info/PKG-INFO
--rw-r--r--   0 kak       (1000) kak       (1000)     1236 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/NonlinearLeastSquares.egg-info/SOURCES.txt
--rw-r--r--   0 kak       (1000) kak       (1000)     6051 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/PKG-INFO
--rw-r--r--   0 kak       (1000) kak       (1000)     1029 2018-10-10 05:25:42.000000 NonlinearLeastSquares-2.0.0/README
--rw-r--r--   0 kak       (1000) kak       (1000)     1249 2018-11-09 18:07:58.000000 NonlinearLeastSquares-2.0.0/MANIFEST.in
--rwxr-xr-x   0 kak       (1000) kak       (1000)     5545 2018-11-09 18:04:05.000000 NonlinearLeastSquares-2.0.0/setup.py
-drwxr-xr-x   0 kak       (1000) kak       (1000)        0 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/OptimizedSurfaceFit/
--rw-r--r--   0 kak       (1000) kak       (1000)    16437 2018-11-09 17:54:26.000000 NonlinearLeastSquares-2.0.0/OptimizedSurfaceFit/OptimizedSurfaceFit.py
--rw-rw-r--   0 kak       (1000) kak       (1000)      807 2018-10-10 00:57:15.000000 NonlinearLeastSquares-2.0.0/OptimizedSurfaceFit/__init__.py
-drwxr-xr-x   0 kak       (1000) kak       (1000)        0 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/
--rwxrwxr-x   0 kak       (1000) kak       (1000)     5940 2018-10-10 01:22:11.000000 NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/grad_descent_with_partial_derivatives.py
--rwxrwxr-x   0 kak       (1000) kak       (1000)     6040 2018-10-10 01:21:37.000000 NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/leven_marq_with_partial_derivatives.py
--rwxrwxr-x   0 kak       (1000) kak       (1000)     5110 2018-10-10 02:35:45.000000 NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/leven_marq.py
--rw-rw-r--   0 kak       (1000) kak       (1000)     3148 2018-10-10 01:24:09.000000 NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/README
--rwxrwxr-x   0 kak       (1000) kak       (1000)     5136 2018-10-10 01:17:02.000000 NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/grad_descent.py
-drwxr-xr-x   0 kak       (1000) kak       (1000)        0 2018-11-09 18:38:52.000000 NonlinearLeastSquares-2.0.0/ProjectiveCamera/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    78309 2018-11-09 17:54:39.000000 NonlinearLeastSquares-2.0.0/ProjectiveCamera/ProjectiveCamera.py
--rw-r--r--   0 kak       (1000) kak       (1000)      792 2018-10-03 14:25:08.000000 NonlinearLeastSquares-2.0.0/ProjectiveCamera/__init__.py
--rw-r--r--   0 kak       (1000) kak       (1000)   178642 2018-11-09 18:28:16.000000 NonlinearLeastSquares-2.0.0/NonlinearLeastSquares-2.0.0.html
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-10-06 05:17:54.042773 NonlinearLeastSquares-2.0.1/
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-10-06 05:17:54.042773 NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/
+-rw-rw-r--   0 kak       (1000) avi       (1000)     3148 2018-10-10 01:24:09.000000 NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/README
+-rwxrwxr-x   0 kak       (1000) avi       (1000)     5136 2018-10-10 01:17:02.000000 NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/grad_descent.py
+-rwxrwxr-x   0 kak       (1000) avi       (1000)     5940 2018-10-10 01:22:11.000000 NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/grad_descent_with_partial_derivatives.py
+-rwxrwxr-x   0 kak       (1000) avi       (1000)     5110 2018-10-10 02:35:45.000000 NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/leven_marq.py
+-rwxrwxr-x   0 kak       (1000) avi       (1000)     6040 2018-10-10 01:21:37.000000 NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/leven_marq_with_partial_derivatives.py
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-10-06 05:17:54.042773 NonlinearLeastSquares-2.0.1/ExamplesStructureFromCameraMotion/
+-rw-r--r--   0 kak       (1000) avi       (1000)     2549 2018-11-09 14:21:19.000000 NonlinearLeastSquares-2.0.1/ExamplesStructureFromCameraMotion/README
+-rwxr-xr-x   0 kak       (1000) avi       (1000)    10600 2018-11-09 17:11:01.000000 NonlinearLeastSquares-2.0.1/ExamplesStructureFromCameraMotion/bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py
+-rwxr-xr-x   0 kak       (1000) avi       (1000)    10746 2018-11-09 17:18:38.000000 NonlinearLeastSquares-2.0.1/ExamplesStructureFromCameraMotion/sfm_with_calibrated_cameras_translations_only.py
+-rwxr-xr-x   0 kak       (1000) avi       (1000)     9393 2018-11-09 17:21:53.000000 NonlinearLeastSquares-2.0.1/ExamplesStructureFromCameraMotion/sfm_with_uncalibrated_cameras_translations_only.py
+-rw-r--r--   0 kak       (1000) avi       (1000)     1249 2022-10-06 04:45:36.000000 NonlinearLeastSquares-2.0.1/MANIFEST.in
+-rw-r--r--   0 kak       (1000) avi       (1000)     1250 2022-10-06 04:44:54.000000 NonlinearLeastSquares-2.0.1/Makefile
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-10-06 05:17:54.042773 NonlinearLeastSquares-2.0.1/NonlinearLeastSquares/
+-rw-r--r--   0 kak       (1000) avi       (1000)   145199 2022-10-06 04:23:03.000000 NonlinearLeastSquares-2.0.1/NonlinearLeastSquares/NonlinearLeastSquares.py
+-rw-rw-r--   0 kak       (1000) avi       (1000)      814 2016-11-28 03:56:34.000000 NonlinearLeastSquares-2.0.1/NonlinearLeastSquares/__init__.py
+-rw-r--r--   0 kak       (1000) avi       (1000)   185694 2022-10-06 05:10:01.000000 NonlinearLeastSquares-2.0.1/NonlinearLeastSquares-2.0.1.html
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-10-06 05:17:54.042773 NonlinearLeastSquares-2.0.1/NonlinearLeastSquares.egg-info/
+-rw-r--r--   0 kak       (1000) avi       (1000)     6049 2022-10-06 05:17:53.000000 NonlinearLeastSquares-2.0.1/NonlinearLeastSquares.egg-info/PKG-INFO
+-rw-r--r--   0 kak       (1000) avi       (1000)     1236 2022-10-06 05:17:53.000000 NonlinearLeastSquares-2.0.1/NonlinearLeastSquares.egg-info/SOURCES.txt
+-rw-r--r--   0 kak       (1000) avi       (1000)        1 2022-10-06 05:17:53.000000 NonlinearLeastSquares-2.0.1/NonlinearLeastSquares.egg-info/dependency_links.txt
+-rw-r--r--   0 kak       (1000) avi       (1000)       59 2022-10-06 05:17:53.000000 NonlinearLeastSquares-2.0.1/NonlinearLeastSquares.egg-info/top_level.txt
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-10-06 05:17:54.042773 NonlinearLeastSquares-2.0.1/OptimizedSurfaceFit/
+-rw-r--r--   0 kak       (1000) avi       (1000)    16666 2022-10-06 00:52:57.000000 NonlinearLeastSquares-2.0.1/OptimizedSurfaceFit/OptimizedSurfaceFit.py
+-rw-rw-r--   0 kak       (1000) avi       (1000)      807 2018-10-10 00:57:15.000000 NonlinearLeastSquares-2.0.1/OptimizedSurfaceFit/__init__.py
+-rw-r--r--   0 kak       (1000) avi       (1000)     6049 2022-10-06 05:17:54.042773 NonlinearLeastSquares-2.0.1/PKG-INFO
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-10-06 05:17:54.042773 NonlinearLeastSquares-2.0.1/ProjectiveCamera/
+-rwxr-xr-x   0 kak       (1000) avi       (1000)    79316 2022-10-06 04:26:10.000000 NonlinearLeastSquares-2.0.1/ProjectiveCamera/ProjectiveCamera.py
+-rw-r--r--   0 kak       (1000) avi       (1000)      792 2018-10-03 14:25:08.000000 NonlinearLeastSquares-2.0.1/ProjectiveCamera/__init__.py
+-rw-r--r--   0 kak       (1000) avi       (1000)     1029 2018-10-10 05:25:42.000000 NonlinearLeastSquares-2.0.1/README
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-10-06 05:17:54.042773 NonlinearLeastSquares-2.0.1/TestNonlinearLeastSquares/
+-rw-r--r--   0 kak       (1000) avi       (1000)   145199 2022-10-06 04:27:33.000000 NonlinearLeastSquares-2.0.1/TestNonlinearLeastSquares/NonlinearLeastSquares.py
+-rw-r--r--   0 kak       (1000) avi       (1000)    16666 2022-10-06 04:32:58.000000 NonlinearLeastSquares-2.0.1/TestNonlinearLeastSquares/OptimizedSurfaceFit.py
+-rwxr-xr-x   0 kak       (1000) avi       (1000)      657 2016-12-01 23:35:09.000000 NonlinearLeastSquares-2.0.1/TestNonlinearLeastSquares/Test.py
+-rw-r--r--   0 kak       (1000) avi       (1000)     1568 2018-10-10 05:19:02.000000 NonlinearLeastSquares-2.0.1/TestNonlinearLeastSquares/TestNonlinearLeastSquaresCalculation.py
+-rw-r--r--   0 kak       (1000) avi       (1000)       38 2022-10-06 05:17:54.042773 NonlinearLeastSquares-2.0.1/setup.cfg
+-rwxr-xr-x   0 kak       (1000) avi       (1000)     5530 2022-10-06 00:42:19.000000 NonlinearLeastSquares-2.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `NonlinearLeastSquares-2.0.0/TestNonlinearLeastSquares/OptimizedSurfaceFit.py` & `NonlinearLeastSquares-2.0.1/OptimizedSurfaceFit/OptimizedSurfaceFit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #from NonlinearLeastSquares import NonlinearLeastSquares
 
 ##  OptimizedSurfaceFit.py
+##  Main Module Version: 2.0.1
 
 ##  OptimizedSurfaceFit is a part of the Avi Kak's NonlinearLeastSquares Python module
 ##  for demonstrating how the module can be used for optimized fitting of a surface 
 ##  (whose analytical form is known) to noisy data over a plane.
 
 ##  The goal of OptimizedSurfaceFit is to fit a model surface to noisy height data
 ##  over the xy-plane in the xyz-coordinate frame, with the model surface being
@@ -165,15 +166,16 @@
             result_dict = self.optimizer.grad_descent()
         return result_dict
 
     def get_initial_params_from_file(self, filename):
         if not filename.endswith('.txt'): 
             sys.exit("Aborted. _get_initial_params_from_file() is only for CSV files")
         initial_params_dict = {}
-        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line is not '']
+#        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line is not '']
+        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line != '']
         for record in initial_params_list:
             initial_params_dict[record[:record.find('=')].rstrip()] = float(record[record.find('=')+1:].lstrip())
         self.params_dict = initial_params_dict
         self.params_ordered_list = sorted(self.params_dict)             #need ordered list for jacobian calculations
         return initial_params_dict
 
     def _get_measured_data_from_text_file(self, filename):
@@ -257,15 +259,16 @@
             w,h = self.display_size
             fig = plt.figure(figsize=(w,h))
         else:
             fig = plt.figure()
         new_error_norm_str = "%.4f" % new_error_norm
         fig.suptitle("iteration: " + str(iteration_index) + "     error: " + 
                                                      new_error_norm_str, fontsize=14, fontweight='bold')
-        ax = fig.gca(projection='3d')
+        ##   ax = fig.gca(projection='3d')                
+        ax = fig.add_subplot(111, projection='3d')  ## Version 2.0.1 fix for the above statement
         ## Version 1.5.0 fix:  xx, yy, and zz needed to be turned into numpy arrays
 #        surf = ax.plot_surface(xx, yy, zz, color="yellow")
         surf = ax.plot_surface(numpy.array(xx), numpy.array(yy), numpy.array(zz), color="yellow")
         ax.set_zlim(zmin, zmax)
         ax.scatter(xxx,yyy,zzz, c='r', marker='o')
         ax.set_xlabel("X")
         ax.set_ylabel("Y")
```

### Comparing `NonlinearLeastSquares-2.0.0/TestNonlinearLeastSquares/Test.py` & `NonlinearLeastSquares-2.0.1/TestNonlinearLeastSquares/Test.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/TestNonlinearLeastSquares/TestNonlinearLeastSquaresCalculation.py` & `NonlinearLeastSquares-2.0.1/TestNonlinearLeastSquares/TestNonlinearLeastSquaresCalculation.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/TestNonlinearLeastSquares/NonlinearLeastSquares.py` & `NonlinearLeastSquares-2.0.1/NonlinearLeastSquares/NonlinearLeastSquares.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 __author__  = "Avinash Kak (kak@purdue.edu)"
-__date__    = '2018-November-9'
-__url__     = 'https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.html'
-__copyright__ = "(C) 2018 Avinash Kak. Python Software Foundation."
+__date__    = '2022-October-6'
+__url__     = 'https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.html'
+__copyright__ = "(C) 2022 Avinash Kak. Python Software Foundation."
 
 
 __doc__ = '''
 
 NonlinearLeastSquares.py
 
 Version: ''' + __version__ + '''
@@ -15,14 +15,22 @@
 
 Date: ''' + __date__ + '''
 
 
 @title
 CHANGE LOG:
 
+  Version 2.0.1:
+
+    Cleaned up the code to make it work with the current version of the
+    matplotlib library that is used for displaying the results.  I have also
+    removed the use of the "is" and "is not" comparison operators for numeric
+    and string literals since such use has now been deprecated.  Also added
+    additional comment blocks to the main functions in the module file.
+
   Version 2.0.0:
 
     This version includes sparse bundle adjustment (SBA) to speed up code
     execution when using nonlinear least-squares for solving
     structure-from-camera-motion problems with uncalibrated cameras.  SBA
     exploits the sparseness of the Jacobian encountered in such problems.
     This version also includes improvements to the Levenberg-Marquardt code
@@ -31,47 +39,46 @@
     provides additional methods for the visualization of the results.
 
   Version 1.5.0:
 
     This version adds a new class, ProjectiveCamera, to the module for
     demonstrating how nonlinear least-squares can be used for estimating
     structure of a scene from the data recorded with a calibrated camera in
-    motion.  For a simulated demonstration, you can create calibrated
-    cameras from a generic instance of the ProjectiveCamera class that is
-    then subject to various translational and rotational transformations.
+    motion.  For a simulated demonstration, you can create calibrated cameras
+    from a generic instance of the ProjectiveCamera class that is then subject
+    to various translational and rotational transformations.
 
   Version 1.1.1:
 
     This version includes constructor options to control the size and the
     position of the graphics for displaying the results of nonlinear
     least-squares optimization.
 
   Version 1.1:
 
-    This version fixes a bug in the synthetic data generator function used
-    for illustrating the functionality of the NonlinearLeastSquares class.
-    Changes also made to the information that is printed out when the
-    module is run in the debug mode.
+    This version fixes a bug in the synthetic data generator function used for
+    illustrating the functionality of the NonlinearLeastSquares class.
+    Changes also made to the information that is printed out when the module
+    is run in the debug mode.
 
   Version 1.0:
 
-    In the form of a class named NonlinearLeastSquares, this module
-    provides a domain agnostic implementation of nonlinear least-squares
-    algorithms (gradient-descent and Levenberg-Marquardt) for fitting a
-    model to observed data.  Typically, the model involves several
-    parameters and each observed data element can be expressed as a
-    function of those parameters plus noise.  The goal of nonlinear
-    least-squares is to estimate the best values for the parameters given
-    all of the observed data.  In order to illustrate how to use the
-    NonlinearLeastSquares class, the module also comes with another class,
-    OptimizeSurfaceFit, whose job is to fit the best surface (of a
-    specified analytical form) to noisy height data over the XY-plane. The
-    model in this case is the analytical description of the surface and the
-    goal of nonlinear least-squares is to estimate the best values for the
-    parameters in the analytical description.
+    In the form of a class named NonlinearLeastSquares, this module provides a
+    domain agnostic implementation of nonlinear least-squares algorithms
+    (gradient-descent and Levenberg-Marquardt) for fitting a model to observed
+    data.  Typically, the model involves several parameters and each observed
+    data element can be expressed as a function of those parameters plus
+    noise.  The goal of nonlinear least-squares is to estimate the best values
+    for the parameters given all of the observed data.  In order to illustrate
+    how to use the NonlinearLeastSquares class, the module also comes with
+    another class, OptimizeSurfaceFit, whose job is to fit the best surface
+    (of a specified analytical form) to noisy height data over the
+    XY-plane. The model in this case is the analytical description of the
+    surface and the goal of nonlinear least-squares is to estimate the best
+    values for the parameters in the analytical description.
 
 
 @title
 USAGE FOR OPTIMAL SURFACE FITTING:
 
     The module includes a domain specific class, OptimizedSurfaceFit, for
     demonstrating how nonlinear least-squares in the form of the
@@ -220,24 +227,25 @@
         camera.construct_parameter_vec_for_uncalibrated_cameras_with_rodrigues_rotations()
                                                                           #(M)
         camera.construct_Fvec_for_bundle_adjustment()                     #(O)
         result = camera.get_scene_structure_from_camera_motion_with_bundle_adjustment()
                                                                           #(P)
 
     The construction of the observation vector X in line (L) is specific to
-    bundle adjustment --- in the sense that you first want to list the
-    pixels in all the cameras for the first world point, then you want to
-    list the pixels in all the cameras for the second world point, and so
-    on.  Ordering the observed data in this fashion is necessary to create
-    the sort of block sparsity in the Jacobian that is exploited in SBA.
+    sparse bundle adjustment --- in the sense that you first want to list
+    the pixels in all the cameras for the first world point, then you want
+    to list the pixels in all the cameras for the second world point, and
+    so on.  Ordering the observed data in this fashion is necessary to
+    create the sort of block sparsity in the Jacobian that is exploited in
+    SBA.
 
     Note that we assume that the intrinsic parameters of the camera are
     known already.  So the goal of the bundle adjustment is to estimate the
-    six extrinsic parameters, the three for translation of the camera and
-    the three (in the form of Rodrigues rotations) for the rotation.
+    six extrinsic parameters, three for translation of the camera and three
+    (in the form of Rodrigues rotations) for the rotation.
         
     See the script 
 
        bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py
 
     in the ExamplesStructureFromCameraMotion subdirectory of the
     distribution for further information on what calls you need to sequence
@@ -553,15 +561,15 @@
          implementation of the Levenberg-Marquardt algorithm and the second
          for the bundle-adjustment version of the same.  This is the data
          to which you which you want to fit a given model and you want
          NonlinearLeastSquares to estimate the best values for the
          parameters of the model.
 
 @title
-NonlinearLeastSquares -- OPTIMIZED SURFACE FITTING:
+OPTIMIZED SURFACE FITTING:
 
     This section presents a class named OptimizedSurfaceFit to illustrate
     how you can use the functionality of NonlinearLeastSquares in your own
     code.  The goal of OptimizedSurfaceFit is to fit a model surface to
     noisy height data over the xy-plane in the xyz-coordinate frame, with
     the model surface being described by a polynomial function.  Here are
     some examples of such polynomials:
@@ -820,16 +828,15 @@
             The responsibility of this method is to take all of the user
             supplied information and reconstitute it into a form that is
             needed by NonlinearLeastSquares taking into account the
             peculiarities of your domain.
 
 
 @title
-NonlinearLeastSquares -- ESTIMATING SCENE STRUCTURE WHEN USING A CALIBRATED 
-                         CAMERA IN MOTION:
+ESTIMATING SCENE STRUCTURE WHEN USING A CALIBRATED CAMERA IN MOTION:
 
     This section presents a class named ProjectiveCamera to illustrate how
     you can use the functionality of NonlinearLeastSquares in your own code
     for estimating the structure of a 3D scene from the data recorded by a
     calibrated camera in motion.
 
     To create a simulated structure-from-camera-motion demonstration with
@@ -1110,16 +1117,15 @@
             that is supplied to it as its argument. The argument
             'translation' consists of a triple of real numbers that stand
             for a displacement along the world-X, along the world-Y, and
             along the world-Z.
 
 
 @title
-NonlinearLeastSquares -- ESTIMATING SCENE STRUCTURE AND CAMERA PARAMETERS
-                         WHEN USING AN UNCALIBRATED CAMERA IN MOTION:
+ESTIMATING SCENE STRUCTURE AND CAMERA PARAMETERS WHEN USING AN UNCALIBRATED CAMERA IN MOTION:
     
     The problem of scene construction becomes a lot more challenging when
     the camera in motion is uncalibrated.  When I say uncalibrated, I mean
     uncalibrated with respect to its extrinsic pararameters.  We assume in
     all cases in this document that the intrinsic parameters of the camera
     are known.
 
@@ -1297,16 +1303,15 @@
 
 @title
 THE ExamplesStructureFromCameraMotion DIRECTORY:
 
     See the 'ExamplesStructureFromCameraMotion' directory in the
     distribution for the following three example scripts that show how you
     can use the NonlinearLeastSquares module for estimating the structure
-    of a 3D scene from the images recorded by a moving camera.  Version 1.5
-    of this module:
+    of a 3D scene from the images recorded by a moving camera:  
 
         sfm_with_calibrated_cameras_translations_only.py
 
         sfm_with_uncalibrated_cameras_translations_only.py
 
         bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py
 
@@ -1337,17 +1342,17 @@
 
     Just to give you an idea of the speed-up you will get with
     bundle-adjustment, when I run the second script listed above on my
     laptop, it takes about 15 minutes for the number of structure points
     and the number of camera positions used in that script.  For exactly
     the same number of structure points and the camera positions, the third
     script takes only a couple of minutes.  You can only imagine the
-    speed-up you will get with a C-based library for bundle adjustment ---
-    such as the "sba" library mentioned in the paper by Lourakis and
-    Argyros that I mentioned earlier in this documentation page.
+    speed-up you will get with a C-based library for sparse bundle
+    adjustment --- such as the "sba" library mentioned in the paper by
+    Lourakis and Argyros that I cited earlier in this documentation page.
 
 
 @title
 CAVEAT
 
     Note the bundle-adjustment variant of the Levenberg-Marquardt algorithm
     that you see in the bundle-adjust() method of the NonlinearLeastSquares
@@ -1371,19 +1376,15 @@
             sudo python setup.py install
     and/or
             sudo python3 setup.py install
 
     On Linux distributions, this will install the module file at a location
     that looks like
 
-             /usr/local/lib/python2.7/dist-packages/
-
-    and for Python3 at a location like
-
-             /usr/local/lib/python3.5/dist-packages/
+             /usr/local/lib/python3.6/dist-packages/
 
     If you do not have root access, you have the option of working directly
     off the directory in which you downloaded the software by simply
     placing the following statements at the top of your scripts that use
     the NonlinearLeastSquares class:
 
             import sys
@@ -1409,34 +1410,34 @@
     email, please place the string 'NonlinearLeastSquares' in the subject
     line.
 
 
 @title
 ABOUT THE AUTHOR:
 
-    The author, Avinash Kak, recently finished a 17-year long "Objects
-    Trilogy Project" with the publication of the book "Designing with
-    Objects" by John-Wiley. If interested, visit his web page at Purdue to
-    find out what this project was all about. You might like "Designing
-    with Objects" especially if you enjoyed reading Harry Potter as a kid
-    (or even as an adult, for that matter).
+    Not too long ago, the author, Avinash Kak, finished a 17-year long
+    "Objects Trilogy Project" with the publication of the last book "Designing
+    with Objects" by John-Wiley. If interested, visit his web page at Purdue
+    to find out what this project was all about. You might like "Designing
+    with Objects" especially if you enjoyed reading Harry Potter as a kid (or
+    even as an adult, for that matter).
 
     For all issues related to this module, contact the author at
     kak@purdue.edu
 
-    If you send email, please place the string "NonlinearLeastSquares" in
-    your subject line to get past the author's spam filter.
+    If you send email, please place the string "NonlinearLeastSquares" in your
+    subject line to get past the author's spam filter.
 
 
 @title
 COPYRIGHT:
 
     Python Software Foundation License
 
-    Copyright 2018 Avinash Kak
+    Copyright 2022 Avinash Kak
 
 @endofdocs
 '''
 
 import numpy
 import numpy.linalg
 import scipy
@@ -1565,15 +1566,159 @@
     def set_display_function(self, display_function):
         self.display_function = display_function
 
     def set_debug(self, debug):
         self.debug = debug
 
 
+    ###%%%
+    #############################  Nonlnear Least-Squares with Basic Gradient Descent ############################
+
+    def grad_descent(self):
+        '''
+        This is an implementation of the basic gradient descent algorithm for nonlinear least-squares as described 
+        in my Lecture 13 notes at the lecture-notes website for Purdue University's ECE661: Computer Vision
+        '''
+        error_norm_with_iteration = []
+        delta_for_jacobian = self.delta_for_jacobian if self.jacobian_functionals_array is None else None
+        if self.delta_for_step_size is not None:
+            delta_for_step_size = self.delta_for_step_size
+        else:
+            raise Exception("You must set the 'delta_for_step_size' option in the constructor for the gradient-descent algorithm")
+        num_elements = len(self.Fvec)
+        num_measurements = len(self.X)
+        params_list = self.params_ordered_list if self.params_ordered_list is not None else self.params_arranged_list
+        num_params  =  len(params_list)
+        current_param_values = [self.params_dict[param] for param in params_list]
+        current_param_values = numpy.matrix(current_param_values).T 
+        current_fit_to_measurements = numpy.asmatrix(numpy.zeros_like(self.X))
+        for i in range(num_measurements):
+            current_fit_to_measurements[i,0] = \
+                                   eval(self._eval_functional_element(self.Fvec[i,0], self.initial_params_dict))
+        if self.debug:
+            print("\ncurrent_fit_to_measurements:")
+            print(str(current_fit_to_measurements))
+        current_error = self.X - current_fit_to_measurements
+        if self.debug:
+            print("\ncurrent error:")
+            print(str(current_error))
+            print("current error shape: %s" % str(current_error.shape))
+        current_error_norm = numpy.linalg.norm(self.X - current_fit_to_measurements)
+        if current_error_norm < 1e-12:
+            print("\nCurrent error norm: %.10f" % current_error_norm)
+            print('''\nLooks like your initial choices for the parameters are perfect. '''
+                  '''Perhaps there is nothing to be gained by invoking nonlinear least-squares '''
+                  '''on your problem.''')
+            sys.exit(1)
+        error_norm_with_iteration.append(current_error_norm)
+        if self.debug:
+            print("current error norm: %s" % str(current_error_norm))
+        new_param_values = new_fit_to_measurements = new_error_norm = None
+        iteration_index = 0
+        for iteration_index in range(self.max_iterations):
+            if self.debug:
+                print("\n\n ========================================  GD ITERATION: %d\n\n" % iteration_index)
+            jacobian = numpy.asmatrix(numpy.zeros((num_measurements, num_params), dtype=float))
+            if self.jacobian_functionals_array is not None:
+                for i in range(num_measurements):
+                    params_dict_local = {params_list[i] : current_param_values[i].tolist()[0][0] for i in range(num_params)}                
+                    if self.debug is True and i == 0: 
+                        print("\ncurrent values for parameters: %s" % str(sorted(params_dict_local.items())))
+                    for j in range(num_params):
+                        jacobian[i,j] = eval(self._eval_functional_element(self.jacobian_functionals_array[i,j], params_dict_local)) 
+            else:
+                for i in range(num_measurements):
+                    params_dict_local = {params_list[i] : current_param_values[i].tolist()[0][0] for i in range(num_params)}
+                    for j in range(num_params):
+                        incremented_params_dict_local = {param : params_dict_local[param] for param in params_dict_local}
+                        param = self.params_ordered_list[j] if self.params_ordered_list is not None else self.params_arranged_list[j]
+
+                        evaled_element1 = self._eval_functional_element(self.Fvec[i][0], params_dict_local)
+                        incremented_params_dict_local[param] = params_dict_local[param] + delta_for_jacobian
+                        evaled_element2 = self._eval_functional_element(self.Fvec[i][0], incremented_params_dict_local)
+                        jacobian[i,j] = (eval(evaled_element2) - eval(evaled_element1)) / delta_for_jacobian
+                    params_dict_local = None
+            if self.debug:
+                print("jacobian:")
+                print(str(jacobian))
+#                print("jacobian shape: %s" % str(jacobian.shape))
+            new_param_values = current_param_values + 2 * delta_for_step_size * (jacobian.T * current_error)
+            if self.debug:
+                print("\nnew parameter values:")
+                print(str(new_param_values.T))
+            new_params_dict = {params_list[i] : new_param_values[i].tolist()[0][0] for i in range(num_params)}
+            if self.debug:
+                print("new_params_dict: %s" % str(new_params_dict))
+            new_fit_to_measurements = numpy.asmatrix(numpy.zeros_like(self.X))
+            for i in range(num_measurements):
+                new_fit_to_measurements[i,0] = eval(self._eval_functional_element(self.Fvec[i][0], new_params_dict))
+            if self.debug:
+                print("new_fit_to_measurements:")
+                print(str(new_fit_to_measurements))
+            new_error =  self.X - new_fit_to_measurements
+            if self.debug:
+                print("\nnew error:")
+                print(str(new_error))
+            new_error_norm = numpy.linalg.norm(self.X - new_fit_to_measurements)
+            if self.debug:
+                print("\nnew error norm: %s" % str(new_error_norm))
+            if new_error_norm > error_norm_with_iteration[-1]:
+                break
+            error_norm_with_iteration.append(new_error_norm)
+            if self.debug:
+                print("\nerror norms with iterations: %s" % str(error_norm_with_iteration))
+            if self.display_function is not None and iteration_index % int(self.max_iterations/5.0) == 0:
+                self.display_function(new_fit_to_measurements, new_error_norm, iteration_index)
+            current_param_values = new_param_values
+        if self.debug:
+            print("\nerror norms with iterations: %s" % str(error_norm_with_iteration))
+            print("\niterations used: %d" % iteration_index)
+            print("\n\nfinal values for the parameters: ") 
+            print(str(new_param_values))
+        if self.debug is True and iteration_index == self.max_iterations - 1:
+            print("\n\nWARNING: max iterations reached without getting to the minimum")
+        if self.display_function:
+            self.display_function(new_fit_to_measurements, new_error_norm, iteration_index)
+        result = {"error_norms_with_iterations" : error_norm_with_iteration,
+                  "number_of_iterations" : iteration_index,
+                  "parameter_values" : new_param_values}
+        return result
+
+
+    ###%%%
+    #############  Nonlnear Least-Squares with the Levenberg-Marquardt Algorithm for Gradient Descent ############
+
     def leven_marq(self):
+        '''
+        This is an implementation of the Levenberg-Marquardt algorithm for nonlinear least-squares as described 
+        in my Lecture 13 notes at the lecture-notes website for Purdue University's ECE661: Computer Vision
+
+        This function is used the following scripts in the ExamplesOptimizedSurfaceFit directory of the distro:
+
+                    leven_marq.py
+
+                    leven_marq_with_partial_derivatives.py
+
+        It is important to note that the above two scripts do NOT call leven_marq() function directly.  AS 
+        stated in the main document page for the NonlinearLeastSquares module, the code in the file 
+        NonlinearLeastSquares.py is written in a domain agnostic manner.  So you need a domain adaptation 
+        class that knows how to package the arguments for calling leven_marq().  For the case of the two scripts
+        listed above, that domain-specific class in the distro is OptimizedSurfaceFit.  It is a co-class of 
+        the main module class NonlinearLeastSquares in the distribution.
+
+        The function leven_marq() defined here is ALSO used in the following two scripts
+
+            sfm_with_calibrated_cameras_translations_only.py
+            sfm_with_uncalibrated_cameras_translations_only.py
+
+        in the ExamplesStructureFromCameraMotion directory of the distribution.  Again, these example scripts
+        do NOT directly call the leven_marq() function.  As shown in the two scripts, they must first construct
+        an instance of the ProjectiveCamera class that knows how to bundle the arugments together for calling
+        the leven_marq() function.
+        '''
         if os.path.isdir("figs"):
             list(map(os.remove, glob.glob('figs/*.png')))
         else:
             os.mkdir("figs")
         error_norm_with_iteration = []
         error_norm_per_measurement_with_iteration = []
         alambda_with_iteration = []
@@ -1748,14 +1893,19 @@
 #                  "number_of_iterations" : len(productive_iteration_index_values),
                   "number_of_iterations" : iterations_used,
                   "parameter_values" : best_param_values}
         return result
 
 
     def leven_marq_v1_5(self):
+        """
+        This is the implementation of the leven_marq() function as it existed in Version 1.5.  On account of the
+        fact that I made significant changes to this function in Version 2.0.0 of the module, I have retained the
+        old version for the old-time users of my module.
+        """
         if os.path.isdir("figs"):
             list(map(os.remove, glob.glob('figs/*.png')))
         else:
             os.mkdir("figs")
         error_norm_with_iteration = []
         delta_for_jacobian = self.delta_for_jacobian if self.jacobian_functionals_array is None else None
 #        delta_for_step_size = self.delta_for_step_size if self.jacobian_functionals_array is None else None
@@ -1914,15 +2064,37 @@
             self.display_function(new_fit_to_measurements, new_error_norm, len(productive_iteration_index_values))
         result = {"error_norms_with_iterations" : error_norm_with_iteration,
                   "number_of_iterations" : len(productive_iteration_index_values) - 1,
                   "parameter_values" : new_param_values}
         return result
 
 
+    ###%%%
+    ################  Nonlnear Least-Squares for SfM (Structure from Motion) with Bundle Adjustment  #############
+
     def bundle_adjust(self, *args, **kwargs):
+        """
+        This is an implementation of the "bundle adjustment" version of the Levenberg-Marquardt algorithm for nonlinear
+        least-squares.  Bundle adjustment takes advantage of the sparsity of the Jacobian that one sees in 
+        applications such as estimating the scene structure with the images recorded with uncalibrated cameras.  
+        The implementation shown here is based on the now celebrated paper "SBA: A Software Package for Generic
+        Sparse Bundle Adjustment" by Manolis Lourakis and Antonis Argyros that appeared in ACM Transactions on 
+        Mathematical Software, March 2009.
+
+        This function is used in the following scripts 
+
+            bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py 
+
+        in the ExamplesStructureFromCameraMotion directory of the distribution.  
+
+        Note that since bundle_adjust() is written in a generic manner, it is not called directly by the example
+        scripts listed above.  As shown in the scripts, you need to first construct an instance of the class
+        ProjectiveCamera that is a co-class of the main module class NonlinearLeastSquares in the distribiution.        
+        """
+
         if args: raise Exception("The bundle_adjust can only be called with keyword arguments")
         allowed_keys = 'num_camera_params,num_structure_elements,num_cameras,num_params_per_camera,num_measurements_per_camera,initial_val_all_params'
         num_cameras=num_world_points=num_camera_params=num_structure_elements=num_cameras=num_cam_params_per_camera=num_measurements_per_camera=initial_val_all_params=None
         num_camera_params            =   kwargs.pop('num_camera_params')
         num_structure_elements       =   kwargs.pop('num_structure_elements')       ## they remain the same for all cams
         num_cameras                  =   kwargs.pop('num_cameras')
         num_cam_params_per_camera    =   kwargs.pop('num_cam_params_per_camera')
@@ -2357,127 +2529,24 @@
         result = {"error_norms_with_iterations" : error_norm_per_measurement_with_iteration,
 #                  "number_of_iterations" : len(productive_iteration_index_values) - 1,
                   "number_of_iterations" : iterations_used,
                   "parameter_values" : new_param_values}
         return result
 
 
-    def grad_descent(self):
-        error_norm_with_iteration = []
-        delta_for_jacobian = self.delta_for_jacobian if self.jacobian_functionals_array is None else None
-        if self.delta_for_step_size is not None:
-            delta_for_step_size = self.delta_for_step_size
-        else:
-            raise Exception("You must set the 'delta_for_step_size' option in the constructor for the gradient-descent algorithm")
-        num_elements = len(self.Fvec)
-        num_measurements = len(self.X)
-        params_list = self.params_ordered_list if self.params_ordered_list is not None else self.params_arranged_list
-        num_params  =  len(params_list)
-        current_param_values = [self.params_dict[param] for param in params_list]
-        current_param_values = numpy.matrix(current_param_values).T 
-        current_fit_to_measurements = numpy.asmatrix(numpy.zeros_like(self.X))
-        for i in range(num_measurements):
-            current_fit_to_measurements[i,0] = \
-                                   eval(self._eval_functional_element(self.Fvec[i,0], self.initial_params_dict))
-        if self.debug:
-            print("\ncurrent_fit_to_measurements:")
-            print(str(current_fit_to_measurements))
-        current_error = self.X - current_fit_to_measurements
-        if self.debug:
-            print("\ncurrent error:")
-            print(str(current_error))
-            print("current error shape: %s" % str(current_error.shape))
-        current_error_norm = numpy.linalg.norm(self.X - current_fit_to_measurements)
-        if current_error_norm < 1e-12:
-            print("\nCurrent error norm: %.10f" % current_error_norm)
-            print('''\nLooks like your initial choices for the parameters are perfect. '''
-                  '''Perhaps there is nothing to be gained by invoking nonlinear least-squares '''
-                  '''on your problem.''')
-            sys.exit(1)
-        error_norm_with_iteration.append(current_error_norm)
-        if self.debug:
-            print("current error norm: %s" % str(current_error_norm))
-        new_param_values = new_fit_to_measurements = new_error_norm = None
-        iteration_index = 0
-        for iteration_index in range(self.max_iterations):
-            if self.debug:
-                print("\n\n ========================================  GD ITERATION: %d\n\n" % iteration_index)
-            jacobian = numpy.asmatrix(numpy.zeros((num_measurements, num_params), dtype=float))
-            if self.jacobian_functionals_array is not None:
-                for i in range(num_measurements):
-                    params_dict_local = {params_list[i] : current_param_values[i].tolist()[0][0] for i in range(num_params)}                
-                    if self.debug is True and i == 0: 
-                        print("\ncurrent values for parameters: %s" % str(sorted(params_dict_local.items())))
-                    for j in range(num_params):
-                        jacobian[i,j] = eval(self._eval_functional_element(self.jacobian_functionals_array[i,j], params_dict_local)) 
-            else:
-                for i in range(num_measurements):
-                    params_dict_local = {params_list[i] : current_param_values[i].tolist()[0][0] for i in range(num_params)}
-                    for j in range(num_params):
-                        incremented_params_dict_local = {param : params_dict_local[param] for param in params_dict_local}
-                        param = self.params_ordered_list[j] if self.params_ordered_list is not None else self.params_arranged_list[j]
-
-                        evaled_element1 = self._eval_functional_element(self.Fvec[i][0], params_dict_local)
-                        incremented_params_dict_local[param] = params_dict_local[param] + delta_for_jacobian
-                        evaled_element2 = self._eval_functional_element(self.Fvec[i][0], incremented_params_dict_local)
-                        jacobian[i,j] = (eval(evaled_element2) - eval(evaled_element1)) / delta_for_jacobian
-                    params_dict_local = None
-            if self.debug:
-                print("jacobian:")
-                print(str(jacobian))
-#                print("jacobian shape: %s" % str(jacobian.shape))
-            new_param_values = current_param_values + 2 * delta_for_step_size * (jacobian.T * current_error)
-            if self.debug:
-                print("\nnew parameter values:")
-                print(str(new_param_values.T))
-            new_params_dict = {params_list[i] : new_param_values[i].tolist()[0][0] for i in range(num_params)}
-            if self.debug:
-                print("new_params_dict: %s" % str(new_params_dict))
-            new_fit_to_measurements = numpy.asmatrix(numpy.zeros_like(self.X))
-            for i in range(num_measurements):
-                new_fit_to_measurements[i,0] = eval(self._eval_functional_element(self.Fvec[i][0], new_params_dict))
-            if self.debug:
-                print("new_fit_to_measurements:")
-                print(str(new_fit_to_measurements))
-            new_error =  self.X - new_fit_to_measurements
-            if self.debug:
-                print("\nnew error:")
-                print(str(new_error))
-            new_error_norm = numpy.linalg.norm(self.X - new_fit_to_measurements)
-            if self.debug:
-                print("\nnew error norm: %s" % str(new_error_norm))
-            if new_error_norm > error_norm_with_iteration[-1]:
-                break
-            error_norm_with_iteration.append(new_error_norm)
-            if self.debug:
-                print("\nerror norms with iterations: %s" % str(error_norm_with_iteration))
-            if self.display_function is not None and iteration_index % int(self.max_iterations/5.0) == 0:
-                self.display_function(new_fit_to_measurements, new_error_norm, iteration_index)
-            current_param_values = new_param_values
-        if self.debug:
-            print("\nerror norms with iterations: %s" % str(error_norm_with_iteration))
-            print("\niterations used: %d" % iteration_index)
-            print("\n\nfinal values for the parameters: ") 
-            print(str(new_param_values))
-        if self.debug is True and iteration_index == self.max_iterations - 1:
-            print("\n\nWARNING: max iterations reached without getting to the minimum")
-        if self.display_function:
-            self.display_function(new_fit_to_measurements, new_error_norm, iteration_index)
-        result = {"error_norms_with_iterations" : error_norm_with_iteration,
-                  "number_of_iterations" : iteration_index,
-                  "parameter_values" : new_param_values}
-        return result
 
-#------------------------------  Private Methods of NonlinearLeastSquares  --------------------
+    ###%%%
+    ##################################  Private Methods of NonlinearLeastSquares  ################################
 
     def _get_initial_params_from_file(self, filename):
         if not filename.endswith('.txt'): 
             sys.exit("Aborted. _get_initial_params_from_file() is only for CSV files")
         initial_params_dict = {}
-        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line is not '']
+#        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line is not '']
+        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line != '']
         for record in initial_params_list:
             initial_params_dict[record[:record.find('=')].rstrip()] = float(record[record.find('=')+1:].lstrip())
         self.params_dict = initial_params_dict
         self.params_ordered_list = sorted(self.params_dict) if self.params_ordered_list is not None else self.params_arranged_list
         return initial_params_dict
 
     def _get_measured_data_from_text_file(self, filename):
@@ -2508,18 +2577,18 @@
                 if re.search(regex, augmented_element):
                     augmented_element = re.sub(regex, str(params_dict[param]), augmented_element)
         return augmented_element
 
     def _eval_functional_element2(self, Fvec_element, param_list, param_val_list):
         '''
         Although this method does basically the same thing as the previous method, this one 
-        is meant for the bundle adjustment implementation of LM.  Now the second argument, param_val_list,
-        is a list for the current values for the camera parameters --- BUT ONLY FOR ONE CAMERA --- and 
-        for the structure parameters.  Note that this method was written assuming that the second argument
-        is a list as opposed to a dict.
+        is meant for the sparse-bundle-adjustment implementation of LM.  Now the second argument, 
+        param_val_list, is a list for the current values for the camera parameters --- BUT ONLY FOR 
+        ONE CAMERA --- and for the structure parameters.  Note that this method was written assuming 
+        that the second argument is a list as opposed to a dict.
         '''
         augmented_element = Fvec_element
         for i,param in enumerate(param_list):
             regex = r'\b' + param + r'\b'         
             if isinstance(augmented_element, (bytes)):
                 if re.search(regex, augmented_element.decode('utf-8')):
                     augmented_element = re.sub(regex, str(param_val_list[i]), augmented_element.decode('utf-8'))
```

### Comparing `NonlinearLeastSquares-2.0.0/ExamplesStructureFromCameraMotion/bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py` & `NonlinearLeastSquares-2.0.1/ExamplesStructureFromCameraMotion/bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/ExamplesStructureFromCameraMotion/sfm_with_uncalibrated_cameras_translations_only.py` & `NonlinearLeastSquares-2.0.1/ExamplesStructureFromCameraMotion/sfm_with_uncalibrated_cameras_translations_only.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/ExamplesStructureFromCameraMotion/sfm_with_calibrated_cameras_translations_only.py` & `NonlinearLeastSquares-2.0.1/ExamplesStructureFromCameraMotion/sfm_with_calibrated_cameras_translations_only.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/ExamplesStructureFromCameraMotion/README` & `NonlinearLeastSquares-2.0.1/ExamplesStructureFromCameraMotion/README`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/NonlinearLeastSquares/NonlinearLeastSquares.py` & `NonlinearLeastSquares-2.0.1/TestNonlinearLeastSquares/NonlinearLeastSquares.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 __author__  = "Avinash Kak (kak@purdue.edu)"
-__date__    = '2018-November-9'
-__url__     = 'https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.html'
-__copyright__ = "(C) 2018 Avinash Kak. Python Software Foundation."
+__date__    = '2022-October-6'
+__url__     = 'https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.html'
+__copyright__ = "(C) 2022 Avinash Kak. Python Software Foundation."
 
 
 __doc__ = '''
 
 NonlinearLeastSquares.py
 
 Version: ''' + __version__ + '''
@@ -15,14 +15,22 @@
 
 Date: ''' + __date__ + '''
 
 
 @title
 CHANGE LOG:
 
+  Version 2.0.1:
+
+    Cleaned up the code to make it work with the current version of the
+    matplotlib library that is used for displaying the results.  I have also
+    removed the use of the "is" and "is not" comparison operators for numeric
+    and string literals since such use has now been deprecated.  Also added
+    additional comment blocks to the main functions in the module file.
+
   Version 2.0.0:
 
     This version includes sparse bundle adjustment (SBA) to speed up code
     execution when using nonlinear least-squares for solving
     structure-from-camera-motion problems with uncalibrated cameras.  SBA
     exploits the sparseness of the Jacobian encountered in such problems.
     This version also includes improvements to the Levenberg-Marquardt code
@@ -31,47 +39,46 @@
     provides additional methods for the visualization of the results.
 
   Version 1.5.0:
 
     This version adds a new class, ProjectiveCamera, to the module for
     demonstrating how nonlinear least-squares can be used for estimating
     structure of a scene from the data recorded with a calibrated camera in
-    motion.  For a simulated demonstration, you can create calibrated
-    cameras from a generic instance of the ProjectiveCamera class that is
-    then subject to various translational and rotational transformations.
+    motion.  For a simulated demonstration, you can create calibrated cameras
+    from a generic instance of the ProjectiveCamera class that is then subject
+    to various translational and rotational transformations.
 
   Version 1.1.1:
 
     This version includes constructor options to control the size and the
     position of the graphics for displaying the results of nonlinear
     least-squares optimization.
 
   Version 1.1:
 
-    This version fixes a bug in the synthetic data generator function used
-    for illustrating the functionality of the NonlinearLeastSquares class.
-    Changes also made to the information that is printed out when the
-    module is run in the debug mode.
+    This version fixes a bug in the synthetic data generator function used for
+    illustrating the functionality of the NonlinearLeastSquares class.
+    Changes also made to the information that is printed out when the module
+    is run in the debug mode.
 
   Version 1.0:
 
-    In the form of a class named NonlinearLeastSquares, this module
-    provides a domain agnostic implementation of nonlinear least-squares
-    algorithms (gradient-descent and Levenberg-Marquardt) for fitting a
-    model to observed data.  Typically, the model involves several
-    parameters and each observed data element can be expressed as a
-    function of those parameters plus noise.  The goal of nonlinear
-    least-squares is to estimate the best values for the parameters given
-    all of the observed data.  In order to illustrate how to use the
-    NonlinearLeastSquares class, the module also comes with another class,
-    OptimizeSurfaceFit, whose job is to fit the best surface (of a
-    specified analytical form) to noisy height data over the XY-plane. The
-    model in this case is the analytical description of the surface and the
-    goal of nonlinear least-squares is to estimate the best values for the
-    parameters in the analytical description.
+    In the form of a class named NonlinearLeastSquares, this module provides a
+    domain agnostic implementation of nonlinear least-squares algorithms
+    (gradient-descent and Levenberg-Marquardt) for fitting a model to observed
+    data.  Typically, the model involves several parameters and each observed
+    data element can be expressed as a function of those parameters plus
+    noise.  The goal of nonlinear least-squares is to estimate the best values
+    for the parameters given all of the observed data.  In order to illustrate
+    how to use the NonlinearLeastSquares class, the module also comes with
+    another class, OptimizeSurfaceFit, whose job is to fit the best surface
+    (of a specified analytical form) to noisy height data over the
+    XY-plane. The model in this case is the analytical description of the
+    surface and the goal of nonlinear least-squares is to estimate the best
+    values for the parameters in the analytical description.
 
 
 @title
 USAGE FOR OPTIMAL SURFACE FITTING:
 
     The module includes a domain specific class, OptimizedSurfaceFit, for
     demonstrating how nonlinear least-squares in the form of the
@@ -220,24 +227,25 @@
         camera.construct_parameter_vec_for_uncalibrated_cameras_with_rodrigues_rotations()
                                                                           #(M)
         camera.construct_Fvec_for_bundle_adjustment()                     #(O)
         result = camera.get_scene_structure_from_camera_motion_with_bundle_adjustment()
                                                                           #(P)
 
     The construction of the observation vector X in line (L) is specific to
-    bundle adjustment --- in the sense that you first want to list the
-    pixels in all the cameras for the first world point, then you want to
-    list the pixels in all the cameras for the second world point, and so
-    on.  Ordering the observed data in this fashion is necessary to create
-    the sort of block sparsity in the Jacobian that is exploited in SBA.
+    sparse bundle adjustment --- in the sense that you first want to list
+    the pixels in all the cameras for the first world point, then you want
+    to list the pixels in all the cameras for the second world point, and
+    so on.  Ordering the observed data in this fashion is necessary to
+    create the sort of block sparsity in the Jacobian that is exploited in
+    SBA.
 
     Note that we assume that the intrinsic parameters of the camera are
     known already.  So the goal of the bundle adjustment is to estimate the
-    six extrinsic parameters, the three for translation of the camera and
-    the three (in the form of Rodrigues rotations) for the rotation.
+    six extrinsic parameters, three for translation of the camera and three
+    (in the form of Rodrigues rotations) for the rotation.
         
     See the script 
 
        bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py
 
     in the ExamplesStructureFromCameraMotion subdirectory of the
     distribution for further information on what calls you need to sequence
@@ -1295,16 +1303,15 @@
 
 @title
 THE ExamplesStructureFromCameraMotion DIRECTORY:
 
     See the 'ExamplesStructureFromCameraMotion' directory in the
     distribution for the following three example scripts that show how you
     can use the NonlinearLeastSquares module for estimating the structure
-    of a 3D scene from the images recorded by a moving camera.  Version 1.5
-    of this module:
+    of a 3D scene from the images recorded by a moving camera:  
 
         sfm_with_calibrated_cameras_translations_only.py
 
         sfm_with_uncalibrated_cameras_translations_only.py
 
         bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py
 
@@ -1335,17 +1342,17 @@
 
     Just to give you an idea of the speed-up you will get with
     bundle-adjustment, when I run the second script listed above on my
     laptop, it takes about 15 minutes for the number of structure points
     and the number of camera positions used in that script.  For exactly
     the same number of structure points and the camera positions, the third
     script takes only a couple of minutes.  You can only imagine the
-    speed-up you will get with a C-based library for bundle adjustment ---
-    such as the "sba" library mentioned in the paper by Lourakis and
-    Argyros that I mentioned earlier in this documentation page.
+    speed-up you will get with a C-based library for sparse bundle
+    adjustment --- such as the "sba" library mentioned in the paper by
+    Lourakis and Argyros that I cited earlier in this documentation page.
 
 
 @title
 CAVEAT
 
     Note the bundle-adjustment variant of the Levenberg-Marquardt algorithm
     that you see in the bundle-adjust() method of the NonlinearLeastSquares
@@ -1369,18 +1376,14 @@
             sudo python setup.py install
     and/or
             sudo python3 setup.py install
 
     On Linux distributions, this will install the module file at a location
     that looks like
 
-             /usr/local/lib/python2.7/dist-packages/
-
-    and for Python3 at a location like
-
              /usr/local/lib/python3.6/dist-packages/
 
     If you do not have root access, you have the option of working directly
     off the directory in which you downloaded the software by simply
     placing the following statements at the top of your scripts that use
     the NonlinearLeastSquares class:
 
@@ -1407,34 +1410,34 @@
     email, please place the string 'NonlinearLeastSquares' in the subject
     line.
 
 
 @title
 ABOUT THE AUTHOR:
 
-    The author, Avinash Kak, recently finished a 17-year long "Objects
-    Trilogy Project" with the publication of the book "Designing with
-    Objects" by John-Wiley. If interested, visit his web page at Purdue to
-    find out what this project was all about. You might like "Designing
-    with Objects" especially if you enjoyed reading Harry Potter as a kid
-    (or even as an adult, for that matter).
+    Not too long ago, the author, Avinash Kak, finished a 17-year long
+    "Objects Trilogy Project" with the publication of the last book "Designing
+    with Objects" by John-Wiley. If interested, visit his web page at Purdue
+    to find out what this project was all about. You might like "Designing
+    with Objects" especially if you enjoyed reading Harry Potter as a kid (or
+    even as an adult, for that matter).
 
     For all issues related to this module, contact the author at
     kak@purdue.edu
 
-    If you send email, please place the string "NonlinearLeastSquares" in
-    your subject line to get past the author's spam filter.
+    If you send email, please place the string "NonlinearLeastSquares" in your
+    subject line to get past the author's spam filter.
 
 
 @title
 COPYRIGHT:
 
     Python Software Foundation License
 
-    Copyright 2018 Avinash Kak
+    Copyright 2022 Avinash Kak
 
 @endofdocs
 '''
 
 import numpy
 import numpy.linalg
 import scipy
@@ -1563,15 +1566,159 @@
     def set_display_function(self, display_function):
         self.display_function = display_function
 
     def set_debug(self, debug):
         self.debug = debug
 
 
+    ###%%%
+    #############################  Nonlnear Least-Squares with Basic Gradient Descent ############################
+
+    def grad_descent(self):
+        '''
+        This is an implementation of the basic gradient descent algorithm for nonlinear least-squares as described 
+        in my Lecture 13 notes at the lecture-notes website for Purdue University's ECE661: Computer Vision
+        '''
+        error_norm_with_iteration = []
+        delta_for_jacobian = self.delta_for_jacobian if self.jacobian_functionals_array is None else None
+        if self.delta_for_step_size is not None:
+            delta_for_step_size = self.delta_for_step_size
+        else:
+            raise Exception("You must set the 'delta_for_step_size' option in the constructor for the gradient-descent algorithm")
+        num_elements = len(self.Fvec)
+        num_measurements = len(self.X)
+        params_list = self.params_ordered_list if self.params_ordered_list is not None else self.params_arranged_list
+        num_params  =  len(params_list)
+        current_param_values = [self.params_dict[param] for param in params_list]
+        current_param_values = numpy.matrix(current_param_values).T 
+        current_fit_to_measurements = numpy.asmatrix(numpy.zeros_like(self.X))
+        for i in range(num_measurements):
+            current_fit_to_measurements[i,0] = \
+                                   eval(self._eval_functional_element(self.Fvec[i,0], self.initial_params_dict))
+        if self.debug:
+            print("\ncurrent_fit_to_measurements:")
+            print(str(current_fit_to_measurements))
+        current_error = self.X - current_fit_to_measurements
+        if self.debug:
+            print("\ncurrent error:")
+            print(str(current_error))
+            print("current error shape: %s" % str(current_error.shape))
+        current_error_norm = numpy.linalg.norm(self.X - current_fit_to_measurements)
+        if current_error_norm < 1e-12:
+            print("\nCurrent error norm: %.10f" % current_error_norm)
+            print('''\nLooks like your initial choices for the parameters are perfect. '''
+                  '''Perhaps there is nothing to be gained by invoking nonlinear least-squares '''
+                  '''on your problem.''')
+            sys.exit(1)
+        error_norm_with_iteration.append(current_error_norm)
+        if self.debug:
+            print("current error norm: %s" % str(current_error_norm))
+        new_param_values = new_fit_to_measurements = new_error_norm = None
+        iteration_index = 0
+        for iteration_index in range(self.max_iterations):
+            if self.debug:
+                print("\n\n ========================================  GD ITERATION: %d\n\n" % iteration_index)
+            jacobian = numpy.asmatrix(numpy.zeros((num_measurements, num_params), dtype=float))
+            if self.jacobian_functionals_array is not None:
+                for i in range(num_measurements):
+                    params_dict_local = {params_list[i] : current_param_values[i].tolist()[0][0] for i in range(num_params)}                
+                    if self.debug is True and i == 0: 
+                        print("\ncurrent values for parameters: %s" % str(sorted(params_dict_local.items())))
+                    for j in range(num_params):
+                        jacobian[i,j] = eval(self._eval_functional_element(self.jacobian_functionals_array[i,j], params_dict_local)) 
+            else:
+                for i in range(num_measurements):
+                    params_dict_local = {params_list[i] : current_param_values[i].tolist()[0][0] for i in range(num_params)}
+                    for j in range(num_params):
+                        incremented_params_dict_local = {param : params_dict_local[param] for param in params_dict_local}
+                        param = self.params_ordered_list[j] if self.params_ordered_list is not None else self.params_arranged_list[j]
+
+                        evaled_element1 = self._eval_functional_element(self.Fvec[i][0], params_dict_local)
+                        incremented_params_dict_local[param] = params_dict_local[param] + delta_for_jacobian
+                        evaled_element2 = self._eval_functional_element(self.Fvec[i][0], incremented_params_dict_local)
+                        jacobian[i,j] = (eval(evaled_element2) - eval(evaled_element1)) / delta_for_jacobian
+                    params_dict_local = None
+            if self.debug:
+                print("jacobian:")
+                print(str(jacobian))
+#                print("jacobian shape: %s" % str(jacobian.shape))
+            new_param_values = current_param_values + 2 * delta_for_step_size * (jacobian.T * current_error)
+            if self.debug:
+                print("\nnew parameter values:")
+                print(str(new_param_values.T))
+            new_params_dict = {params_list[i] : new_param_values[i].tolist()[0][0] for i in range(num_params)}
+            if self.debug:
+                print("new_params_dict: %s" % str(new_params_dict))
+            new_fit_to_measurements = numpy.asmatrix(numpy.zeros_like(self.X))
+            for i in range(num_measurements):
+                new_fit_to_measurements[i,0] = eval(self._eval_functional_element(self.Fvec[i][0], new_params_dict))
+            if self.debug:
+                print("new_fit_to_measurements:")
+                print(str(new_fit_to_measurements))
+            new_error =  self.X - new_fit_to_measurements
+            if self.debug:
+                print("\nnew error:")
+                print(str(new_error))
+            new_error_norm = numpy.linalg.norm(self.X - new_fit_to_measurements)
+            if self.debug:
+                print("\nnew error norm: %s" % str(new_error_norm))
+            if new_error_norm > error_norm_with_iteration[-1]:
+                break
+            error_norm_with_iteration.append(new_error_norm)
+            if self.debug:
+                print("\nerror norms with iterations: %s" % str(error_norm_with_iteration))
+            if self.display_function is not None and iteration_index % int(self.max_iterations/5.0) == 0:
+                self.display_function(new_fit_to_measurements, new_error_norm, iteration_index)
+            current_param_values = new_param_values
+        if self.debug:
+            print("\nerror norms with iterations: %s" % str(error_norm_with_iteration))
+            print("\niterations used: %d" % iteration_index)
+            print("\n\nfinal values for the parameters: ") 
+            print(str(new_param_values))
+        if self.debug is True and iteration_index == self.max_iterations - 1:
+            print("\n\nWARNING: max iterations reached without getting to the minimum")
+        if self.display_function:
+            self.display_function(new_fit_to_measurements, new_error_norm, iteration_index)
+        result = {"error_norms_with_iterations" : error_norm_with_iteration,
+                  "number_of_iterations" : iteration_index,
+                  "parameter_values" : new_param_values}
+        return result
+
+
+    ###%%%
+    #############  Nonlnear Least-Squares with the Levenberg-Marquardt Algorithm for Gradient Descent ############
+
     def leven_marq(self):
+        '''
+        This is an implementation of the Levenberg-Marquardt algorithm for nonlinear least-squares as described 
+        in my Lecture 13 notes at the lecture-notes website for Purdue University's ECE661: Computer Vision
+
+        This function is used the following scripts in the ExamplesOptimizedSurfaceFit directory of the distro:
+
+                    leven_marq.py
+
+                    leven_marq_with_partial_derivatives.py
+
+        It is important to note that the above two scripts do NOT call leven_marq() function directly.  AS 
+        stated in the main document page for the NonlinearLeastSquares module, the code in the file 
+        NonlinearLeastSquares.py is written in a domain agnostic manner.  So you need a domain adaptation 
+        class that knows how to package the arguments for calling leven_marq().  For the case of the two scripts
+        listed above, that domain-specific class in the distro is OptimizedSurfaceFit.  It is a co-class of 
+        the main module class NonlinearLeastSquares in the distribution.
+
+        The function leven_marq() defined here is ALSO used in the following two scripts
+
+            sfm_with_calibrated_cameras_translations_only.py
+            sfm_with_uncalibrated_cameras_translations_only.py
+
+        in the ExamplesStructureFromCameraMotion directory of the distribution.  Again, these example scripts
+        do NOT directly call the leven_marq() function.  As shown in the two scripts, they must first construct
+        an instance of the ProjectiveCamera class that knows how to bundle the arugments together for calling
+        the leven_marq() function.
+        '''
         if os.path.isdir("figs"):
             list(map(os.remove, glob.glob('figs/*.png')))
         else:
             os.mkdir("figs")
         error_norm_with_iteration = []
         error_norm_per_measurement_with_iteration = []
         alambda_with_iteration = []
@@ -1746,14 +1893,19 @@
 #                  "number_of_iterations" : len(productive_iteration_index_values),
                   "number_of_iterations" : iterations_used,
                   "parameter_values" : best_param_values}
         return result
 
 
     def leven_marq_v1_5(self):
+        """
+        This is the implementation of the leven_marq() function as it existed in Version 1.5.  On account of the
+        fact that I made significant changes to this function in Version 2.0.0 of the module, I have retained the
+        old version for the old-time users of my module.
+        """
         if os.path.isdir("figs"):
             list(map(os.remove, glob.glob('figs/*.png')))
         else:
             os.mkdir("figs")
         error_norm_with_iteration = []
         delta_for_jacobian = self.delta_for_jacobian if self.jacobian_functionals_array is None else None
 #        delta_for_step_size = self.delta_for_step_size if self.jacobian_functionals_array is None else None
@@ -1912,15 +2064,37 @@
             self.display_function(new_fit_to_measurements, new_error_norm, len(productive_iteration_index_values))
         result = {"error_norms_with_iterations" : error_norm_with_iteration,
                   "number_of_iterations" : len(productive_iteration_index_values) - 1,
                   "parameter_values" : new_param_values}
         return result
 
 
+    ###%%%
+    ################  Nonlnear Least-Squares for SfM (Structure from Motion) with Bundle Adjustment  #############
+
     def bundle_adjust(self, *args, **kwargs):
+        """
+        This is an implementation of the "bundle adjustment" version of the Levenberg-Marquardt algorithm for nonlinear
+        least-squares.  Bundle adjustment takes advantage of the sparsity of the Jacobian that one sees in 
+        applications such as estimating the scene structure with the images recorded with uncalibrated cameras.  
+        The implementation shown here is based on the now celebrated paper "SBA: A Software Package for Generic
+        Sparse Bundle Adjustment" by Manolis Lourakis and Antonis Argyros that appeared in ACM Transactions on 
+        Mathematical Software, March 2009.
+
+        This function is used in the following scripts 
+
+            bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py 
+
+        in the ExamplesStructureFromCameraMotion directory of the distribution.  
+
+        Note that since bundle_adjust() is written in a generic manner, it is not called directly by the example
+        scripts listed above.  As shown in the scripts, you need to first construct an instance of the class
+        ProjectiveCamera that is a co-class of the main module class NonlinearLeastSquares in the distribiution.        
+        """
+
         if args: raise Exception("The bundle_adjust can only be called with keyword arguments")
         allowed_keys = 'num_camera_params,num_structure_elements,num_cameras,num_params_per_camera,num_measurements_per_camera,initial_val_all_params'
         num_cameras=num_world_points=num_camera_params=num_structure_elements=num_cameras=num_cam_params_per_camera=num_measurements_per_camera=initial_val_all_params=None
         num_camera_params            =   kwargs.pop('num_camera_params')
         num_structure_elements       =   kwargs.pop('num_structure_elements')       ## they remain the same for all cams
         num_cameras                  =   kwargs.pop('num_cameras')
         num_cam_params_per_camera    =   kwargs.pop('num_cam_params_per_camera')
@@ -2355,127 +2529,24 @@
         result = {"error_norms_with_iterations" : error_norm_per_measurement_with_iteration,
 #                  "number_of_iterations" : len(productive_iteration_index_values) - 1,
                   "number_of_iterations" : iterations_used,
                   "parameter_values" : new_param_values}
         return result
 
 
-    def grad_descent(self):
-        error_norm_with_iteration = []
-        delta_for_jacobian = self.delta_for_jacobian if self.jacobian_functionals_array is None else None
-        if self.delta_for_step_size is not None:
-            delta_for_step_size = self.delta_for_step_size
-        else:
-            raise Exception("You must set the 'delta_for_step_size' option in the constructor for the gradient-descent algorithm")
-        num_elements = len(self.Fvec)
-        num_measurements = len(self.X)
-        params_list = self.params_ordered_list if self.params_ordered_list is not None else self.params_arranged_list
-        num_params  =  len(params_list)
-        current_param_values = [self.params_dict[param] for param in params_list]
-        current_param_values = numpy.matrix(current_param_values).T 
-        current_fit_to_measurements = numpy.asmatrix(numpy.zeros_like(self.X))
-        for i in range(num_measurements):
-            current_fit_to_measurements[i,0] = \
-                                   eval(self._eval_functional_element(self.Fvec[i,0], self.initial_params_dict))
-        if self.debug:
-            print("\ncurrent_fit_to_measurements:")
-            print(str(current_fit_to_measurements))
-        current_error = self.X - current_fit_to_measurements
-        if self.debug:
-            print("\ncurrent error:")
-            print(str(current_error))
-            print("current error shape: %s" % str(current_error.shape))
-        current_error_norm = numpy.linalg.norm(self.X - current_fit_to_measurements)
-        if current_error_norm < 1e-12:
-            print("\nCurrent error norm: %.10f" % current_error_norm)
-            print('''\nLooks like your initial choices for the parameters are perfect. '''
-                  '''Perhaps there is nothing to be gained by invoking nonlinear least-squares '''
-                  '''on your problem.''')
-            sys.exit(1)
-        error_norm_with_iteration.append(current_error_norm)
-        if self.debug:
-            print("current error norm: %s" % str(current_error_norm))
-        new_param_values = new_fit_to_measurements = new_error_norm = None
-        iteration_index = 0
-        for iteration_index in range(self.max_iterations):
-            if self.debug:
-                print("\n\n ========================================  GD ITERATION: %d\n\n" % iteration_index)
-            jacobian = numpy.asmatrix(numpy.zeros((num_measurements, num_params), dtype=float))
-            if self.jacobian_functionals_array is not None:
-                for i in range(num_measurements):
-                    params_dict_local = {params_list[i] : current_param_values[i].tolist()[0][0] for i in range(num_params)}                
-                    if self.debug is True and i == 0: 
-                        print("\ncurrent values for parameters: %s" % str(sorted(params_dict_local.items())))
-                    for j in range(num_params):
-                        jacobian[i,j] = eval(self._eval_functional_element(self.jacobian_functionals_array[i,j], params_dict_local)) 
-            else:
-                for i in range(num_measurements):
-                    params_dict_local = {params_list[i] : current_param_values[i].tolist()[0][0] for i in range(num_params)}
-                    for j in range(num_params):
-                        incremented_params_dict_local = {param : params_dict_local[param] for param in params_dict_local}
-                        param = self.params_ordered_list[j] if self.params_ordered_list is not None else self.params_arranged_list[j]
-
-                        evaled_element1 = self._eval_functional_element(self.Fvec[i][0], params_dict_local)
-                        incremented_params_dict_local[param] = params_dict_local[param] + delta_for_jacobian
-                        evaled_element2 = self._eval_functional_element(self.Fvec[i][0], incremented_params_dict_local)
-                        jacobian[i,j] = (eval(evaled_element2) - eval(evaled_element1)) / delta_for_jacobian
-                    params_dict_local = None
-            if self.debug:
-                print("jacobian:")
-                print(str(jacobian))
-#                print("jacobian shape: %s" % str(jacobian.shape))
-            new_param_values = current_param_values + 2 * delta_for_step_size * (jacobian.T * current_error)
-            if self.debug:
-                print("\nnew parameter values:")
-                print(str(new_param_values.T))
-            new_params_dict = {params_list[i] : new_param_values[i].tolist()[0][0] for i in range(num_params)}
-            if self.debug:
-                print("new_params_dict: %s" % str(new_params_dict))
-            new_fit_to_measurements = numpy.asmatrix(numpy.zeros_like(self.X))
-            for i in range(num_measurements):
-                new_fit_to_measurements[i,0] = eval(self._eval_functional_element(self.Fvec[i][0], new_params_dict))
-            if self.debug:
-                print("new_fit_to_measurements:")
-                print(str(new_fit_to_measurements))
-            new_error =  self.X - new_fit_to_measurements
-            if self.debug:
-                print("\nnew error:")
-                print(str(new_error))
-            new_error_norm = numpy.linalg.norm(self.X - new_fit_to_measurements)
-            if self.debug:
-                print("\nnew error norm: %s" % str(new_error_norm))
-            if new_error_norm > error_norm_with_iteration[-1]:
-                break
-            error_norm_with_iteration.append(new_error_norm)
-            if self.debug:
-                print("\nerror norms with iterations: %s" % str(error_norm_with_iteration))
-            if self.display_function is not None and iteration_index % int(self.max_iterations/5.0) == 0:
-                self.display_function(new_fit_to_measurements, new_error_norm, iteration_index)
-            current_param_values = new_param_values
-        if self.debug:
-            print("\nerror norms with iterations: %s" % str(error_norm_with_iteration))
-            print("\niterations used: %d" % iteration_index)
-            print("\n\nfinal values for the parameters: ") 
-            print(str(new_param_values))
-        if self.debug is True and iteration_index == self.max_iterations - 1:
-            print("\n\nWARNING: max iterations reached without getting to the minimum")
-        if self.display_function:
-            self.display_function(new_fit_to_measurements, new_error_norm, iteration_index)
-        result = {"error_norms_with_iterations" : error_norm_with_iteration,
-                  "number_of_iterations" : iteration_index,
-                  "parameter_values" : new_param_values}
-        return result
 
-#------------------------------  Private Methods of NonlinearLeastSquares  --------------------
+    ###%%%
+    ##################################  Private Methods of NonlinearLeastSquares  ################################
 
     def _get_initial_params_from_file(self, filename):
         if not filename.endswith('.txt'): 
             sys.exit("Aborted. _get_initial_params_from_file() is only for CSV files")
         initial_params_dict = {}
-        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line is not '']
+#        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line is not '']
+        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line != '']
         for record in initial_params_list:
             initial_params_dict[record[:record.find('=')].rstrip()] = float(record[record.find('=')+1:].lstrip())
         self.params_dict = initial_params_dict
         self.params_ordered_list = sorted(self.params_dict) if self.params_ordered_list is not None else self.params_arranged_list
         return initial_params_dict
 
     def _get_measured_data_from_text_file(self, filename):
@@ -2506,18 +2577,18 @@
                 if re.search(regex, augmented_element):
                     augmented_element = re.sub(regex, str(params_dict[param]), augmented_element)
         return augmented_element
 
     def _eval_functional_element2(self, Fvec_element, param_list, param_val_list):
         '''
         Although this method does basically the same thing as the previous method, this one 
-        is meant for the bundle adjustment implementation of LM.  Now the second argument, param_val_list,
-        is a list for the current values for the camera parameters --- BUT ONLY FOR ONE CAMERA --- and 
-        for the structure parameters.  Note that this method was written assuming that the second argument
-        is a list as opposed to a dict.
+        is meant for the sparse-bundle-adjustment implementation of LM.  Now the second argument, 
+        param_val_list, is a list for the current values for the camera parameters --- BUT ONLY FOR 
+        ONE CAMERA --- and for the structure parameters.  Note that this method was written assuming 
+        that the second argument is a list as opposed to a dict.
         '''
         augmented_element = Fvec_element
         for i,param in enumerate(param_list):
             regex = r'\b' + param + r'\b'         
             if isinstance(augmented_element, (bytes)):
                 if re.search(regex, augmented_element.decode('utf-8')):
                     augmented_element = re.sub(regex, str(param_val_list[i]), augmented_element.decode('utf-8'))
```

### Comparing `NonlinearLeastSquares-2.0.0/NonlinearLeastSquares/__init__.py` & `NonlinearLeastSquares-2.0.1/NonlinearLeastSquares/__init__.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/Makefile` & `NonlinearLeastSquares-2.0.1/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # GNU -*- makefile -*-
 
 #VERSION := ${shell python -c "import NonlinearLeastSquares;print NonlinearLeastSquares.__version__"}
-VERSION := ${shell python -c "import os; os.chdir('NonlinearLeastSquares'); import NonlinearLeastSquares;print NonlinearLeastSquares.__version__"}
+VERSION := ${shell python3 -c "import os; os.chdir('NonlinearLeastSquares'); import NonlinearLeastSquares;print(NonlinearLeastSquares.__version__)"}
 
 default:
 	@echo
 	@echo "  *** Welcome to NonlinearLeastSquares ${VERSION} ***"
 	@echo
 	@echo "  docs   -  Build documentation (html)"
 	@echo "  help   -  Open the documentation"
@@ -13,15 +13,15 @@
 	@echo "  clean  -  Remove temporary files"
 	@echo "  test   -  Run the unittests"
 	@echo "  check  -  Look for rough spots"
 	@echo "  sdist  -  Build a source distribution tar ball"
 
 docs:
 #	pydoc -w NonlinearLeastSquares
-	pydoc -w NonlinearLeastSquares/NonlinearLeastSquares.py
+	pydoc3 -w NonlinearLeastSquares/NonlinearLeastSquares.py
 
 help:
 	open NonlinearLeastSquares-${VERSION}.html
 
 clean:
 	rm -f *.pyc *~
 
@@ -30,15 +30,15 @@
 	rm -rf build dist
 
 # Run the unittest
 test:
 	@echo
 	@echo Testing...
 	@echo
-	./TestNonlinearLeastSquares/Test.py 
+	python3 ./TestNonlinearLeastSquares/Test.py 
 
 sdist: test
 	@echo
 	@echo Building a source distribution...
 	@echo
 	./setup.py sdist --formats=gztar,bztar
```

### Comparing `NonlinearLeastSquares-2.0.0/NonlinearLeastSquares.egg-info/PKG-INFO` & `NonlinearLeastSquares-2.0.1/NonlinearLeastSquares.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: NonlinearLeastSquares
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python module for solving optimization problems with nonlinear least-squares
-Home-page: https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.html
+Home-page: https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.html
 Author: Avinash Kak
 Author-email: kak@purdue.edu
+Maintainer: Avinash Kak
+Maintainer-email: kak@purdue.edu
 License: Python Software Foundation License
-Download-URL: https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.tar.gz
-Description-Content-Type: UNKNOWN
+Download-URL: https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.tar.gz
 Description:  
         
         Consult the module API page at 
         
-              https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.html
+              https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.html
         
         for all information related to this module, including
         information regarding the latest changes to the code. The
         page at the URL shown above lists all of the module
         functionality you can invoke in your own code.  
         
         With regard to the basic purpose of this module, it provides
@@ -46,16 +47,16 @@
         You feed the pixels thus recorded into the
         NonlinearLeastSquares class to estimate the coordinates of
         the scene structure points and, when using uncalibrated
         cameras, to also estimate the extrinsic parameters of the
         camera at each of its positions.
         
         Starting with Version 2.0.0, the module includes code for
-        the bundle-adjustment variant of the Levenberg-Marquardt
-        algorithm.
+        the sparse-bundle-adjustment variant of the
+        Levenberg-Marquardt algorithm.
         
         Typical usage syntax for invoking the domain-agnostic
         NonlinearLeastSquares through your own domain-specific class
         such as OptimizedSurfaceFit or ProjectiveCamera is shown below:
         
         ::
         
@@ -109,12 +110,11 @@
                 result = camera.get_scene_structure_from_camera_motion('lm')
         
                                                OR
         
                 result = camera.get_scene_structure_from_camera_motion_with_bundle_adjustment()
         
                   
-Keywords: gradient descent,nonlinear least-squares,optimization
+Keywords: gradient descent,nonlinear least-squares,optimization,bundle adjustment
 Platform: All platforms
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
```

### Comparing `NonlinearLeastSquares-2.0.0/NonlinearLeastSquares.egg-info/SOURCES.txt` & `NonlinearLeastSquares-2.0.1/NonlinearLeastSquares.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MANIFEST.in
 Makefile
-NonlinearLeastSquares-2.0.0.html
+NonlinearLeastSquares-2.0.1.html
 README
 setup.py
 ExamplesOptimizedSurfaceFit/README
 ExamplesOptimizedSurfaceFit/grad_descent.py
 ExamplesOptimizedSurfaceFit/grad_descent_with_partial_derivatives.py
 ExamplesOptimizedSurfaceFit/leven_marq.py
 ExamplesOptimizedSurfaceFit/leven_marq_with_partial_derivatives.py
```

### Comparing `NonlinearLeastSquares-2.0.0/PKG-INFO` & `NonlinearLeastSquares-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: NonlinearLeastSquares
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python module for solving optimization problems with nonlinear least-squares
-Home-page: https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.html
+Home-page: https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.html
 Author: Avinash Kak
 Author-email: kak@purdue.edu
+Maintainer: Avinash Kak
+Maintainer-email: kak@purdue.edu
 License: Python Software Foundation License
-Download-URL: https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.tar.gz
-Description-Content-Type: UNKNOWN
+Download-URL: https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.tar.gz
 Description:  
         
         Consult the module API page at 
         
-              https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.html
+              https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.html
         
         for all information related to this module, including
         information regarding the latest changes to the code. The
         page at the URL shown above lists all of the module
         functionality you can invoke in your own code.  
         
         With regard to the basic purpose of this module, it provides
@@ -46,16 +47,16 @@
         You feed the pixels thus recorded into the
         NonlinearLeastSquares class to estimate the coordinates of
         the scene structure points and, when using uncalibrated
         cameras, to also estimate the extrinsic parameters of the
         camera at each of its positions.
         
         Starting with Version 2.0.0, the module includes code for
-        the bundle-adjustment variant of the Levenberg-Marquardt
-        algorithm.
+        the sparse-bundle-adjustment variant of the
+        Levenberg-Marquardt algorithm.
         
         Typical usage syntax for invoking the domain-agnostic
         NonlinearLeastSquares through your own domain-specific class
         such as OptimizedSurfaceFit or ProjectiveCamera is shown below:
         
         ::
         
@@ -109,12 +110,11 @@
                 result = camera.get_scene_structure_from_camera_motion('lm')
         
                                                OR
         
                 result = camera.get_scene_structure_from_camera_motion_with_bundle_adjustment()
         
                   
-Keywords: gradient descent,nonlinear least-squares,optimization
+Keywords: gradient descent,nonlinear least-squares,optimization,bundle adjustment
 Platform: All platforms
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
```

### Comparing `NonlinearLeastSquares-2.0.0/README` & `NonlinearLeastSquares-2.0.1/README`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/MANIFEST.in` & `NonlinearLeastSquares-2.0.1/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 include MANIFEST.in
-include NonlinearLeastSquares-2.0.0.html
+include NonlinearLeastSquares-2.0.1.html
 include NonlinearLeastSquares/NonlinearLeastSquares.py
 include NonlinearLeastSquares/__init__.py
 include OptimizedSurfaceFit/OptimizedSurfaceFit.py
 include OptimizedSurfaceFit/__init__.py
 include ProjectiveCamera/ProjectiveCamera.py
 include ProjectiveCamera/__init__.py
 include setup.py
```

### Comparing `NonlinearLeastSquares-2.0.0/setup.py` & `NonlinearLeastSquares-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 #from distutils.core import setup
 
 from setuptools import setup, find_packages
 import sys, os
 
 setup(name='NonlinearLeastSquares',
-      version='2.0.0',
+      version='2.0.1',
       author='Avinash Kak',
       author_email='kak@purdue.edu',
       maintainer='Avinash Kak',
       maintainer_email='kak@purdue.edu',
-      url='https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.html',
-      download_url='https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.tar.gz', 
+      url='https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.html',
+      download_url='https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.tar.gz', 
       description='A Python module for solving optimization problems with nonlinear least-squares',
       long_description=''' 
 
 Consult the module API page at 
 
-      https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.html
+      https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.html
 
 for all information related to this module, including
 information regarding the latest changes to the code. The
 page at the URL shown above lists all of the module
 functionality you can invoke in your own code.  
 
 With regard to the basic purpose of this module, it provides
@@ -54,16 +54,16 @@
 You feed the pixels thus recorded into the
 NonlinearLeastSquares class to estimate the coordinates of
 the scene structure points and, when using uncalibrated
 cameras, to also estimate the extrinsic parameters of the
 camera at each of its positions.
 
 Starting with Version 2.0.0, the module includes code for
-the bundle-adjustment variant of the Levenberg-Marquardt
-algorithm.
+the sparse-bundle-adjustment variant of the
+Levenberg-Marquardt algorithm.
 
 Typical usage syntax for invoking the domain-agnostic
 NonlinearLeastSquares through your own domain-specific class
 such as OptimizedSurfaceFit or ProjectiveCamera is shown below:
 
 ::
 
@@ -119,12 +119,12 @@
                                        OR
 
         result = camera.get_scene_structure_from_camera_motion_with_bundle_adjustment()
 
           ''',
 
       license='Python Software Foundation License',
-      keywords='gradient descent, nonlinear least-squares, optimization',
+      keywords='gradient descent, nonlinear least-squares, optimization, bundle adjustment',
       platforms='All platforms',
-      classifiers=['Topic :: Scientific/Engineering :: Information Analysis', 'Programming Language :: Python :: 2.7', 'Programming Language :: Python :: 3.6'],
+      classifiers=['Topic :: Scientific/Engineering :: Information Analysis', 'Programming Language :: Python :: 3.8'],
       packages=['NonlinearLeastSquares','OptimizedSurfaceFit','ProjectiveCamera']
 )
```

### Comparing `NonlinearLeastSquares-2.0.0/OptimizedSurfaceFit/OptimizedSurfaceFit.py` & `NonlinearLeastSquares-2.0.1/TestNonlinearLeastSquares/OptimizedSurfaceFit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #from NonlinearLeastSquares import NonlinearLeastSquares
 
 ##  OptimizedSurfaceFit.py
-##  Main Module Version: 2.0.0
+##  Main Module Version: 2.0.1
 
 ##  OptimizedSurfaceFit is a part of the Avi Kak's NonlinearLeastSquares Python module
 ##  for demonstrating how the module can be used for optimized fitting of a surface 
 ##  (whose analytical form is known) to noisy data over a plane.
 
 ##  The goal of OptimizedSurfaceFit is to fit a model surface to noisy height data
 ##  over the xy-plane in the xyz-coordinate frame, with the model surface being
@@ -166,15 +166,16 @@
             result_dict = self.optimizer.grad_descent()
         return result_dict
 
     def get_initial_params_from_file(self, filename):
         if not filename.endswith('.txt'): 
             sys.exit("Aborted. _get_initial_params_from_file() is only for CSV files")
         initial_params_dict = {}
-        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line is not '']
+#        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line is not '']
+        initial_params_list = [line for line in [line.strip() for line in open(filename,"rU")] if line != '']
         for record in initial_params_list:
             initial_params_dict[record[:record.find('=')].rstrip()] = float(record[record.find('=')+1:].lstrip())
         self.params_dict = initial_params_dict
         self.params_ordered_list = sorted(self.params_dict)             #need ordered list for jacobian calculations
         return initial_params_dict
 
     def _get_measured_data_from_text_file(self, filename):
@@ -258,15 +259,16 @@
             w,h = self.display_size
             fig = plt.figure(figsize=(w,h))
         else:
             fig = plt.figure()
         new_error_norm_str = "%.4f" % new_error_norm
         fig.suptitle("iteration: " + str(iteration_index) + "     error: " + 
                                                      new_error_norm_str, fontsize=14, fontweight='bold')
-        ax = fig.gca(projection='3d')
+        ##   ax = fig.gca(projection='3d')                
+        ax = fig.add_subplot(111, projection='3d')  ## Version 2.0.1 fix for the above statement
         ## Version 1.5.0 fix:  xx, yy, and zz needed to be turned into numpy arrays
 #        surf = ax.plot_surface(xx, yy, zz, color="yellow")
         surf = ax.plot_surface(numpy.array(xx), numpy.array(yy), numpy.array(zz), color="yellow")
         ax.set_zlim(zmin, zmax)
         ax.scatter(xxx,yyy,zzz, c='r', marker='o')
         ax.set_xlabel("X")
         ax.set_ylabel("Y")
```

### Comparing `NonlinearLeastSquares-2.0.0/OptimizedSurfaceFit/__init__.py` & `NonlinearLeastSquares-2.0.1/OptimizedSurfaceFit/__init__.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/grad_descent_with_partial_derivatives.py` & `NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/grad_descent_with_partial_derivatives.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/leven_marq_with_partial_derivatives.py` & `NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/leven_marq_with_partial_derivatives.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/leven_marq.py` & `NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/leven_marq.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/README` & `NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/README`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/ExamplesOptimizedSurfaceFit/grad_descent.py` & `NonlinearLeastSquares-2.0.1/ExamplesOptimizedSurfaceFit/grad_descent.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/ProjectiveCamera/ProjectiveCamera.py` & `NonlinearLeastSquares-2.0.1/ProjectiveCamera/ProjectiveCamera.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 ##  ProjectiveCamera.py
 
-##  Main Module Version: 2.0.0
+##  Main Module Version: 2.0.1
 
 ##  This class is a part of Avi Kak's Python module named NonlinearLeastSquares.  The purpose of this 
 ##  class is to demonstrate how Nonlinear Least Squares can be used to estimate the scene structure 
 ##  from the motion of the camera.  That is, you move the camera to different positions (and, if 
 ##  desired, different orientations) and record the pixels at each position.  It is relatively easy
 ##  to reconstruct the scene from the pixels thus recorded --- especially if you know the camera
 ##  parameters.  This class simulates the camera and then transforms the pixel data recorded and 
@@ -32,15 +32,21 @@
     '''
     inhomogeneous 3D coordinates expected
     '''
     distance = math.sqrt(reduce(lambda x,y: x+y, map(lambda x: x**2, [(point1[i] - point2[i]) for i in range(len(point1))])))
     return distance
 
 class ProjectiveCamera(object):
-
+    '''    
+    The parameters 'alpha_x' and 'alpha_y' are for the focal length in terms of the image 
+    sampling intervals along the x-axis and along the y-axis, respectively.   The parameters 
+    'x0' and 'y0' are for the coordinates of the point in the camera image plane where the 
+    optic axis penetrates the image plane with respect to the origin in the image plane 
+    (which is usually a corner of the image):
+    '''
     def __init__(self, *args, **kwargs):
         if args:
             raise ValueError(
                     '''Camera constructor can only be called with keyword arguments for the follwoing 
                        keywords: camera_type,alpha_x,alpha_y,x0,y0,camera_rotation,
                        camera_translation, partials_for_jacobian, display_needed''')
         allowed_keys = 'camera_type','alpha_x','alpha_y','x0','y0','camera_rotation','camera_translation','partials_for_jacobian','display_needed'
@@ -188,16 +194,14 @@
     def translate_a_previously_initialized_camera(self, translation):
         '''
         The parameter 'translation' is a 3-element list, with the first element indicating the
         translation along X, the second along Y, and the third along Z.
         '''
         left_3by3 = self.P[0:3,0:3]
         last_column   =  self.P[:,3]
-#        new_last_column = -1.0 * left_3by3 * numpy.asmatrix(translation).T
-#        new_last_column += last_column
         new_last_column = last_column + self.K * numpy.asmatrix(translation).T
         self.P = numpy.append(left_3by3, new_last_column, 1)
         self.motion_history.append(['translate', translation])
 
     def add_new_camera_to_list_of_cameras(self):
         how_many_already = len(self.list_of_cameras)
         self.list_of_cameras[how_many_already] = self.P
@@ -276,18 +280,18 @@
             gt_dict['Z_' + str(point_index)] = world_point_coords[point_index][2]
 #            ground_truth_for_structure += world_point_coords[point_index]
         self.ground_truth_for_structure = ground_truth_for_structure
         return gt_dict
 
     def set_all_parameters_to_ground_truth_for_sanity_check(self, world_point_coords, camera_gt):
         '''
-        This method is useful for sanity checks in your implementation of bundle adjustment.  When you set the
-        camera parameters to their ground truth values, the optimizer should not wander off from those values
-        in its search for the optimum.  Ideally, this would be case if you set ALL the parameters to their
-        ground-truth values.
+        This method is useful for sanity checks in an implementation of sparse bundle adjustment.  When you 
+        set the camera parameters to their ground truth values, the optimizer should not wander off from 
+        those values in its search for the optimum.  Ideally, this would be case if you set ALL the parameters 
+        to their ground-truth values.
         '''
 #        all_params = self.p.flatten().tolist()[0]
         all_params = self.all_params_list
         number_of_cams = len(self.list_of_cameras)
         all_camera_params = all_params[:6*number_of_cams]
         structure_params =  all_params[6*number_of_cams:]
         gt_dict = {all_params[i] : 0.0 for i in range(len(all_params))}
@@ -468,44 +472,14 @@
         world_points_xformed = []
         for pt in world_points_xformed_homogeneous:
             world_points_xformed.append( pt[:,0].flatten().tolist()[0] )
         print("\nworld points transformed: %s" % str(world_points_xformed))
         self.world_points_xformed = world_points_xformed
         return world_points_xformed
 
-    def display_structure_and_pixels_XXXXXXXXXXXXXXXX(self, measured_pixels, predicted_pixels):
-        fig = plt.figure(1)
-#        fig1.suptitle("Showing the measured pixels")
-        ax1 = fig.add_subplot(211)
-        subplt1 = plt.subplot(211)
-        plt.title("Showing the measured pixels")
-        xm_coords = [pixel[0] for pixel in measured_pixels]
-        ym_coords = [pixel[1] for pixel in measured_pixels]
-        subplt1.plot(xm_coords, ym_coords, 'ro')
-        xp_coords = [pixel[0] for pixel in predicted_pixels]
-        yp_coords = [pixel[1] for pixel in predicted_pixels]
-        subplt1.plot(xp_coords, yp_coords, 'bo')
-        ax1.set_xlabel('x')
-        ax1.set_ylabel('y')
-
-        plt.subplots_adjust(hspace = 0.5)                     # h stands for height space between the two subplots
-
-#        fig2 = plt.figure(2)
-        ax2 = fig.add_subplot(211)
-        subplt2 = plt.subplot(212)
-        plt.title("Showing more pixels")
-        x_coords = [pixel[0] for pixel in measured_pixels]
-        y_coords = [pixel[1] for pixel in measured_pixels]
-#        min_x,max_x = min(x_coords),max(x_coords)
-#        min_y,max_y = min(y_coords),max(y_coords)
-        subplt2.plot(x_coords, y_coords, 'bx')
-        plt.show()
-
-
-
     def display_structure_and_pixels(self, predicted_pixels=None, scene_structure=None, reprojection_error=None, iteration_index=None):
         try:
             measured_pixel_coords =  self.X.flatten().tolist()[0]
         except:
             measured_pixel_coords =  self.X_BA.flatten().tolist()[0]
         measured_pixels = [(measured_pixel_coords[2*x], measured_pixel_coords[2*x+1]) for x in range(len(measured_pixel_coords) // 2)]
         if self.tracked_point_indexes_for_display is not None:
@@ -709,21 +683,21 @@
 
 
     def construct_X_vector_for_bundle_adjustment(self, pixel_coordinates):
         '''
         The function parameter 'pixel_coordinates' is a list of lists (LoL), with each list in LoL being 
         the set of pixels recorded from one position and orientation of the camera.
 
-        For bundle adjustment logic, the elements of the measurement vector X need to be arranged differently
-        from what is accomplished by the previous method.  You need to arrange the pixels in the world-point
-        order as opposed to the camera order.  To explan, let's say you have m cameras and n world points.
-        Your first 2m elements in the X vector will be for THE FIRST WORLD POINT in ALL of the m cameras.
-        Of these 2m elements, the first two elements will be for the x- and the y-coordinates of the first
-        world point in the first camera.  The next pair of two elements will be for the SAME world point
-        but in the second camera, and so on.
+        For sparse bundle adjustment logic, the elements of the measurement vector X need to be arranged 
+        differently from what is accomplished by the previous method.  You need to arrange the pixels in 
+        the world-point order as opposed to the camera order.  To explan, let's say you have m cameras and 
+        n world points. Your first 2m elements in the X vector will be for THE FIRST WORLD POINT in ALL 
+        of the m cameras.  Of these 2m elements, the first two elements will be for the x- and the 
+        y-coordinates of the first world point in the first camera.  The next pair of two elements will be 
+        for the SAME world point but in the second camera, and so on.
         '''
         #  Since 'pixel_coordinates' is a LIST OF LISTS, with each list being for one camera pos, 
         #  we can say:
         print("\nnumber of camera positions: %d" % self.num_cameras)        
         X = []
         for point_index in range(self.num_world_points):
             for cam_index in range(self.num_cameras):
@@ -749,15 +723,18 @@
         ''' 
         This method is for demonstrating the most general case of estimating the camera matrix directly
         for each position of the camera WITHOUT placing any R-induced constraints on the elements of the
         matrix --- which is NEVER a good thing to do but nonethless useful for educational purposes.
 
         This method constructs the Prediction Vector for the observed data in "self.X". This is a vector 
         of the same size as the number of measurements in "self.X". The elements of the Prediction Vector 
-        are functional involving the parameters to be estimated.
+        are functionals involving the parameters to be estimated.
+
+        Think of p_c as your 3x4 camera projection matrix for the camera indexed 'c' and p_c_ij its 
+        ij-th element.
         '''
         functional_x =  '(p_c_11*X_ + p_c_12*Y_ + p_c_13*Z_ + p_c_14) / (p_c_31*X_ + p_c_32*Y_ + p_c_33*Z_ + p_c_34)' 
         functional_y =  '(p_c_21*X_ + p_c_22*Y_ + p_c_23*Z_ + p_c_24) / (p_c_31*X_ + p_c_32*Y_ + p_c_33*Z_ + p_c_34)' 
         Fvec = []
         for i in range(self.num_cameras):
             functional_x_for_cam = str.replace( functional_x, 'c', str(i) )
             functional_y_for_cam = str.replace( functional_y, 'c', str(i) )
@@ -842,32 +819,45 @@
         return R
     
     def construct_Fvec_for_uncalibrated_cameras_with_known_intrinsic_params_no_rodrigues(self):
         ''' 
         We assume that the intrinsic parameter matrix K is known, but the extrinsic parameters for
         each of the camara positions is NOT known.  However, we place no R-induced constraints when
         calculating the extrinsic parameters --- WHICH IS NEVER A SAFE THING TO DO but nonetheless
-        useful for educational demonstrations.
+        useful for educational demonstrations.  "No R-induced" stands for "no Rodrigues".
 
         This method constructs the Prediction Vector for the observed data in "self.X". This is a vector 
         of the same size as the number of measurements in "self.X". The elements of the Prediction Vector 
-        are functional involving the parameters to be estimated.
+        are functionals involving the parameters to be estimated.
 
         Since we know the intrinsic parameters of the camera, we know (p_x,p_y).  These are the coordinates
-        of the center of the image frame where the optic axis penetrates with the image origin in the 
-        camera image plane.
+        of the center of the image frame where the optic axis penetrates origin in the camera image plane.
+        Notice how we replace p_x by the intrinsic element K[0,2] and p_y by K[1,2] when we construct
+        functional_x_for_cam and functional_y_for_cam which are the x- and the y-coordinates of the
+        predicted position of the pixel for a given world point.
+
+        As can be seen from the constructions for functional_x_for_cam and functional_y_for_cam, 
+        the meaning of f_x is the same as K[0,0] and that of f_y the same as K[1,1] where K is the
+        3x3 intrinsic matrix for for the camera.
+
+        r_c is the 3x3 rotation matrix and t_c the 3-element translational vector for the c-th camera.
         '''
         functional_x =  '(  f_x   * (r_c_11*X_ + r_c_12*Y_ + r_c_13*Z_ + t_c_x)  +             \
                             alpha * (r_c_21*X_ + r_c_22*Y_ + r_c_23*Z_ + t_c_y)  +             \
                             p_x   * (r_c_31*X_ + r_c_32*Y_ + r_c_33*Z_ + t_c_z)   )  /         \
                                     (r_c_31*X_ + r_c_32*Y_ + r_c_33*Z_ + t_c_z)'
         functional_y =  '(  f_y   * (r_c_21*X_ + r_c_22*Y_ + r_c_23*Z_ + t_c_y)  +             \
                             p_y   * (r_c_31*X_ + r_c_32*Y_ + r_c_33*Z_ + t_c_z)   )  /         \
                                     (r_c_31*X_ + r_c_32*Y_ + r_c_33*Z_ + t_c_z)'
 
+        ##  Our goal now is to construct a prediction for each of the observed pixels in all of
+        ##  the camera positions. The functional_x shown above is a generic form of this prediction
+        ##  for the horizontal coordinate of a pixel and functional_y for the vertical coordinate
+        ##  in the the c-th camera in terms of the rotation matrix r_c and the translation vector
+        ##  t_c for the camera.
         Fvec = []
         for i in range(self.num_cameras):
             functional_x_for_cam = str.replace( functional_x, 'c', str(i) )
             functional_x_for_cam = str.replace( functional_x_for_cam, 'f_x',   str(self.K[0,0]) )
             functional_x_for_cam = str.replace( functional_x_for_cam, 'alpha', str(self.K[0,1]) )
             functional_x_for_cam = str.replace( functional_x_for_cam, 'p_x',   str(self.K[0,2]) )
             functional_y_for_cam = str.replace( functional_y, 'c', str(i) )
@@ -890,20 +880,30 @@
 
     def construct_Fvec_for_uncalibrated_cameras_with_known_intrinsic_params_and_with_rodrigues_rotations(self):
         ''' 
         This method constructs the Prediction Vector for the observed data in "self.X". This is a vector 
         of the same size as the number of measurements in "self.X". The elements of the Prediction Vector 
         are functional involving the parameters to be estimated.
 
+        Recall that the elements of self.X alternate between the x- and the y-coordinates for all the pixels
+        observed in all of the camera positions.  So if you are tracking N world points in M camera images,
+        the size of self.X is 2NM.
+
         Since we know the intrinsic parameters of the camera, we know (p_x,p_y).  These are the coordinates
         of the center of the image frame where the optic axis penetrates with the image origin in the 
-        camera image plane.
+        camera image plane.  As mentioned earlier, the meaning of p_x is the same as that for K[0,2] and
+        of p_y the same as for K[1,2] in the 3x3 intrinsic parameter matrix K.
 
         You need to place each element that eventually is replaced by a numerical value by a parenthesized form.
         If you don't, you end up with things like '+-0.45634**2' which confuses the math processor.
+
+        In what follows, w_c is the 3-element Rodrigues vector that represents for the 3x3 rotation matrix
+        r_c for the c-th camera.  The three elements of w_c are denoted (w_c_x, w_c_y, w_c_z).  We start with
+        how to get the nine elements of the matrix r_c from the 3 elements of the vector w_c.
+
         '''
 #       r_11  =  wx**2             +      (1-wx**2)*cphi                          (shown without normalization)
         r_c_11  =  '((w_c_x)**2) / ((w_c_x)**2+(w_c_y)**2+(w_c_z)**2)  +  (1 - ((w_c_x)**2) / ((w_c_x)**2+(w_c_y)**2+(w_c_z)**2))*scipy.cos(math.sqrt((w_c_x)**2+(w_c_y)**2+(w_c_z)**2))' 
 #       r_12  =  wx*wy*(1-cphi)    -      wz*sphi
         r_c_12  =  '((w_c_x)*(w_c_y)/((w_c_x)**2+(w_c_y)**2+(w_c_z)**2))*(1 - scipy.cos(math.sqrt((w_c_x)**2+(w_c_y)**2+(w_c_z)**2)))  -   ((w_c_z) / math.sqrt((w_c_x)**2+(w_c_y)**2+(w_c_z)**2)) * scipy.sin(math.sqrt((w_c_x)**2+(w_c_y)**2+(w_c_z)**2))'
 #       r_13  =  wx*wz*(1-cphi)    +      wy*sphi
         r_c_13  =  '((w_c_x)*(w_c_z)/((w_c_x)**2+(w_c_y)**2+(w_c_z)**2))*(1 - scipy.cos(math.sqrt((w_c_x)**2+(w_c_y)**2+(w_c_z)**2)))  +   ((w_c_y) / math.sqrt((w_c_x)**2+(w_c_y)**2+(w_c_z)**2))*scipy.sin(math.sqrt((w_c_x)**2+(w_c_y)**2+(w_c_z)**2))'
```

### Comparing `NonlinearLeastSquares-2.0.0/ProjectiveCamera/__init__.py` & `NonlinearLeastSquares-2.0.1/ProjectiveCamera/__init__.py`

 * *Files identical despite different names*

### Comparing `NonlinearLeastSquares-2.0.0/NonlinearLeastSquares-2.0.0.html` & `NonlinearLeastSquares-2.0.1/NonlinearLeastSquares-2.0.1.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <!doctype html PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
 <html><head>
 <title>
-NonlinearLeastSquares-2.0.0.html
+NonlinearLeastSquares-2.0.1.html
 </title>
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
 </head>
 <body bgcolor="#f0f0f8">
 <table width="100%" cellspacing="0" cellpadding="2" border="0" summary="heading">
 <tr bgcolor="#7799ee">
 <td valign=bottom>&nbsp;<br>
-<font color="#ffffff" face="helvetica, arial">&nbsp;<br><big><big><strong>NonlinearLeastSquares</strong></big></big> (version 2.0.0, 2018-November-9)</font></td
+<font color="#ffffff" face="helvetica, arial">&nbsp;<br><big><big><strong>NonlinearLeastSquares</strong></big></big> (version 2.0.1, 2022-October-6)</font></td
 ><td align=right valign=bottom
 ><font color="#ffffff" face="helvetica, arial">
 </font></td></tr></table>
 <p><a href="#NonlinearLeastSquares"><tt>NonlinearLeastSquares</tt></a>.py<br>
 <tt>
 &nbsp;<br>
-Version:&nbsp;2.0.0<br>
+Version:&nbsp;2.0.1<br>
 &nbsp;&nbsp;&nbsp;<br>
 Author:&nbsp;Avinash&nbsp;Kak&nbsp;(kak@purdue.edu)<br>
 &nbsp;<br>
-Date:&nbsp;2018-November-9<br>
+Date:&nbsp;2022-October-6<br>
 &nbsp;<br>
 &nbsp;<br>
 </tt>
 <TABLE BORDER="0" CELLPADDING="0" CELLSPACING="2"> 
 <TR>
 <TH ALIGN=left>
 <tt>
-<b>Download Version 2.0.0:</b>&nbsp;  
-<a HREF="https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.tar.gz?download">gztar</a> 
+<b>Download Version 2.0.1:</b>&nbsp;  
+<a HREF="https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.tar.gz?download">gztar</a> 
 &nbsp;             
 <br>
 <br>
 &nbsp;
 </tt>
 </TH>
 <TD>
@@ -65,27 +65,36 @@
 ?>
 </font>
 </tt>
 </center>
 </TD>
 </TR>
 </TABLE>
+<br>
 <tt>
-<a HREF="NonlinearLeastSquares-2.0.0_CodeOnly.html">View the main module file in your browser</a> 
-&nbsp;<br><br>
-<a HREF="OptimizedSurfaceFit-2.0.0_CodeOnly.html">View the code for OptimizedSurfaceFit for optimized surface fitting to noisy height data </a> <br><br>
-<a HREF="ProjectiveCamera-2.0.0_CodeOnly.html">View the code for ProjectiveCamera that shows how to calculate the structure of a scene with a moving camera </a> <br>
+<a HREF="NonlinearLeastSquares-2.0.1_CodeOnly.html">View the main module file in your browser</a> 
+&nbsp;<br>
+<a HREF="OptimizedSurfaceFit-2.0.1_CodeOnly.html">View the code for OptimizedSurfaceFit for optimized surface fitting to noisy height data </a> <br>
+<a HREF="ProjectiveCamera-2.0.1_CodeOnly.html">View the code for ProjectiveCamera for camera modeling</a> <br>
 
 &nbsp;<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">CHANGES:<br>
 </font>
 <br>
 
+&nbsp;&nbsp;Version&nbsp;2.0.1:<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Cleaned&nbsp;up&nbsp;the&nbsp;code&nbsp;to&nbsp;make&nbsp;it&nbsp;work&nbsp;with&nbsp;the&nbsp;current&nbsp;version&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;matplotlib&nbsp;library&nbsp;that&nbsp;is&nbsp;used&nbsp;for&nbsp;displaying&nbsp;the&nbsp;results.&nbsp;&nbsp;I&nbsp;have&nbsp;also<br>
+&nbsp;&nbsp;&nbsp;&nbsp;removed&nbsp;the&nbsp;use&nbsp;of&nbsp;the&nbsp;"is"&nbsp;and&nbsp;"is&nbsp;not"&nbsp;comparison&nbsp;operators&nbsp;for&nbsp;numeric<br>
+&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;string&nbsp;literals&nbsp;since&nbsp;such&nbsp;use&nbsp;has&nbsp;now&nbsp;been&nbsp;deprecated.&nbsp;&nbsp;Also&nbsp;added<br>
+&nbsp;&nbsp;&nbsp;&nbsp;additional&nbsp;comment&nbsp;blocks&nbsp;to&nbsp;the&nbsp;main&nbsp;functions&nbsp;in&nbsp;the&nbsp;module&nbsp;file.<br>
+&nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.0.0:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;includes&nbsp;sparse&nbsp;bundle&nbsp;adjustment&nbsp;(SBA)&nbsp;to&nbsp;speed&nbsp;up&nbsp;code<br>
 &nbsp;&nbsp;&nbsp;&nbsp;execution&nbsp;when&nbsp;using&nbsp;nonlinear&nbsp;least-squares&nbsp;for&nbsp;solving<br>
 &nbsp;&nbsp;&nbsp;&nbsp;structure-from-camera-motion&nbsp;problems&nbsp;with&nbsp;uncalibrated&nbsp;cameras.&nbsp;&nbsp;SBA<br>
 &nbsp;&nbsp;&nbsp;&nbsp;exploits&nbsp;the&nbsp;sparseness&nbsp;of&nbsp;the&nbsp;Jacobian&nbsp;encountered&nbsp;in&nbsp;such&nbsp;problems.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;also&nbsp;includes&nbsp;improvements&nbsp;to&nbsp;the&nbsp;Levenberg-Marquardt&nbsp;code<br>
@@ -94,47 +103,46 @@
 &nbsp;&nbsp;&nbsp;&nbsp;provides&nbsp;additional&nbsp;methods&nbsp;for&nbsp;the&nbsp;visualization&nbsp;of&nbsp;the&nbsp;results.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;1.5.0:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;adds&nbsp;a&nbsp;new&nbsp;class,&nbsp;ProjectiveCamera,&nbsp;to&nbsp;the&nbsp;module&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;demonstrating&nbsp;how&nbsp;nonlinear&nbsp;least-squares&nbsp;can&nbsp;be&nbsp;used&nbsp;for&nbsp;estimating<br>
 &nbsp;&nbsp;&nbsp;&nbsp;structure&nbsp;of&nbsp;a&nbsp;scene&nbsp;from&nbsp;the&nbsp;data&nbsp;recorded&nbsp;with&nbsp;a&nbsp;calibrated&nbsp;camera&nbsp;in<br>
-&nbsp;&nbsp;&nbsp;&nbsp;motion.&nbsp;&nbsp;For&nbsp;a&nbsp;simulated&nbsp;demonstration,&nbsp;you&nbsp;can&nbsp;create&nbsp;calibrated<br>
-&nbsp;&nbsp;&nbsp;&nbsp;cameras&nbsp;from&nbsp;a&nbsp;generic&nbsp;instance&nbsp;of&nbsp;the&nbsp;ProjectiveCamera&nbsp;class&nbsp;that&nbsp;is<br>
-&nbsp;&nbsp;&nbsp;&nbsp;then&nbsp;subject&nbsp;to&nbsp;various&nbsp;translational&nbsp;and&nbsp;rotational&nbsp;transformations.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;motion.&nbsp;&nbsp;For&nbsp;a&nbsp;simulated&nbsp;demonstration,&nbsp;you&nbsp;can&nbsp;create&nbsp;calibrated&nbsp;cameras<br>
+&nbsp;&nbsp;&nbsp;&nbsp;from&nbsp;a&nbsp;generic&nbsp;instance&nbsp;of&nbsp;the&nbsp;ProjectiveCamera&nbsp;class&nbsp;that&nbsp;is&nbsp;then&nbsp;subject<br>
+&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;various&nbsp;translational&nbsp;and&nbsp;rotational&nbsp;transformations.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;1.1.1:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;includes&nbsp;constructor&nbsp;options&nbsp;to&nbsp;control&nbsp;the&nbsp;size&nbsp;and&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;position&nbsp;of&nbsp;the&nbsp;graphics&nbsp;for&nbsp;displaying&nbsp;the&nbsp;results&nbsp;of&nbsp;nonlinear<br>
 &nbsp;&nbsp;&nbsp;&nbsp;least-squares&nbsp;optimization.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;1.1:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;fixes&nbsp;a&nbsp;bug&nbsp;in&nbsp;the&nbsp;synthetic&nbsp;data&nbsp;generator&nbsp;function&nbsp;used<br>
-&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;illustrating&nbsp;the&nbsp;functionality&nbsp;of&nbsp;the&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;class.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Changes&nbsp;also&nbsp;made&nbsp;to&nbsp;the&nbsp;information&nbsp;that&nbsp;is&nbsp;printed&nbsp;out&nbsp;when&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;module&nbsp;is&nbsp;run&nbsp;in&nbsp;the&nbsp;debug&nbsp;mode.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;fixes&nbsp;a&nbsp;bug&nbsp;in&nbsp;the&nbsp;synthetic&nbsp;data&nbsp;generator&nbsp;function&nbsp;used&nbsp;for<br>
+&nbsp;&nbsp;&nbsp;&nbsp;illustrating&nbsp;the&nbsp;functionality&nbsp;of&nbsp;the&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;class.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Changes&nbsp;also&nbsp;made&nbsp;to&nbsp;the&nbsp;information&nbsp;that&nbsp;is&nbsp;printed&nbsp;out&nbsp;when&nbsp;the&nbsp;module<br>
+&nbsp;&nbsp;&nbsp;&nbsp;is&nbsp;run&nbsp;in&nbsp;the&nbsp;debug&nbsp;mode.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;1.0:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;In&nbsp;the&nbsp;form&nbsp;of&nbsp;a&nbsp;class&nbsp;named&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>,&nbsp;this&nbsp;module<br>
-&nbsp;&nbsp;&nbsp;&nbsp;provides&nbsp;a&nbsp;domain&nbsp;agnostic&nbsp;implementation&nbsp;of&nbsp;nonlinear&nbsp;least-squares<br>
-&nbsp;&nbsp;&nbsp;&nbsp;algorithms&nbsp;(gradient-descent&nbsp;and&nbsp;Levenberg-Marquardt)&nbsp;for&nbsp;fitting&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;model&nbsp;to&nbsp;observed&nbsp;data.&nbsp;&nbsp;Typically,&nbsp;the&nbsp;model&nbsp;involves&nbsp;several<br>
-&nbsp;&nbsp;&nbsp;&nbsp;parameters&nbsp;and&nbsp;each&nbsp;observed&nbsp;data&nbsp;element&nbsp;can&nbsp;be&nbsp;expressed&nbsp;as&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;function&nbsp;of&nbsp;those&nbsp;parameters&nbsp;plus&nbsp;noise.&nbsp;&nbsp;The&nbsp;goal&nbsp;of&nbsp;nonlinear<br>
-&nbsp;&nbsp;&nbsp;&nbsp;least-squares&nbsp;is&nbsp;to&nbsp;estimate&nbsp;the&nbsp;best&nbsp;values&nbsp;for&nbsp;the&nbsp;parameters&nbsp;given<br>
-&nbsp;&nbsp;&nbsp;&nbsp;all&nbsp;of&nbsp;the&nbsp;observed&nbsp;data.&nbsp;&nbsp;In&nbsp;order&nbsp;to&nbsp;illustrate&nbsp;how&nbsp;to&nbsp;use&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;class,&nbsp;the&nbsp;module&nbsp;also&nbsp;comes&nbsp;with&nbsp;another&nbsp;class,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;OptimizeSurfaceFit,&nbsp;whose&nbsp;job&nbsp;is&nbsp;to&nbsp;fit&nbsp;the&nbsp;best&nbsp;surface&nbsp;(of&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;specified&nbsp;analytical&nbsp;form)&nbsp;to&nbsp;noisy&nbsp;height&nbsp;data&nbsp;over&nbsp;the&nbsp;XY-plane.&nbsp;The<br>
-&nbsp;&nbsp;&nbsp;&nbsp;model&nbsp;in&nbsp;this&nbsp;case&nbsp;is&nbsp;the&nbsp;analytical&nbsp;description&nbsp;of&nbsp;the&nbsp;surface&nbsp;and&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;goal&nbsp;of&nbsp;nonlinear&nbsp;least-squares&nbsp;is&nbsp;to&nbsp;estimate&nbsp;the&nbsp;best&nbsp;values&nbsp;for&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;parameters&nbsp;in&nbsp;the&nbsp;analytical&nbsp;description.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;In&nbsp;the&nbsp;form&nbsp;of&nbsp;a&nbsp;class&nbsp;named&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>,&nbsp;this&nbsp;module&nbsp;provides&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;domain&nbsp;agnostic&nbsp;implementation&nbsp;of&nbsp;nonlinear&nbsp;least-squares&nbsp;algorithms<br>
+&nbsp;&nbsp;&nbsp;&nbsp;(gradient-descent&nbsp;and&nbsp;Levenberg-Marquardt)&nbsp;for&nbsp;fitting&nbsp;a&nbsp;model&nbsp;to&nbsp;observed<br>
+&nbsp;&nbsp;&nbsp;&nbsp;data.&nbsp;&nbsp;Typically,&nbsp;the&nbsp;model&nbsp;involves&nbsp;several&nbsp;parameters&nbsp;and&nbsp;each&nbsp;observed<br>
+&nbsp;&nbsp;&nbsp;&nbsp;data&nbsp;element&nbsp;can&nbsp;be&nbsp;expressed&nbsp;as&nbsp;a&nbsp;function&nbsp;of&nbsp;those&nbsp;parameters&nbsp;plus<br>
+&nbsp;&nbsp;&nbsp;&nbsp;noise.&nbsp;&nbsp;The&nbsp;goal&nbsp;of&nbsp;nonlinear&nbsp;least-squares&nbsp;is&nbsp;to&nbsp;estimate&nbsp;the&nbsp;best&nbsp;values<br>
+&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;the&nbsp;parameters&nbsp;given&nbsp;all&nbsp;of&nbsp;the&nbsp;observed&nbsp;data.&nbsp;&nbsp;In&nbsp;order&nbsp;to&nbsp;illustrate<br>
+&nbsp;&nbsp;&nbsp;&nbsp;how&nbsp;to&nbsp;use&nbsp;the&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;class,&nbsp;the&nbsp;module&nbsp;also&nbsp;comes&nbsp;with<br>
+&nbsp;&nbsp;&nbsp;&nbsp;another&nbsp;class,&nbsp;OptimizeSurfaceFit,&nbsp;whose&nbsp;job&nbsp;is&nbsp;to&nbsp;fit&nbsp;the&nbsp;best&nbsp;surface<br>
+&nbsp;&nbsp;&nbsp;&nbsp;(of&nbsp;a&nbsp;specified&nbsp;analytical&nbsp;form)&nbsp;to&nbsp;noisy&nbsp;height&nbsp;data&nbsp;over&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;XY-plane.&nbsp;The&nbsp;model&nbsp;in&nbsp;this&nbsp;case&nbsp;is&nbsp;the&nbsp;analytical&nbsp;description&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;surface&nbsp;and&nbsp;the&nbsp;goal&nbsp;of&nbsp;nonlinear&nbsp;least-squares&nbsp;is&nbsp;to&nbsp;estimate&nbsp;the&nbsp;best<br>
+&nbsp;&nbsp;&nbsp;&nbsp;values&nbsp;for&nbsp;the&nbsp;parameters&nbsp;in&nbsp;the&nbsp;analytical&nbsp;description.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size=+2 color="red">USAGE&nbsp;FOR&nbsp;OPTIMAL&nbsp;SURFACE&nbsp;FITTING:<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;module&nbsp;includes&nbsp;a&nbsp;domain&nbsp;specific&nbsp;class,&nbsp;OptimizedSurfaceFit,&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;demonstrating&nbsp;how&nbsp;nonlinear&nbsp;least-squares&nbsp;in&nbsp;the&nbsp;form&nbsp;of&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Levenberg-Marquardt&nbsp;algorithm&nbsp;can&nbsp;be&nbsp;used&nbsp;for&nbsp;optimally&nbsp;fitting<br>
@@ -265,39 +273,40 @@
 &nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;ExamplesStructureFromCameraMotion&nbsp;subdirectory&nbsp;of&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;distribution&nbsp;for&nbsp;further&nbsp;information&nbsp;on&nbsp;what&nbsp;calls&nbsp;you&nbsp;need&nbsp;to&nbsp;sequence<br>
 &nbsp;&nbsp;&nbsp;&nbsp;together&nbsp;for&nbsp;estimating&nbsp;the&nbsp;structure&nbsp;of&nbsp;a&nbsp;scene&nbsp;that&nbsp;is&nbsp;being&nbsp;viewed<br>
 &nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;a&nbsp;moving&nbsp;camera.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size=+2 color="red">USING&nbsp;SPARSE&nbsp;BUNDLE&nbsp;ADJUSTMENT&nbsp;FOR&nbsp;ESTIMATING&nbsp;THE&nbsp;SCENE&nbsp;STRUCTURE&nbsp;WITH&nbsp;<br>
-AN&nbsp;UNCALIBRATED&nbsp;CAMERA&nbsp;IN&nbsp;MOTION:<br></font>
+</font>AN&nbsp;UNCALIBRATED&nbsp;CAMERA&nbsp;IN&nbsp;MOTION:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;You&nbsp;would&nbsp;again&nbsp;need&nbsp;to&nbsp;construct&nbsp;an&nbsp;instance&nbsp;of&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;and&nbsp;an&nbsp;instance&nbsp;of&nbsp;the&nbsp;ProjectiveCamera&nbsp;class&nbsp;as<br>
 &nbsp;&nbsp;&nbsp;&nbsp;shown&nbsp;in&nbsp;lines&nbsp;(F)&nbsp;and&nbsp;(G)&nbsp;above.&nbsp;&nbsp;But&nbsp;now&nbsp;you&nbsp;would&nbsp;need&nbsp;to&nbsp;replace<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;code&nbsp;in&nbsp;lines&nbsp;(H)&nbsp;through&nbsp;(K)&nbsp;by:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;camera.construct_X_vector_for_bundle_adjustment(&nbsp;all_pixels&nbsp;)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#(L)<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;camera.construct_parameter_vec_for_uncalibrated_cameras_with_rodrigues_rotations()<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#(M)<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;camera.construct_Fvec_for_bundle_adjustment()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#(O)<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;result&nbsp;=&nbsp;camera.get_scene_structure_from_camera_motion_with_bundle_adjustment()<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#(P)<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;construction&nbsp;of&nbsp;the&nbsp;observation&nbsp;vector&nbsp;X&nbsp;in&nbsp;line&nbsp;(L)&nbsp;is&nbsp;specific&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;bundle&nbsp;adjustment&nbsp;---&nbsp;in&nbsp;the&nbsp;sense&nbsp;that&nbsp;you&nbsp;first&nbsp;want&nbsp;to&nbsp;list&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;pixels&nbsp;in&nbsp;all&nbsp;the&nbsp;cameras&nbsp;for&nbsp;the&nbsp;first&nbsp;world&nbsp;point,&nbsp;then&nbsp;you&nbsp;want&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;list&nbsp;the&nbsp;pixels&nbsp;in&nbsp;all&nbsp;the&nbsp;cameras&nbsp;for&nbsp;the&nbsp;second&nbsp;world&nbsp;point,&nbsp;and&nbsp;so<br>
-&nbsp;&nbsp;&nbsp;&nbsp;on.&nbsp;&nbsp;Ordering&nbsp;the&nbsp;observed&nbsp;data&nbsp;in&nbsp;this&nbsp;fashion&nbsp;is&nbsp;necessary&nbsp;to&nbsp;create<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;sort&nbsp;of&nbsp;block&nbsp;sparsity&nbsp;in&nbsp;the&nbsp;Jacobian&nbsp;that&nbsp;is&nbsp;exploited&nbsp;in&nbsp;SBA.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;sparse&nbsp;bundle&nbsp;adjustment&nbsp;---&nbsp;in&nbsp;the&nbsp;sense&nbsp;that&nbsp;you&nbsp;first&nbsp;want&nbsp;to&nbsp;list<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;pixels&nbsp;in&nbsp;all&nbsp;the&nbsp;cameras&nbsp;for&nbsp;the&nbsp;first&nbsp;world&nbsp;point,&nbsp;then&nbsp;you&nbsp;want<br>
+&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;list&nbsp;the&nbsp;pixels&nbsp;in&nbsp;all&nbsp;the&nbsp;cameras&nbsp;for&nbsp;the&nbsp;second&nbsp;world&nbsp;point,&nbsp;and<br>
+&nbsp;&nbsp;&nbsp;&nbsp;so&nbsp;on.&nbsp;&nbsp;Ordering&nbsp;the&nbsp;observed&nbsp;data&nbsp;in&nbsp;this&nbsp;fashion&nbsp;is&nbsp;necessary&nbsp;to<br>
+&nbsp;&nbsp;&nbsp;&nbsp;create&nbsp;the&nbsp;sort&nbsp;of&nbsp;block&nbsp;sparsity&nbsp;in&nbsp;the&nbsp;Jacobian&nbsp;that&nbsp;is&nbsp;exploited&nbsp;in<br>
+&nbsp;&nbsp;&nbsp;&nbsp;SBA.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Note&nbsp;that&nbsp;we&nbsp;assume&nbsp;that&nbsp;the&nbsp;intrinsic&nbsp;parameters&nbsp;of&nbsp;the&nbsp;camera&nbsp;are<br>
 &nbsp;&nbsp;&nbsp;&nbsp;known&nbsp;already.&nbsp;&nbsp;So&nbsp;the&nbsp;goal&nbsp;of&nbsp;the&nbsp;bundle&nbsp;adjustment&nbsp;is&nbsp;to&nbsp;estimate&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;six&nbsp;extrinsic&nbsp;parameters,&nbsp;the&nbsp;three&nbsp;for&nbsp;translation&nbsp;of&nbsp;the&nbsp;camera&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;three&nbsp;(in&nbsp;the&nbsp;form&nbsp;of&nbsp;Rodrigues&nbsp;rotations)&nbsp;for&nbsp;the&nbsp;rotation.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;six&nbsp;extrinsic&nbsp;parameters,&nbsp;three&nbsp;for&nbsp;translation&nbsp;of&nbsp;the&nbsp;camera&nbsp;and&nbsp;three<br>
+&nbsp;&nbsp;&nbsp;&nbsp;(in&nbsp;the&nbsp;form&nbsp;of&nbsp;Rodrigues&nbsp;rotations)&nbsp;for&nbsp;the&nbsp;rotation.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;See&nbsp;the&nbsp;script&nbsp;<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;ExamplesStructureFromCameraMotion&nbsp;subdirectory&nbsp;of&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;distribution&nbsp;for&nbsp;further&nbsp;information&nbsp;on&nbsp;what&nbsp;calls&nbsp;you&nbsp;need&nbsp;to&nbsp;sequence<br>
@@ -874,18 +883,16 @@
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;responsibility&nbsp;of&nbsp;this&nbsp;method&nbsp;is&nbsp;to&nbsp;take&nbsp;all&nbsp;of&nbsp;the&nbsp;user<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;supplied&nbsp;information&nbsp;and&nbsp;reconstitute&nbsp;it&nbsp;into&nbsp;a&nbsp;form&nbsp;that&nbsp;is<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;needed&nbsp;by&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;taking&nbsp;into&nbsp;account&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;peculiarities&nbsp;of&nbsp;your&nbsp;domain.<br>
 &nbsp;<br>
 &nbsp;<br>
-<font size=+2 color="red">ESTIMATING&nbsp;SCENE&nbsp;STRUCTURE&nbsp;WHEN&nbsp;USING&nbsp;A&nbsp;CALIBRATED&nbsp;<br>
-CAMERA&nbsp;IN&nbsp;MOTION:<br>
-</font>
-&nbsp;<br>
+<font size=+2 color="red">ESTIMATING&nbsp;SCENE&nbsp;STRUCTURE&nbsp;WHEN&nbsp;USING&nbsp;A&nbsp;CALIBRATED&nbsp;CAMERA&nbsp;IN&nbsp;MOTION:<br>
+</font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;section&nbsp;presents&nbsp;a&nbsp;class&nbsp;named&nbsp;ProjectiveCamera&nbsp;to&nbsp;illustrate&nbsp;how<br>
 &nbsp;&nbsp;&nbsp;&nbsp;you&nbsp;can&nbsp;use&nbsp;the&nbsp;functionality&nbsp;of&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;in&nbsp;your&nbsp;own&nbsp;code<br>
 &nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;estimating&nbsp;the&nbsp;structure&nbsp;of&nbsp;a&nbsp;3D&nbsp;scene&nbsp;from&nbsp;the&nbsp;data&nbsp;recorded&nbsp;by&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;calibrated&nbsp;camera&nbsp;in&nbsp;motion.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;To&nbsp;create&nbsp;a&nbsp;simulated&nbsp;structure-from-camera-motion&nbsp;demonstration&nbsp;with<br>
 &nbsp;&nbsp;&nbsp;&nbsp;this&nbsp;module,&nbsp;you&nbsp;must&nbsp;first&nbsp;create&nbsp;an&nbsp;instance&nbsp;the&nbsp;ProjectiveCamera<br>
@@ -906,15 +913,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;the&nbsp;image&nbsp;sampling&nbsp;intervals&nbsp;along&nbsp;the&nbsp;x-axis&nbsp;and&nbsp;along&nbsp;the&nbsp;y-axis,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;respectively.&nbsp;&nbsp;The&nbsp;parameters&nbsp;'x0'&nbsp;and&nbsp;'y0'&nbsp;are&nbsp;for&nbsp;the&nbsp;coordinates&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;point&nbsp;in&nbsp;the&nbsp;camera&nbsp;image&nbsp;plane&nbsp;where&nbsp;the&nbsp;optic&nbsp;axis&nbsp;penetrates&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;plane&nbsp;with&nbsp;respect&nbsp;to&nbsp;the&nbsp;origin&nbsp;in&nbsp;the&nbsp;image&nbsp;plane&nbsp;(which&nbsp;is<br>
 &nbsp;&nbsp;&nbsp;&nbsp;usually&nbsp;a&nbsp;corner&nbsp;of&nbsp;the&nbsp;image).<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;world_points&nbsp;=&nbsp;camera.make_world_points_for_triangle()<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;world_points_xformed&nbsp;=&nbsp;camera.apply_transformation_to_generic_world_points(&nbsp;world_points, (0,0,0),&nbsp;(0.0,0.0,5000.0),&nbsp;1.0)<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;world_points_xformed&nbsp;=&nbsp;camera.apply_transformation_to_generic_world_points(&nbsp;world_points,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(0,0,0),&nbsp;(0.0,0.0,5000.0),&nbsp;1.0)<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;which&nbsp;generates&nbsp;a&nbsp;triangle&nbsp;defined&nbsp;by&nbsp;its&nbsp;three&nbsp;vertices&nbsp;from&nbsp;a&nbsp;method<br>
 &nbsp;&nbsp;&nbsp;&nbsp;defined&nbsp;for&nbsp;the&nbsp;ProjectiveCamera&nbsp;class&nbsp;and&nbsp;then&nbsp;moves&nbsp;the&nbsp;scene<br>
 &nbsp;&nbsp;&nbsp;&nbsp;triangle&nbsp;along&nbsp;the&nbsp;optic&nbsp;axis&nbsp;of&nbsp;the&nbsp;camera&nbsp;(the&nbsp;world-Z&nbsp;axis)&nbsp;by&nbsp;5000<br>
 &nbsp;&nbsp;&nbsp;&nbsp;units.&nbsp;&nbsp;After&nbsp;the&nbsp;transformation,&nbsp;the&nbsp;three&nbsp;vertices&nbsp;are&nbsp;at&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;coordinates&nbsp;(3000,3000,5000),&nbsp;(4000,3000,5000),&nbsp;and&nbsp;(4000,5000,5000).<br>
 &nbsp;<br>
@@ -1004,25 +1011,25 @@
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;You&nbsp;will&nbsp;find&nbsp;this&nbsp;utility&nbsp;method&nbsp;useful&nbsp;for&nbsp;enumerating&nbsp;all<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;different&nbsp;camera&nbsp;positions&nbsp;you&nbsp;will&nbsp;be&nbsp;using&nbsp;in&nbsp;a&nbsp;simulated<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;structure-from-camera-motion&nbsp;experiment.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(2)&nbsp;apply_transformation_to_generic_world_points()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;After&nbsp;you&nbsp;have&nbsp;constructed&nbsp;a&nbsp;scene&nbsp;<a href="__builtin__.html#object">object</a>&nbsp;(typically&nbsp;just&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;After&nbsp;you&nbsp;have&nbsp;constructed&nbsp;a&nbsp;scene&nbsp;<a href="builtins.html#object">object</a>&nbsp;(typically&nbsp;just&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;simple&nbsp;shape&nbsp;like&nbsp;a&nbsp;triangle&nbsp;or&nbsp;a&nbsp;tetrahedron),&nbsp;you&nbsp;can&nbsp;call&nbsp;on<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;this&nbsp;method&nbsp;to&nbsp;change&nbsp;its&nbsp;position&nbsp;and&nbsp;the&nbsp;pose&nbsp;in&nbsp;the&nbsp;world<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;frame.&nbsp;&nbsp;The&nbsp;method&nbsp;takes&nbsp;FOUR&nbsp;arguments:&nbsp;(1)&nbsp;The&nbsp;scene<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;structure&nbsp;in&nbsp;the&nbsp;form&nbsp;of&nbsp;a&nbsp;list&nbsp;of&nbsp;homogeneous&nbsp;coordinates&nbsp;for<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;world&nbsp;points&nbsp;on&nbsp;the&nbsp;<a href="__builtin__.html#object">object</a>.&nbsp;&nbsp;(2)&nbsp;The&nbsp;first&nbsp;is&nbsp;a&nbsp;triple&nbsp;that<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;world&nbsp;points&nbsp;on&nbsp;the&nbsp;<a href="builtins.html#object">object</a>.&nbsp;&nbsp;(2)&nbsp;The&nbsp;first&nbsp;is&nbsp;a&nbsp;triple&nbsp;that<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specifies&nbsp;the&nbsp;rotation&nbsp;using&nbsp;the&nbsp;(roll,pitch,yaw)<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;convention.&nbsp;(3)&nbsp;The&nbsp;second&nbsp;argument&nbsp;is&nbsp;a&nbsp;triple&nbsp;for&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;displacement&nbsp;along&nbsp;the&nbsp;world-X,&nbsp;world-Y,&nbsp;and&nbsp;world-Z<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;coordinates.&nbsp;(4)&nbsp;The&nbsp;scale&nbsp;factor&nbsp;by&nbsp;which&nbsp;you&nbsp;want&nbsp;to&nbsp;expand<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;or&nbsp;shrink&nbsp;the&nbsp;scene&nbsp;<a href="__builtin__.html#object">object</a>.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;or&nbsp;shrink&nbsp;the&nbsp;scene&nbsp;<a href="builtins.html#object">object</a>.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(3)&nbsp;construct_Fvec_for_calibrated_cameras(camera_params_dict)<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;constructs&nbsp;the&nbsp;prediction&nbsp;vector&nbsp;Fvec&nbsp;vector&nbsp;that<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;needs&nbsp;for&nbsp;comparing&nbsp;with&nbsp;the&nbsp;measurement<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vector&nbsp;X.&nbsp;Each&nbsp;element&nbsp;of&nbsp;Fvec&nbsp;is&nbsp;a&nbsp;prediction&nbsp;for&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;corresponding&nbsp;element&nbsp;of&nbsp;X&nbsp;and&nbsp;this&nbsp;prediction&nbsp;is&nbsp;a&nbsp;functional<br>
@@ -1053,15 +1060,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;scene&nbsp;points&nbsp;in&nbsp;world-3D.&nbsp;&nbsp;<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(7)&nbsp;display_structure()<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;is&nbsp;used&nbsp;to&nbsp;display&nbsp;in&nbsp;the&nbsp;form&nbsp;of&nbsp;a&nbsp;Matplotlib<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;figure&nbsp;the&nbsp;following&nbsp;three&nbsp;things&nbsp;simultaneously:&nbsp;the&nbsp;estimated<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;scene&nbsp;structure,&nbsp;the&nbsp;actual&nbsp;world&nbsp;points&nbsp;used&nbsp;for&nbsp;the&nbsp;scene<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="__builtin__.html#object">object</a>,&nbsp;and&nbsp;the&nbsp;initial&nbsp;guesses&nbsp;supplied&nbsp;for&nbsp;those&nbsp;coordinates<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="builtins.html#object">object</a>,&nbsp;and&nbsp;the&nbsp;initial&nbsp;guesses&nbsp;supplied&nbsp;for&nbsp;those&nbsp;coordinates<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;the&nbsp;nonlinear&nbsp;least-squares&nbsp;algorithm.&nbsp;&nbsp;The&nbsp;three&nbsp;parameters<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;this&nbsp;method&nbsp;are&nbsp;named&nbsp;'structure_points_estimated',<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;'world_points_xformed',&nbsp;and&nbsp;'initial_values_supplied'.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(8)&nbsp;get_all_cameras()<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;utility&nbsp;method&nbsp;is&nbsp;convenient&nbsp;for&nbsp;getting&nbsp;hold&nbsp;of&nbsp;all&nbsp;the<br>
@@ -1099,15 +1106,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;intrinsic&nbsp;parameter&nbsp;matrix&nbsp;K.&nbsp;&nbsp;If&nbsp;a&nbsp;translation&nbsp;and/or&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rotation&nbsp;is&nbsp;specified&nbsp;for&nbsp;the&nbsp;camera&nbsp;through&nbsp;the&nbsp;constructor,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;those&nbsp;are&nbsp;also&nbsp;incorporated&nbsp;in&nbsp;the&nbsp;3x4&nbsp;camera&nbsp;matrix&nbsp;P&nbsp;put<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;together&nbsp;by&nbsp;this&nbsp;method.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(12)&nbsp;make_world_points_for_triangle()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;returns&nbsp;a&nbsp;scene&nbsp;<a href="__builtin__.html#object">object</a>&nbsp;that&nbsp;consists&nbsp;of&nbsp;a&nbsp;triangle<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;returns&nbsp;a&nbsp;scene&nbsp;<a href="builtins.html#object">object</a>&nbsp;that&nbsp;consists&nbsp;of&nbsp;a&nbsp;triangle<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;world&nbsp;3D.&nbsp;I&nbsp;have&nbsp;found&nbsp;a&nbsp;triangle&nbsp;defined&nbsp;by&nbsp;its&nbsp;three&nbsp;world<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;points&nbsp;to&nbsp;be&nbsp;convenient&nbsp;for&nbsp;testing&nbsp;the&nbsp;basic&nbsp;logic&nbsp;of&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;algorithm&nbsp;for&nbsp;solving&nbsp;a&nbsp;structure-from-camera-motion&nbsp;problem.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;triangle&nbsp;returned&nbsp;by&nbsp;this&nbsp;method&nbsp;can&nbsp;be&nbsp;subject&nbsp;to&nbsp;any<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;orientation&nbsp;changing&nbsp;and&nbsp;position&nbsp;changing&nbsp;transformation.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(13)&nbsp;make_world_points_from_tetrahedron_generic()<br>
@@ -1163,17 +1170,16 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;incrementally&nbsp;displaces&nbsp;the&nbsp;camera&nbsp;by&nbsp;'translation'<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;is&nbsp;supplied&nbsp;to&nbsp;it&nbsp;as&nbsp;its&nbsp;argument.&nbsp;The&nbsp;argument<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;'translation'&nbsp;consists&nbsp;of&nbsp;a&nbsp;triple&nbsp;of&nbsp;real&nbsp;numbers&nbsp;that&nbsp;stand<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;a&nbsp;displacement&nbsp;along&nbsp;the&nbsp;world-X,&nbsp;along&nbsp;the&nbsp;world-Y,&nbsp;and<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;along&nbsp;the&nbsp;world-Z.<br>
 &nbsp;<br>
 &nbsp;<br>
-<font size=+2 color="red">ESTIMATING&nbsp;SCENE&nbsp;STRUCTURE&nbsp;AND&nbsp;CAMERA&nbsp;PARAMETERS<br>
-WHEN&nbsp;USING&nbsp;AN&nbsp;UNCALIBRATED&nbsp;CAMERA&nbsp;IN&nbsp;MOTION:<br></font>
-&nbsp;&nbsp;&nbsp;&nbsp;<br>
+<font size=+2 color="red">ESTIMATING&nbsp;SCENE&nbsp;STRUCTURE&nbsp;AND&nbsp;CAMERA&nbsp;PARAMETERS&nbsp;WHEN&nbsp;USING&nbsp;AN&nbsp;UNCALIBRATED&nbsp;CAMERA&nbsp;IN&nbsp;MOTION:<br>
+</font>&nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;problem&nbsp;of&nbsp;scene&nbsp;construction&nbsp;becomes&nbsp;a&nbsp;lot&nbsp;more&nbsp;challenging&nbsp;when<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;camera&nbsp;in&nbsp;motion&nbsp;is&nbsp;uncalibrated.&nbsp;&nbsp;When&nbsp;I&nbsp;say&nbsp;uncalibrated,&nbsp;I&nbsp;mean<br>
 &nbsp;&nbsp;&nbsp;&nbsp;uncalibrated&nbsp;with&nbsp;respect&nbsp;to&nbsp;its&nbsp;extrinsic&nbsp;pararameters.&nbsp;&nbsp;We&nbsp;assume&nbsp;in<br>
 &nbsp;&nbsp;&nbsp;&nbsp;all&nbsp;cases&nbsp;in&nbsp;this&nbsp;document&nbsp;that&nbsp;the&nbsp;intrinsic&nbsp;parameters&nbsp;of&nbsp;the&nbsp;camera<br>
 &nbsp;&nbsp;&nbsp;&nbsp;are&nbsp;known.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;What&nbsp;makes&nbsp;structure&nbsp;estimation&nbsp;more&nbsp;complicated&nbsp;in&nbsp;this&nbsp;case&nbsp;is&nbsp;that<br>
@@ -1348,16 +1354,15 @@
 &nbsp;<br>
 &nbsp;<br>
 <font size=+2 color="red">THE&nbsp;ExamplesStructureFromCameraMotion&nbsp;DIRECTORY:<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;See&nbsp;the&nbsp;'ExamplesStructureFromCameraMotion'&nbsp;directory&nbsp;in&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;distribution&nbsp;for&nbsp;the&nbsp;following&nbsp;three&nbsp;example&nbsp;scripts&nbsp;that&nbsp;show&nbsp;how&nbsp;you<br>
 &nbsp;&nbsp;&nbsp;&nbsp;can&nbsp;use&nbsp;the&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;module&nbsp;for&nbsp;estimating&nbsp;the&nbsp;structure<br>
-&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;a&nbsp;3D&nbsp;scene&nbsp;from&nbsp;the&nbsp;images&nbsp;recorded&nbsp;by&nbsp;a&nbsp;moving&nbsp;camera.&nbsp;&nbsp;Version&nbsp;1.5<br>
-&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;this&nbsp;module:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;a&nbsp;3D&nbsp;scene&nbsp;from&nbsp;the&nbsp;images&nbsp;recorded&nbsp;by&nbsp;a&nbsp;moving&nbsp;camera:&nbsp;&nbsp;<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sfm_with_calibrated_cameras_translations_only.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sfm_with_uncalibrated_cameras_translations_only.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py<br>
 &nbsp;<br>
@@ -1388,17 +1393,17 @@
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Just&nbsp;to&nbsp;give&nbsp;you&nbsp;an&nbsp;idea&nbsp;of&nbsp;the&nbsp;speed-up&nbsp;you&nbsp;will&nbsp;get&nbsp;with<br>
 &nbsp;&nbsp;&nbsp;&nbsp;bundle-adjustment,&nbsp;when&nbsp;I&nbsp;run&nbsp;the&nbsp;second&nbsp;script&nbsp;listed&nbsp;above&nbsp;on&nbsp;my<br>
 &nbsp;&nbsp;&nbsp;&nbsp;laptop,&nbsp;it&nbsp;takes&nbsp;about&nbsp;15&nbsp;minutes&nbsp;for&nbsp;the&nbsp;number&nbsp;of&nbsp;structure&nbsp;points<br>
 &nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;the&nbsp;number&nbsp;of&nbsp;camera&nbsp;positions&nbsp;used&nbsp;in&nbsp;that&nbsp;script.&nbsp;&nbsp;For&nbsp;exactly<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;same&nbsp;number&nbsp;of&nbsp;structure&nbsp;points&nbsp;and&nbsp;the&nbsp;camera&nbsp;positions,&nbsp;the&nbsp;third<br>
 &nbsp;&nbsp;&nbsp;&nbsp;script&nbsp;takes&nbsp;only&nbsp;a&nbsp;couple&nbsp;of&nbsp;minutes.&nbsp;&nbsp;You&nbsp;can&nbsp;only&nbsp;imagine&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;speed-up&nbsp;you&nbsp;will&nbsp;get&nbsp;with&nbsp;a&nbsp;C-based&nbsp;library&nbsp;for&nbsp;bundle&nbsp;adjustment&nbsp;---<br>
-&nbsp;&nbsp;&nbsp;&nbsp;such&nbsp;as&nbsp;the&nbsp;"sba"&nbsp;library&nbsp;mentioned&nbsp;in&nbsp;the&nbsp;paper&nbsp;by&nbsp;Lourakis&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Argyros&nbsp;that&nbsp;I&nbsp;mentioned&nbsp;earlier&nbsp;in&nbsp;this&nbsp;documentation&nbsp;page.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;speed-up&nbsp;you&nbsp;will&nbsp;get&nbsp;with&nbsp;a&nbsp;C-based&nbsp;library&nbsp;for&nbsp;sparse&nbsp;bundle<br>
+&nbsp;&nbsp;&nbsp;&nbsp;adjustment&nbsp;---&nbsp;such&nbsp;as&nbsp;the&nbsp;"sba"&nbsp;library&nbsp;mentioned&nbsp;in&nbsp;the&nbsp;paper&nbsp;by<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Lourakis&nbsp;and&nbsp;Argyros&nbsp;that&nbsp;I&nbsp;cited&nbsp;earlier&nbsp;in&nbsp;this&nbsp;documentation&nbsp;page.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size=+2 color="red">CAVEAT<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Note&nbsp;the&nbsp;bundle-adjustment&nbsp;variant&nbsp;of&nbsp;the&nbsp;Levenberg-Marquardt&nbsp;algorithm<br>
 &nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;you&nbsp;see&nbsp;in&nbsp;the&nbsp;bundle-adjust()&nbsp;method&nbsp;of&nbsp;the&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a><br>
 &nbsp;&nbsp;&nbsp;&nbsp;module&nbsp;is&nbsp;meant&nbsp;for&nbsp;just&nbsp;educational&nbsp;purposes.&nbsp;&nbsp;Being&nbsp;pure&nbsp;Python,&nbsp;it<br>
@@ -1420,19 +1425,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sudo&nbsp;python&nbsp;setup.py&nbsp;install<br>
 &nbsp;&nbsp;&nbsp;&nbsp;and/or<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sudo&nbsp;python3&nbsp;setup.py&nbsp;install<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;On&nbsp;Linux&nbsp;distributions,&nbsp;this&nbsp;will&nbsp;install&nbsp;the&nbsp;module&nbsp;file&nbsp;at&nbsp;a&nbsp;location<br>
 &nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;looks&nbsp;like<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;/usr/local/lib/python2.7/dist-packages/<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;for&nbsp;Python3&nbsp;at&nbsp;a&nbsp;location&nbsp;like<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;/usr/local/lib/python3.5/dist-packages/<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;/usr/local/lib/python3.6/dist-packages/<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;do&nbsp;not&nbsp;have&nbsp;root&nbsp;access,&nbsp;you&nbsp;have&nbsp;the&nbsp;option&nbsp;of&nbsp;working&nbsp;directly<br>
 &nbsp;&nbsp;&nbsp;&nbsp;off&nbsp;the&nbsp;directory&nbsp;in&nbsp;which&nbsp;you&nbsp;downloaded&nbsp;the&nbsp;software&nbsp;by&nbsp;simply<br>
 &nbsp;&nbsp;&nbsp;&nbsp;placing&nbsp;the&nbsp;following&nbsp;statements&nbsp;at&nbsp;the&nbsp;top&nbsp;of&nbsp;your&nbsp;scripts&nbsp;that&nbsp;use<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;class:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;import&nbsp;sys<br>
@@ -1456,33 +1457,33 @@
 &nbsp;&nbsp;&nbsp;&nbsp;Please&nbsp;notify&nbsp;the&nbsp;author&nbsp;if&nbsp;you&nbsp;encounter&nbsp;any&nbsp;bugs.&nbsp;&nbsp;When&nbsp;sending<br>
 &nbsp;&nbsp;&nbsp;&nbsp;email,&nbsp;please&nbsp;place&nbsp;the&nbsp;string&nbsp;'<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>'&nbsp;in&nbsp;the&nbsp;subject<br>
 &nbsp;&nbsp;&nbsp;&nbsp;line.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size=+2 color="red">ABOUT&nbsp;THE&nbsp;AUTHOR:<br>
 </font>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;author,&nbsp;Avinash&nbsp;Kak,&nbsp;recently&nbsp;finished&nbsp;a&nbsp;17-year&nbsp;long&nbsp;"Objects<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Trilogy&nbsp;Project"&nbsp;with&nbsp;the&nbsp;publication&nbsp;of&nbsp;the&nbsp;book&nbsp;"Designing&nbsp;with<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Objects"&nbsp;by&nbsp;John-Wiley.&nbsp;If&nbsp;interested,&nbsp;visit&nbsp;his&nbsp;web&nbsp;page&nbsp;at&nbsp;Purdue&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;find&nbsp;out&nbsp;what&nbsp;this&nbsp;project&nbsp;was&nbsp;all&nbsp;about.&nbsp;You&nbsp;might&nbsp;like&nbsp;"Designing<br>
-&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;Objects"&nbsp;especially&nbsp;if&nbsp;you&nbsp;enjoyed&nbsp;reading&nbsp;Harry&nbsp;Potter&nbsp;as&nbsp;a&nbsp;kid<br>
-&nbsp;&nbsp;&nbsp;&nbsp;(or&nbsp;even&nbsp;as&nbsp;an&nbsp;adult,&nbsp;for&nbsp;that&nbsp;matter).<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Not&nbsp;too&nbsp;long&nbsp;ago,&nbsp;the&nbsp;author,&nbsp;Avinash&nbsp;Kak,&nbsp;finished&nbsp;a&nbsp;17-year&nbsp;long<br>
+&nbsp;&nbsp;&nbsp;&nbsp;"Objects&nbsp;Trilogy&nbsp;Project"&nbsp;with&nbsp;the&nbsp;publication&nbsp;of&nbsp;the&nbsp;last&nbsp;book&nbsp;"Designing<br>
+&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;Objects"&nbsp;by&nbsp;John-Wiley.&nbsp;If&nbsp;interested,&nbsp;visit&nbsp;his&nbsp;web&nbsp;page&nbsp;at&nbsp;Purdue<br>
+&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;find&nbsp;out&nbsp;what&nbsp;this&nbsp;project&nbsp;was&nbsp;all&nbsp;about.&nbsp;You&nbsp;might&nbsp;like&nbsp;"Designing<br>
+&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;Objects"&nbsp;especially&nbsp;if&nbsp;you&nbsp;enjoyed&nbsp;reading&nbsp;Harry&nbsp;Potter&nbsp;as&nbsp;a&nbsp;kid&nbsp;(or<br>
+&nbsp;&nbsp;&nbsp;&nbsp;even&nbsp;as&nbsp;an&nbsp;adult,&nbsp;for&nbsp;that&nbsp;matter).<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;For&nbsp;all&nbsp;issues&nbsp;related&nbsp;to&nbsp;this&nbsp;module,&nbsp;contact&nbsp;the&nbsp;author&nbsp;at<br>
 &nbsp;&nbsp;&nbsp;&nbsp;kak@purdue.edu<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;send&nbsp;email,&nbsp;please&nbsp;place&nbsp;the&nbsp;string&nbsp;"<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>"&nbsp;in<br>
-&nbsp;&nbsp;&nbsp;&nbsp;your&nbsp;subject&nbsp;line&nbsp;to&nbsp;get&nbsp;past&nbsp;the&nbsp;author's&nbsp;spam&nbsp;filter.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;send&nbsp;email,&nbsp;please&nbsp;place&nbsp;the&nbsp;string&nbsp;"<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>"&nbsp;in&nbsp;your<br>
+&nbsp;&nbsp;&nbsp;&nbsp;subject&nbsp;line&nbsp;to&nbsp;get&nbsp;past&nbsp;the&nbsp;author's&nbsp;spam&nbsp;filter.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size=+2 color="red">COPYRIGHT:<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Python&nbsp;Software&nbsp;Foundation&nbsp;License<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Copyright&nbsp;2018&nbsp;Avinash&nbsp;Kak<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Copyright&nbsp;2022&nbsp;Avinash&nbsp;Kak<br>
 &nbsp;<br>
 @endofdocs
 <p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#aa55cc">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#ffffff" face="helvetica, arial"><big><strong>Imported Modules</strong></big></font></td></tr>
@@ -1500,38 +1501,84 @@
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#ee77aa">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#ffffff" face="helvetica, arial"><big><strong>Classes</strong></big></font></td></tr>
     
 <tr><td bgcolor="#ee77aa"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
 <td width="100%"><dl>
-<dt><font face="helvetica, arial"><a href="__builtin__.html#object">__builtin__.object</a>
+<dt><font face="helvetica, arial"><a href="builtins.html#object">builtins.object</a>
 </font></dt><dd>
 <dl>
 <dt><font face="helvetica, arial"><a href="NonlinearLeastSquares.html#NonlinearLeastSquares">NonlinearLeastSquares</a>
 </font></dt></dl>
 </dd>
 </dl>
  <p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#ffc8d8">
 <td colspan=3 valign=bottom>&nbsp;<br>
-<font color="#000000" face="helvetica, arial"><a name="NonlinearLeastSquares">class <strong>NonlinearLeastSquares</strong></a>(<a href="__builtin__.html#object">__builtin__.object</a>)</font></td></tr>
+<font color="#000000" face="helvetica, arial"><a name="NonlinearLeastSquares">class <strong>NonlinearLeastSquares</strong></a>(<a href="builtins.html#object">builtins.object</a>)</font></td></tr>
     
-<tr><td bgcolor="#ffc8d8"><tt>&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
+<tr bgcolor="#ffc8d8"><td rowspan=2><tt>&nbsp;&nbsp;&nbsp;</tt></td>
+<td colspan=2><tt><a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>(*args,&nbsp;**kwargs)<br>
+&nbsp;<br>
+<br>&nbsp;</tt></td></tr>
+<tr><td>&nbsp;</td>
 <td width="100%">Methods defined here:<br>
 <dl><dt><a name="NonlinearLeastSquares-__init__"><strong>__init__</strong></a>(self, *args, **kwargs)</dt><dd><tt>constructor</tt></dd></dl>
 
-<dl><dt><a name="NonlinearLeastSquares-bundle_adjust"><strong>bundle_adjust</strong></a>(self, *args, **kwargs)</dt></dl>
+<dl><dt><a name="NonlinearLeastSquares-bundle_adjust"><strong>bundle_adjust</strong></a>(self, *args, **kwargs)</dt><dd><tt>This&nbsp;is&nbsp;an&nbsp;implementation&nbsp;of&nbsp;the&nbsp;"bundle&nbsp;adjustment"&nbsp;version&nbsp;of&nbsp;the&nbsp;Levenberg-Marquardt&nbsp;algorithm&nbsp;for&nbsp;nonlinear<br>
+least-squares.&nbsp;&nbsp;Bundle&nbsp;adjustment&nbsp;takes&nbsp;advantage&nbsp;of&nbsp;the&nbsp;sparsity&nbsp;of&nbsp;the&nbsp;Jacobian&nbsp;that&nbsp;one&nbsp;sees&nbsp;in&nbsp;<br>
+applications&nbsp;such&nbsp;as&nbsp;estimating&nbsp;the&nbsp;scene&nbsp;structure&nbsp;with&nbsp;the&nbsp;images&nbsp;recorded&nbsp;with&nbsp;uncalibrated&nbsp;cameras.&nbsp;&nbsp;<br>
+The&nbsp;implementation&nbsp;shown&nbsp;here&nbsp;is&nbsp;based&nbsp;on&nbsp;the&nbsp;now&nbsp;celebrated&nbsp;paper&nbsp;"SBA:&nbsp;A&nbsp;Software&nbsp;Package&nbsp;for&nbsp;Generic<br>
+Sparse&nbsp;Bundle&nbsp;Adjustment"&nbsp;by&nbsp;Manolis&nbsp;Lourakis&nbsp;and&nbsp;Antonis&nbsp;Argyros&nbsp;that&nbsp;appeared&nbsp;in&nbsp;ACM&nbsp;Transactions&nbsp;on&nbsp;<br>
+Mathematical&nbsp;Software,&nbsp;March&nbsp;2009.<br>
+&nbsp;<br>
+This&nbsp;function&nbsp;is&nbsp;used&nbsp;in&nbsp;the&nbsp;following&nbsp;scripts&nbsp;<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py&nbsp;<br>
+&nbsp;<br>
+in&nbsp;the&nbsp;ExamplesStructureFromCameraMotion&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution.&nbsp;&nbsp;<br>
+&nbsp;<br>
+Note&nbsp;that&nbsp;since&nbsp;<a href="#NonlinearLeastSquares-bundle_adjust">bundle_adjust</a>()&nbsp;is&nbsp;written&nbsp;in&nbsp;a&nbsp;generic&nbsp;manner,&nbsp;it&nbsp;is&nbsp;not&nbsp;called&nbsp;directly&nbsp;by&nbsp;the&nbsp;example<br>
+scripts&nbsp;listed&nbsp;above.&nbsp;&nbsp;As&nbsp;shown&nbsp;in&nbsp;the&nbsp;scripts,&nbsp;you&nbsp;need&nbsp;to&nbsp;first&nbsp;construct&nbsp;an&nbsp;instance&nbsp;of&nbsp;the&nbsp;class<br>
+ProjectiveCamera&nbsp;that&nbsp;is&nbsp;a&nbsp;co-class&nbsp;of&nbsp;the&nbsp;main&nbsp;module&nbsp;class&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;in&nbsp;the&nbsp;distribiution.</tt></dd></dl>
 
-<dl><dt><a name="NonlinearLeastSquares-grad_descent"><strong>grad_descent</strong></a>(self)</dt></dl>
+<dl><dt><a name="NonlinearLeastSquares-grad_descent"><strong>grad_descent</strong></a>(self)</dt><dd><tt>This&nbsp;is&nbsp;an&nbsp;implementation&nbsp;of&nbsp;the&nbsp;basic&nbsp;gradient&nbsp;descent&nbsp;algorithm&nbsp;for&nbsp;nonlinear&nbsp;least-squares&nbsp;as&nbsp;described&nbsp;<br>
+in&nbsp;my&nbsp;Lecture&nbsp;13&nbsp;notes&nbsp;at&nbsp;the&nbsp;lecture-notes&nbsp;website&nbsp;for&nbsp;Purdue&nbsp;University's&nbsp;ECE661:&nbsp;Computer&nbsp;Vision</tt></dd></dl>
 
-<dl><dt><a name="NonlinearLeastSquares-leven_marq"><strong>leven_marq</strong></a>(self)</dt></dl>
+<dl><dt><a name="NonlinearLeastSquares-leven_marq"><strong>leven_marq</strong></a>(self)</dt><dd><tt>This&nbsp;is&nbsp;an&nbsp;implementation&nbsp;of&nbsp;the&nbsp;Levenberg-Marquardt&nbsp;algorithm&nbsp;for&nbsp;nonlinear&nbsp;least-squares&nbsp;as&nbsp;described&nbsp;<br>
+in&nbsp;my&nbsp;Lecture&nbsp;13&nbsp;notes&nbsp;at&nbsp;the&nbsp;lecture-notes&nbsp;website&nbsp;for&nbsp;Purdue&nbsp;University's&nbsp;ECE661:&nbsp;Computer&nbsp;Vision<br>
+&nbsp;<br>
+This&nbsp;function&nbsp;is&nbsp;used&nbsp;the&nbsp;following&nbsp;scripts&nbsp;in&nbsp;the&nbsp;ExamplesOptimizedSurfaceFit&nbsp;directory&nbsp;of&nbsp;the&nbsp;distro:<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;leven_marq.py<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;leven_marq_with_partial_derivatives.py<br>
+&nbsp;<br>
+It&nbsp;is&nbsp;important&nbsp;to&nbsp;note&nbsp;that&nbsp;the&nbsp;above&nbsp;two&nbsp;scripts&nbsp;do&nbsp;NOT&nbsp;call&nbsp;<a href="#NonlinearLeastSquares-leven_marq">leven_marq</a>()&nbsp;function&nbsp;directly.&nbsp;&nbsp;AS&nbsp;<br>
+stated&nbsp;in&nbsp;the&nbsp;main&nbsp;document&nbsp;page&nbsp;for&nbsp;the&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;module,&nbsp;the&nbsp;code&nbsp;in&nbsp;the&nbsp;file&nbsp;<br>
+<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>.py&nbsp;is&nbsp;written&nbsp;in&nbsp;a&nbsp;domain&nbsp;agnostic&nbsp;manner.&nbsp;&nbsp;So&nbsp;you&nbsp;need&nbsp;a&nbsp;domain&nbsp;adaptation&nbsp;<br>
+class&nbsp;that&nbsp;knows&nbsp;how&nbsp;to&nbsp;package&nbsp;the&nbsp;arguments&nbsp;for&nbsp;calling&nbsp;<a href="#NonlinearLeastSquares-leven_marq">leven_marq</a>().&nbsp;&nbsp;For&nbsp;the&nbsp;case&nbsp;of&nbsp;the&nbsp;two&nbsp;scripts<br>
+listed&nbsp;above,&nbsp;that&nbsp;domain-specific&nbsp;class&nbsp;in&nbsp;the&nbsp;distro&nbsp;is&nbsp;OptimizedSurfaceFit.&nbsp;&nbsp;It&nbsp;is&nbsp;a&nbsp;co-class&nbsp;of&nbsp;<br>
+the&nbsp;main&nbsp;module&nbsp;class&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;in&nbsp;the&nbsp;distribution.<br>
+&nbsp;<br>
+The&nbsp;function&nbsp;<a href="#NonlinearLeastSquares-leven_marq">leven_marq</a>()&nbsp;defined&nbsp;here&nbsp;is&nbsp;ALSO&nbsp;used&nbsp;in&nbsp;the&nbsp;following&nbsp;two&nbsp;scripts<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;sfm_with_calibrated_cameras_translations_only.py<br>
+&nbsp;&nbsp;&nbsp;&nbsp;sfm_with_uncalibrated_cameras_translations_only.py<br>
+&nbsp;<br>
+in&nbsp;the&nbsp;ExamplesStructureFromCameraMotion&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution.&nbsp;&nbsp;Again,&nbsp;these&nbsp;example&nbsp;scripts<br>
+do&nbsp;NOT&nbsp;directly&nbsp;call&nbsp;the&nbsp;<a href="#NonlinearLeastSquares-leven_marq">leven_marq</a>()&nbsp;function.&nbsp;&nbsp;As&nbsp;shown&nbsp;in&nbsp;the&nbsp;two&nbsp;scripts,&nbsp;they&nbsp;must&nbsp;first&nbsp;construct<br>
+an&nbsp;instance&nbsp;of&nbsp;the&nbsp;ProjectiveCamera&nbsp;class&nbsp;that&nbsp;knows&nbsp;how&nbsp;to&nbsp;bundle&nbsp;the&nbsp;arugments&nbsp;together&nbsp;for&nbsp;calling<br>
+the&nbsp;<a href="#NonlinearLeastSquares-leven_marq">leven_marq</a>()&nbsp;function.</tt></dd></dl>
 
-<dl><dt><a name="NonlinearLeastSquares-leven_marq_v1_5"><strong>leven_marq_v1_5</strong></a>(self)</dt></dl>
+<dl><dt><a name="NonlinearLeastSquares-leven_marq_v1_5"><strong>leven_marq_v1_5</strong></a>(self)</dt><dd><tt>This&nbsp;is&nbsp;the&nbsp;implementation&nbsp;of&nbsp;the&nbsp;<a href="#NonlinearLeastSquares-leven_marq">leven_marq</a>()&nbsp;function&nbsp;as&nbsp;it&nbsp;existed&nbsp;in&nbsp;Version&nbsp;1.5.&nbsp;&nbsp;On&nbsp;account&nbsp;of&nbsp;the<br>
+fact&nbsp;that&nbsp;I&nbsp;made&nbsp;significant&nbsp;changes&nbsp;to&nbsp;this&nbsp;function&nbsp;in&nbsp;Version&nbsp;2.0.0&nbsp;of&nbsp;the&nbsp;module,&nbsp;I&nbsp;have&nbsp;retained&nbsp;the<br>
+old&nbsp;version&nbsp;for&nbsp;the&nbsp;old-time&nbsp;users&nbsp;of&nbsp;my&nbsp;module.</tt></dd></dl>
 
 <dl><dt><a name="NonlinearLeastSquares-set_Fvec"><strong>set_Fvec</strong></a>(self, Fvector)</dt><dd><tt>This&nbsp;method&nbsp;supplies&nbsp;the&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;class&nbsp;with&nbsp;the&nbsp;prediction&nbsp;vector<br>
 whose&nbsp;each&nbsp;element&nbsp;is&nbsp;a&nbsp;functional&nbsp;form&nbsp;of&nbsp;the&nbsp;prediction&nbsp;in&nbsp;the&nbsp;observed&nbsp;data&nbsp;vector<br>
 X.&nbsp;&nbsp;Note&nbsp;that&nbsp;&nbsp;Fvec&nbsp;is&nbsp;a&nbsp;column&nbsp;vector&nbsp;---&nbsp;meaning&nbsp;a&nbsp;numpy&nbsp;matrix&nbsp;with&nbsp;just&nbsp;one&nbsp;column.</tt></dd></dl>
 
 <dl><dt><a name="NonlinearLeastSquares-set_Fvec_BA"><strong>set_Fvec_BA</strong></a>(self, Fvector_BA)</dt><dd><tt>You&nbsp;need&nbsp;to&nbsp;call&nbsp;this&nbsp;method&nbsp;for&nbsp;providing&nbsp;the&nbsp;<a href="#NonlinearLeastSquares">NonlinearLeastSquares</a>&nbsp;class&nbsp;with&nbsp;the<br>
 prediction&nbsp;vector&nbsp;if&nbsp;you&nbsp;are&nbsp;going&nbsp;to&nbsp;be&nbsp;using&nbsp;the&nbsp;bundle-adjustment&nbsp;capabilities<br>
@@ -1582,18 +1629,18 @@
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#55aa55">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#ffffff" face="helvetica, arial"><big><strong>Data</strong></big></font></td></tr>
     
 <tr><td bgcolor="#55aa55"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
 <td width="100%"><strong>__author__</strong> = 'Avinash Kak (kak@purdue.edu)'<br>
-<strong>__copyright__</strong> = '(C) 2018 Avinash Kak. Python Software Foundation.'<br>
-<strong>__date__</strong> = '2018-November-9'<br>
-<strong>__url__</strong> = 'https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.html'<br>
-<strong>__version__</strong> = '2.0.0'</td></tr></table>
+<strong>__copyright__</strong> = '(C) 2022 Avinash Kak. Python Software Foundation.'<br>
+<strong>__date__</strong> = '2022-October-6'<br>
+<strong>__url__</strong> = 'https://engineering.purdue.edu/kak/distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.html'<br>
+<strong>__version__</strong> = '2.0.1'</td></tr></table>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#7799ee">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#ffffff" face="helvetica, arial"><big><strong>Author</strong></big></font></td></tr>
 <tr><td bgcolor="#7799ee"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
 <td width="100%">Avinash&nbsp;Kak&nbsp;(kak@purdue.edu)</td></tr></table>
 </body></html>
```

#### html2text {}

```diff
@@ -1,38 +1,44 @@
  
  
-NonlinearLeastSquares (version 2.0.0, 2018-November-9)
+NonlinearLeastSquares (version 2.0.1, 2022-October-6)
 NonlinearLeastSquares.py
  
-Version: 2.0.0
+Version: 2.0.1
    
 Author: Avinash Kak (kak@purdue.edu)
  
-Date: 2018-November-9
+Date: 2022-October-6
  
  
                                          Total number of downloads (all versions): <?php $file = fopen
                                     ("HowManyCounts.txt", "r") or exit("Unable to open file!"); echo fgets($file);
-Download Version 2.0.0:  gztar    fclose($file); ?>
+Download Version 2.0.1:  gztar    fclose($file); ?>
                                                    This count is automatically updated at every rotation of
                                                      the weblogs (normally once every two to four days)
                                          Last updated: <?php $file = fopen("LastUpdated.txt", "r") or exit("Unable to
                                                     open file!"); echo fgets($file); fclose($file); ?>
-View_the_main_module_file_in_your_browser  
 
+View_the_main_module_file_in_your_browser  
 View_the_code_for_OptimizedSurfaceFit_for_optimized_surface_fitting_to_noisy
 height_data
-
-View_the_code_for_ProjectiveCamera_that_shows_how_to_calculate_the_structure_of
-a_scene_with_a_moving_camera
+View_the_code_for_ProjectiveCamera_for_camera_modeling
  
  
  
 CHANGES:
 
+  Version 2.0.1:
+ 
+    Cleaned up the code to make it work with the current version of the
+    matplotlib library that is used for displaying the results.  I have also
+    removed the use of the "is" and "is not" comparison operators for numeric
+    and string literals since such use has now been deprecated.  Also added
+    additional comment blocks to the main functions in the module file.
+ 
   Version 2.0.0:
  
     This version includes sparse bundle adjustment (SBA) to speed up code
     execution when using nonlinear least-squares for solving
     structure-from-camera-motion problems with uncalibrated cameras.  SBA
     exploits the sparseness of the Jacobian encountered in such problems.
     This version also includes improvements to the Levenberg-Marquardt code
@@ -41,47 +47,46 @@
     provides additional methods for the visualization of the results.
  
   Version 1.5.0:
  
     This version adds a new class, ProjectiveCamera, to the module for
     demonstrating how nonlinear least-squares can be used for estimating
     structure of a scene from the data recorded with a calibrated camera in
-    motion.  For a simulated demonstration, you can create calibrated
-    cameras from a generic instance of the ProjectiveCamera class that is
-    then subject to various translational and rotational transformations.
+    motion.  For a simulated demonstration, you can create calibrated cameras
+    from a generic instance of the ProjectiveCamera class that is then subject
+    to various translational and rotational transformations.
  
   Version 1.1.1:
  
     This version includes constructor options to control the size and the
     position of the graphics for displaying the results of nonlinear
     least-squares optimization.
  
   Version 1.1:
  
-    This version fixes a bug in the synthetic data generator function used
-    for illustrating the functionality of the NonlinearLeastSquares class.
-    Changes also made to the information that is printed out when the
-    module is run in the debug mode.
+    This version fixes a bug in the synthetic data generator function used for
+    illustrating the functionality of the NonlinearLeastSquares class.
+    Changes also made to the information that is printed out when the module
+    is run in the debug mode.
  
   Version 1.0:
  
-    In the form of a class named NonlinearLeastSquares, this module
-    provides a domain agnostic implementation of nonlinear least-squares
-    algorithms (gradient-descent and Levenberg-Marquardt) for fitting a
-    model to observed data.  Typically, the model involves several
-    parameters and each observed data element can be expressed as a
-    function of those parameters plus noise.  The goal of nonlinear
-    least-squares is to estimate the best values for the parameters given
-    all of the observed data.  In order to illustrate how to use the
-    NonlinearLeastSquares class, the module also comes with another class,
-    OptimizeSurfaceFit, whose job is to fit the best surface (of a
-    specified analytical form) to noisy height data over the XY-plane. The
-    model in this case is the analytical description of the surface and the
-    goal of nonlinear least-squares is to estimate the best values for the
-    parameters in the analytical description.
+    In the form of a class named NonlinearLeastSquares, this module provides a
+    domain agnostic implementation of nonlinear least-squares algorithms
+    (gradient-descent and Levenberg-Marquardt) for fitting a model to observed
+    data.  Typically, the model involves several parameters and each observed
+    data element can be expressed as a function of those parameters plus
+    noise.  The goal of nonlinear least-squares is to estimate the best values
+    for the parameters given all of the observed data.  In order to illustrate
+    how to use the NonlinearLeastSquares class, the module also comes with
+    another class, OptimizeSurfaceFit, whose job is to fit the best surface
+    (of a specified analytical form) to noisy height data over the
+    XY-plane. The model in this case is the analytical description of the
+    surface and the goal of nonlinear least-squares is to estimate the best
+    values for the parameters in the analytical description.
  
  
 USAGE FOR OPTIMAL SURFACE FITTING:
  
     The module includes a domain specific class, OptimizedSurfaceFit, for
     demonstrating how nonlinear least-squares in the form of the
     Levenberg-Marquardt algorithm can be used for optimally fitting
@@ -223,15 +228,15 @@
     distribution for further information on what calls you need to sequence
     together for estimating the structure of a scene that is being viewed
     with a moving camera.
  
  
 USING SPARSE BUNDLE ADJUSTMENT FOR ESTIMATING THE SCENE STRUCTURE WITH 
 AN UNCALIBRATED CAMERA IN MOTION:
-  
+ 
     You would again need to construct an instance of the
     NonlinearLeastSquares and an instance of the ProjectiveCamera class as
     shown in lines (F) and (G) above.  But now you would need to replace
     the code in lines (H) through (K) by:
  
         camera.construct_X_vector_for_bundle_adjustment( all_pixels )     #(L)
         camera.construct_parameter_vec_for_uncalibrated_cameras_with_rodrigues_rotations
@@ -239,24 +244,25 @@
                                                                           #(M)
         camera.construct_Fvec_for_bundle_adjustment()                     #(O)
         result = camera.get_scene_structure_from_camera_motion_with_bundle_adjustment
 ()
                                                                           #(P)
  
     The construction of the observation vector X in line (L) is specific to
-    bundle adjustment --- in the sense that you first want to list the
-    pixels in all the cameras for the first world point, then you want to
-    list the pixels in all the cameras for the second world point, and so
-    on.  Ordering the observed data in this fashion is necessary to create
-    the sort of block sparsity in the Jacobian that is exploited in SBA.
+    sparse bundle adjustment --- in the sense that you first want to list
+    the pixels in all the cameras for the first world point, then you want
+    to list the pixels in all the cameras for the second world point, and
+    so on.  Ordering the observed data in this fashion is necessary to
+    create the sort of block sparsity in the Jacobian that is exploited in
+    SBA.
  
     Note that we assume that the intrinsic parameters of the camera are
     known already.  So the goal of the bundle adjustment is to estimate the
-    six extrinsic parameters, the three for translation of the camera and
-    the three (in the form of Rodrigues rotations) for the rotation.
+    six extrinsic parameters, three for translation of the camera and three
+    (in the form of Rodrigues rotations) for the rotation.
         
     See the script 
  
        bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py
  
     in the ExamplesStructureFromCameraMotion subdirectory of the
     distribution for further information on what calls you need to sequence
@@ -838,17 +844,16 @@
  
             The responsibility of this method is to take all of the user
             supplied information and reconstitute it into a form that is
             needed by NonlinearLeastSquares taking into account the
             peculiarities of your domain.
  
  
-ESTIMATING SCENE STRUCTURE WHEN USING A CALIBRATED 
-CAMERA IN MOTION:
-  
+ESTIMATING SCENE STRUCTURE WHEN USING A CALIBRATED CAMERA IN MOTION:
+ 
     This section presents a class named ProjectiveCamera to illustrate how
     you can use the functionality of NonlinearLeastSquares in your own code
     for estimating the structure of a 3D scene from the data recorded by a
     calibrated camera in motion.
  
     To create a simulated structure-from-camera-motion demonstration with
     this module, you must first create an instance the ProjectiveCamera
@@ -870,15 +875,16 @@
     respectively.  The parameters 'x0' and 'y0' are for the coordinates of
     the point in the camera image plane where the optic axis penetrates the
     image plane with respect to the origin in the image plane (which is
     usually a corner of the image).
  
         world_points = camera.make_world_points_for_triangle()
         world_points_xformed = camera.apply_transformation_to_generic_world_points
-( world_points, (0,0,0), (0.0,0.0,5000.0), 1.0)
+( world_points,                                                                     
+(0,0,0), (0.0,0.0,5000.0), 1.0)
  
     which generates a triangle defined by its three vertices from a method
     defined for the ProjectiveCamera class and then moves the scene
     triangle along the optic axis of the camera (the world-Z axis) by 5000
     units.  After the transformation, the three vertices are at the
     coordinates (3000,3000,5000), (4000,3000,5000), and (4000,5000,5000).
  
@@ -1129,17 +1135,16 @@
             This method incrementally displaces the camera by 'translation'
             that is supplied to it as its argument. The argument
             'translation' consists of a triple of real numbers that stand
             for a displacement along the world-X, along the world-Y, and
             along the world-Z.
  
  
-ESTIMATING SCENE STRUCTURE AND CAMERA PARAMETERS
-WHEN USING AN UNCALIBRATED CAMERA IN MOTION:
-     
+ESTIMATING SCENE STRUCTURE AND CAMERA PARAMETERS WHEN USING AN UNCALIBRATED CAMERA IN MOTION:
+    
     The problem of scene construction becomes a lot more challenging when
     the camera in motion is uncalibrated.  When I say uncalibrated, I mean
     uncalibrated with respect to its extrinsic pararameters.  We assume in
     all cases in this document that the intrinsic parameters of the camera
     are known.
  
     What makes structure estimation more complicated in this case is that
@@ -1316,16 +1321,15 @@
  
  
 THE ExamplesStructureFromCameraMotion DIRECTORY:
  
     See the 'ExamplesStructureFromCameraMotion' directory in the
     distribution for the following three example scripts that show how you
     can use the NonlinearLeastSquares module for estimating the structure
-    of a 3D scene from the images recorded by a moving camera.  Version 1.5
-    of this module:
+    of a 3D scene from the images recorded by a moving camera:  
  
         sfm_with_calibrated_cameras_translations_only.py
  
         sfm_with_uncalibrated_cameras_translations_only.py
  
         bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py
  
@@ -1356,17 +1360,17 @@
  
     Just to give you an idea of the speed-up you will get with
     bundle-adjustment, when I run the second script listed above on my
     laptop, it takes about 15 minutes for the number of structure points
     and the number of camera positions used in that script.  For exactly
     the same number of structure points and the camera positions, the third
     script takes only a couple of minutes.  You can only imagine the
-    speed-up you will get with a C-based library for bundle adjustment ---
-    such as the "sba" library mentioned in the paper by Lourakis and
-    Argyros that I mentioned earlier in this documentation page.
+    speed-up you will get with a C-based library for sparse bundle
+    adjustment --- such as the "sba" library mentioned in the paper by
+    Lourakis and Argyros that I cited earlier in this documentation page.
  
  
 CAVEAT
  
     Note the bundle-adjustment variant of the Levenberg-Marquardt algorithm
     that you see in the bundle-adjust() method of the NonlinearLeastSquares
     module is meant for just educational purposes.  Being pure Python, it
@@ -1388,19 +1392,15 @@
             sudo python setup.py install
     and/or
             sudo python3 setup.py install
  
     On Linux distributions, this will install the module file at a location
     that looks like
  
-             /usr/local/lib/python2.7/dist-packages/
- 
-    and for Python3 at a location like
- 
-             /usr/local/lib/python3.5/dist-packages/
+             /usr/local/lib/python3.6/dist-packages/
  
     If you do not have root access, you have the option of working directly
     off the directory in which you downloaded the software by simply
     placing the following statements at the top of your scripts that use
     the NonlinearLeastSquares class:
  
             import sys
@@ -1424,68 +1424,118 @@
     Please notify the author if you encounter any bugs.  When sending
     email, please place the string 'NonlinearLeastSquares' in the subject
     line.
  
  
 ABOUT THE AUTHOR:
  
-    The author, Avinash Kak, recently finished a 17-year long "Objects
-    Trilogy Project" with the publication of the book "Designing with
-    Objects" by John-Wiley. If interested, visit his web page at Purdue to
-    find out what this project was all about. You might like "Designing
-    with Objects" especially if you enjoyed reading Harry Potter as a kid
-    (or even as an adult, for that matter).
+    Not too long ago, the author, Avinash Kak, finished a 17-year long
+    "Objects Trilogy Project" with the publication of the last book "Designing
+    with Objects" by John-Wiley. If interested, visit his web page at Purdue
+    to find out what this project was all about. You might like "Designing
+    with Objects" especially if you enjoyed reading Harry Potter as a kid (or
+    even as an adult, for that matter).
  
     For all issues related to this module, contact the author at
     kak@purdue.edu
  
-    If you send email, please place the string "NonlinearLeastSquares" in
-    your subject line to get past the author's spam filter.
+    If you send email, please place the string "NonlinearLeastSquares" in your
+    subject line to get past the author's spam filter.
  
  
 COPYRIGHT:
  
     Python Software Foundation License
  
-    Copyright 2018 Avinash Kak
+    Copyright 2022 Avinash Kak
  
 @endofdocs
  
 Imported Modules
    � glob      math  os scipy
          itertools numpy re sys
  
 Classes
-           __builtin__.object
+           builtins.object
                  NonlinearLeastSquares
           
-         class NonlinearLeastSquares(__builtin__.object)
+         class NonlinearLeastSquares(builtins.object)
+             NonlinearLeastSquares(*args, **kwargs)
+              
+
+              
                Methods defined here:
                  __init__(self, *args, **kwargs)
                      constructor
                  bundle_adjust(self, *args, **kwargs)
+                     This is an implementation of the "bundle adjustment" version of the Levenberg-Marquardt algorithm for nonlinear
+                     least-squares.  Bundle adjustment takes advantage of the sparsity of the Jacobian that one sees in 
+                     applications such as estimating the scene structure with the images recorded with uncalibrated cameras.  
+                     The implementation shown here is based on the now celebrated paper "SBA: A Software Package for Generic
+                     Sparse Bundle Adjustment" by Manolis Lourakis and Antonis Argyros that appeared in ACM Transactions on 
+                     Mathematical Software, March 2009.
+                      
+                     This function is used in the following scripts 
+                      
+                         bundle_adjust_sfm_with_uncalibrated_cameras_translations_only.py 
+                      
+                     in the ExamplesStructureFromCameraMotion directory of the distribution.  
+                      
+                     Note that since bundle_adjust() is written in a generic manner, it is not called directly by the example
+                     scripts listed above.  As shown in the scripts, you need to first construct an instance of the class
+                     ProjectiveCamera that is a co-class of the main module class NonlinearLeastSquares in the distribiution.
                  grad_descent(self)
+                     This is an implementation of the basic gradient descent algorithm for nonlinear least-squares as described 
+                     in my Lecture 13 notes at the lecture-notes website for Purdue University's ECE661: Computer Vision
                  leven_marq(self)
+                     This is an implementation of the Levenberg-Marquardt algorithm for nonlinear least-squares as described 
+                     in my Lecture 13 notes at the lecture-notes website for Purdue University's ECE661: Computer Vision
+                      
+                     This function is used the following scripts in the ExamplesOptimizedSurfaceFit directory of the distro:
+                      
+                                 leven_marq.py
+                      
+                                 leven_marq_with_partial_derivatives.py
+                      
+                     It is important to note that the above two scripts do NOT call leven_marq() function directly.  AS 
+                     stated in the main document page for the NonlinearLeastSquares module, the code in the file 
+                     NonlinearLeastSquares.py is written in a domain agnostic manner.  So you need a domain adaptation 
+                     class that knows how to package the arguments for calling leven_marq().  For the case of the two scripts
+                     listed above, that domain-specific class in the distro is OptimizedSurfaceFit.  It is a co-class of 
+                     the main module class NonlinearLeastSquares in the distribution.
+                      
+                     The function leven_marq() defined here is ALSO used in the following two scripts
+   �              
+                         sfm_with_calibrated_cameras_translations_only.py
+                      sfm_with_uncalibrated_cameras_translations_only.py
+                      
+                    in the ExamplesStructureFromCameraMotion directory of the distribution.  Again, these example scripts
+                     do NOT directly call the leven_marq() function.  As shown in the two scripts, they must first construct
+                     an instance of the ProjectiveCamera class that knows how to bundle the arugments together for calling
+                     the leven_marq() function.
                  leven_marq_v1_5(self)
+                     This is the implementation of the leven_marq() function as it existed in Version 1.5.  On account of the
+                     fact that I made significant changes to this function in Version 2.0.0 of the module, I have retained the
+                     old version for the old-time users of my module.
                  set_Fvec(self, Fvector)
                      This method supplies the NonlinearLeastSquares class with the prediction vector
                      whose each element is a functional form of the prediction in the observed data vector
                      X.  Note that  Fvec is a column vector --- meaning a numpy matrix with just one column.
                  set_Fvec_BA(self, Fvector_BA)
                      You need to call this method for providing the NonlinearLeastSquares class with the
                      prediction vector if you are going to be using the bundle-adjustment capabilities
                      of the class.
                  set_X(self, X)
                  set_X_BA(self, X_BA)
                  set_debug(self, debug)
                  set_display_function(self, display_function)
                  set_initial_params(self, initial_params_dict)
-   �         set_jacobian_functionals_array(self, jacobian_functionals_array)
+                 set_jacobian_functionals_array(self, jacobian_functionals_array)
                      This method expects for its argument an Nxp matrix of functionals for the partial 
-                  derivatives needed for the Jacobian matrix.  N is the number of measurements in
+                     derivatives needed for the Jacobian matrix.  N is the number of measurements in
                      the X vector and p is the number of parameters in the model.  If you are using
                      nonlinear least-squares to fit optimal surfaces to noisy measurements over the
                      xy-plane, each element of the X vector would correspond to one such measurement at
                      some (x,y) coordinates. And an element the argument jacobian_functionals_array chararray
                      would correspond to the partial derivative of the model functional that already
                      has incorporated the (x,y) coordinates corresponding to that row and that is 
                      a partial derivative of the model with respect to the parameter corresponding to
@@ -1494,24 +1544,24 @@
                  set_num_parameters(self, how_many_parameters)
                  set_params_arranged_list(self, params_list)
                  set_params_ordered_list(self, params_list)
                  set_problem(self, prob)
                      If you are using this module to solve structure from camera motion (sfm) problems, use this method
                      to set 'self.problem' to 'sfm_N' where 'N' is the number of world points you are tracking.   This 
                      is needed because sfm needs the specialized display function defined for the ProjectiveCamera class.
-               ===========================================================================================================================
+               ===================================================================================================================================
                Data descriptors defined here:
                  __dict__
                      dictionary for instance variables (if defined)
                  __weakref__
                      list of weak references to the object (if defined)
  
 Data
          __author__ = 'Avinash Kak (kak@purdue.edu)'
-         __copyright__ = '(C) 2018 Avinash Kak. Python Software Foundation.'
-   � __date__ = '2018-November-9'
+         __copyright__ = '(C) 2022 Avinash Kak. Python Software Foundation.'
+   � __date__ = '2022-October-6'
          __url__ = 'https://engineering.purdue.edu/kak/
-         distNonlinearLeastSquares/NonlinearLeastSquares-2.0.0.html'
-         __version__ = '2.0.0'
+         distNonlinearLeastSquares/NonlinearLeastSquares-2.0.1.html'
+         __version__ = '2.0.1'
  
 Author
    � Avinash Kak (kak@purdue.edu)
```

