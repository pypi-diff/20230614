# Comparing `tmp/cmo_dataviz-0.0.1.tar.gz` & `tmp/cmo_dataviz-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmo_dataviz-0.0.1.tar", last modified: Tue Apr 25 10:19:32 2023, max compression
+gzip compressed data, was "cmo_dataviz-0.1.0.tar", last modified: Wed Jun 14 07:51:57 2023, max compression
```

## Comparing `cmo_dataviz-0.0.1.tar` & `cmo_dataviz-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 10:19:32.699469 cmo_dataviz-0.0.1/
--rw-rw-rw-   0        0        0     2985 2023-04-25 10:19:32.696980 cmo_dataviz-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2023-04-25 08:31:41.000000 cmo_dataviz-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 10:19:32.625808 cmo_dataviz-0.0.1/cmo_dataviz/
--rw-rw-rw-   0        0        0       22 2023-04-24 09:23:29.000000 cmo_dataviz-0.0.1/cmo_dataviz/__init__.py
--rw-rw-rw-   0        0        0    17691 2023-04-25 10:10:30.000000 cmo_dataviz-0.0.1/cmo_dataviz/dataviz.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:19:32.691092 cmo_dataviz-0.0.1/cmo_dataviz/notebooks/
--rw-rw-rw-   0        0        0   104198 2023-04-25 08:27:02.000000 cmo_dataviz-0.0.1/cmo_dataviz/notebooks/Cmotions Dataviz tutorial.ipynb
--rw-rw-rw-   0        0        0     1354 2023-04-25 08:28:40.000000 cmo_dataviz-0.0.1/cmo_dataviz/resources.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:19:32.686687 cmo_dataviz-0.0.1/cmo_dataviz.egg-info/
--rw-rw-rw-   0        0        0     2985 2023-04-25 10:19:32.000000 cmo_dataviz-0.0.1/cmo_dataviz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-25 10:19:32.000000 cmo_dataviz-0.0.1/cmo_dataviz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 10:19:32.000000 cmo_dataviz-0.0.1/cmo_dataviz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2023-04-25 10:19:32.000000 cmo_dataviz-0.0.1/cmo_dataviz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-25 10:19:32.000000 cmo_dataviz-0.0.1/cmo_dataviz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 10:19:32.699469 cmo_dataviz-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1293 2023-04-25 08:41:26.000000 cmo_dataviz-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:19:32.694333 cmo_dataviz-0.0.1/tests/
--rw-rw-rw-   0        0        0     2874 2023-04-25 10:10:59.000000 cmo_dataviz-0.0.1/tests/test_dataviz.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:51:57.659214 cmo_dataviz-0.1.0/
+-rw-rw-rw-   0        0        0     2985 2023-06-14 07:51:57.657195 cmo_dataviz-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2023-04-25 10:48:58.000000 cmo_dataviz-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 07:51:57.602691 cmo_dataviz-0.1.0/cmo_dataviz/
+-rw-rw-rw-   0        0        0       22 2023-04-24 09:23:29.000000 cmo_dataviz-0.1.0/cmo_dataviz/__init__.py
+-rw-rw-rw-   0        0        0    25658 2023-06-14 07:22:39.000000 cmo_dataviz-0.1.0/cmo_dataviz/dataviz.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:51:57.653051 cmo_dataviz-0.1.0/cmo_dataviz/notebooks/
+-rw-rw-rw-   0        0        0    94012 2023-06-12 13:01:16.000000 cmo_dataviz-0.1.0/cmo_dataviz/notebooks/Cmotions Dataviz tutorial.ipynb
+-rw-rw-rw-   0        0        0     1354 2023-04-25 10:48:58.000000 cmo_dataviz-0.1.0/cmo_dataviz/resources.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:51:57.650694 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/
+-rw-rw-rw-   0        0        0     2985 2023-06-14 07:51:57.000000 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-06-14 07:51:57.000000 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 07:51:57.000000 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2023-06-14 07:51:57.000000 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-14 07:51:57.000000 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 07:51:57.659214 cmo_dataviz-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1293 2023-06-14 07:24:42.000000 cmo_dataviz-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:51:57.655061 cmo_dataviz-0.1.0/tests/
+-rw-rw-rw-   0        0        0     4075 2023-06-14 06:50:17.000000 cmo_dataviz-0.1.0/tests/test_dataviz.py
```

### Comparing `cmo_dataviz-0.0.1/PKG-INFO` & `cmo_dataviz-0.1.0/cmo_dataviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cmo_dataviz
-Version: 0.0.1
+Name: cmo-dataviz
+Version: 0.1.0
 Summary: Easily create graphs using custom styling
 Home-page: https://Cmotions@dev.azure.com/Cmotions/Packages/_git/cmo_dataviz
 Author: Jeanine Schoonemann
 Author-email: service@cmotions.nl
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `cmo_dataviz-0.0.1/README.md` & `cmo_dataviz-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cmo_dataviz-0.0.1/cmo_dataviz/dataviz.py` & `cmo_dataviz-0.1.0/cmo_dataviz/dataviz.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,126 @@
 import warnings
 import matplotlib.pyplot as plt
-import networkx as nx
 import numpy as np
 import seaborn as sns
 from pandas.api.types import is_numeric_dtype
+import pandas as pd
 
 
 def import_style(filepath: str) -> None:
     """
     This function imports a style file for matplotlib plots.
 
     Args:
       filepath (str):   A string representing the file path of the style sheet to be imported. The style
                         sheet should be in the correct format for matplotlib to use.
     """
     plt.style.use(filepath)
 
 
 def create_horizontal_barplot(
-    data, x_var, y_var, x_label="", title="", ax=None
+    data,
+    x_var,
+    y_var,
+    x_label="",
+    title="",
+    titlefontsize=12,
+    figsize=(10, 10),
+    ax=None,
 ) -> plt.Axes:
     """
-    This function creates a horizontal bar plot using the input data and variables, with options for
-    customizing the x-axis label and plot title.
-
+    This function creates a horizontal bar plot using the input data and variables.
+    
     Args:
-      data:     The dataset containing the variables to be plotted.
-      x_var:    The variable to be plotted on the x-axis of the horizontal barplot.
-      y_var:    The variable used for the y-axis of the horizontal barplot.
-      x_label:  The label for the x-axis of the horizontal barplot.
-      title:    The title of the horizontal barplot.
-      ax:       The ax parameter is an optional parameter that allows the user to specify a specific subplot
-                to plot the horizontal barplot on. If ax is not specified, the function will create a new subplot.
-
+      data: The data to be plotted, in the form of a pandas DataFrame or a dictionary.
+      x_var: The variable to be plotted on the x-axis.
+      y_var: The variable used for the y-axis of the horizontal barplot.
+      x_label: The label for the x-axis of the horizontal barplot.
+      title: The title of the horizontal bar plot.
+      titlefontsize: The font size of the title of the horizontal bar plot. Defaults to 12
+      figsize: The size of the figure in inches (width, height).
+      ax: The ax parameter is an optional parameter that allows the user to pass in an existing
+    matplotlib Axes object to plot on. If this parameter is not provided, the function will create a new
+    figure and Axes object to plot on.
+    
     Returns:
-      a matplotlib axis object.
+      a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if ax is None:
-            fig = plt.figure(figsize=(10, 10))
+            fig = plt.figure(figsize=figsize)
             ax = fig.add_subplot(111)
         y_pos = np.arange(len(data[y_var]))
         _ = ax.barh(y_pos, data[x_var], align="center")
         ax.set_yticks(y_pos)
         ax.set_yticklabels(data[y_var])
         ax.invert_yaxis()
         ax.set_xlabel(x_label)
-        ax.set_title(title)
+        ax.set_title(title, fontsize=titlefontsize)
         return ax
 
 
-def create_scatterplot(data, x_var, y_var, title="", ax=None) -> plt.Axes:
+def create_scatterplot(data, x_var, y_var, title="", titlefontsize=12, figsize=(10, 10), ax=None) -> plt.Axes:
     """
-    This function creates a scatterplot with specified data, x and y variables, and title.
-
-    Args:
-      data:     The dataset containing the variables to be plotted.
-      x_var:    The variable to be plotted on the x-axis of the scatterplot.
-      y_var:    The variable to be plotted on the y-axis of the scatterplot.
-      title:    The title of the scatterplot (optional)
-      ax:       The ax parameter is an optional parameter that allows the user to specify a specific subplot
-                to plot the scatterplot on. If ax is not specified, a new subplot will be created.
-
+    This function creates a scatterplot with specified data, x and y variables, title, and axis
+    parameters.
+    
+    Args:
+      data: The dataset that contains the variables to be plotted.
+      x_var: The name of the variable to be plotted on the x-axis of the scatterplot.
+      y_var: The variable to be plotted on the y-axis of the scatterplot.
+      title: The title of the scatterplot (default is an empty string).
+      titlefontsize: The font size of the title of the scatterplot. Defaults to 12
+      figsize: The size of the figure in inches (width, height).
+      ax: The ax parameter is an optional parameter that allows the user to specify an existing
+    matplotlib Axes object to plot the scatterplot on. If ax is not provided, a new figure and Axes
+    object will be created.
+    
     Returns:
       a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if ax is None:
-            fig = plt.figure(figsize=(10, 10))
+            fig = plt.figure(figsize=figsize)
             ax = fig.add_subplot(111)
         ax.scatter(data[x_var], data[y_var])
         ax.set_xlabel(x_var)
         ax.set_ylabel(y_var)
-        ax.set_title(title)
+        ax.set_title(title, fontsize=titlefontsize)
         return ax
 
 
 def create_heatmap(
     data,
     complete=True,
+    title="",
+    titlefontsize=12,
     figsize=(10, 10),
-    figtitle="",
     ax=None,
 ) -> plt.Axes:
     """
-    This function creates a heatmap with customizable options and the ability to save the figure.
-
+    This function creates a heatmap with customizable options using the Seaborn library in Python.
+    
     Args:
-      data:         The data to be plotted in the heatmap. It should be a 2D array or a pandas DataFrame.
-      complete:     A boolean parameter that determines whether to show the complete heatmap or only the
-                    bottom half of it. If set to True, the complete heatmap will be shown. If set to False, only the
-                    bottom half of the heatmap will be shown. Defaults to True
-      figsize:      The size of the figure in inches (width, height).
-      figtitle:     The title of the heatmap figure.
-      ax:           The matplotlib Axes object to plot the heatmap on. If it is not provided, a new figure and
-                    Axes object will be created.
-
+      data: The data to be plotted in the heatmap. It should be a 2D array or a pandas DataFrame.
+      complete: A boolean parameter that determines whether to show the complete heatmap or only the
+    bottom half of it. If set to True, the complete heatmap will be shown. If set to False, only the
+    bottom half of the heatmap will be shown. Defaults to True
+      title: The title of the heatmap plot.
+      titlefontsize: The font size of the title of the heatmap. Defaults to 12
+      figsize: The size of the figure (width, height) in inches.
+      ax: The matplotlib Axes object to plot the heatmap on. If None, a new figure and Axes object will
+    be created.
+    
     Returns:
-      the axis object (ax) of the heatmap plot.
+      a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if complete:
             mask = None
         else:
@@ -125,15 +140,15 @@
             yticklabels=1,
             center=0,
             square=True,
             linewidths=0.5,
             cbar_kws={"shrink": 0.5},
             cmap="coolwarm",
         )
-        ax.set_title(figtitle, fontsize=12, y=1.0)
+        ax.set_title(title, fontsize=titlefontsize, y=1.0)
         return ax
 
 
 def make_barplot_labels(ax, rects) -> None:
     """
     The function adds labels to a barplot with the height of each bar.
 
@@ -194,15 +209,22 @@
     ax.text(xlabel, captop, "top cap: {:6.3g}".format(captop), va="center")
     # Many fliers, so we loop over them and create a label for each one
     for flier in fly.get_ydata():
         ax.text(1 + xoff, flier, "{:6.3g}".format(flier), va="center")
 
 
 def create_boxplot(
-    data, x_var, y_var=None, color_by=None, ax=None, title=""
+    data,
+    x_var,
+    y_var=None,
+    color_by=None,
+    title="",
+    titlefontsize=12,
+    figsize=(10, 10),
+    ax=None,
 ) -> plt.Axes:
     """
     This function creates a boxplot using seaborn library with optional parameters for color and title.
 
     Args:
       data:     The dataset to be used for creating the boxplot.
       x_var:    The variable to be plotted on the x-axis of the boxplot.
@@ -218,85 +240,110 @@
     Returns:
       the axis object (ax) after creating a boxplot using the input data and parameters.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if ax is None:
-            fig = plt.figure(figsize=(10, 10))
+            fig = plt.figure(figsize=figsize)
             ax = fig.add_subplot(111)
         sns.boxplot(x=x_var, y=y_var, hue=color_by, data=data, ax=ax)
-        ax.set_title(title)
+        ax.set_title(title, fontsize=titlefontsize)
     return ax
 
 
-def create_swarmplot(data, x_var, y_var=None, color_by=None, ax=None) -> plt.Axes:
+def create_swarmplot(
+    data,
+    x_var,
+    y_var=None,
+    color_by=None,
+    title="",
+    titlefontsize=12,
+    figsize=(10, 10),
+    ax=None,
+) -> plt.Axes:
     """
-    This function creates a swarmplot using the Seaborn library in Python, with options to customize the
-    plot's variables and appearance.
-
+    This function creates a swarmplot using seaborn library with customizable parameters.
+    
     Args:
-      data:     The dataset that contains the variables to be plotted.
-      x_var:    The variable to be plotted on the x-axis.
-      y_var:    The variable to be plotted on the y-axis. It is optional and can be set to None if only the
-                x-axis variable is to be plotted.
-      color_by: The variable used to color the points in the swarmplot.
-      ax:       The ax parameter is an optional parameter that specifies the matplotlib Axes object on which
-                the swarmplot will be drawn. If it is not provided, a new figure and Axes object will be created.
-
+      data: The dataset that contains the variables to be plotted.
+      x_var: The variable to be plotted on the x-axis of the swarmplot.
+      y_var: The variable to be plotted on the y-axis. It is optional and can be left as None if only
+    the x-axis variable is to be plotted.
+      color_by: The variable used to color the points in the swarmplot. If not specified, all points
+    will have the same color.
+      title: The title of the plot.
+      titlefontsize: The font size of the title of the plot. Defaults to 12
+      figsize: The size of the figure in inches (width, height).
+      ax: The ax parameter is an optional parameter that allows the user to specify the matplotlib Axes
+    object on which the swarmplot will be drawn. If ax is not provided, a new figure and Axes object
+    will be created.
+    
     Returns:
       a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if ax is None:
-            fig = plt.figure(figsize=(10, 10))
+            fig = plt.figure(figsize=figsize)
             ax = fig.add_subplot(111)
         with warnings.catch_warnings(record=True):
             sns.swarmplot(
                 x=x_var,
                 y=y_var,
                 hue=color_by,
                 dodge=True,
                 data=data,
                 alpha=0.8,
                 s=4,
                 ax=ax,
             )
+        ax.set_title(title, fontsize=titlefontsize)
     return ax
 
 
 def create_histogram(
-    data, var, color_by=None, bins=10, max_categories=50, ax=None, title=""
+    data,
+    var,
+    color_by=None,
+    bins=10,
+    max_categories=50,
+    title="",
+    titlefontsize=12,
+    figsize=(10, 10),
+    ax=None,
 ) -> plt.Axes:
     """
-    This function creates a histogram plot for a given variable in a dataset, with the option to color
-    by another variable.
-
-    Args:
-      data:             The dataset that contains the variable(s) to be plotted.
-      var:              The variable/column in the dataset that we want to create a histogram for.
-      color_by:         A variable to group the data by and display different colors for each group in the
-                        histogram.
-      bins:             The number of bins to use for the histogram. Defaults to 10
-      max_categories:   The maximum number of categories allowed in a categorical variable before it is
-                        replaced with an "OTHER" category. Defaults to 50
-      ax:               The matplotlib axis object to plot the histogram on.
-                        If it is None, a new figure and axis will be created.
-      title:            The title of the histogram plot.
-
+    The function creates a histogram plot of a given variable in a dataset, with options for
+    color-coding and binning.
+    
+    Args:
+      data: The input data for creating the histogram.
+      var: The variable/column name from the input data that will be used to create the histogram.
+      color_by: The variable to use for coloring the histogram bars or stacking them. If None or the
+    same as the variable being plotted, the bars will not be colored or stacked.
+      bins: The number of bins to use for the histogram. Defaults to 10
+      max_categories: The maximum number of categories allowed in the histogram. If the number of
+    categories exceeds this value, an option to replace the longtail into "OTHER" is created. Defaults
+    to 50
+      title: The title of the histogram plot.
+      titlefontsize: The font size of the title of the histogram. Defaults to 12
+      figsize: The size of the figure in inches (width, height).
+      ax: The matplotlib Axes object to plot the histogram on. If None, a new figure and Axes object
+    will be created.
+    
     Returns:
-      a matplotlib axis object.
+      a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if ax is None:
-            fig = plt.figure(figsize=(10, 10))
+            fig = plt.figure(figsize=figsize)
             ax = fig.add_subplot(111)
 
         if is_numeric_dtype(data[var]):
             if (color_by is None) | (color_by == var):
                 plotdata = data[var]
                 stacked = False
             else:
@@ -338,79 +385,94 @@
                             height=plotdata[col],
                             bottom=barheight,
                         )
                     barheight.add(plotdata[col], fill_value=0)
                 highest_value = plotdata.sum(axis=1).max()
             ax.set_ylim([None, highest_value * 1.25])
             ax.tick_params(axis="x", labelrotation=45)
-        ax.set_title(title)
+        ax.set_title(title, fontsize=titlefontsize)
         return ax
 
 
-def create_confusion_matrix_heatmap(conf_matrix, model_accuracy=None, figsize=(9, 9), ax=None) -> plt.Axes:
+def create_confusion_matrix_heatmap(
+    conf_matrix, model_accuracy=None, figsize=(10, 10), ax=None
+) -> plt.Axes:
     """
     This function creates a heatmap of a confusion matrix with optional model accuracy score.
-
+    
     Args:
-      conf_matrix:      The confusion matrix to be visualized as a heatmap.
-      model_accuracy:   The accuracy score of a machine learning model, expressed as a percentage.
-                        If not None, this value will be shown in the title of the heatmap
+      conf_matrix: The confusion matrix to be visualized as a heatmap.
+      model_accuracy: The accuracy score of the model, expressed as a percentage. It is an optional
+    parameter that can be used to add a title to the heatmap.
+      figsize: The size of the figure in inches (width, height).
+      ax: An optional parameter that specifies the matplotlib Axes object to plot the heatmap on. If not
+    provided, a new figure and Axes object will be created.
+    
+    Returns:
+      a matplotlib Axes object.
     """
     if ax is None:
-        fig, ax = plt.subplots(figsize=figsize)
+        fig = plt.figure(figsize=figsize)
+        ax = fig.add_subplot(111)
     sns.heatmap(
         conf_matrix,
         annot=True,
         fmt=".0f",
         linewidths=0.5,
         square=True,
         cmap="Blues_r",
-        ax=ax
+        ax=ax,
     )
     plt.ylabel("Actual label")
     plt.xlabel("Predicted label")
     if model_accuracy is not None:
         all_sample_title = "Accuracy Score: {0} %".format(
             round(model_accuracy * 100, 2)
         )
         plt.title(all_sample_title, size=15)
     return ax
 
 
-def create_tableplot(data, colLabels=None, figsize=(9, 9), ax=None) -> plt.Axes:
+def create_tableplot(data, colLabels=None, figsize=(10, 10), ax=None) -> plt.Axes:
     """
-    The function creates a table plot with column labels and returns the plot object.
-
+    The function creates a table plot using the given data and column labels.
+    
     Args:
-      ax:           The matplotlib axis object on which the tableplot will be created.
-      data:         a pandas DataFrame containing the data to be displayed in the tableplot
-      colLabels:    A list of column labels for the tableplot. If not provided, the column labels will be
-                    taken from the column names of the input data.
-
+      data: a pandas DataFrame containing the data to be plotted in the table
+      colLabels: A list of column labels for the tableplot. If not provided, the column labels will be
+    the column names of the input data.
+      figsize: The size of the figure in inches (width, height).
+      ax: An optional parameter that specifies the matplotlib Axes object to plot the table on. If it is
+    not provided, a new figure and Axes object will be created.
+    
     Returns:
-      a tableplot object.
+      a matplotlib Axes object.
     """
     if ax is None:
-        fig, ax = plt.subplots(figsize=figsize)
+        fig = plt.figure(figsize=figsize)
+        ax = fig.add_subplot(111)
     if colLabels is None:
         colLabels = data.columns
     tableplot = ax.table(cellText=data.values, colLabels=colLabels, loc="center")
     tableplot.scale(1, 2)
     ax.axis("off")
     return ax
 
 
 def create_single_tableplot(data, colLabels=None):
     """
     The function creates a table plot with given data and column labels.
-
+    
     Args:
-      data:         a pandas DataFrame containing the data to be plotted in a table format
-      colLabels:    A list of column labels for the table. If not provided, the column labels will be the
-                    column names of the input data.
+      data: a pandas DataFrame containing the data to be plotted in a table format
+      colLabels: A list of column labels for the table. If not provided, the column labels will be the
+    column names of the input data.
+    
+    Returns:
+      a matplotlib figure object.
     """
     if colLabels is None:
         colLabels = data.columns
     if len(data) + 1 > len(colLabels):
         nrows, ncols = len(data) + 1, len(colLabels)
     else:
         ncols, nrows = len(data) + 1, len(colLabels)
@@ -419,24 +481,25 @@
     ax.axis("off")
     tableplot = ax.table(cellText=data.values, colLabels=colLabels, loc="center")
     tableplot.set_fontsize(14)
     tableplot.scale(2, 2)
     return fig
 
 
-def create_pairplot(
-    data, figtitle=""
-):
+def create_pairplot(data, figtitle=""):
     """
-    The function creates a pairplot using seaborn library
-
+    This function creates a pairplot using seaborn library with customized settings and a given title.
+    
     Args:
-      data:     The data to be plotted in the pairplot.
-      figsize:  The size of the figure in inches (width, height).
-      figtitle: The title of the figure
+      data: The data to be plotted in the pairplot.
+      figtitle: The title of the figure. It is an optional parameter and if not provided, the figure
+    will not have a title.
+    
+    Returns:
+      a matplotlib figure object.
     """
     with plt.rc_context(
         {
             "axes.labelcolor": "black",
             "ytick.labelleft": True,
             "xtick.labelbottom": True,
             "axes.linewidth": 1.0,
@@ -448,7 +511,171 @@
             plot_kws=dict(color="#003D7C"),
             diag_kws={"color": "#003D7C"},
         )
         fig = fig_pairplot.fig
         fig.suptitle(figtitle, fontsize=12, y=1.0)
         return fig
 
+
+def create_barplot(
+    data,
+    x_var,
+    y_var,
+    add_value_labels=True,
+    x_label="",
+    title="",
+    figsize=(10, 10),
+    ax=None,
+) -> plt.Axes:
+    """
+    The function creates a bar plot with optional value labels and customizable labels and title.
+    
+    Args:
+      data: The data to be plotted in the barplot.
+      x_var: The variable to be plotted on the x-axis of the barplot.
+      y_var: The variable used for the height of the bars in the barplot.
+      add_value_labels: A boolean parameter that determines whether or not to add labels to the top of
+    each bar in the barplot indicating the height of the bar. Defaults to True
+      x_label: The label for the x-axis of the barplot.
+      title: The title of the barplot.
+      figsize: The size of the figure (width, height) in inches.
+      ax: The ax parameter is an optional parameter that allows the user to pass in an existing
+    matplotlib Axes object to plot on. If this parameter is not provided, a new figure and Axes object
+    will be created.
+    
+    Returns:
+      a matplotlib Axes object.
+    """
+    with plt.rc_context(
+        {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
+    ):
+        if ax is None:
+            fig = plt.figure(figsize=figsize)
+            ax = fig.add_subplot(111)
+        barplot = ax.bar(x=data[x_var], height=data[y_var], align="center")
+        _ = ax.set_xlabel(x_label)
+        _ = ax.set_xticks(
+            ax.get_xticks(), ax.get_xticklabels(), rotation=45, ha="right"
+        )
+        _ = ax.set_title(title)
+        if add_value_labels:
+            for p in barplot:
+                height = p.get_height()
+                ax.annotate(
+                    "{}".format(height),
+                    xy=(p.get_x() + p.get_width() / 2, height),
+                    xytext=(0, 3),  # 3 points vertical offset
+                    textcoords="offset points",
+                    ha="center",
+                    va="bottom",
+                )
+        return ax
+
+
+def create_stacked_barplot(
+    data, x_var, y_var, color_by, x_label="", title="", figsize=(10, 10), ax=None
+) -> plt.Axes:
+    """
+    This function creates a stacked barplot with multiple categories and colors based on a given
+    dataset.
+    
+    Args:
+      data: The input data for the plot.
+      x_var: The variable to be plotted on the x-axis.
+      y_var: The variable to be plotted on the y-axis of the stacked barplot.
+      color_by: The variable used to determine the color of the bars in the stacked barplot.
+      x_label: The label for the x-axis of the plot.
+      title: The title of the stacked barplot.
+      figsize: The size of the figure (width, height) in inches.
+      ax: The ax parameter is an optional parameter that allows the user to specify the matplotlib Axes
+    object on which to draw the plot. If it is not specified, a new Axes object will be created.
+    
+    Returns:
+      a matplotlib Axes object.
+    """
+    categories = data[color_by].unique()
+    init_data = pd.DataFrame(data[x_var].unique(), columns=[x_var]).sort_values(
+        by=x_var
+    )
+    init_data[y_var] = 0
+    bottom = np.zeros(init_data.shape[0])
+
+    with plt.rc_context(
+        {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
+    ):
+        if ax is None:
+            fig = plt.figure(figsize=figsize)
+            ax = fig.add_subplot(111)
+
+        _ = ax.bar(
+            x=init_data[x_var],
+            height=init_data[y_var],
+            bottom=bottom,
+            label=None,
+            align="center",
+        )
+
+        for cat in categories:
+            data_cat = (
+                init_data[[x_var]]
+                .merge(data[data[color_by] == cat], on=x_var, how="left")
+                .fillna(0)
+            )
+            _ = ax.bar(
+                x=data_cat[x_var],
+                height=data_cat[y_var],
+                label=cat,
+                bottom=bottom,
+                align="center",
+            )
+            bottom += data_cat[y_var]
+        _ = ax.set_xlabel(x_label)
+        _ = ax.set_xticks(
+            ax.get_xticks(), ax.get_xticklabels(), rotation=45, ha="right"
+        )
+        _ = ax.set_title(title)
+        _ = ax.legend(loc="upper right", ncol=len(categories))
+        return ax
+
+
+def create_lineplot(
+    data, x_var, y_var, color_by=None, x_label="", title="", figsize=(10, 10), ax=None
+) -> plt.Axes:
+    """
+    This function creates a line plot with optional color grouping based on a specified data set and
+    variables.
+    
+    Args:
+      data: The data to be plotted in the line plot.
+      x_var: The variable to be plotted on the x-axis of the line plot.
+      y_var: The variable to be plotted on the y-axis of the line plot.
+      color_by: The variable used to color the lines in the line plot. If this parameter is not
+    specified, all lines will have the same color.
+      x_label: The label for the x-axis of the line plot.
+      title: The title of the line plot.
+      figsize: The size of the figure in inches (width, height).
+      ax: The ax parameter is an optional parameter that allows the user to pass in an existing
+    matplotlib Axes object to plot the lineplot on. If ax is not provided, a new figure and Axes object
+    will be created.
+    
+    Returns:
+      a matplotlib Axes object.
+    """
+    categories = data[color_by].unique()
+
+    with plt.rc_context(
+        {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
+    ):
+        if ax is None:
+            fig = plt.figure(figsize=figsize)
+            ax = fig.add_subplot(111)
+
+        for cat in categories:
+            data_cat = data[data[color_by] == cat].sort_values(x_var)
+            _ = ax.plot(data_cat[x_var], data_cat[y_var], label=cat, linewidth=1)
+        _ = ax.set_xlabel(x_label)
+        _ = ax.set_xticks(
+            ax.get_xticks(), ax.get_xticklabels(), rotation=45, ha="right"
+        )
+        _ = ax.set_title(title)
+        _ = ax.legend(loc="upper right", ncol=len(categories))
+        return ax
```

### Comparing `cmo_dataviz-0.0.1/cmo_dataviz/resources.py` & `cmo_dataviz-0.1.0/cmo_dataviz/resources.py`

 * *Files identical despite different names*

### Comparing `cmo_dataviz-0.0.1/cmo_dataviz.egg-info/PKG-INFO` & `cmo_dataviz-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cmo-dataviz
-Version: 0.0.1
+Name: cmo_dataviz
+Version: 0.1.0
 Summary: Easily create graphs using custom styling
 Home-page: https://Cmotions@dev.azure.com/Cmotions/Packages/_git/cmo_dataviz
 Author: Jeanine Schoonemann
 Author-email: service@cmotions.nl
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `cmo_dataviz-0.0.1/setup.py` & `cmo_dataviz-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="cmo_dataviz",
-    version="0.0.1",
+    version="0.1.0",
     python_requires='>=3.6',
     description='Easily create graphs using custom styling',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jeanine Schoonemann',
     author_email='service@cmotions.nl',
     url='https://Cmotions@dev.azure.com/Cmotions/Packages/_git/cmo_dataviz',
```

### Comparing `cmo_dataviz-0.0.1/tests/test_dataviz.py` & `cmo_dataviz-0.1.0/tests/test_dataviz.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,80 +48,125 @@
 @pytest.mark.mpl_image_compare
 def test_create_heatmap():
     fig, ax = plt.subplots()
     dv.create_heatmap(
         data=df.select_dtypes(include=np.number).corr(),
         complete=True,
         figsize=(10, 10),
-        figtitle="",
+        title="",
         ax=ax,
     )
     return fig
 
 
 # make_barplot_labels()
 
 # make_boxplot_labels()
 
 
 @pytest.mark.mpl_image_compare
 def test_create_boxplot():
-    fig, ax = plt.subplots()
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
     dv.create_boxplot(
         data=df, x_var="Petal.Length", y_var="Species", color_by=None, ax=ax, title=""
     )
     return fig
 
 
 @pytest.mark.mpl_image_compare
 def test_create_swarmplot():
-    fig, ax = plt.subplots()
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
     dv.create_swarmplot(
         data=df, x_var="Sepal.Width", y_var=None, color_by="Species", ax=ax
     )
     return fig
 
 
 @pytest.mark.mpl_image_compare
 def test_create_histogram():
-    fig, ax = plt.subplots()
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
     dv.create_histogram(
         data=df,
         var="Petal.Width",
         color_by="Species",
         bins=10,
         max_categories=50,
         ax=ax,
         title="",
     )
     return fig
 
 
 @pytest.mark.mpl_image_compare
 def test_create_confusion_matrix_heatmap():
-    fig, ax = plt.subplots()
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
     dv.create_confusion_matrix_heatmap(
         conf_matrix=df[["Sepal.Width", "Sepal.Length"]]
         .select_dtypes(include=np.number)
         .corr(),
         model_accuracy=0.8,
         figsize=(5, 5),
         ax=ax,
     )
     return fig
 
 
 @pytest.mark.mpl_image_compare
 def test_create_tableplot():
-    fig, ax = plt.subplots()
-    dv.create_tableplot(data=df_summary, colLabels=None, figsize=(9, 9), ax=ax)
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
+    dv.create_tableplot(data=df_summary, colLabels=None, ax=ax)
     return fig
 
 
 @pytest.mark.mpl_image_compare
 def test_create_single_tableplot():
     return dv.create_single_tableplot(data=df_summary, colLabels=None)
 
 
 @pytest.mark.mpl_image_compare
 def test_create_pairplot():
     return dv.create_pairplot(data=df, figtitle="")
+
+
+@pytest.mark.mpl_image_compare
+def test_create_barplot():
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
+    dv.create_barplot(
+        data=df_summary,
+        x_var="Species",
+        y_var="Sepal.Length",
+        add_value_labels=True,
+        x_label="",
+        title="",
+        ax=ax,
+    )
+    return fig
+
+
+@pytest.mark.mpl_image_compare
+def test_create_stacked_barplot():
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
+    dv.create_stacked_barplot(
+        data=df_summary,
+        x_var="Species",
+        y_var="Sepal.Length",
+        color_by="Sepal.Width",
+        x_label="",
+        title="",
+        ax=ax,
+    )
+    return fig
+
+
+@pytest.mark.mpl_image_compare
+def test_create_lineplot():
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
+    dv.create_lineplot(
+        data=df,
+        x_var="Sepal.Width",
+        y_var="Sepal.Length",
+        color_by="Species",
+        x_label="",
+        title="",
+        ax=ax,
+    )
+    return fig
```

