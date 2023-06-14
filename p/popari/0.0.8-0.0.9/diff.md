# Comparing `tmp/popari-0.0.8.tar.gz` & `tmp/popari-0.0.9.tar.gz`

## Comparing `popari-0.0.8.tar` & `popari-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/__init__.py
--rw-r--r--   0        0        0    12242 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/analysis.py
--rw-r--r--   0        0        0    58046 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/components.py
--rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/estimate_parameters.py
--rw-r--r--   0        0        0    16360 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/estimate_weights.py
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/initialization.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/io.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/main.py
--rw-r--r--   0        0        0    22196 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/model.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/sample_for_integral.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/simulation_framework.py
--rw-r--r--   0        0        0    23777 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/synthesize.py
--rw-r--r--   0        0        0    18275 2020-02-02 00:00:00.000000 popari-0.0.8/spicemix/util.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 popari-0.0.8/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 popari-0.0.8/LICENSE
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 popari-0.0.8/README.md
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 popari-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 popari-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/__init__.py
+-rw-r--r--   0        0        0    14140 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/analysis.py
+-rw-r--r--   0        0        0    58046 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/components.py
+-rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/estimate_parameters.py
+-rw-r--r--   0        0        0    16360 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/estimate_weights.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/initialization.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/io.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/main.py
+-rw-r--r--   0        0        0    22196 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/model.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/sample_for_integral.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/simulation_framework.py
+-rw-r--r--   0        0        0    23777 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/synthesize.py
+-rw-r--r--   0        0        0    18275 2020-02-02 00:00:00.000000 popari-0.0.9/spicemix/util.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 popari-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 popari-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 popari-0.0.9/README.md
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 popari-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 popari-0.0.9/PKG-INFO
```

### Comparing `popari-0.0.8/spicemix/analysis.py` & `popari-0.0.9/spicemix/analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -176,14 +176,60 @@
             image = dataset.obsp[obsp][dataset.name]
         if uns:
             image = dataset.uns[uns][dataset.name]
        
         im = ax.imshow(image, cmap=cmap, interpolation='nearest', aspect=aspect, **heatmap_kwargs)
         fig.colorbar(im, cax=cax, orientation='vertical')
 
+
+def multigroup_heatmap(trained_model: SpiceMixPlus,
+    group_type: str = "metagene",
+    axes: Optional[Sequence[Axes]] = None,
+    key: Optional[str] = None,
+    **heatmap_kwargs
+  ):
+    r"""Plot 2D heatmap data across all datasets.
+
+    Wrapper function to enable plotting of continuous 2D data across multiple replicates. Only
+    one of ``obsm``, ``obsp`` or ``uns`` should be used.
+
+    Args:
+        trained_model: the trained SpiceMixPlus model.
+        axes: A predefined set of matplotlib axes to plot on.
+        obsm: the key in the ``.obsm`` dataframe to plot.
+        obsp: the key in the ``.obsp`` dataframe to plot.
+        uns: the key in the ``.uns`` dataframe to plot. Unstructured data must be 2D in shape.
+        **heatmap_kwargs: arguments to pass to the `ax.imshow` call for each dataset
+    """
+    datasets = trained_model.datasets
+    groups = trained_model.metagene_groups if group_type == "metagene" else trained_model.spatial_affinity_groups
+    
+
+    fig = None
+    if axes is None:
+        fig, axes = setup_squarish_axes(len(groups))
+
+    aspect = 0.05 if "aspect" not in heatmap_kwargs else heatmap_kwargs.pop("aspect")    
+    cmap = "hot" if "cmap" not in heatmap_kwargs else heatmap_kwargs.pop("cmap")    
+
+    for group_index, (ax, group_name) in enumerate(zip(axes.flat, groups)):
+        first_dataset_name = groups[group_name][0]
+        first_dataset = next(filter(lambda dataset: dataset.name == first_dataset_name, datasets))
+
+        divider = make_axes_locatable(ax)
+        cax = divider.append_axes('right', size='5%', pad=0.05)
+        if group_index > len(groups):
+            ax.set_visible(False)
+            continue
+        
+        image = first_dataset.uns[key][group_name]
+       
+        im = ax.imshow(image, cmap=cmap, interpolation='nearest', aspect=aspect, **heatmap_kwargs)
+        fig.colorbar(im, cax=cax, orientation='vertical')
+
 def compute_ari_scores(trained_model: SpiceMixPlus, labels: str, predictions: str, ari_key: str = "ari"):
     r"""Compute adjusted Rand index (ARI) score  between a set of ground truth labels and an unsupervised clustering.
 
     Useful for assessing clustering validity. ARI score is computed per dataset.
 
     Args:
         trained_model: the trained SpiceMixPlus model.
```

### Comparing `popari-0.0.8/spicemix/components.py` & `popari-0.0.9/spicemix/components.py`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/spicemix/estimate_parameters.py` & `popari-0.0.9/spicemix/estimate_parameters.py`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/spicemix/estimate_weights.py` & `popari-0.0.9/spicemix/estimate_weights.py`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/spicemix/initialization.py` & `popari-0.0.9/spicemix/initialization.py`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/spicemix/io.py` & `popari-0.0.9/spicemix/io.py`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/spicemix/main.py` & `popari-0.0.9/spicemix/main.py`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/spicemix/model.py` & `popari-0.0.9/spicemix/model.py`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/spicemix/sample_for_integral.py` & `popari-0.0.9/spicemix/sample_for_integral.py`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/spicemix/synthesize.py` & `popari-0.0.9/spicemix/synthesize.py`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/spicemix/util.py` & `popari-0.0.9/spicemix/util.py`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/LICENSE` & `popari-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/README.md` & `popari-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `popari-0.0.8/pyproject.toml` & `popari-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "popari"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Shahul Alam", email="alam.shahul@gmail.com.com" },
 ]
 dependencies = [
     "numpy>=1.20.1",
     "scipy>=1.7.1",
     "scikit-learn>=0.24.1",
```

### Comparing `popari-0.0.8/PKG-INFO` & `popari-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popari
-Version: 0.0.8
+Version: 0.0.9
 Summary: SpiceMix: a probabilistic graphical model for spatial transcriptomics data
 Project-URL: Homepage, https://github.com/alam-shahul/popari
 Project-URL: Bug Tracker, https://github.com/alam-shahul/popari/issues
 Author-email: Shahul Alam <alam.shahul@gmail.com.com>
 License: MIT License
         
         Copyright (c) 2020 Ma Lab at CMU
```

