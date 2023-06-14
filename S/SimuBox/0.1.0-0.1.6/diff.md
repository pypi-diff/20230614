# Comparing `tmp/SimuBox-0.1.0.tar.gz` & `tmp/SimuBox-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimuBox-0.1.0.tar", last modified: Sat May 27 14:46:46 2023, max compression
+gzip compressed data, was "SimuBox-0.1.6.tar", last modified: Wed Jun 14 07:50:11 2023, max compression
```

## Comparing `SimuBox-0.1.0.tar` & `SimuBox-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 14:46:46.515618 SimuBox-0.1.0/
--rw-rw-rw-   0        0        0     1093 2023-05-20 08:53:35.000000 SimuBox-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2331 2023-05-27 14:46:46.515618 SimuBox-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-05-22 07:25:23.000000 SimuBox-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 14:46:46.503618 SimuBox-0.1.0/demo/
--rw-rw-rw-   0        0        0   313145 2023-05-27 14:16:16.000000 SimuBox-0.1.0/demo/base.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-27 14:46:46.505618 SimuBox-0.1.0/demo/datasets/
--rw-rw-rw-   0        0        0    64956 2022-11-29 02:28:07.000000 SimuBox-0.1.0/demo/datasets/interp.csv
--rw-rw-rw-   0        0        0      598 2023-05-20 09:04:14.000000 SimuBox-0.1.0/environment.yaml
--rw-rw-rw-   0        0        0      884 2023-05-27 14:45:07.000000 SimuBox-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 14:46:46.515618 SimuBox-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 14:46:46.499619 SimuBox-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 14:46:46.511618 SimuBox-0.1.0/src/SimuBox.egg-info/
--rw-rw-rw-   0        0        0     2331 2023-05-27 14:46:46.000000 SimuBox-0.1.0/src/SimuBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-27 14:46:46.000000 SimuBox-0.1.0/src/SimuBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 14:46:46.000000 SimuBox-0.1.0/src/SimuBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-27 14:46:46.000000 SimuBox-0.1.0/src/SimuBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 14:46:46.000000 SimuBox-0.1.0/src/SimuBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 14:46:46.514618 SimuBox-0.1.0/src/plotter/
--rw-rw-rw-   0        0        0       67 2023-05-20 08:35:59.000000 SimuBox-0.1.0/src/plotter/__init__.py
--rw-rw-rw-   0        0        0     8549 2023-05-26 03:24:56.000000 SimuBox-0.1.0/src/plotter/compare.py
--rw-rw-rw-   0        0        0     5643 2023-05-19 06:07:58.000000 SimuBox-0.1.0/src/plotter/land.py
--rw-rw-rw-   0        0        0    16447 2023-05-26 08:19:23.000000 SimuBox-0.1.0/src/plotter/phase.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.261655 SimuBox-0.1.6/
+-rw-rw-rw-   0        0        0     1093 2023-05-20 08:53:35.000000 SimuBox-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1789 2023-06-14 07:50:11.260665 SimuBox-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.195655 SimuBox-0.1.6/demo/
+-rw-rw-rw-   0        0        0   394698 2023-06-14 05:56:45.000000 SimuBox-0.1.6/demo/base.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.187656 SimuBox-0.1.6/demo/datasets/
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.196661 SimuBox-0.1.6/demo/datasets/Info/
+-rw-rw-rw-   0        0        0   331784 2023-06-05 11:15:08.000000 SimuBox-0.1.6/demo/datasets/Info/block.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.197655 SimuBox-0.1.6/demo/datasets/Iso/
+-rw-rw-rw-   0        0        0  9437194 2023-06-14 04:59:55.000000 SimuBox-0.1.6/demo/datasets/Iso/phout.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.208659 SimuBox-0.1.6/demo/datasets/Land/
+-rw-rw-rw-   0        0        0    64956 2022-11-29 02:28:07.000000 SimuBox-0.1.6/demo/datasets/Land/interp.csv
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.211667 SimuBox-0.1.6/demo/datasets/Vori/
+-rw-rw-rw-   0        0        0  1066469 2023-06-05 11:41:01.000000 SimuBox-0.1.6/demo/datasets/Vori/phout.txt
+-rw-rw-rw-   0        0        0    62157 2023-06-05 11:41:23.000000 SimuBox-0.1.6/demo/datasets/Vori/printout.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.244664 SimuBox-0.1.6/demo/datasets/scatter/
+-rw-rw-rw-   0        0        0   331786 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/Joint_B2A2.txt
+-rw-rw-rw-   0        0        0  2396170 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/LargeC4.txt
+-rw-rw-rw-   0        0        0    10650 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/aa.txt
+-rw-rw-rw-   0        0        0  2985994 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/block.txt
+-rw-rw-rw-   0        0        0      405 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/bridge_cal.txt
+-rw-rw-rw-   0        0        0      199 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/fet.txt
+-rw-rw-rw-   0        0        0     8516 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/input.json
+-rw-rw-rw-   0        0        0     8518 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/input_Large.json
+-rw-rw-rw-   0        0        0  3575818 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/joint.txt
+-rw-rw-rw-   0        0        0        9 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/log_bridge.txt
+-rw-rw-rw-   0        0        0      135 2022-12-09 02:14:11.000000 SimuBox-0.1.6/demo/datasets/scatter/para
+-rw-rw-rw-   0        0        0  2396170 2022-12-09 02:14:12.000000 SimuBox-0.1.6/demo/datasets/scatter/phin.txt
+-rw-rw-rw-   0        0        0  2248730 2022-12-09 02:14:12.000000 SimuBox-0.1.6/demo/datasets/scatter/phin_with_mask.txt
+-rw-rw-rw-   0        0        0  1762966 2022-12-09 02:14:12.000000 SimuBox-0.1.6/demo/datasets/scatter/phout.txt
+-rw-rw-rw-   0        0        0     1010 2022-12-09 02:14:12.000000 SimuBox-0.1.6/demo/datasets/scatter/printout.txt
+-rw-rw-rw-   0        0        0      288 2022-12-09 02:14:12.000000 SimuBox-0.1.6/demo/datasets/scatter/printout_c.txt
+-rw-rw-rw-   0        0        0     1260 2022-12-09 02:14:12.000000 SimuBox-0.1.6/demo/datasets/scatter/small.printout.txt
+-rw-rw-rw-   0        0        0     7332 2022-12-09 02:14:12.000000 SimuBox-0.1.6/demo/datasets/scatter/tau0.13_ksi0.55_phaseC4_.jpg
+-rw-rw-rw-   0        0        0      440 2022-12-09 02:14:12.000000 SimuBox-0.1.6/demo/datasets/scatter/tau0.13_ksi0.55_phaseC4_.npz
+-rw-rw-rw-   0        0        0     1570 2022-12-09 02:14:12.000000 SimuBox-0.1.6/demo/datasets/scatter/tau0.13_ksi0.55_phaseC4__mask.jpg
+-rw-rw-rw-   0        0        0       42 2022-12-09 02:14:12.000000 SimuBox-0.1.6/demo/datasets/scatter/width_log.txt
+-rw-rw-rw-   0        0        0      709 2023-06-14 07:48:14.000000 SimuBox-0.1.6/demo/iso_plot_trisurf.py
+-rw-rw-rw-   0        0        0      739 2023-06-14 05:22:55.000000 SimuBox-0.1.6/demo/iso_vista.py
+-rw-rw-rw-   0        0        0      230 2023-06-14 07:10:03.000000 SimuBox-0.1.6/demo/scatter_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.245664 SimuBox-0.1.6/dist/
+-rw-rw-rw-   0        0        0    11470 2023-05-27 14:46:59.000000 SimuBox-0.1.6/dist/SimuBox-0.1.0-py3-none-any.whl
+-rw-rw-rw-   0        0        0   256809 2023-05-27 14:46:46.000000 SimuBox-0.1.6/dist/SimuBox-0.1.0.tar.gz
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.246664 SimuBox-0.1.6/docs/
+-rw-rw-rw-   0        0        0       90 2023-06-14 06:55:25.000000 SimuBox-0.1.6/docs/build_flow.md
+-rw-rw-rw-   0        0        0      650 2023-05-27 14:59:30.000000 SimuBox-0.1.6/environment.yaml
+-rw-rw-rw-   0        0        0     1004 2023-06-14 07:49:48.000000 SimuBox-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 07:50:11.261655 SimuBox-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.247655 SimuBox-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.247655 SimuBox-0.1.6/src/SimuBox/
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.254656 SimuBox-0.1.6/src/SimuBox/SciCalc/
+-rw-rw-rw-   0        0        0       76 2023-06-14 05:54:52.000000 SimuBox-0.1.6/src/SimuBox/SciCalc/__init__.py
+-rw-rw-rw-   0        0        0     4249 2023-06-07 03:20:21.000000 SimuBox-0.1.6/src/SimuBox/SciCalc/correlation.py
+-rw-rw-rw-   0        0        0     6443 2023-06-14 06:24:19.000000 SimuBox-0.1.6/src/SimuBox/SciCalc/scatter.py
+-rw-rw-rw-   0        0        0     9034 2023-06-07 03:24:47.000000 SimuBox-0.1.6/src/SimuBox/SciCalc/voronoi.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.258664 SimuBox-0.1.6/src/SimuBox/SciPlot/
+-rw-rw-rw-   0        0        0       67 2023-05-20 08:35:59.000000 SimuBox-0.1.6/src/SimuBox/SciPlot/__init__.py
+-rw-rw-rw-   0        0        0     9993 2023-06-13 06:56:23.000000 SimuBox-0.1.6/src/SimuBox/SciPlot/compare.py
+-rw-rw-rw-   0        0        0     5643 2023-05-19 06:07:58.000000 SimuBox-0.1.6/src/SimuBox/SciPlot/land.py
+-rw-rw-rw-   0        0        0    16672 2023-05-29 02:12:55.000000 SimuBox-0.1.6/src/SimuBox/SciPlot/phase.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.260665 SimuBox-0.1.6/src/SimuBox/SciTools/
+-rw-rw-rw-   0        0        0       42 2023-06-07 03:22:15.000000 SimuBox-0.1.6/src/SimuBox/SciTools/__init__.py
+-rw-rw-rw-   0        0        0     5431 2023-06-14 05:23:21.000000 SimuBox-0.1.6/src/SimuBox/SciTools/tools.py
+-rw-rw-rw-   0        0        0     4516 2023-05-27 13:27:18.000000 SimuBox-0.1.6/src/SimuBox/SciTools/xml.py
+-rw-rw-rw-   0        0        0       73 2023-06-14 07:49:13.000000 SimuBox-0.1.6/src/SimuBox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:50:11.252665 SimuBox-0.1.6/src/SimuBox.egg-info/
+-rw-rw-rw-   0        0        0     1789 2023-06-14 07:50:10.000000 SimuBox-0.1.6/src/SimuBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1680 2023-06-14 07:50:11.000000 SimuBox-0.1.6/src/SimuBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 07:50:10.000000 SimuBox-0.1.6/src/SimuBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 07:50:10.000000 SimuBox-0.1.6/src/SimuBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 07:50:10.000000 SimuBox-0.1.6/src/SimuBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       24 2023-06-14 07:48:14.000000 SimuBox-0.1.6/src/__init__.py
```

### Comparing `SimuBox-0.1.0/LICENSE` & `SimuBox-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SimuBox-0.1.0/demo/datasets/interp.csv` & `SimuBox-0.1.6/demo/datasets/Land/interp.csv`

 * *Files identical despite different names*

### Comparing `SimuBox-0.1.0/environment.yaml` & `SimuBox-0.1.6/environment.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -7,7 +7,8 @@
   - pandas==1.4.0
   - scipy==1.10.0
   - matplotlib==3.6.2
   - numpy==1.19.5
   - opencv-contrib-python==4.7.0.72
   - opencv-python==4.5.3.56
   - opencv-python-headless==3.4.18.65
+  - pytorch==1.8.2+cu111
```

### Comparing `SimuBox-0.1.0/pyproject.toml` & `SimuBox-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 "setuptools-scm",
 "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
+include = ["SimuBox*"]  # package names should match these glob patterns (["*"] by default)
+exclude = ["SimuBox.ScriptRun*", "demo*"]
 
 [project]
 name = "SimuBox"
-version = "0.1.0"
+version = "0.1.6"
 authors = [
     { name = "Alkaid Yuan", email = "kryuan@qq.com" }
 ]
 description = "Free python package to do some science calculation."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers =[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "pytorch",
     "matplotlib",
     "scipy",
     "opencv-python",
     "numpy",
     "pandas"
 ]
```

### Comparing `SimuBox-0.1.0/src/plotter/compare.py` & `SimuBox-0.1.6/src/SimuBox/SciPlot/compare.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,18 +65,23 @@
         'phi_AB': r'$\phi _{\rm AB}$',
         
         'freeAB1': r'$\rm A/B_1$',
         'freeAB2': r'$\rm A/B_2$',
     }
 
 
-_style_ref = (cycler(color=list('rbm')) +
-          cycler(marker=['s', 'X', 'v']))
-_style_abs = (cycler(color=list('krbm')) +
-          cycler(marker=['o', 's', 'X', 'v']))
+_style_ref = (cycler(color=list('rbm') + [
+                'indianred', 'tomato', 'chocolate',
+                'olivedrab', 'teal', 'deepskyblue', 'darkviolet']) +
+          cycler(marker=list('sXvoP*D><p')))
+
+_style_abs = (cycler(color=list('krbm') + [
+                'indianred', 'tomato', 'chocolate',
+                'olivedrab', 'teal', 'deepskyblue']) +
+              cycler(marker=list('osXvP*D><p')))
 
 class CompareJudger():
     
     def __init__(self, 
                  path:str,
                  div:Union[int, float]=1,
                  acc:int=3,
@@ -86,25 +91,29 @@
         self.div = div
         self.acc = acc
         pass
     
     # @lazyproperty
     def data(self, subset=['lx', 'ly', 'lz', 'phase', 'freeE'], **kwargs):
         df = pd.read_csv(self.path)
+        df = df.dropna(axis=0)
         df = df.drop_duplicates(subset=subset)
         df['lylz'] = np.around(df['ly']/df['lz'], self.acc)
         df['lxly'] = np.around(df['lx']/df['ly'], self.acc)
         try:
             df['chiN'] = df['chiN']/self.div
-        except:
+        except KeyError:
             pass
         return df
     
     def ref_compare(self, base, others, xlabel, ylabel, ax:Optional[object]=None, horiline:bool=False, **kwargs):
         
+        ref_labels = Labels.ref_label.copy()
+        ref_labels.update(kwargs.get('labels', {}))
+        
         data = self.data()
         data = data.sort_values(by=xlabel)
         
         plt.figure(figsize=kwargs.get('figsize', (9, 6.5)))
         if not ax:
             ax = plt.gca()
             ax.set_prop_cycle(_style_ref)
@@ -123,63 +132,83 @@
             o_xticks = o_xticks[mask]
             o_yticks = o_yticks[mask]
             
             inverse_mask = np.in1d(base_xticks, o_xticks)
             # base_xticks_mask = base_xticks[inverse_mask]
             base_yticks_mask = base_yticks[inverse_mask]
             ax.plot(o_xticks, o_yticks-base_yticks_mask, 
-                    label=Labels.ref_label[o],
+                    label=ref_labels.get(o, o),
                      lw=2.5, markersize=8, alpha=1.0)
         
         if horiline:
+            rest = data[data['phase'] != base]
+            rest_xticks = rest[xlabel].unique()
+            mask = np.in1d(base_xticks, rest_xticks)
+            base_xticks_mask = base_xticks[mask]
             ax.plot(
-                base_xticks, [0]*len(base_xticks),
-                label=Labels.ref_label[base],
+                base_xticks_mask, np.zeros_like(base_xticks_mask), 
+                label=ref_labels.get(base, base),
                 lw=2.5, c='k', marker='o', markersize=8, alpha=0.8)
         
         if trans := kwargs.get('trans'):
             for t in trans:
                 ax.axvline(x=t, c='k', alpha=0.5, ls='--', lw=2.5)
-        
-        ax.xaxis.set_minor_locator(AutoMinorLocator(5))
-        ax.yaxis.set_minor_locator(AutoMinorLocator(5))
-        ax.yaxis.set_major_locator(MultipleLocator(kwargs.get('ymain', 0.005)))
+        if xminor := kwargs.get('xminor', 5):
+            ax.xaxis.set_minor_locator(AutoMinorLocator(xminor))
+        if yminor := kwargs.get('yminor', 5):
+            ax.yaxis.set_minor_locator(AutoMinorLocator(yminor))
+        if xmain := kwargs.get('xmain', False):
+            ax.yaxis.set_major_locator(MultipleLocator(xmain))
+        if ymain := kwargs.get('ymain', False):
+            ax.yaxis.set_major_locator(MultipleLocator(ymain))
         
         plt.tick_params(axis='both', labelsize=25, pad=8)
-        plt.ylabel(Labels.ref_label.get(ylabel, ylabel), fontsize=30)
-        plt.xlabel(Labels.ref_label.get(xlabel, xlabel), fontsize=30)
-        if kwargs.get('legend', True):
-            plt.legend(fontsize=25)
+        plt.ylabel(ref_labels.get(ylabel, ylabel), fontsize=30)
+        plt.xlabel(ref_labels.get(xlabel, xlabel), fontsize=30)
+        if loc := kwargs.get('legend', 'in'):
+            if loc == 'in':
+                plt.legend(fontsize=25, loc='best')
+            elif loc == 'out':
+                plt.legend(fontsize=25, loc='upper left', bbox_to_anchor=(1, 1))
         plt.margins(*kwargs.get('margin',(0.15,0.15)))
         plt.tight_layout()
         if save := kwargs.get('save', False):
             plt.savefig(save, dpi=300)
 
     def abs_compare(self, phases: Union[list, str], xlabel, ylabel, **kwargs):
+        
+        abs_labels = Labels.abs_label.copy()
+        abs_labels.update(kwargs.get('labels', {}))
 
         data = self.data()
         data = data.sort_values(by=xlabel)
         
         plt.figure(figsize=kwargs.get('figsize', (9, 6.5)))
         ax = plt.gca()
         ax.set_prop_cycle(_style_abs)
         
         phases = [phases] if isinstance(phases, str) else phases
         
         for p in phases:
             tmp = data[data.phase == p]
             ax.plot(tmp[xlabel], tmp[ylabel],
-                    label=Labels.abs_label.get(p, p),
+                    label=abs_labels.get(p, p),
                     lw=2.5, markersize=8)
             
-        plt.xlabel(Labels.abs_label.get(xlabel, xlabel), fontsize=30)
-        plt.ylabel(Labels.abs_label.get(ylabel, ylabel), fontsize=30)
+        plt.xlabel(abs_labels.get(xlabel, xlabel), fontsize=30)
+        plt.ylabel(abs_labels.get(ylabel, ylabel), fontsize=30)
         plt.tick_params(axis='both', labelsize=25, pad=8)
-        ax.xaxis.set_minor_locator(AutoMinorLocator(5))
-        ax.yaxis.set_minor_locator(AutoMinorLocator(5))
+        if xminor := kwargs.get('xminor', 5):
+            ax.xaxis.set_minor_locator(AutoMinorLocator(xminor))
+        if yminor := kwargs.get('yminor', 5):
+            ax.yaxis.set_minor_locator(AutoMinorLocator(yminor))
+        if xmain := kwargs.get('xmain', False):
+            ax.yaxis.set_major_locator(MultipleLocator(xmain))
+        if ymain := kwargs.get('ymain', False):
+            ax.yaxis.set_major_locator(MultipleLocator(ymain))
         if trans := kwargs.get('trans'):
             for i in trans:
                 plt.axvline(x=i, c='k', alpha=0.5, ls='--', lw=2.5)
             
         if kwargs.get('legend', True):
             plt.legend(fontsize=25, loc='upper left',bbox_to_anchor=(0.98, 0.8))
```

### Comparing `SimuBox-0.1.0/src/plotter/land.py` & `SimuBox-0.1.6/src/SimuBox/SciPlot/land.py`

 * *Files identical despite different names*

### Comparing `SimuBox-0.1.0/src/plotter/phase.py` & `SimuBox-0.1.6/src/SimuBox/SciPlot/phase.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,25 +33,23 @@
                         'tau': r'$\tau$',
                         'ksi': r'$\xi$',
                         'volH': r'$\phi_{\rm{H}}$',
                         'fA': r'$f_{\rm{A}}$',
                         'fA': r'$f_{\rm{A}}$',
                         'chiN': r'$\chi \rm{N}$'
                     },
-                    div = 1,
                     **kwargs
                     ) -> None:
         
         self.color_dict = color_dict
         self.color_dict.update(kwargs.get('color', {}))
         self.label_dict = label_dict
         self.label_dict.update(kwargs.get('label', {}))
         self.xlabel = xlabel
         self.ylabel = ylabel
-        self.div = div
         pass
     
     def query_point(self, df, xval=None, yval=None, **kwargs):
         res = df.copy()
         if xval:
             res = res[res[self.xlabel] == xval]
         if yval:
@@ -68,28 +66,39 @@
     @staticmethod
     def checkin(phase, candidates):
         if len(phase) == 0: return False
         for i in phase:
             if i in candidates:
                 return True
         return False
-    
+
+    def data(self, path, **kwargs):
+        dropset = kwargs.get('dropset', ['lx', 'ly', 'lz', 'phase', 'freeE'])
+        div = kwargs.get('div', 1)
+        div_var = kwargs.get('div_var', 'chiN')
+        acc = kwargs.get('acc', 3)
+
+        df = pd.read_csv(path)
+        if dropset:
+            df = df.drop_duplicates(subset=dropset)
+        df['lylz'] = np.around(df['ly']/df['lz'], acc)
+        df['lxly'] = np.around(df['lx']/df['ly'], acc)
+        try:
+            df[div_var] = df[div_var]/div
+        except KeyError:
+            pass
+        return df
+
     def compare(self,
                 path:str,
                 plot:bool=True,
                 acc:int=3,
                 **kwargs):
         
-        dropset = kwargs.get('dropset', ['lx', 'ly', 'lz', 'phase'])
-        df = pd.read_csv(path)
-        if dropset:
-            df = df.drop_duplicates(subset=dropset)
-        df['lylz'] = np.around(df['ly']/df['lz'], acc)
-        df['lxly'] = np.around(df['lx']/df['ly'], acc)
-        df[self.ylabel] = df[self.ylabel]/self.div
+        df = self.data(path=path, acc=acc)
         print(f"Include phase: {set(df['phase'].values)}")
         
         plot_dict = dict()
         y_set = np.sort(df[self.ylabel].unique())
         x_set = np.sort(df[self.xlabel].unique())
 
         exclude = kwargs.get('exclude', [])
```

