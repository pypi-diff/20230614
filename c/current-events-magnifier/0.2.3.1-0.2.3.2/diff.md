# Comparing `tmp/current_events_magnifier-0.2.3.1.tar.gz` & `tmp/current_events_magnifier-0.2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.2.3.1.tar", last modified: Wed Jun 14 11:40:22 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.2.3.2.tar", last modified: Wed Jun 14 11:49:44 2023, max compression
```

## Comparing `current_events_magnifier-0.2.3.1.tar` & `current_events_magnifier-0.2.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:40:22.711737 current_events_magnifier-0.2.3.1/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.2.3.1/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-14 11:40:22.707737 current_events_magnifier-0.2.3.1/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5408 2023-06-14 11:16:12.000000 current_events_magnifier-0.2.3.1/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:40:22.707737 current_events_magnifier-0.2.3.1/current_events_magnifier/
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5883 2023-06-14 11:39:50.000000 current_events_magnifier-0.2.3.1/current_events_magnifier/CE_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.2.3.1/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.2.3.1/current_events_magnifier/cem_utils.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.2.3.1/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7487 2023-06-14 08:32:18.000000 current_events_magnifier-0.2.3.1/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.3.1/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13271 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.3.1/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:40:22.707737 current_events_magnifier-0.2.3.1/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-14 11:40:22.000000 current_events_magnifier-0.2.3.1/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      554 2023-06-14 11:40:22.000000 current_events_magnifier-0.2.3.1/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 11:40:22.000000 current_events_magnifier-0.2.3.1/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 11:40:22.000000 current_events_magnifier-0.2.3.1/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-14 11:40:22.000000 current_events_magnifier-0.2.3.1/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 11:40:22.711737 current_events_magnifier-0.2.3.1/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1044 2023-06-14 11:40:18.000000 current_events_magnifier-0.2.3.1/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:49:44.033876 current_events_magnifier-0.2.3.2/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.2.3.2/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-14 11:49:44.033876 current_events_magnifier-0.2.3.2/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5408 2023-06-14 11:16:12.000000 current_events_magnifier-0.2.3.2/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:49:44.033876 current_events_magnifier-0.2.3.2/current_events_magnifier/
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5889 2023-06-14 11:45:23.000000 current_events_magnifier-0.2.3.2/current_events_magnifier/CE_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.2.3.2/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.2.3.2/current_events_magnifier/cem_utils.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.2.3.2/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7556 2023-06-14 11:49:38.000000 current_events_magnifier-0.2.3.2/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.3.2/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13271 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.3.2/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:49:44.033876 current_events_magnifier-0.2.3.2/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-14 11:49:44.000000 current_events_magnifier-0.2.3.2/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      554 2023-06-14 11:49:44.000000 current_events_magnifier-0.2.3.2/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 11:49:44.000000 current_events_magnifier-0.2.3.2/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-14 11:49:44.000000 current_events_magnifier-0.2.3.2/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-14 11:49:44.000000 current_events_magnifier-0.2.3.2/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 11:49:44.033876 current_events_magnifier-0.2.3.2/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1094 2023-06-14 11:49:38.000000 current_events_magnifier-0.2.3.2/setup.py
```

### Comparing `current_events_magnifier-0.2.3.1/LICENSE` & `current_events_magnifier-0.2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.3.1/PKG-INFO` & `current_events_magnifier-0.2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.2.3.1
+Version: 0.2.3.2
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.2.3.1/README.md` & `current_events_magnifier-0.2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.3.1/current_events_magnifier/CE_magnifier.py` & `current_events_magnifier-0.2.3.2/current_events_magnifier/CE_magnifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             df_ivt, aligned_num_ivt = extract_group(args, ivt_file, subsample_num)
             df_ivt['type'] = 'Control'
             df = pd.concat([df_wt, df_ivt])
             title = title + '   Sample:' + str(aligned_num_wt) + '  Control:' + str(aligned_num_ivt)
             category = pd.api.types.CategoricalDtype(categories=['Sample', "Control"], ordered=True)
             df['type'] = df['type'].astype(category)
         except:
-            args.control = None
+            args.control_fast5 = None
         if args.control_fast5 is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
     elif args.function == 'f5c':
         from current_events_magnifier.read_f5c_resquiggle import read_blow5
         df_wt, aligned_num_wt = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand, subsample_num)
```

### Comparing `current_events_magnifier-0.2.3.1/current_events_magnifier/cem_utils.py` & `current_events_magnifier-0.2.3.2/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.3.1/current_events_magnifier/normalization.py` & `current_events_magnifier-0.2.3.2/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.3.1/current_events_magnifier/plot.py` & `current_events_magnifier-0.2.3.2/current_events_magnifier/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,16 @@
             if plot_type == 'boxplot':
                 plot = plot + p9.geom_boxplot( outlier_shape='',position=p9.position_dodge(0.9),size=0.25)
             elif plot_type == 'violin_plot':
                 plot = plot + p9.geom_violin(style='left-right',position=p9.position_dodge(0),color='none',width=1.5)
             else:
                 raise Exception("Unsupported figure type!")
             # plot.render_matplotlib()
+            if item=='Dwell time':
+                item='Dwell_time'
             plot.save(filename=results_path + "/" + item + "_"+plot_type+".pdf", dpi=300)
     else:
         new_df=None
         for item in item_list:
             # collect data
             temp= df[[item,'position','type']]
             temp.columns=['value','position','type']
```

### Comparing `current_events_magnifier-0.2.3.1/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.2.3.2/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.3.1/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.2.3.2/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.3.1/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.2.3.2/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.2.3.1
+Version: 0.2.3.2
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.2.3.1/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.2.3.2/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.3.1/setup.py` & `current_events_magnifier-0.2.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.2.3.1",
+    version="0.2.3.2",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
@@ -22,10 +22,12 @@
     python_requires='>=3.7',
     install_requires=[
         'h5py==3.8.0',
         'numpy>=1.21.6',
         'pandas>=1.1.5',
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
+        "pyslow5>=1.0.0",
+        "pysam>=0.21.0"
     ],
     scripts=['current_events_magnifier/CE_magnifier.py']
 )
```

