# Comparing `tmp/plotly_resampler-0.9.0rc5.tar.gz` & `tmp/plotly_resampler-0.9.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly_resampler-0.9.0rc5.tar", max compression
+gzip compressed data, was "plotly_resampler-0.9.0rc6.tar", max compression
```

## Comparing `plotly_resampler-0.9.0rc5.tar` & `plotly_resampler-0.9.0rc6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1115 2023-05-04 08:48:30.616798 plotly_resampler-0.9.0rc5/LICENSE
--rw-r--r--   0        0        0    11180 2023-05-14 08:56:23.448441 plotly_resampler-0.9.0rc5/README.md
--rw-r--r--   0        0        0      853 2023-05-30 14:40:07.477729 plotly_resampler-0.9.0rc5/plotly_resampler/__init__.py
--rw-r--r--   0        0        0      796 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/__init__.py
--rw-r--r--   0        0        0     6934 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/aggregation_interface.py
--rw-r--r--   0        0        0    11877 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/aggregators.py
--rw-r--r--   0        0        0     3489 2023-05-30 12:53:12.547957 plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/gap_handler_interface.py
--rw-r--r--   0        0        0     3179 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/gap_handlers.py
--rw-r--r--   0        0        0     9063 2023-05-30 14:16:09.462114 plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/plotly_aggregator_parser.py
--rw-r--r--   0        0        0      473 2022-12-28 21:53:17.053836 plotly_resampler-0.9.0rc5/plotly_resampler/figure_resampler/__init__.py
--rw-r--r--   0        0        0    23690 2023-05-04 08:48:30.660798 plotly_resampler-0.9.0rc5/plotly_resampler/figure_resampler/figure_resampler.py
--rw-r--r--   0        0        0    62492 2023-05-14 08:41:15.136035 plotly_resampler-0.9.0rc5/plotly_resampler/figure_resampler/figure_resampler_interface.py
--rw-r--r--   0        0        0    13669 2023-05-04 08:48:30.660798 plotly_resampler-0.9.0rc5/plotly_resampler/figure_resampler/figurewidget_resampler.py
--rw-r--r--   0        0        0     5376 2023-05-15 07:51:36.039672 plotly_resampler-0.9.0rc5/plotly_resampler/figure_resampler/utils.py
--rw-r--r--   0        0        0     4911 2022-12-28 21:53:17.053836 plotly_resampler-0.9.0rc5/plotly_resampler/registering.py
--rw-r--r--   0        0        0     2857 2023-05-30 14:39:58.165654 plotly_resampler-0.9.0rc5/pyproject.toml
--rw-r--r--   0        0        0    12876 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1115 2023-05-04 08:48:30.616798 plotly_resampler-0.9.0rc6/LICENSE
+-rw-r--r--   0        0        0    11180 2023-05-14 08:56:23.448441 plotly_resampler-0.9.0rc6/README.md
+-rw-r--r--   0        0        0      853 2023-06-14 07:46:24.712021 plotly_resampler-0.9.0rc6/plotly_resampler/__init__.py
+-rw-r--r--   0        0        0      796 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/__init__.py
+-rw-r--r--   0        0        0     6934 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/aggregation_interface.py
+-rw-r--r--   0        0        0    11877 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/aggregators.py
+-rw-r--r--   0        0        0     3489 2023-05-30 12:53:12.547957 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/gap_handler_interface.py
+-rw-r--r--   0        0        0     3179 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/gap_handlers.py
+-rw-r--r--   0        0        0     9063 2023-05-30 14:16:09.462114 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/plotly_aggregator_parser.py
+-rw-r--r--   0        0        0      473 2022-12-28 21:53:17.053836 plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/__init__.py
+-rw-r--r--   0        0        0    23690 2023-05-04 08:48:30.660798 plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figure_resampler.py
+-rw-r--r--   0        0        0    63030 2023-06-14 07:27:57.588994 plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figure_resampler_interface.py
+-rw-r--r--   0        0        0    13669 2023-05-04 08:48:30.660798 plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figurewidget_resampler.py
+-rw-r--r--   0        0        0     5376 2023-05-15 07:51:36.039672 plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/utils.py
+-rw-r--r--   0        0        0     4911 2022-12-28 21:53:17.053836 plotly_resampler-0.9.0rc6/plotly_resampler/registering.py
+-rw-r--r--   0        0        0     2857 2023-06-14 07:46:36.788373 plotly_resampler-0.9.0rc6/pyproject.toml
+-rw-r--r--   0        0        0    12876 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc6/PKG-INFO
```

### Comparing `plotly_resampler-0.9.0rc5/LICENSE` & `plotly_resampler-0.9.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/README.md` & `plotly_resampler-0.9.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/__init__.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .aggregation import LTTB, EveryNthPoint, MinMaxLTTB
 from .figure_resampler import FigureResampler, FigureWidgetResampler
 from .registering import register_plotly_resampler, unregister_plotly_resampler
 
 __docformat__ = "numpy"
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
-__version__ = "0.9.0rc5"
+__version__ = "0.9.0rc6"
 
 __all__ = [
     "__version__",
     "FigureResampler",
     "FigureWidgetResampler",
     "MinMaxLTTB",
     "LTTB",
```

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/__init__.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/aggregation_interface.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/aggregation_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/aggregators.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/aggregators.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/gap_handler_interface.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/gap_handler_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/gap_handlers.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/gap_handlers.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/aggregation/plotly_aggregator_parser.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/plotly_aggregator_parser.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/figure_resampler/figure_resampler.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figure_resampler.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/figure_resampler/figure_resampler_interface.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figure_resampler_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -668,31 +668,39 @@
             # When the x or y of a trace has more than 1 dimension, it is not at all
             # straightforward how it should be resampled.
             assert hf_y.ndim <= 1 and np.ndim(hf_x) <= 1, (
                 "plotly-resampler requires scatter data "
                 "(i.e., x and y, or hf_x and hf_y) to be <= 1 dimensional!"
             )
 
-            # Note: this also converts hf_text and hf_hovertext to a np.ndarray
-            if isinstance(hf_text, (list, np.ndarray, pd.Series)):
+            # Note: this converts the hf property to a np.ndarray
+            if isinstance(hf_text, (tuple, list, np.ndarray, pd.Series)):
                 hf_text = np.asarray(hf_text)
-            if isinstance(hf_hovertext, (list, np.ndarray, pd.Series)):
+            if isinstance(hf_hovertext, (tuple, list, np.ndarray, pd.Series)):
                 hf_hovertext = np.asarray(hf_hovertext)
+            if isinstance(hf_marker_size, (tuple, list, np.ndarray, pd.Series)):
+                hf_marker_size = np.asarray(hf_marker_size)
+            if isinstance(hf_marker_color, (tuple, list, np.ndarray, pd.Series)):
+                hf_marker_color = np.asarray(hf_marker_color)
 
             # Remove NaNs for efficiency (storing less meaningless data)
             # NaNs introduce gaps between enclosing non-NaN data points & might distort
             # the resampling algorithms
             if check_nans and pd.isna(hf_y).any():
                 not_nan_mask = ~pd.isna(hf_y)
                 hf_x = hf_x[not_nan_mask]
                 hf_y = hf_y[not_nan_mask]
                 if isinstance(hf_text, np.ndarray):
                     hf_text = hf_text[not_nan_mask]
                 if isinstance(hf_hovertext, np.ndarray):
                     hf_hovertext = hf_hovertext[not_nan_mask]
+                if isinstance(hf_marker_size, np.ndarray):
+                    hf_marker_size = hf_marker_size[not_nan_mask]
+                if isinstance(hf_marker_color, np.ndarray):
+                    hf_marker_color = hf_marker_color[not_nan_mask]
 
             # Try to parse the hf_x data if it is of object type or
             if len(hf_x) and (hf_x.dtype.type is np.str_ or hf_x.dtype == "object"):
                 try:
                     # Try to parse to numeric
                     hf_x = pd.to_numeric(hf_x, errors="raise")
                 except (ValueError, TypeError):
```

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/figure_resampler/figurewidget_resampler.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figurewidget_resampler.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/figure_resampler/utils.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/utils.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/plotly_resampler/registering.py` & `plotly_resampler-0.9.0rc6/plotly_resampler/registering.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc5/pyproject.toml` & `plotly_resampler-0.9.0rc6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plotly-resampler"  # Do not forget to update the __init__.py __version__ variable
-version = "0.9.0rc5"
+version = "0.9.0rc6"
 description = "Visualizing large time series with plotly"
 authors = ["Jonas Van Der Donckt", "Jeroen Van Der Donckt", "Emiel Deprost"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/predict-idlab/plotly-resampler"
 documentation = "https://predict-idlab.github.io/plotly-resampler"
 keywords = ["time-series", "visualization", "resampling", "plotly", "plotly-dash"]
```

### Comparing `plotly_resampler-0.9.0rc5/PKG-INFO` & `plotly_resampler-0.9.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotly-resampler
-Version: 0.9.0rc5
+Version: 0.9.0rc6
 Summary: Visualizing large time series with plotly
 Home-page: https://github.com/predict-idlab/plotly-resampler
 License: MIT
 Keywords: time-series,visualization,resampling,plotly,plotly-dash
 Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc5 Summary:
+Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc6 Summary:
 Visualizing large time series with plotly Home-page: https://github.com/
 predict-idlab/plotly-resampler License: MIT Keywords: time-
 series,visualization,resampling,plotly,plotly-dash Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
```

