# Comparing `tmp/chartart-0.0.3.dev16.tar.gz` & `tmp/chartart-0.0.3.dev17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartart-0.0.3.dev16.tar", last modified: Thu Jun  1 06:11:02 2023, max compression
+gzip compressed data, was "chartart-0.0.3.dev17.tar", last modified: Wed Jun 14 20:59:57 2023, max compression
```

## Comparing `chartart-0.0.3.dev16.tar` & `chartart-0.0.3.dev17.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.535534 chartart-0.0.3.dev16/
--rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/LICENSE
--rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-06-01 06:11:02.535934 chartart-0.0.3.dev16/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)     1814 2023-05-31 13:18:32.000000 chartart-0.0.3.dev16/README.md
--rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/pyproject.toml
--rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-06-01 06:11:02.540001 chartart-0.0.3.dev16/setup.cfg
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.489453 chartart-0.0.3.dev16/src/
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.512547 chartart-0.0.3.dev16/src/chartart/
--rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/conftest.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/helpers.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    80851 2023-06-01 06:10:01.000000 chartart-0.0.3.dev16/src/chartart/plot.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/simple_eda_template.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/test_plot.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.529989 chartart-0.0.3.dev16/src/chartart/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/tests/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/tests/test_simple.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.520333 chartart-0.0.3.dev16/src/chartart.egg-info/
--rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-06-01 06:11:02.000000 chartart-0.0.3.dev16/src/chartart.egg-info/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-06-01 06:11:02.000000 chartart-0.0.3.dev16/src/chartart.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-06-01 06:11:02.000000 chartart-0.0.3.dev16/src/chartart.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-06-01 06:11:02.000000 chartart-0.0.3.dev16/src/chartart.egg-info/requires.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-06-01 06:11:02.000000 chartart-0.0.3.dev16/src/chartart.egg-info/top_level.txt
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.533020 chartart-0.0.3.dev16/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.048427 chartart-0.0.3.dev17/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/LICENSE
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-06-14 20:59:57.048776 chartart-0.0.3.dev17/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1814 2023-05-31 13:18:32.000000 chartart-0.0.3.dev17/README.md
+-rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/pyproject.toml
+-rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-06-14 20:59:57.050186 chartart-0.0.3.dev17/setup.cfg
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.027644 chartart-0.0.3.dev17/src/
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.038546 chartart-0.0.3.dev17/src/chartart/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/conftest.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/helpers.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    84149 2023-06-14 18:51:32.000000 chartart-0.0.3.dev17/src/chartart/plot.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/simple_eda_template.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/test_plot.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.045651 chartart-0.0.3.dev17/src/chartart/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/tests/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.043469 chartart-0.0.3.dev17/src/chartart.egg-info/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-06-14 20:59:57.000000 chartart-0.0.3.dev17/src/chartart.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-06-14 20:59:57.000000 chartart-0.0.3.dev17/src/chartart.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-06-14 20:59:57.000000 chartart-0.0.3.dev17/src/chartart.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-06-14 20:59:57.000000 chartart-0.0.3.dev17/src/chartart.egg-info/requires.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-06-14 20:59:57.000000 chartart-0.0.3.dev17/src/chartart.egg-info/top_level.txt
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.046923 chartart-0.0.3.dev17/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/tests/test_simple.py
```

### Comparing `chartart-0.0.3.dev16/LICENSE` & `chartart-0.0.3.dev17/LICENSE`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev16/PKG-INFO` & `chartart-0.0.3.dev17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev16
+Version: 0.0.3.dev17
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chartart-0.0.3.dev16/README.md` & `chartart-0.0.3.dev17/README.md`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev16/setup.cfg` & `chartart-0.0.3.dev17/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chartart
-version = 0.0.3.dev16
+version = 0.0.3.dev17
 author = BR-Advisers
 author_email = info@br-advisers.com
 description = ChartArt python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `chartart-0.0.3.dev16/src/chartart/__init__.py` & `chartart-0.0.3.dev17/src/chartart/__init__.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev16/src/chartart/conftest.py` & `chartart-0.0.3.dev17/src/chartart/conftest.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev16/src/chartart/helpers.py` & `chartart-0.0.3.dev17/src/chartart/helpers.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev16/src/chartart/plot.py` & `chartart-0.0.3.dev17/src/chartart/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,16 +135,16 @@
         return False 
 
 isNotebook = isNotebook()
 
 class Figure:
     def __init__(self, chart_id: Union[int, float, str], title: str = None,
                  x_axis_label: str = None, y_axis_label: str = None, isRealTime:bool = False,
-                 xAxisMaximum: Optional[Union[int, float, str]] = None, xAxisMinimum: Optional[Union[int, float, str]] = None, xAxisOpposedPosition: Optional[bool] = None, xAxisLabelRotation: Optional[int] = None,  xAxisIsVisible: Optional[bool] = None, xAxisDateFormat: Optional[str] = None, xAxisRangePadding: Optional[str] = None, xAxisPlotOffset: Optional[float] = None,
-                 yAxisMaximum: Optional[Union[int, float, str]] = None, yAxisMinimum: Optional[Union[int, float, str]] = None, yAxisOpposedPosition: Optional[bool] = None, yAxisLabelRotation: Optional[int] = None,  yAxisIsVisible: Optional[bool] = None, yAxisDateFormat: Optional[str] = None, yAxisRangePadding: Optional[str] = None, yAxisPlotOffset: Optional[float] = None,
+                 xAxisMaximum: Optional[Union[int, float, str]] = None, xAxisMinimum: Optional[Union[int, float, str]] = None, xAxisOpposedPosition: Optional[bool] = None, xAxisLabelRotation: Optional[int] = None,  xAxisIsVisible: Optional[bool] = None, xAxisDateFormat: Optional[str] = None, xAxisNumberFormat: Optional[str] = None, xAxisRangePadding: Optional[str] = None, xAxisPlotOffset: Optional[float] = None,
+                 yAxisMaximum: Optional[Union[int, float, str]] = None, yAxisMinimum: Optional[Union[int, float, str]] = None, yAxisOpposedPosition: Optional[bool] = None, yAxisLabelRotation: Optional[int] = None,  yAxisIsVisible: Optional[bool] = None, yAxisDateFormat: Optional[str] = None, yAxisNumberFormat: Optional[str] = None, yAxisRangePadding: Optional[str] = None, yAxisPlotOffset: Optional[float] = None,
                  flex: int = 1):
         # TODO: Convert the instance attributes to class attributes?
         # TODO: Add support for X and Y axis limits.
         # TODO: Add support for dual Y axis.
         self.notebook_name = get_notebook_name()
         """
         Chart ID needs to be compulsorily specified by the user. It seems cumbersome but let's wait for
@@ -158,27 +158,34 @@
         Preview collection are not deleted after they are converted into Posts.
         :param xAxisMaximum: In the maximum properties of the axis, you can specify the maximum values with respect to the entire data source.
         :param xAxisMinimum: In the minimum properties of the axis, you can specify the minimum values with respect to the entire data source.
         :param xAxisOpposedPosition: The opposedPosition property of axis can be used to place the axis at the opposite side of its default position.
         :param xAxisLabelRotation: The labelRotation property of axis can be used to rotate the axis labels position.
         :param xAxisIsVisible: When the axis visibility is set to false, then the axis elements like ticks, labels, title, etc will be hidden.
         :param xAxisDateFormat: Date time format in case of date time axis
+        :param xAxisNumberFormat: Number format in case of numeric axis. possible values are.
+                                none : 1200000
+                                comma : 1,200,000
+                                compact :  1.2M
+                                compactLong : 1.2 million
+                                scientific : 1.2E6
         :param xAxisRangePadding:   auto :  will apply `none` as padding for horizontal numeric axis, while the vertical numeric axis takes `normal` as padding calculation.
                                     none : ChartRangePadding.none, will not add any padding to the minimum and maximum values.
                                     normal : ChartRangePadding.normal, will apply padding to the axis based on the default range calculation.
                                     additional : will add an interval to the minimum and maximum of the axis.
                                     round :  will round the minimum and maximum values to the nearest possible value.
         :param xAxisPlotOffset: The plotOffset property is used to offset the rendering of the axis at start and end position.
         
         :param yAxisMaximum: In the maximum properties of the axis, you can specify the maximum values with respect to the entire data source.
         :param yAxisMinimum: In the minimum properties of the axis, you can specify the minimum values with respect to the entire data source.
         :param yAxisOpposedPosition: The opposedPosition property of axis can be used to place the axis at the opposite side of its default position.
         :param yAxisLabelRotation: The labelRotation property of axis can be used to rotate the axis labels position.
         :param yAxisIsVisible: When the axis visibility is set to false, then the axis elements like ticks, labels, title, etc will be hidden.
         :param yAxisDateFormat: Date time format in case of date time axis
+        :param yAxisNumberFormat: Number format in case of numeric axis
         :param yAxisRangePadding:   auto :  will apply `none` as padding for horizontal numeric axis, while the vertical numeric axis takes `normal` as padding calculation.
                                     none : ChartRangePadding.none, will not add any padding to the minimum and maximum values.
                                     normal : ChartRangePadding.normal, will apply padding to the axis based on the default range calculation.
                                     additional : will add an interval to the minimum and maximum of the axis.
                                     round :  will round the minimum and maximum values to the nearest possible value.
         :param yAxisPlotOffset: The plotOffset property is used to offset the rendering of the axis at start and end position.
         :param flex: In grid/split layout this is the ratio of size
@@ -222,14 +229,16 @@
             self.xAxisProperties['opposedPosition'] = xAxisOpposedPosition
         if xAxisLabelRotation:
             self.xAxisProperties['labelRotation'] = xAxisLabelRotation
         if xAxisIsVisible:
             self.xAxisProperties['isVisible'] = xAxisIsVisible
         if xAxisDateFormat:
             self.xAxisProperties['dateFormat'] = xAxisDateFormat
+        if xAxisNumberFormat:
+            self.xAxisProperties['numberFormat'] = xAxisNumberFormat
         if xAxisRangePadding:
            self. xAxisProperties['rangePadding'] = xAxisRangePadding
         if xAxisPlotOffset:
             self.xAxisProperties['plotOffset'] = xAxisPlotOffset
 
         # y axis params
         self.yAxisProperties: dict = {}
@@ -241,14 +250,16 @@
             self.yAxisProperties['opposedPosition'] = yAxisOpposedPosition
         if yAxisLabelRotation:
             self.yAxisProperties['labelRotation'] = yAxisLabelRotation
         if yAxisIsVisible:
             self.yAxisProperties['isVisible'] = yAxisIsVisible
         if yAxisDateFormat:
             self.yAxisProperties['dateFormat'] = yAxisDateFormat
+        if yAxisNumberFormat:
+            self.yAxisProperties['numberFormat'] = yAxisNumberFormat
         if yAxisRangePadding:
             self.yAxisProperties['rangePadding'] = yAxisRangePadding
         if yAxisPlotOffset:
             self.yAxisProperties['plotOffset'] = yAxisPlotOffset
 
         self.colour_map: dict = {
             'g': '#15b01a',
@@ -320,14 +331,20 @@
          self.xAxisProperties['labelRotation'] = xAxisLabelRotation
 
     def set_xAxisIsVisible(self, xAxisIsVisible: bool):
          self.xAxisProperties['isVisible'] = xAxisIsVisible
 
     def set_xAxisDateFormat(self, xAxisDateFormat: str):
          self.xAxisProperties['dateFormat'] = xAxisDateFormat
+    
+    def set_xAxisNumberFormat(self, xAxisNumberFormat: str):
+         self.xAxisProperties['numberFormat'] = xAxisNumberFormat
+
+    def set_xAxisNumberFormat(self, xAxisNumberFormat: str):
+         self.xAxisProperties['numberFormat'] = xAxisNumberFormat
 
     def set_xAxisRangePadding(self, xAxisRangePadding: str):
          self.xAxisProperties['rangePadding'] = xAxisRangePadding
 
     def set_xAxisPlotOffset(self, xAxisPlotOffset: float):
          self.xAxisProperties['plotOffset'] = xAxisPlotOffset
 
@@ -345,14 +362,20 @@
 
     def set_yAxisIsVisible(self, yAxisIsVisible: bool):
          self.yAxisProperties['isVisible'] = yAxisIsVisible
 
     def set_yAxisDateFormat(self, yAxisDateFormat: str):
          self.yAxisProperties['dateFormat'] = yAxisDateFormat
 
+    def set_yAxisNumberFormat(self, yAxisNumberFormat: str):
+         self.yAxisProperties['numberFormat'] = yAxisNumberFormat
+
+    def set_yAxisNumberFormat(self, yAxisNumberFormat: str):
+         self.yAxisProperties['numberFormat'] = yAxisNumberFormat
+
     def set_yAxisRangePadding(self, yAxisRangePadding: str):
          self.yAxisProperties['rangePadding'] = yAxisRangePadding
 
     def set_yAxisPlotOffset(self, yAxisPlotOffset: float):
          self.yAxisProperties['plotOffset'] = yAxisPlotOffset
 
     def set_annotation(self, htmlText: str, x: Optional[Union[int, float, str]] = None, y: Optional[Union[int, float, str]] = None, radius: Optional[str] = None):
@@ -378,28 +401,31 @@
     def get_chartIds(self):
         return [{'type':'chart','id':self.chart_id}]
 
 
     def line(self, x: Union[str, list, np.ndarray, pd.Series], y: Union[str, list, np.ndarray, pd.Series],
              data: Optional[pd.DataFrame] = None, c: Optional[str] = None, ls: str = '-', lw: float = 1.0,
              type: Optional[str]='line', labels: Union[Optional[str], Optional[list]] = None, animationDelay: Optional[float] = None, 
-             animationDuration: Optional[float]=None, animationType: Optional[str]='parallel'):
+             animationDuration: Optional[float]=None, animationType: Optional[str]='parallel'
+             ,sortOrder: Optional[str]= None, sortOn: Optional[str]=None):
         """
         Constructs a line plot.
 
         :param x: A list, NumPy array, Pandas series or a column name from `data` to plot on the X-axis.
         :param y: A list, NumPy array, Pandas series or a column name from `data` to plot on the X-axis.
         :param data: A Pandas data frame whose columns are to be plotted.
         :param c: A string of either hex colour code, a column name from `data`, or one of the following
         ['g', 'green', 'b', 'blue', 'r', 'red', 'c', 'cyan', 'm', 'magenta', 'y', 'yellow', 'k', 'black',
         'w', 'white'] to be used to colour the line(s).
         :param ls: A string specifying line style which can be one of ['-', '--', '.-'].
         :param lw: A float specifying line width.
         :param type: type of line chart possible values are line, area, spline, stepLine, splineArea, stepArea, stackedLine, stackedArea, stackedArea100, stackedLine100
         :param labels: A string or list of strings specifying labels of each line.
+        :param sortOrder: sort order or series. possible values asc/ascending , des/descending
+        :param sortOn: sort on value of x or y. possible values are x/X , y/Y
         :return:
         """
         self.check_input_data_validity(x, y, data)
         self.axes_type = 'line'
         if animationType == 'sequential':
             current_fig_type: str = 'lineRace'
         else:   
@@ -446,14 +472,18 @@
                 'name': line_label,
             }
 
             if animationDelay is not None:
                 line_info['animationDelay'] = animationDelay
             if animationDuration is not None:
                 line_info['animationDuration'] = animationDuration
+            if sortOrder is not None:
+                line_info['sortOrder'] = sortOrder
+            if sortOn is not None:
+                line_info['sortOn'] = sortOn
 
             self.data.insert(line_info)
 
             i += 1
 
     def race(self,x: Union[str, list, np.ndarray, pd.Series], y: Union[str, list, np.ndarray, pd.Series],
              data: Optional[pd.DataFrame] = None, c: Optional[str] = None, ls: str = '-', lw: float = 1.0,
@@ -720,28 +750,30 @@
                 'text': label
             }
         })
 
     def scatter(self, x: Union[str, list, np.ndarray, pd.Series], y: Union[str, list, np.ndarray, pd.Series],
                 data: Optional[pd.DataFrame] = None, c: Optional[str] = None, size: Union[float, list] = 1.0, marker: str = 'o',
                 alpha: float = 1.0, labels: Union[Optional[str], Optional[list]] = None,animationDelay: Optional[float] = None, 
-                animationDuration: Optional[float]=None, animationType: Optional[str]='parallel'):
+                animationDuration: Optional[float]=None, animationType: Optional[str]='parallel', sortOrder: Optional[str]= None, sortOn: Optional[str]=None):
         """
         Constructs a scatter plot.
 
         :param x: A list, NumPy array, Pandas series or a column name from `data` to plot on the X-axis.
         :param y: A list, NumPy array, Pandas series or a column name from `data` to plot on the X-axis.
         :param data: A Pandas data frame whose columns are to be plotted.
         :param c: A string of either hex colour code, a column name from `data`, or one of the following
         ['g', 'green', 'b', 'blue', 'r', 'red', 'c', 'cyan', 'm', 'magenta', 'y', 'yellow', 'k', 'black',
         'w', 'white'] to be used to colour the points.
         :param size: A float specifying the point size. if not specified its 1.0. If list of size specified it will be ploted as bubble chart
         :param marker: A string specifying the point shape which can be one of ['o', '*'].
         :param alpha: A float between 0 and 1 denoting opacity of points.
         :param labels: A string or list of strings specifying labels of each point.
+        :param sortOrder: sort order or series. possible values asc/ascending , des/descending
+        :param sortOn: sort on value of x or y. possible values are x/X , y/Y
         :return:
         """
         self.check_input_data_validity(x, y, data)
         type = 'scatter'
         if isinstance(size, list):
             type = 'bubble'
 
@@ -798,23 +830,28 @@
                 'name': point_label,
             }
 
             if animationDelay is not None:
                 point_info['animationDelay'] = animationDelay
             if animationDuration is not None:
                 point_info['animationDuration'] = animationDuration
+            if sortOrder is not None:
+                point_info['sortOrder'] = sortOrder
+            if sortOn is not None:
+                point_info['sortOn'] = sortOn
 
             self.data.insert(point_info)
 
             i += 1
 
     def bar(self, x: Union[str, list, np.ndarray, pd.Series, pd.Index],
             height: Union[str, list, np.ndarray, pd.Series], data: Optional[pd.DataFrame] = None, c: str = None,
             labels: Optional[list] = None,barType:Optional[str]='vertical', type: Optional[str]='column', animationDelay: Optional[float] = None, 
-             animationDuration: Optional[float] = None, animationType: Optional[str]='parallel', animationRollingWindow: Optional[int] = None):
+             animationDuration: Optional[float] = None, animationType: Optional[str]='parallel', animationRollingWindow: Optional[int] = None,
+             sortOrder: Optional[str]= None, sortOn: Optional[str]=None):
         """
         Constructs a bar chart.
 
         :param x: A list, NumPy array, Pandas series, Pandas index, or column name of `data` to plot bars for.
         :param height: A list, NumPy array, Pandas series, or column name of `data` denoting height of each bar.
         :param data: A Pandas data frame whose columns are to be plotted.
         :param c: A string of either hex colour code, a column name from `data`, or one of the following
@@ -823,14 +860,16 @@
         :param labels: A string or list of strings specifying labels of each bar.
         :param barType: This is legacy parameter just for matplot or plotly friendly terminology users. Use type parameter wherever possible.
         :param type: type of chart allowed values are bar,column,stackedBar,stackedColumn,stackedBar,stackedBar100,stackedColumn100  
         :param animationDelay: wait before starting animation. applicable if animationType == parallel
         :param animationDuration: total time to animate entire series
         :param animationType: parallel or sequential, dapapoints will get printed accordingly.
         :param animationRollingWindow: rolling window for animation, applicable only if animationType == sequential
+        :param sortOrder: sort order or series. possible values asc/ascending , des/descending
+        :param sortOn: sort on value of x or y. possible values are x/X , y/Y
         :return:
         """
         self.check_not_datetime(x[0])
         self.axes_type = 'bar'
         self.check_input_data_validity(x, height, data)
 
         if animationType == 'sequential':
@@ -878,29 +917,37 @@
 
             if animationDelay is not None:
                 bar_info['animationDelay'] = animationDelay
             if animationDuration is not None:
                 bar_info['animationDuration'] = animationDuration
             if animationRollingWindow is not None:
                 bar_info['animationRollingWindow'] = animationRollingWindow
+            if sortOrder is not None:
+                bar_info['sortOrder'] = sortOrder
+            if sortOn is not None:
+                bar_info['sortOn'] = sortOn
 
             self.data.insert(bar_info)
 
             i += 1
 
     def check_not_datetime(self, x: Union[int, float, datetime.datetime,
                                           np.datetime64]):
         if self.get_axis_type(x) in ['datetime', 'np.datetime64']:
             raise TypeError('Pie/Bar chart does not support datetime values.')
 
     def box(self, x: Union[str, list, np.ndarray, pd.Series, pd.Index],
             y: Union[str, list, np.ndarray, pd.Series],
             data: Optional[pd.DataFrame] = None, c: str = None,
             labels: Optional[list] = None, animationDelay: Optional[float] = None, 
-             animationDuration: Optional[float] = None):
+             animationDuration: Optional[float] = None, sortOrder: Optional[str]= None, sortOn: Optional[str]=None):
+        """
+        :param sortOrder: sort order or series. possible values asc/ascending , des/descending
+        :param sortOn: sort on value of x or y. possible values are x/X , y/Y
+        """
         self.check_not_datetime(x[0])
         self.axes_type = 'box'
         self.check_input_data_validity(x, y, data)
         current_fig_type: str = 'boxWhisker'
         if self.check_multi_axes_consistency(current_fig_type):
             self.fig_type = current_fig_type
         self.axes_count += 1
@@ -942,14 +989,18 @@
                 'name': box_label,
             }
 
             if animationDelay is not None:
                 box_info['animationDelay'] = animationDelay
             if animationDuration is not None:
                 box_info['animationDuration']= animationDuration
+            if sortOrder is not None:
+                box_info['sortOrder'] = sortOrder
+            if sortOn is not None:
+                box_info['sortOn'] = sortOn
 
             self.data.insert(box_info)
 
             i += 1
 
     @staticmethod
     def format_data_for_box_plot(x_data: list,
@@ -966,15 +1017,19 @@
 
         return formatted_x_data, formatted_y_data
 
     def hist(self, y: Union[str, list, np.ndarray, pd.Series],
              data: Optional[pd.DataFrame] = None, c: Optional[str] = None,
              binwidth: int = 50, show_normal_curve: bool = False,
              labels: Optional[list] = None, animationDelay: Optional[float] = None, 
-             animationDuration: Optional[float] = None):
+             animationDuration: Optional[float] = None, sortOrder: Optional[str]= None, sortOn: Optional[str]=None):
+        """
+        :param sortOrder: sort order or series. possible values asc/ascending , des/descending
+        :param sortOn: sort on value of x or y. possible values are x/X , y/Y
+        """
         if data is None:
             x: list = [0 for _ in range(len(y))]
         else:
             x: str = 'x'
             data.loc[:, 'x'] = [0 for _ in range(len(data))]
 
         self.check_not_datetime(y[0])
@@ -1019,14 +1074,18 @@
             }
 
             if animationDelay is not None:
                 hist_info['animationDelay'] = animationDelay
             if animationDuration is not None:
                 hist_info['animationDuration'] = animationDuration
 
+            if sortOrder is not None:
+                hist_info['sortOrder'] = sortOrder
+            if sortOn is not None:
+                hist_info['sortOn'] = sortOn
             self.data.insert(hist_info)
 
             i += 1
 
     def pie(self, x: Union[list, np.ndarray, pd.Series], label: Union[list, np.ndarray, pd.Series, pd.Index],
             c: Union[list,str] = None, animationDelay: Optional[float] = None, animationDuration: Optional[float] = None, animationType: Optional[str]='parallel'):
         """
```

### Comparing `chartart-0.0.3.dev16/src/chartart/simple_eda_template.py` & `chartart-0.0.3.dev17/src/chartart/simple_eda_template.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev16/src/chartart/test_plot.py` & `chartart-0.0.3.dev17/src/chartart/test_plot.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev16/src/chartart.egg-info/PKG-INFO` & `chartart-0.0.3.dev17/src/chartart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev16
+Version: 0.0.3.dev17
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
```

