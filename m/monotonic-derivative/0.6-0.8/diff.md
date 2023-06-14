# Comparing `tmp/monotonic derivative-0.6.tar.gz` & `tmp/monotonic derivative-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic derivative-0.6.tar", last modified: Thu May 25 11:00:07 2023, max compression
+gzip compressed data, was "monotonic derivative-0.8.tar", last modified: Tue Jun 13 15:15:46 2023, max compression
```

## Comparing `monotonic derivative-0.6.tar` & `monotonic derivative-0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:00:07.220100 monotonic derivative-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 10:59:52.000000 monotonic derivative-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-25 11:00:07.220100 monotonic derivative-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-25 10:59:52.000000 monotonic derivative-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:00:07.220100 monotonic derivative-0.6/monotonic_derivative/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 10:59:52.000000 monotonic derivative-0.6/monotonic_derivative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 10:59:52.000000 monotonic derivative-0.6/monotonic_derivative/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-25 10:59:52.000000 monotonic derivative-0.6/monotonic_derivative/curve_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-25 10:59:52.000000 monotonic derivative-0.6/monotonic_derivative/monotonic_derivative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:00:07.220100 monotonic derivative-0.6/monotonic_derivative.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-25 11:00:07.000000 monotonic derivative-0.6/monotonic_derivative.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 11:00:07.000000 monotonic derivative-0.6/monotonic_derivative.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:00:07.000000 monotonic derivative-0.6/monotonic_derivative.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 11:00:07.000000 monotonic derivative-0.6/monotonic_derivative.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 11:00:07.000000 monotonic derivative-0.6/monotonic_derivative.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:00:07.220100 monotonic derivative-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-25 10:59:52.000000 monotonic derivative-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:00:07.220100 monotonic derivative-0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-25 10:59:52.000000 monotonic derivative-0.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:15:46.138499 monotonic derivative-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 15:15:34.000000 monotonic derivative-0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-13 15:15:46.138499 monotonic derivative-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-13 15:15:34.000000 monotonic derivative-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:15:46.134499 monotonic derivative-0.8/monotonic_derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 15:15:34.000000 monotonic derivative-0.8/monotonic_derivative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 15:15:34.000000 monotonic derivative-0.8/monotonic_derivative/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-13 15:15:34.000000 monotonic derivative-0.8/monotonic_derivative/curve_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12737 2023-06-13 15:15:34.000000 monotonic derivative-0.8/monotonic_derivative/monotonic_derivative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:15:46.138499 monotonic derivative-0.8/monotonic_derivative.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-13 15:15:46.000000 monotonic derivative-0.8/monotonic_derivative.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-13 15:15:46.000000 monotonic derivative-0.8/monotonic_derivative.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:15:46.000000 monotonic derivative-0.8/monotonic_derivative.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 15:15:46.000000 monotonic derivative-0.8/monotonic_derivative.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 15:15:46.000000 monotonic derivative-0.8/monotonic_derivative.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:15:46.138499 monotonic derivative-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-13 15:15:34.000000 monotonic derivative-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:15:46.138499 monotonic derivative-0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-13 15:15:34.000000 monotonic derivative-0.8/tests/test.py
```

### Comparing `monotonic derivative-0.6/LICENSE` & `monotonic derivative-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.6/PKG-INFO` & `monotonic derivative-0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: monotonic derivative
-Version: 0.6
-Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
+Version: 0.8
+Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. How ? thanks to it's derivative ! There is also a genetic base curve smoothing tool with several parameter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific constraints, such as in scientific modeling/engineering applications.
 Home-page: https://github.com/A-Wpro/monotonic_derivative
 Author: Adam Wecker
 Author-email: adam.wecker0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -58,36 +58,46 @@
 
 #### Example
 
 ```python
 import numpy as np
 from monotonic_derivative import ensure_monotonic_derivative
 
-x = np.array([0, 1, 2, 3, 4, 5])
-y = np.array([100, 55, 53, 40, 35, 5])
+y = np.array([289.624, 430.174, 437.31, 434.67, 427.255, 408.902, 379.064])
+x = np.array([0.078, 1.298, 2.791, 4.65, 6.002, 7.747, 10.0])
 
 modified_y = ensure_monotonic_derivative(
-    x, y, degree=2, force_negative_derivative=True, verbose=True, save_plot=True)
+    x=x,
+    y=y,
+    degree=3, 
+    force_negative_derivative=False,
+    verbose=True,
+    save_plot=True,
+)
 ```
 
 #### Result :
 
 We got a new curve that follow one rule : The Xth degree (depending of paramter degree) derivate must be increasing/decreasing (depending of force_negative_derivative parameter) curve.
 
 ```
-#from
-y = [100, 55, 53, 40, 35, 5]
-#to
-modified_y = [99.78638543 56.7089208  48.94131484 44.05868538 33.29107987  5.21361543]
+Original y    : [289.624 430.174 437.31  434.67  427.255 408.902 379.064]
+Modified y    : [290.6626736  423.94170784 445.4551795  434.69854619 424.27831859 407.55132434 380.41124237]
+Similarity score : 0.9982442661935377 
+Optimization success: True
+Optimization message: Optimization terminated successfully
 ```
 
-As you can see, slight change on y can totaly change how react the 2rd derivate.
+As you can see, big change on 3rd derivate have small impact of the 1st derivate curve but force it to be monotonicaly decreasing. 
 
 ![Derivative Example](./images/derivative.png)
 
+Obvisouly and depending of which degree to lock below or above 0 you can force a curve to be closer to their mathematical reality.
+
+
 #### Genetic algorithm smoothing tool:
 
 ```python
 ### Test for curve smoothing with genetic algo
 from monotonic_derivative.curve_smoothing import  curve_smoothing
 ```
 
@@ -103,15 +113,15 @@
 
 The function returns the best individual (smoothed curve) found by the genetic algorithm as a numpy array.
 
 #### Example
 
 ```python
 import numpy as np
-from monotonic_derivative.curve_smoothing import  curve_smoothing
+from monotonic_derivative.curve_smoothing import curve_smoothing
 
 points = np.array([125, 55, 53, 40, 35, -25])
 best_individual = curve_smoothing(points, alpha=0.5,save_plots = True)
 #best_individual is the smoothed curve
 ```
 
 #### Result :
@@ -120,15 +130,15 @@
 
 ![Derivative Example](./images/progress.gif)
 
 ### Real-life Applications
 
 In many real-life scenarios, the collected data may produce curves that are not logical or do not follow the expected constraints. For example, the data representing the velocity of a car over time should show an increasing or decreasing acceleration, but due to measurement errors or other factors, the collected data points may not reflect this.
 
-The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing, making your data analysis more accurate and reliable.
+The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative always monotonically increasing or decreasing, by forcing the value of a derivative to be below or above 0, making your data analysis more accurate and reliable.
 
 ### Limit
 
 There are certain limitations to consider when using this library. For example, if you want to enforce a 2nd-degree monotonic increasing derivative on a curve that already has an originally monotonic increasing 2nd-degree derivative, the modification applied to the original curve will be much more pronounced. In this case, the resulting 2nd-degree derivative will be almost flat, but still slightly increasing.
 
 It's important to remember that the purpose of this library is to modify a curve based on the physical/mathematical reality that the curve represents. When using the monotonic_derivative library, keep in mind that the goal is to create a more realistic or physically plausible representation of the original curve while preserving its essential characteristics. This can be particularly useful in applications where the original data may be subject to noise or other inaccuracies, and a more idealized or smoothed curve is required for analysis or presentation purposes.
```

### Comparing `monotonic derivative-0.6/README.md` & `monotonic derivative-0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -42,36 +42,46 @@
 
 #### Example
 
 ```python
 import numpy as np
 from monotonic_derivative import ensure_monotonic_derivative
 
-x = np.array([0, 1, 2, 3, 4, 5])
-y = np.array([100, 55, 53, 40, 35, 5])
+y = np.array([289.624, 430.174, 437.31, 434.67, 427.255, 408.902, 379.064])
+x = np.array([0.078, 1.298, 2.791, 4.65, 6.002, 7.747, 10.0])
 
 modified_y = ensure_monotonic_derivative(
-    x, y, degree=2, force_negative_derivative=True, verbose=True, save_plot=True)
+    x=x,
+    y=y,
+    degree=3, 
+    force_negative_derivative=False,
+    verbose=True,
+    save_plot=True,
+)
 ```
 
 #### Result :
 
 We got a new curve that follow one rule : The Xth degree (depending of paramter degree) derivate must be increasing/decreasing (depending of force_negative_derivative parameter) curve.
 
 ```
-#from
-y = [100, 55, 53, 40, 35, 5]
-#to
-modified_y = [99.78638543 56.7089208  48.94131484 44.05868538 33.29107987  5.21361543]
+Original y    : [289.624 430.174 437.31  434.67  427.255 408.902 379.064]
+Modified y    : [290.6626736  423.94170784 445.4551795  434.69854619 424.27831859 407.55132434 380.41124237]
+Similarity score : 0.9982442661935377 
+Optimization success: True
+Optimization message: Optimization terminated successfully
 ```
 
-As you can see, slight change on y can totaly change how react the 2rd derivate.
+As you can see, big change on 3rd derivate have small impact of the 1st derivate curve but force it to be monotonicaly decreasing. 
 
 ![Derivative Example](./images/derivative.png)
 
+Obvisouly and depending of which degree to lock below or above 0 you can force a curve to be closer to their mathematical reality.
+
+
 #### Genetic algorithm smoothing tool:
 
 ```python
 ### Test for curve smoothing with genetic algo
 from monotonic_derivative.curve_smoothing import  curve_smoothing
 ```
 
@@ -87,15 +97,15 @@
 
 The function returns the best individual (smoothed curve) found by the genetic algorithm as a numpy array.
 
 #### Example
 
 ```python
 import numpy as np
-from monotonic_derivative.curve_smoothing import  curve_smoothing
+from monotonic_derivative.curve_smoothing import curve_smoothing
 
 points = np.array([125, 55, 53, 40, 35, -25])
 best_individual = curve_smoothing(points, alpha=0.5,save_plots = True)
 #best_individual is the smoothed curve
 ```
 
 #### Result :
@@ -104,15 +114,15 @@
 
 ![Derivative Example](./images/progress.gif)
 
 ### Real-life Applications
 
 In many real-life scenarios, the collected data may produce curves that are not logical or do not follow the expected constraints. For example, the data representing the velocity of a car over time should show an increasing or decreasing acceleration, but due to measurement errors or other factors, the collected data points may not reflect this.
 
-The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing, making your data analysis more accurate and reliable.
+The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative always monotonically increasing or decreasing, by forcing the value of a derivative to be below or above 0, making your data analysis more accurate and reliable.
 
 ### Limit
 
 There are certain limitations to consider when using this library. For example, if you want to enforce a 2nd-degree monotonic increasing derivative on a curve that already has an originally monotonic increasing 2nd-degree derivative, the modification applied to the original curve will be much more pronounced. In this case, the resulting 2nd-degree derivative will be almost flat, but still slightly increasing.
 
 It's important to remember that the purpose of this library is to modify a curve based on the physical/mathematical reality that the curve represents. When using the monotonic_derivative library, keep in mind that the goal is to create a more realistic or physically plausible representation of the original curve while preserving its essential characteristics. This can be particularly useful in applications where the original data may be subject to noise or other inaccuracies, and a more idealized or smoothed curve is required for analysis or presentation purposes.
```

### Comparing `monotonic derivative-0.6/monotonic_derivative/curve_smoothing.py` & `monotonic derivative-0.8/monotonic_derivative/curve_smoothing.py`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.6/monotonic_derivative/monotonic_derivative.py` & `monotonic derivative-0.8/monotonic_derivative/monotonic_derivative.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,147 +1,221 @@
 import numpy as np
 from scipy.interpolate import CubicSpline
 from scipy.optimize import minimize
 import matplotlib.pyplot as plt
 from io import BytesIO
 import imageio
+from scipy.interpolate import interp1d
+from scipy.interpolate import PchipInterpolator
 
 
 def extend_data(x, y, dx=0.1, dy=0.1, force_negative_derivative=False):
     """
-    Add a new data point before the first point in the dataset.
+    Add a new data point before the first point and after the last point in the dataset.
 
     Parameters:
     x: numpy array, the independent variable data points
     y: numpy array, the dependent variable data points
-    dx: float, the distance between the new data point and the first data point in x
-    dy: float, the distance between the new data point and the first data point in y
+    dx: float, the distance between the new data point and the first/last data point in x
+    dy: float, the distance between the new data point and the first/last data point in y
     force_negative_derivative: bool, force the specified degree derivative to be monotonically decreasing if True
 
     Returns:
     x_extended: numpy array, the extended x data points
     y_extended: numpy array, the extended y data points
     """
-    x = np.insert(x, 0, x[0] - dx)
-    x_extended = np.insert(x, len(x), x[-1] + dx)
-    y = np.insert(y, 0, y[0] - dy if not force_negative_derivative else y[0] + dy)
-    y_extended = np.insert(
-        y, len(y), y[-1] - dy if not force_negative_derivative else y[-1] + dy
+    x_extended = np.concatenate(([x[0] - dx], x, [x[-1] + dx]))
+    y_extended = np.concatenate(
+        (
+            [y[0] * (1 - dy) if not force_negative_derivative else y[0] * (1 + dy)],
+            y,
+            [y[-1] * (1 - dy) if not force_negative_derivative else y[-1] * (1 + dy)],
+        )
     )
 
     return x_extended, y_extended
 
 
+def calculate_similarity(curve1, curve2):
+    # Interpolate curve2 to have the same length as curve1
+    f = interp1d(np.arange(len(curve2)), curve2)
+    curve2_interp = f(np.linspace(0, len(curve2) - 1, len(curve1)))
+
+    # Calculate correlation coefficient
+    correlation = np.corrcoef(curve1, curve2_interp)[0, 1]
+
+    # Convert correlation coefficient to similarity score
+    similarity = (correlation + 1) / 2
+
+    return similarity
+
+
+def interpolated_curve(x, y, step=0.01):
+    # Create a cubic spline interpolation
+    interp = PchipInterpolator(x, y, extrapolate=True)
+
+    # Control 2 decimals for GL
+    x_pchip_original = np.arange(
+        round(float(x.min()), 2),
+        round(float(x.max()), 2) + step,
+        step,
+    )
+    y_pchip_original = interp(x_pchip_original)
+
+    return x_pchip_original, y_pchip_original
+
+
 def ensure_monotonic_derivative(
     x,
     y,
     degree=2,
     force_negative_derivative=False,
     verbose=False,
     save_plot=False,
-    use_interpolated_data=False,
     max_iter_minimize=50000,
+    return_interpolated_curve=False,
+    use_interpolated_data=False,  # Should not be use, except you know what you do
+    extending_data=False,  # Should not be use, except you know what you do
 ):
     """
     Modify the given data points to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing.
 
     Parameters:
     x: numpy array, the independent variable data points
     y: numpy array, the dependent variable data points
     degree: int, the degree of the derivative to check for monotonicity
     force_negative_derivative: bool, force the specified degree derivative to be monotonically decreasing if True
     verbose: bool, print additional information if True
     save_plot: bool, save the plots as GIF images if True
-    use_interpolated_data: bool, use interpolated data points instead of the original ones if True
     max_iter_minimize: int, maximum number of iterations for the optimization method
-    num_points: int, the number of points to use for interpolation if use_interpolated_data is True
+    return_interpolated_curve : bool, instead of return the modified y alone we return a tuple of interpolated array.
+    use_interpolated_data: bool, use interpolated data points instead of the original ones if True # Should not be use, except you know what you do
+    extending_data: bool, create new data point before our data and after  # Should not be use, except you know what you do
 
     Returns:
     modified_y: numpy array, the modified dependent variable data points
     """
     # Extend the data with a new point before the first point
-    x, y = extend_data(
-        x, y, dx=1, dy=0, force_negative_derivative=force_negative_derivative
-    )
-
-    def objective_function(y, x, y_original):
-        # This is the original objective
+    if extending_data:
+        x, y = extend_data(
+            x,
+            y,
+            dx=(sum(x) / len(x)),
+            dy=0.05,
+            force_negative_derivative=force_negative_derivative,
+        )  ## TODO, add dy,dx as value that can change to force the monotinic value, bad idea ?
+
+    def objective_function(
+        y, x, y_original, force_negative_derivative, degree
+    ):  # parameter will be used to modify penalty if needed
+        penalty = 0  # no penalty, it's here for potential futur update
         mse = np.sum((y - y_original) ** 2)
+        # We add the penalty term to the MSE
+        return mse + penalty
 
-        # This is the penalty term. You can adjust the scale factor (e.g., 1e3)
-        # to make the penalty larger or smaller.
-        # first_point_penalty = 1e3 * max(0, 0.1 - abs(y[0] - y_original[0])) ** 4
-
-        return mse  # + first_point_penalty
-
-    def constraint_second_derivative_increasing(y, x):
+    def constraint_degree_derivative_positive(y, x, degree):
         """
         Function to create a constraint function to be used in the optimization problem.
-        The constraint function calculates the minimum difference between consecutive second derivatives.
+        The constraint function checks if all points of the `degree`-th derivative are less than 0.
 
         Parameters:
         y: numpy array, the dependent variable data points
         x: numpy array, the independent variable data points
+        degree: int, the degree of the derivative to check for negativity
 
         Returns:
         constraint: function, the constraint function for the optimization problem
         """
 
         def constraint(y):
             cs = CubicSpline(x, y)
-            y_2nd_derivative = cs(x, 2)
-            return np.min(np.diff(y_2nd_derivative))
+            x_resampled = np.arange(np.min(x), np.max(x), 0.01)
+            derivative_resampled = cs(x_resampled, degree)
+            return (
+                derivative_resampled - 0.00000000001
+            )  # 0.00000000001 instead of 0 to avoid critic state problem and other calculation problem
 
         return constraint
 
-    def constraint_second_derivative_decreasing(y, x):
+    def constraint_degree_derivative_negative(y, x, degree):
         """
         Function to create a constraint function to be used in the optimization problem.
-        The constraint function calculates the maximum difference between consecutive second derivatives.
+        The constraint function checks if all points of the `degree`-th derivative are less than 0.
 
         Parameters:
         y: numpy array, the dependent variable data points
         x: numpy array, the independent variable data points
+        degree: int, the degree of the derivative to check for negativity
 
         Returns:
         constraint: function, the constraint function for the optimization problem
         """
 
         def constraint(y):
             cs = CubicSpline(x, y)
-            y_2nd_derivative = cs(x, 2)
-            return np.min(-np.diff(y_2nd_derivative))
+            x_resampled = np.arange(np.min(x), np.max(x), 0.01)
+            derivative_resampled = cs(x_resampled, degree)
+            return (
+                -derivative_resampled - 0.00000000001
+            )  # 0.00000000001 instead of 0 to avoid critic state problem and other calculation problem
 
         return constraint
 
-    def interpolate_data(x, y, num_points=1000):
+    def interpolate_data(
+        x, y, num_points_between=1000
+    ):  # should be change very soon and should not be used like this except you know what yo do
         """
         Create a cubic spline interpolation of the given data points with the specified degree.
+        New points are added between original points, but original points are also kept.
 
         Parameters:
         x: numpy array, the independent variable data points
         y: numpy array, the dependent variable data points
-        num_points: int, the number of points to use for interpolation
+        num_points_between: int, the number of points to interpolate between each original pair of points
 
         Returns:
         x_new: numpy array, the new x values used for interpolation
         y_new: numpy array, the new y values obtained from interpolation
         """
-        cs = CubicSpline(x, y, bc_type="natural")
 
-        x_new = np.linspace(x[0], x[-1], num_points)
-        y_new = cs(x_new)
+        x_new = []
+        y_new = []
+
+        # Iterate over pairs of points in the original data
+        for i in range(len(x) - 1):
+            # Create a cubic spline for this pair of points
+            cs = CubicSpline(x[i : i + 2], y[i : i + 2], bc_type="natural")
+
+            # Generate new x values between this pair of original points
+            x_interp = np.linspace(x[i], x[i + 1], num_points_between + 2)
+
+            # Generate new y values for these x values
+            y_interp = cs(x_interp)
+
+            # Append new values to the list, excluding the last point to avoid duplicates
+            x_new.extend(x_interp[:-1])
+            y_new.extend(y_interp[:-1])
+
+        # Append the last point from the original data
+        x_new.append(x[-1])
+        y_new.append(y[-1])
+
+        # Convert lists to numpy arrays
+        x_new = np.array(x_new)
+        y_new = np.array(y_new)
 
         return x_new, y_new
 
     # Use interpolated data if use_interpolated_data is True
     label_original_point = "Original data points"
     if use_interpolated_data:
+        y_not_intra = y
+        x_not_intra = x
         x, y = interpolate_data(x, y, len(y) + degree)
-        label_original_point = "Original extrapoled data points"
+        label_original_point_intra = "Original intrapoled data points"
 
     # Check if x and y have the same length
     if len(x) != len(y):
         raise ValueError("x and y must have the same length")
 
     # Check if the specified degree is valid
     if degree >= len(y) - 1:
@@ -149,80 +223,107 @@
             "Degree must be less than the length of the data minus 1, since we lose one data point for each derivative and need at least two data points"
         )
     if degree < 0:
         raise ValueError("The degree parameter cannot be negative")
 
     # Define the constraint for the optimization problem
     if force_negative_derivative:
-        cons = {"type": "ineq", "fun": constraint_second_derivative_decreasing(y, x)}
+        cons = {
+            "type": "ineq",
+            "fun": constraint_degree_derivative_negative(y, x, degree),
+        }
     else:
-        cons = {"type": "ineq", "fun": constraint_second_derivative_increasing(y, x)}
+        cons = {
+            "type": "ineq",
+            "fun": constraint_degree_derivative_positive(y, x, degree),
+        }
 
     # Solve the optimization problem
     # List of methods to try
     methods = [
         "SLSQP",
         "CG",
         "BFGS",
-        "Newton-CG",
         "L-BFGS-B",
         "TNC",
         "COBYLA",
         "trust-constr",
     ]
 
     # Solve the optimization problem
     res = None
     for method in methods:
         res = minimize(
             objective_function,
             y,
-            args=(x, y),
+            args=(x, y, force_negative_derivative, degree),
             constraints=cons,
             method=method,
             options={"maxiter": max_iter_minimize},
         )
         # if optimization is successful and the termination condition is not 'xtol', break the loop
         if res.success and "xtol" not in res.message:
             break
-    y = y[1:-1]  # to remove 1st fake dot and last
-    modified_y = res.x[1:-1] if res else y
-    x = x[1:-1]
+    if extending_data:
+        y = y[0:-1]  # to remove 1st fake dot and last
+        modified_y = res.x[0:-1] if res else y
+        x = x[0:-1]
+    else:
+        modified_y = res.x if res else y
+
     if verbose:
-        print("Original y    :", y)
-        print("Modified y    :", modified_y)
+        if use_interpolated_data:
+            print("Original y    :", y_not_intra)
+            print("Original intrapoled y    :", y)
+            print("Modified y    :", modified_y)
+            similarity_score_intra = calculate_similarity(modified_y, y)
+            similarity_score = calculate_similarity(modified_y, y_not_intra)
+            print("Similarity score intrapoled:", similarity_score_intra)
+            print("Similarity score :", similarity_score)
+        else:
+            similarity_score = calculate_similarity(modified_y, y)
+            print("Original y    :", y)
+            print("Modified y    :", modified_y)
+            print("Similarity score :", similarity_score)
+
         print("Optimization success:", res.success)
         print("Optimization message:", res.message)
 
     # Save and display plots of original and modified data and their derivatives if save_plot is True
     if save_plot:
         fig, ax = plt.subplots(degree + 1, 1, figsize=(8, 3 * (degree + 1)))
 
         # Plot the original and modified data points
-        ax[0].plot(x, y, "o--", label=label_original_point)
-        ax[0].plot(x, modified_y, "o--", label="Modified data points")
+
+        if use_interpolated_data:
+            ax[0].plot(x, y, "b-", label=label_original_point_intra)
+            ax[0].plot(x_not_intra, y_not_intra, "m-", label=label_original_point)
+        else:
+            ax[0].plot(x, y, "b-", label=label_original_point)
+        ax[0].plot(x, modified_y, "g-", label="Modified data points")
         ax[0].set_xlabel("x")
         ax[0].set_ylabel("y")
         ax[0].legend()
 
         cs_original = CubicSpline(x, y)
         cs_modified = CubicSpline(x, modified_y)
 
         # Plot derivatives from 1st to the specified degree
         for d, ax_i in enumerate(ax[1:], start=1):
+            # Compute the Xth derivative
+            y_first_derivative = cs_original(x, d)
+            y_smoothed_first_derivative = cs_modified(x, d)
             ax_i.plot(
-                x[:-d],
-                np.diff(y, n=d) / np.prod([np.diff(x) for _ in range(d)]),
-                "o--",
+                x,
+                y_first_derivative,
                 label=f"{d}th derivative (original)",
             )
             ax_i.plot(
-                x[:-d],
-                np.diff(modified_y, n=d) / np.prod([np.diff(x) for _ in range(d)]),
-                "o--",
+                x,
+                y_smoothed_first_derivative,
                 label=f"{d}th derivative (modified)",
             )
             ax_i.set_xlabel("x")
             ax_i.set_ylabel(f"{d}th derivative")
             ax_i.legend()
 
         plt.tight_layout()
@@ -232,8 +333,10 @@
         buf.seek(0)
         image = imageio.imread(buf)
         plt.close(fig)
 
         # Save the image as a png
         imageio.imwrite("derivative.png", image)
 
+    if return_interpolated_curve:
+        return interpolated_curve(x, modified_y)
     return modified_y
```

### Comparing `monotonic derivative-0.6/monotonic_derivative.egg-info/PKG-INFO` & `monotonic derivative-0.8/monotonic_derivative.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: monotonic-derivative
-Version: 0.6
-Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
+Version: 0.8
+Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. How ? thanks to it's derivative ! There is also a genetic base curve smoothing tool with several parameter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific constraints, such as in scientific modeling/engineering applications.
 Home-page: https://github.com/A-Wpro/monotonic_derivative
 Author: Adam Wecker
 Author-email: adam.wecker0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -58,36 +58,46 @@
 
 #### Example
 
 ```python
 import numpy as np
 from monotonic_derivative import ensure_monotonic_derivative
 
-x = np.array([0, 1, 2, 3, 4, 5])
-y = np.array([100, 55, 53, 40, 35, 5])
+y = np.array([289.624, 430.174, 437.31, 434.67, 427.255, 408.902, 379.064])
+x = np.array([0.078, 1.298, 2.791, 4.65, 6.002, 7.747, 10.0])
 
 modified_y = ensure_monotonic_derivative(
-    x, y, degree=2, force_negative_derivative=True, verbose=True, save_plot=True)
+    x=x,
+    y=y,
+    degree=3, 
+    force_negative_derivative=False,
+    verbose=True,
+    save_plot=True,
+)
 ```
 
 #### Result :
 
 We got a new curve that follow one rule : The Xth degree (depending of paramter degree) derivate must be increasing/decreasing (depending of force_negative_derivative parameter) curve.
 
 ```
-#from
-y = [100, 55, 53, 40, 35, 5]
-#to
-modified_y = [99.78638543 56.7089208  48.94131484 44.05868538 33.29107987  5.21361543]
+Original y    : [289.624 430.174 437.31  434.67  427.255 408.902 379.064]
+Modified y    : [290.6626736  423.94170784 445.4551795  434.69854619 424.27831859 407.55132434 380.41124237]
+Similarity score : 0.9982442661935377 
+Optimization success: True
+Optimization message: Optimization terminated successfully
 ```
 
-As you can see, slight change on y can totaly change how react the 2rd derivate.
+As you can see, big change on 3rd derivate have small impact of the 1st derivate curve but force it to be monotonicaly decreasing. 
 
 ![Derivative Example](./images/derivative.png)
 
+Obvisouly and depending of which degree to lock below or above 0 you can force a curve to be closer to their mathematical reality.
+
+
 #### Genetic algorithm smoothing tool:
 
 ```python
 ### Test for curve smoothing with genetic algo
 from monotonic_derivative.curve_smoothing import  curve_smoothing
 ```
 
@@ -103,15 +113,15 @@
 
 The function returns the best individual (smoothed curve) found by the genetic algorithm as a numpy array.
 
 #### Example
 
 ```python
 import numpy as np
-from monotonic_derivative.curve_smoothing import  curve_smoothing
+from monotonic_derivative.curve_smoothing import curve_smoothing
 
 points = np.array([125, 55, 53, 40, 35, -25])
 best_individual = curve_smoothing(points, alpha=0.5,save_plots = True)
 #best_individual is the smoothed curve
 ```
 
 #### Result :
@@ -120,15 +130,15 @@
 
 ![Derivative Example](./images/progress.gif)
 
 ### Real-life Applications
 
 In many real-life scenarios, the collected data may produce curves that are not logical or do not follow the expected constraints. For example, the data representing the velocity of a car over time should show an increasing or decreasing acceleration, but due to measurement errors or other factors, the collected data points may not reflect this.
 
-The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing, making your data analysis more accurate and reliable.
+The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative always monotonically increasing or decreasing, by forcing the value of a derivative to be below or above 0, making your data analysis more accurate and reliable.
 
 ### Limit
 
 There are certain limitations to consider when using this library. For example, if you want to enforce a 2nd-degree monotonic increasing derivative on a curve that already has an originally monotonic increasing 2nd-degree derivative, the modification applied to the original curve will be much more pronounced. In this case, the resulting 2nd-degree derivative will be almost flat, but still slightly increasing.
 
 It's important to remember that the purpose of this library is to modify a curve based on the physical/mathematical reality that the curve represents. When using the monotonic_derivative library, keep in mind that the goal is to create a more realistic or physically plausible representation of the original curve while preserving its essential characteristics. This can be particularly useful in applications where the original data may be subject to noise or other inaccuracies, and a more idealized or smoothed curve is required for analysis or presentation purposes.
```

### Comparing `monotonic derivative-0.6/setup.py` & `monotonic derivative-0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="monotonic derivative",
-    version="0.6",
-    description="Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.",
+    version="0.8",
+    description="Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. How ? thanks to it's derivative ! There is also a genetic base curve smoothing tool with several parameter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific constraints, such as in scientific modeling/engineering applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Adam Wecker",
     author_email="adam.wecker0@gmail.com",
     url="https://github.com/A-Wpro/monotonic_derivative",
     packages=["monotonic_derivative"],
     install_requires=["numpy", "scipy", "matplotlib", "imageio"],
```

### Comparing `monotonic derivative-0.6/tests/test.py` & `monotonic derivative-0.8/tests/test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import numpy as np
 import pytest
 
 ### Test for monotonic derivative smoothing
 from monotonic_derivative import ensure_monotonic_derivative
+from scipy.interpolate import CubicSpline
 
 
 def test_basic_usage():
     x = np.array([0, 1, 2, 3, 4, 5])
     y = np.array([100, 55, 53, 40, 35, 5])
     d = 2
     modified_y = ensure_monotonic_derivative(
-        x, y, degree=d, force_negative_derivative=False, verbose=False, save_plot=False
+        x, y, degree=d, force_negative_derivative=False, verbose=True, save_plot=False
     )
     assert len(modified_y) == len(y)
-    d2nd = np.diff(modified_y, n=d) / np.prod([np.diff(x) for _ in range(d)])
-    assert all(d2nd[i] <= d2nd[i + 1] for i in range(len(d2nd) - 1))
+    cs = CubicSpline(x, modified_y)
+    y_original_Xst_derivative = cs(x, d)
+    print(y_original_Xst_derivative)
+    assert all(
+        y_original_Xst_derivative[i] >= 0
+        for i in range(len(y_original_Xst_derivative) - 1)
+    )
 
 
 def test_invalid_degree():
     x = np.array([0, 1, 2, 3, 4, 5])
     y = np.array([100, 55, 53, 40, 35, 5])
 
     with pytest.raises(ValueError):
@@ -29,16 +35,20 @@
     x = np.array([0, 1, 2, 3, 4, 5])
     y = np.array([100, 55, 53, 40, 35, 5])
     d = 2
     modified_y = ensure_monotonic_derivative(
         x, y, degree=d, force_negative_derivative=True, verbose=False, save_plot=False
     )
     assert len(modified_y) == len(y)
-    d2nd = np.diff(modified_y, n=d) / np.prod([np.diff(x) for _ in range(d)])
-    assert all(d2nd[i] >= d2nd[i + 1] for i in range(len(d2nd) - 1))
+    cs = CubicSpline(x, modified_y)
+    y_original_1st_derivative = cs(x, d)
+    assert all(
+        y_original_1st_derivative[i] <= 0
+        for i in range(len(y_original_1st_derivative) - 1)
+    )
 
 
 def test_mismatched_lengths():
     x = np.array([0, 1, 2, 3, 4, 5])
     y = np.array([100, 55, 53, 40, 35])
 
     with pytest.raises(ValueError):
```

