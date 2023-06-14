# Comparing `tmp/bluepyefe-2.2.51.tar.gz` & `tmp/bluepyefe-2.2.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepyefe-2.2.51.tar", last modified: Thu Apr 20 09:33:56 2023, max compression
+gzip compressed data, was "bluepyefe-2.2.53.tar", last modified: Wed Jun 14 13:45:43 2023, max compression
```

## Comparing `bluepyefe-2.2.51.tar` & `bluepyefe-2.2.53.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:33:55.996212 bluepyefe-2.2.51/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-20 09:33:55.996212 bluepyefe-2.2.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:33:55.996212 bluepyefe-2.2.51/bluepyefe/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-20 09:33:55.996212 bluepyefe-2.2.51/bluepyefe/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/auto_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:33:55.996212 bluepyefe-2.2.51/bluepyefe/ecode/
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/DeHyperPol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/HyperDePol.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/SpikeRec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/negCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/posCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/sAHP.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/sineSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/ecode/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:33:55.996212 bluepyefe-2.2.51/bluepyefe/igorpy/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/igorpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/nwbreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/rheobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/bluepyefe/translate_legacy_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:33:55.996212 bluepyefe-2.2.51/bluepyefe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-20 09:33:55.000000 bluepyefe-2.2.51/bluepyefe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-20 09:33:55.000000 bluepyefe-2.2.51/bluepyefe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:33:55.000000 bluepyefe-2.2.51/bluepyefe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 09:33:55.000000 bluepyefe-2.2.51/bluepyefe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 09:33:55.000000 bluepyefe-2.2.51/bluepyefe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:33:55.996212 bluepyefe-2.2.51/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 09:33:55.996212 bluepyefe-2.2.51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-04-20 09:33:49.000000 bluepyefe-2.2.51/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:45:43.427150 bluepyefe-2.2.53/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-14 13:45:43.427150 bluepyefe-2.2.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:45:43.427150 bluepyefe-2.2.53/bluepyefe/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-14 13:45:43.427150 bluepyefe-2.2.53/bluepyefe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/auto_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:45:43.427150 bluepyefe-2.2.53/bluepyefe/ecode/
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/DeHyperPol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/HyperDePol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/SpikeRec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/negCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/posCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/sAHP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/sineSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/ecode/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:45:43.427150 bluepyefe-2.2.53/bluepyefe/igorpy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/igorpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/nwbreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/rheobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/bluepyefe/translate_legacy_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:45:43.423150 bluepyefe-2.2.53/bluepyefe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-14 13:45:43.000000 bluepyefe-2.2.53/bluepyefe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-14 13:45:43.000000 bluepyefe-2.2.53/bluepyefe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:45:43.000000 bluepyefe-2.2.53/bluepyefe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 13:45:43.000000 bluepyefe-2.2.53/bluepyefe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 13:45:43.000000 bluepyefe-2.2.53/bluepyefe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:45:43.427150 bluepyefe-2.2.53/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-14 13:45:43.427150 bluepyefe-2.2.53/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-06-14 13:45:40.000000 bluepyefe-2.2.53/versioneer.py
```

### Comparing `bluepyefe-2.2.51/LICENSE.txt` & `bluepyefe-2.2.53/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/PKG-INFO` & `bluepyefe-2.2.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.51
+Version: 2.2.53
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.51/README.md` & `bluepyefe-2.2.53/README.md`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/__init__.py` & `bluepyefe-2.2.53/bluepyefe/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/auto_targets.py` & `bluepyefe-2.2.53/bluepyefe/auto_targets.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/cell.py` & `bluepyefe-2.2.53/bluepyefe/cell.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/DeHyperPol.py` & `bluepyefe-2.2.53/bluepyefe/ecode/DeHyperPol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/HyperDePol.py` & `bluepyefe-2.2.53/bluepyefe/ecode/HyperDePol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/SpikeRec.py` & `bluepyefe-2.2.53/bluepyefe/ecode/SpikeRec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/__init__.py` & `bluepyefe-2.2.53/bluepyefe/ecode/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/negCheops.py` & `bluepyefe-2.2.53/bluepyefe/ecode/negCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/posCheops.py` & `bluepyefe-2.2.53/bluepyefe/ecode/posCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/ramp.py` & `bluepyefe-2.2.53/bluepyefe/ecode/ramp.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/sAHP.py` & `bluepyefe-2.2.53/bluepyefe/ecode/sAHP.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/sineSpec.py` & `bluepyefe-2.2.53/bluepyefe/ecode/sineSpec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/step.py` & `bluepyefe-2.2.53/bluepyefe/ecode/step.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/ecode/tools.py` & `bluepyefe-2.2.53/bluepyefe/ecode/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/extract.py` & `bluepyefe-2.2.53/bluepyefe/extract.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/igorpy/__init__.py` & `bluepyefe-2.2.53/bluepyefe/igorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/nwbreader.py` & `bluepyefe-2.2.53/bluepyefe/nwbreader.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/plotting.py` & `bluepyefe-2.2.53/bluepyefe/plotting.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/protocol.py` & `bluepyefe-2.2.53/bluepyefe/protocol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/reader.py` & `bluepyefe-2.2.53/bluepyefe/reader.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/recording.py` & `bluepyefe-2.2.53/bluepyefe/recording.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/rheobase.py` & `bluepyefe-2.2.53/bluepyefe/rheobase.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/target.py` & `bluepyefe-2.2.53/bluepyefe/target.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/tools.py` & `bluepyefe-2.2.53/bluepyefe/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe/translate_legacy_config.py` & `bluepyefe-2.2.53/bluepyefe/translate_legacy_config.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/bluepyefe.egg-info/PKG-INFO` & `bluepyefe-2.2.53/bluepyefe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.51
+Version: 2.2.53
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.51/bluepyefe.egg-info/SOURCES.txt` & `bluepyefe-2.2.53/bluepyefe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/examples/__init__.py` & `bluepyefe-2.2.53/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/setup.py` & `bluepyefe-2.2.53/setup.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.51/versioneer.py` & `bluepyefe-2.2.53/versioneer.py`

 * *Files identical despite different names*

