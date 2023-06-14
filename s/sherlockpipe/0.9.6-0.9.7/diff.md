# Comparing `tmp/sherlockpipe-0.9.6.tar.gz` & `tmp/sherlockpipe-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sherlockpipe-0.9.6.tar", last modified: Fri Aug  7 11:54:43 2020, max compression
+gzip compressed data, was "dist/sherlockpipe-0.9.7.tar", last modified: Sun Aug 16 19:02:52 2020, max compression
```

## Comparing `sherlockpipe-0.9.6.tar` & `sherlockpipe-0.9.7.tar`

### file list

```diff
@@ -1,17 +1,57 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-07 11:54:43.000000 sherlockpipe-0.9.6/
--rwxrwxrwx   0 root         (0) root         (0)    13033 2020-08-07 11:54:43.000000 sherlockpipe-0.9.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    10970 2020-08-07 11:00:56.000000 sherlockpipe-0.9.6/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2020-08-07 11:54:43.000000 sherlockpipe-0.9.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1096 2020-08-07 11:54:33.000000 sherlockpipe-0.9.6/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-07 11:54:43.000000 sherlockpipe-0.9.6/sherlockpipe/
--rwxrwxrwx   0 root         (0) root         (0)    45873 2020-08-07 11:44:33.000000 sherlockpipe-0.9.6/sherlockpipe/sherlock.py
--rwxrwxrwx   0 root         (0) root         (0)     8679 2020-08-07 11:45:03.000000 sherlockpipe-0.9.6/sherlockpipe/sherlock_tests.py
--rwxrwxrwx   0 root         (0) root         (0)      540 2020-08-07 11:53:36.000000 sherlockpipe-0.9.6/sherlockpipe/transitresult.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-08-03 20:36:11.000000 sherlockpipe-0.9.6/sherlockpipe/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8619 2020-08-07 11:40:54.000000 sherlockpipe-0.9.6/sherlockpipe/__main__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-07 11:54:43.000000 sherlockpipe-0.9.6/sherlockpipe.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2020-08-07 11:54:43.000000 sherlockpipe-0.9.6/sherlockpipe.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)    13033 2020-08-07 11:54:43.000000 sherlockpipe-0.9.6/sherlockpipe.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       85 2020-08-07 11:54:43.000000 sherlockpipe-0.9.6/sherlockpipe.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)      333 2020-08-07 11:54:43.000000 sherlockpipe-0.9.6/sherlockpipe.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2020-08-07 11:54:43.000000 sherlockpipe-0.9.6/sherlockpipe.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/
+-rwxrwxrwx   0 root         (0) root         (0)    13708 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    11557 2020-08-16 15:51:59.000000 sherlockpipe-0.9.7/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1096 2020-08-16 19:01:12.000000 sherlockpipe-0.9.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/sherlockpipe/
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/
+-rwxrwxrwx   0 root         (0) root         (0)      949 2020-08-10 16:01:51.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/InputObjectInfo.py
+-rwxrwxrwx   0 root         (0) root         (0)      147 2020-08-09 07:19:02.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/InvalidNumberOfSectorsError.py
+-rwxrwxrwx   0 root         (0) root         (0)     1134 2020-08-10 16:01:51.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/MissionFfiCoordsObjectInfo.py
+-rwxrwxrwx   0 root         (0) root         (0)     1088 2020-08-10 16:01:51.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/MissionFfiIdObjectInfo.py
+-rwxrwxrwx   0 root         (0) root         (0)     1121 2020-08-10 16:01:51.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/MissionInputObjectInfo.py
+-rwxrwxrwx   0 root         (0) root         (0)     1114 2020-08-10 16:01:51.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/MissionObjectInfo.py
+-rwxrwxrwx   0 root         (0) root         (0)      865 2020-08-10 16:01:51.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/ObjectInfo.py
+-rwxrwxrwx   0 root         (0) root         (0)      145 2020-08-06 20:50:55.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/ObjectProcessingError.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/preparer/
+-rwxrwxrwx   0 root         (0) root         (0)     1430 2020-08-07 11:46:54.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/preparer/LightcurveBuilder.py
+-rwxrwxrwx   0 root         (0) root         (0)     2226 2020-08-07 11:46:30.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/preparer/MissionFfiLightcurveBuilder.py
+-rwxrwxrwx   0 root         (0) root         (0)     1553 2020-08-10 07:32:47.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/preparer/MissionInputLightcurveBuilder.py
+-rwxrwxrwx   0 root         (0) root         (0)     2269 2020-08-07 11:45:51.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/preparer/MissionLightcurveBuilder.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-08-03 20:36:11.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/preparer/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-08-03 20:36:11.000000 sherlockpipe-0.9.7/sherlockpipe/objectinfo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/sherlockpipe/ois/
+-rwxrwxrwx   0 root         (0) root         (0)     8882 2020-08-06 20:50:07.000000 sherlockpipe-0.9.7/sherlockpipe/ois/OisManager.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-08-03 20:36:11.000000 sherlockpipe-0.9.7/sherlockpipe/ois/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/sherlockpipe/scoring/
+-rwxrwxrwx   0 root         (0) root         (0)      835 2020-08-07 11:47:21.000000 sherlockpipe-0.9.7/sherlockpipe/scoring/BasicSignalSelector.py
+-rwxrwxrwx   0 root         (0) root         (0)     4139 2020-08-07 11:47:47.000000 sherlockpipe-0.9.7/sherlockpipe/scoring/QuorumSnrBorderCorrectedSignalSelector.py
+-rwxrwxrwx   0 root         (0) root         (0)      925 2020-08-06 20:49:31.000000 sherlockpipe-0.9.7/sherlockpipe/scoring/SignalSelector.py
+-rwxrwxrwx   0 root         (0) root         (0)     2636 2020-08-07 11:47:24.000000 sherlockpipe-0.9.7/sherlockpipe/scoring/SnrBorderCorrectedSignalSelector.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-08-03 20:36:11.000000 sherlockpipe-0.9.7/sherlockpipe/scoring/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/sherlockpipe/search_zones/
+-rwxrwxrwx   0 root         (0) root         (0)      679 2020-08-13 14:27:44.000000 sherlockpipe-0.9.7/sherlockpipe/search_zones/HabitableSearchZone.py
+-rwxrwxrwx   0 root         (0) root         (0)      689 2020-08-13 14:27:44.000000 sherlockpipe-0.9.7/sherlockpipe/search_zones/OptimisticHabitableSearchZone.py
+-rwxrwxrwx   0 root         (0) root         (0)      596 2020-08-13 12:43:29.000000 sherlockpipe-0.9.7/sherlockpipe/search_zones/SearchZone.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-08-03 20:36:11.000000 sherlockpipe-0.9.7/sherlockpipe/search_zones/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    57297 2020-08-16 14:41:48.000000 sherlockpipe-0.9.7/sherlockpipe/sherlock.py
+-rwxrwxrwx   0 root         (0) root         (0)     8679 2020-08-07 11:45:03.000000 sherlockpipe-0.9.7/sherlockpipe/sherlock_tests.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/sherlockpipe/star/
+-rwxrwxrwx   0 root         (0) root         (0)     1328 2020-08-07 11:46:49.000000 sherlockpipe-0.9.7/sherlockpipe/star/EpicStarCatalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     5806 2020-08-13 14:38:22.000000 sherlockpipe-0.9.7/sherlockpipe/star/HabitabilityCalculator.py
+-rwxrwxrwx   0 root         (0) root         (0)     1207 2020-08-07 11:47:07.000000 sherlockpipe-0.9.7/sherlockpipe/star/KicStarCatalog.py
+-rwxrwxrwx   0 root         (0) root         (0)      310 2020-08-06 20:50:36.000000 sherlockpipe-0.9.7/sherlockpipe/star/StarCatalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     1177 2020-08-06 20:50:36.000000 sherlockpipe-0.9.7/sherlockpipe/star/starinfo.py
+-rwxrwxrwx   0 root         (0) root         (0)     1096 2020-08-07 11:51:42.000000 sherlockpipe-0.9.7/sherlockpipe/star/TicStarCatalog.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-08-03 20:36:11.000000 sherlockpipe-0.9.7/sherlockpipe/star/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5202 2020-08-15 06:07:03.000000 sherlockpipe-0.9.7/sherlockpipe/test.py
+-rwxrwxrwx   0 root         (0) root         (0)      540 2020-08-07 11:53:36.000000 sherlockpipe-0.9.7/sherlockpipe/transitresult.py
+-rwxrwxrwx   0 root         (0) root         (0)    15945 2020-08-16 15:23:40.000000 sherlockpipe-0.9.7/sherlockpipe/watson.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-08-03 20:36:11.000000 sherlockpipe-0.9.7/sherlockpipe/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8876 2020-08-16 16:05:15.000000 sherlockpipe-0.9.7/sherlockpipe/__main__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-08-16 19:02:52.000000 sherlockpipe-0.9.7/sherlockpipe.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)        1 2020-08-16 19:02:51.000000 sherlockpipe-0.9.7/sherlockpipe.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)    13708 2020-08-16 19:02:51.000000 sherlockpipe-0.9.7/sherlockpipe.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       85 2020-08-16 19:02:51.000000 sherlockpipe-0.9.7/sherlockpipe.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1815 2020-08-16 19:02:51.000000 sherlockpipe-0.9.7/sherlockpipe.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2020-08-16 19:02:51.000000 sherlockpipe-0.9.7/sherlockpipe.egg-info/top_level.txt
```

### Comparing `sherlockpipe-0.9.6/PKG-INFO` & `sherlockpipe-0.9.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherlockpipe
-Version: 0.9.6
+Version: 0.9.7
 Summary: Search for Hints of Exoplanets fRom Lightcurves Of spaCe based seeKers
 Home-page: https://github.com/franpoz/SHERLOCK
 Author: F.J. Pozuelos & M. Dévora
 Author-email: fjpozuelos@uliege.be
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/sherlock3.png?raw=true">
@@ -31,19 +31,30 @@
         You can run SHERLOCK PIPEline as a standalone package by using:
         
         ```python3 -m sherlockpipe --properties my_properties.yaml```
         
         You only need to provide a YAML file with any of the properties contained in the internal 
         [properties.yaml](https://github.com/franpoz/SHERLOCK/blob/master/sherlockpipe/properties.yaml)
         provided by the pipeline. The most important keys to be defined in your YAML file are those under
-        the `GLOBAL OBJECTS RUN SETUP` and `SECTOR OBJECTS RUN SETUP` because they contain the object ids
+        the `GLOBAL OBJECTS RUN SETUP` and `SECTOR OBJECTS RUN SETUP` sections because they contain the object ids
         or files to be analysed in the execution. You'd need to fill at least one of those keys for the
         pipeline to do anything. If you still have any doubts please refer to the 
         [examples/properties](https://github.com/franpoz/SHERLOCK/tree/master/examples/properties.) directory 
         
+        ### WATSON launch
+        SHERLOCK PIPEline comes with a submodule to examine and fit the most promising transit candidates
+        found by any of its executions. By calling:
+        
+        ```python3 sherlockpipe.watson --object_dir $your_sherlock_object_results_dir```
+        
+        you will run the vetting and fitting process for the object. You will be prompted to select which
+        of the found candidates you'd like to vet & fit and then, an automatic (long) task will begin.
+        You could watch the generated results under `$your_sherlock_object_results_dir/$candidate_selection_number`
+        `vetting` and `fit` directories.
+        
         ## SHERLOCK PIPEline Workflow
         It is important to note that SHERLOCK PIPEline uses some csv files with TOIs, KOIs and EPIC IDs
         from the TESS, Kepler and K2 missions. Therefore your first execution of the pipeline might
         take longer because it will download the information.
         
         ### Provisioning of light curve
         The light curve for every input object needs to be obtained from its mission database. For this we 
@@ -122,46 +133,46 @@
         1           0.8111  29.04     1816.10 9.08    5.88    0.068667  0.88          nan           0.01116           I                   
         2           1.0093  32.41     1817.05 8.80    5.59    nan       0.90          nan           0.01291           I                   
         6           3.4035  45.05     1819.35 6.68    5.97    0.059784  1.00          nan           0.02904           I      
         ```
         * Runs directories: Containing png images of the detrended fluxes and their suggested transits.
         Example of one detrended flux transit selection image:
         <p align="center">
-          <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/example_run.png">
+          <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/example_run.png">
         </p>
         
         * Light curve csv file: The original (before pre-processing) PDCSAP signal stored in three columns: 
-        `#TBJD`, `flux` and `flux_err`. Example content:
+        `#time`, `flux` and `flux_err`. Example content:
         ```
-        #TBJD,flux,flux_err
+        #time,flux,flux_err
         1816.0895073542242,0.9916135,0.024114653
         1816.0908962630185,1.0232307,0.024185425
         1816.0922851713472,1.0293404,0.024151148
         1816.0936740796774,1.000998,0.024186047
         1816.0950629880074,1.0168158,0.02415397
         1816.0964518968017,1.0344968,0.024141008
         1816.0978408051305,1.0061758,0.024101004
         ...
         ```
         * Candidates csv file: Containing the same information than the Most Promising Candidates log but
         in a csv format so it can be read by future additions to the pipeline like vetting or fitting
         endpoints.
         * Lomb-Scargle periodogram plot: Showing the period strengths. Example:
         <p align="center">
-          <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/periodogram.png">
+          <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/periodogram.png">
         </p>
         
         * RMS masking plot: In case the High RMS masking pre-processing is enabled. Example:
         <p align="center">
-          <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/rms.png">
+          <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/rms.png">
         </p>
         
         * Phase-folded period plot: In case auto-detrend or manual period detrend is enabled.
         <p align="center">
-          <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/autodetrend.png">
+          <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/autodetrend.png">
         </p>
         
         ### Dependencies
         All the needed dependencies should be included by your `pip` installation of SHERLOCK. 
         These are the Python libraries which are <b>required</b> for <i>SHERLOCK</i> to be run:
         * numpy: If you run into problems by installing numpy, it might be helpful to install 
         the next packages (if you're under an Ubuntu distribution)
```

### Comparing `sherlockpipe-0.9.6/README.md` & `sherlockpipe-0.9.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,30 @@
 You can run SHERLOCK PIPEline as a standalone package by using:
 
 ```python3 -m sherlockpipe --properties my_properties.yaml```
 
 You only need to provide a YAML file with any of the properties contained in the internal 
 [properties.yaml](https://github.com/franpoz/SHERLOCK/blob/master/sherlockpipe/properties.yaml)
 provided by the pipeline. The most important keys to be defined in your YAML file are those under
-the `GLOBAL OBJECTS RUN SETUP` and `SECTOR OBJECTS RUN SETUP` because they contain the object ids
+the `GLOBAL OBJECTS RUN SETUP` and `SECTOR OBJECTS RUN SETUP` sections because they contain the object ids
 or files to be analysed in the execution. You'd need to fill at least one of those keys for the
 pipeline to do anything. If you still have any doubts please refer to the 
 [examples/properties](https://github.com/franpoz/SHERLOCK/tree/master/examples/properties.) directory 
 
+### WATSON launch
+SHERLOCK PIPEline comes with a submodule to examine and fit the most promising transit candidates
+found by any of its executions. By calling:
+
+```python3 sherlockpipe.watson --object_dir $your_sherlock_object_results_dir```
+
+you will run the vetting and fitting process for the object. You will be prompted to select which
+of the found candidates you'd like to vet & fit and then, an automatic (long) task will begin.
+You could watch the generated results under `$your_sherlock_object_results_dir/$candidate_selection_number`
+`vetting` and `fit` directories.
+
 ## SHERLOCK PIPEline Workflow
 It is important to note that SHERLOCK PIPEline uses some csv files with TOIs, KOIs and EPIC IDs
 from the TESS, Kepler and K2 missions. Therefore your first execution of the pipeline might
 take longer because it will download the information.
 
 ### Provisioning of light curve
 The light curve for every input object needs to be obtained from its mission database. For this we 
@@ -114,46 +125,46 @@
 1           0.8111  29.04     1816.10 9.08    5.88    0.068667  0.88          nan           0.01116           I                   
 2           1.0093  32.41     1817.05 8.80    5.59    nan       0.90          nan           0.01291           I                   
 6           3.4035  45.05     1819.35 6.68    5.97    0.059784  1.00          nan           0.02904           I      
 ```
 * Runs directories: Containing png images of the detrended fluxes and their suggested transits.
 Example of one detrended flux transit selection image:
 <p align="center">
-  <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/example_run.png">
+  <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/example_run.png">
 </p>
 
 * Light curve csv file: The original (before pre-processing) PDCSAP signal stored in three columns: 
-`#TBJD`, `flux` and `flux_err`. Example content:
+`#time`, `flux` and `flux_err`. Example content:
 ```
-#TBJD,flux,flux_err
+#time,flux,flux_err
 1816.0895073542242,0.9916135,0.024114653
 1816.0908962630185,1.0232307,0.024185425
 1816.0922851713472,1.0293404,0.024151148
 1816.0936740796774,1.000998,0.024186047
 1816.0950629880074,1.0168158,0.02415397
 1816.0964518968017,1.0344968,0.024141008
 1816.0978408051305,1.0061758,0.024101004
 ...
 ```
 * Candidates csv file: Containing the same information than the Most Promising Candidates log but
 in a csv format so it can be read by future additions to the pipeline like vetting or fitting
 endpoints.
 * Lomb-Scargle periodogram plot: Showing the period strengths. Example:
 <p align="center">
-  <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/periodogram.png">
+  <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/periodogram.png">
 </p>
 
 * RMS masking plot: In case the High RMS masking pre-processing is enabled. Example:
 <p align="center">
-  <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/rms.png">
+  <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/rms.png">
 </p>
 
 * Phase-folded period plot: In case auto-detrend or manual period detrend is enabled.
 <p align="center">
-  <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/autodetrend.png">
+  <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/autodetrend.png">
 </p>
 
 ### Dependencies
 All the needed dependencies should be included by your `pip` installation of SHERLOCK. 
 These are the Python libraries which are <b>required</b> for <i>SHERLOCK</i> to be run:
 * numpy: If you run into problems by installing numpy, it might be helpful to install 
 the next packages (if you're under an Ubuntu distribution)
```

### Comparing `sherlockpipe-0.9.6/setup.py` & `sherlockpipe-0.9.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sherlockpipe", # Replace with your own username
-    version="0.9.6",
+    version="0.9.7",
     author="F.J. Pozuelos & M. Dévora",
     author_email="fjpozuelos@uliege.be",
     description="Search for Hints of Exoplanets fRom Lightcurves Of spaCe based seeKers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/franpoz/SHERLOCK",
     packages=setuptools.find_packages(),
```

### Comparing `sherlockpipe-0.9.6/sherlockpipe/sherlock.py` & `sherlockpipe-0.9.7/sherlockpipe/sherlock.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,28 +15,35 @@
 from sherlockpipe.objectinfo.InputObjectInfo import InputObjectInfo
 from sherlockpipe.objectinfo.MissionFfiIdObjectInfo import MissionFfiIdObjectInfo
 from sherlockpipe.objectinfo.MissionInputObjectInfo import MissionInputObjectInfo
 from sherlockpipe.objectinfo.MissionFfiCoordsObjectInfo import MissionFfiCoordsObjectInfo
 from sherlockpipe.objectinfo.preparer.MissionFfiLightcurveBuilder import MissionFfiLightcurveBuilder
 from sherlockpipe.objectinfo.preparer.MissionInputLightcurveBuilder import MissionInputLightcurveBuilder
 from sherlockpipe.objectinfo.preparer.MissionLightcurveBuilder import MissionLightcurveBuilder
+from sherlockpipe.objectinfo.InvalidNumberOfSectorsError import InvalidNumberOfSectorsError
 from sherlockpipe.scoring.BasicSignalSelector import BasicSignalSelector
 from sherlockpipe.scoring.SnrBorderCorrectedSignalSelector import SnrBorderCorrectedSignalSelector
 from sherlockpipe.scoring.QuorumSnrBorderCorrectedSignalSelector import QuorumSnrBorderCorrectedSignalSelector
 from sherlockpipe.ois.OisManager import OisManager
+from sherlockpipe.search_zones.HabitableSearchZone import HabitableSearchZone
+from sherlockpipe.search_zones.OptimisticHabitableSearchZone import OptimisticHabitableSearchZone
 from sherlockpipe.star.HabitabilityCalculator import HabitabilityCalculator
 from sherlockpipe.transitresult import TransitResult
 from multiprocessing import Pool
 from scipy.signal import argrelextrema, savgol_filter
 from scipy.ndimage.interpolation import shift
 from scipy import stats
 from wotan import flatten
 from astropy.stats import sigma_clip
 
 class Sherlock:
+    """
+    Main SHERLOCK PIPEline class to be used for loading input, setting up the running parameters and launch the
+    analysis of the desired TESS, Kepler, K2 or csv objects light curves.
+    """
     TOIS_CSV_URL = 'https://exofop.ipac.caltech.edu/tess/download_toi.php?sort=toi&output=csv'
     CTOIS_CSV_URL = 'https://exofop.ipac.caltech.edu/tess/download_ctoi.php?sort=ctoi&output=csv'
     KOIS_LIST_URL = 'https://exofop.ipac.caltech.edu/kepler/targets.php?sort=num-pc&page1=1&ipp1=100000&koi1=&koi2='
     KOI_TARGET_URL = 'https://exofop.ipac.caltech.edu/kepler/edit_target.php?id={$id}'
     KOI_TARGET_URL_NEW = 'https://exoplanetarchive.ipac.caltech.edu/cgi-bin/nstedAPI/nph-nstedAPI?table=cumulative'
     EPIC_TARGET_URL_NEW = 'https://exoplanetarchive.ipac.caltech.edu/cgi-bin/nstedAPI/nph-nstedAPI?table=k2candidates'
     MASK_MODES = ['mask', 'subtract']
@@ -59,34 +66,67 @@
     wl_max = {}
     report = {}
     ois = None
     config_step = 0
     ois_manager = OisManager()
     use_ois = False
 
-    def __init__(self, object_infos):
+    def __init__(self, object_infos: list):
+        """
+        Initializes a Sherlock object, loading the OIs from the csvs, setting up the detrend and transit configurations,
+        storing the provided object_infos list and initializing the builders to be used to prepare the light curves for
+        the provided object_infos.
+        @param object_infos: a list of objects information to be analysed
+        @type object_infos: a list of ObjectInfo implementations to be resolved and analysed
+        """
         self.setup_files()
         self.setup_detrend()
         self.setup_transit_adjust_params()
         self.object_infos = object_infos
-        self.lightcurve_builders = {}
-        self.lightcurve_builders[InputObjectInfo] = MissionInputLightcurveBuilder()
-        self.lightcurve_builders[MissionInputObjectInfo] = MissionInputLightcurveBuilder()
-        self.lightcurve_builders[MissionObjectInfo] = MissionLightcurveBuilder()
-        self.lightcurve_builders[MissionFfiIdObjectInfo] = MissionFfiLightcurveBuilder()
-        self.lightcurve_builders[MissionFfiCoordsObjectInfo] = MissionFfiLightcurveBuilder()
+        self.lightcurve_builders = {InputObjectInfo: MissionInputLightcurveBuilder(),
+                                    MissionInputObjectInfo: MissionInputLightcurveBuilder(),
+                                    MissionObjectInfo: MissionLightcurveBuilder(),
+                                    MissionFfiIdObjectInfo: MissionFfiLightcurveBuilder(),
+                                    MissionFfiCoordsObjectInfo: MissionFfiLightcurveBuilder()}
+        self.search_zones_resolvers = {'hz': HabitableSearchZone(),
+                                       'ohz': OptimisticHabitableSearchZone()}
 
     def setup_files(self, results_dir=RESULTS_DIR):
+        """
+        Loads the objects of interest data from the downloaded CSVs.
+        @param results_dir:
+        @type results_dir:
+        @return: the Sherlock object itself
+        @rtype: Sherlock
+        """
         self.results_dir = results_dir
         self.load_ois()
         return self
 
     def setup_detrend(self, initial_smooth=True, initial_rms_mask=True, initial_rms_threshold=1.5,
                       initial_rms_bin_hours=3, n_detrends=6, detrend_method="biweight", cores=1,
                       auto_detrend_periodic_signals=False, auto_detrend_ratio=1/4, auto_detrend_method="biweight"):
+        """
+        Configures the values for the detrends steps.
+        @param initial_smooth: whether to execute an initial local noise reduction before the light curve analysis
+        @param initial_rms_mask: whether to execute high RMS areas masking before the light curve analysis
+        @param initial_rms_threshold: the high RMS areas limit to be applied multiplied by the RMS median
+        @param initial_rms_bin_hours: the high RMS areas binning
+        @param n_detrends: the number of detrends to be applied to the PDCSAP_FLUX curve for each run.
+        @param detrend_method: the type of algorithm to be used for the detrending
+        @param cores: the number of CPU cores to be used for the detrending process
+        @param auto_detrend_periodic_signals: whether to search for intense periodicities from the LS periodogram and
+        perform an initial detrending based on them.
+        @param auto_detrend_ratio: the factor to apply to the highest periodicity found in the LS periodogram which will
+        be used for the initial detrend.
+        @param auto_detrend_method: the detrend method to be applied with the highest periodicity found in the LS
+        periodogram
+        @return: the Sherlock object itself
+        @rtype: Sherlock
+        """
         if detrend_method not in self.VALID_DETREND_METHODS:
             raise ValueError("Provided detrend method '" + detrend_method + "' is not allowed.")
         if auto_detrend_method not in self.VALID_PERIODIC_DETREND_METHODS:
             raise ValueError("Provided periodic detrend method '" + auto_detrend_method + "' is not allowed.")
         self.initial_rms_mask = initial_rms_mask
         self.initial_rms_threshold = initial_rms_threshold
         self.initial_rms_bin_hours = initial_rms_bin_hours
@@ -101,88 +141,154 @@
                                   [4, 3], [4, 3], [4, 4], [4, 4], [4, 4], [4, 4], [5, 4], [5, 4], [5, 4], [5, 4],
                                   [6, 4], [6, 4], [6, 4], [6, 4]]
         self.detrend_plot_axis.append([1,1])
         self.detrend_plot_axis.append([2,1])
         self.detrend_plot_axis.append([3,1])
         return self
 
-    def setup_transit_adjust_params(self, max_runs=10, period_protec=10, period_min=0.5, period_max=20, bin_minutes=10,
-                                    run_cores=NUM_CORES, snr_min=5, sde_min=5, fap_max=0.1, mask_mode="mask",
-                                    best_signal_algorithm='border-correct', quorum_strength=1):
+    def setup_transit_adjust_params(self, max_runs=10, min_sectors=1, max_sectors=999999, period_protec=10,
+                                    search_zone=None, period_min=0.5, period_max=20, bin_minutes=10, run_cores=NUM_CORES, snr_min=5,
+                                    sde_min=5, fap_max=0.1, mask_mode="mask", best_signal_algorithm='border-correct',
+                                    quorum_strength=1):
+        """
+        Configures the values to be used for the transit fitting and the main run loop.
+        @param max_runs: the max number of runs to be executed for each object.
+        @param min_sectors: the minimum number of sectors/quarters for an object to be analysed
+        @param max_sectors: the maximum number of sectors/quarters for an object to be analysed
+        @param period_protec: the maximum period to be used to calculate the minimum transit duration
+        @param search_zone: the zone where sherlock should be searching transits for. If set, period_min and period_max
+        are to be ignored because they will be generated for the selected zone.
+        @param period_min: the minimum period to search transits for
+        @param period_max: the maximum period to search transits for
+        @param bin_minutes:
+        @param run_cores: the number of CPU cores to use for the transit fitting
+        @param snr_min: the minimum SNR accepted to continue the analysis for an object
+        @param sde_min: the minimum SDE accepted to continue the analysis for an object
+        @param fap_max: the maximum FAP accepted to continue the analysis for an object
+        @param mask_mode: the way to remove every run-selected transit influence in the light curve. 'mask' and
+        'subtract' are available
+        @param best_signal_algorithm: the way to calculate the best signal for each object run. 'basic', 'border-correct'
+        and 'quorum' are available.
+        @param quorum_strength: if quorum is selected as best_signal_algorithm this value will be used for the votes
+        weight.
+        @return: the Sherlock object itself
+        @rtype: Sherlock
+        """
         if mask_mode not in self.MASK_MODES:
             raise ValueError("Provided mask mode '" + mask_mode + "' is not allowed.")
         if best_signal_algorithm not in self.VALID_SIGNAL_SELECTORS:
             raise ValueError("Provided best signal algorithm '" + best_signal_algorithm + "' is not allowed.")
         self.max_runs = max_runs
+        self.min_sectors = min_sectors
+        self.max_sectors = max_sectors
         self.run_cores = run_cores
         self.mask_mode = mask_mode
         self.period_protec = period_protec
         self.period_min = period_min
         self.period_max = period_max
         self.bin_minutes = bin_minutes
         self.snr_min = snr_min
         self.sde_min = sde_min
         self.fap_max = fap_max
-        self.signal_score_selectors = {}
-        self.signal_score_selectors[self.VALID_SIGNAL_SELECTORS[0]] = BasicSignalSelector()
-        self.signal_score_selectors[self.VALID_SIGNAL_SELECTORS[1]] = SnrBorderCorrectedSignalSelector()
-        self.signal_score_selectors[self.VALID_SIGNAL_SELECTORS[2]] = QuorumSnrBorderCorrectedSignalSelector(quorum_strength)
+        self.search_zone = search_zone
+        self.signal_score_selectors = {self.VALID_SIGNAL_SELECTORS[0]: BasicSignalSelector(),
+                                       self.VALID_SIGNAL_SELECTORS[1]: SnrBorderCorrectedSignalSelector(),
+                                       self.VALID_SIGNAL_SELECTORS[2]: QuorumSnrBorderCorrectedSignalSelector(
+                                           quorum_strength)}
         self.best_signal_algorithm = best_signal_algorithm
         return self
 
     def refresh_ois(self):
+        """
+        Downloads the TOIs, KOIs and EPIC OIs into csv files.
+        @return: the Sherlock object itself
+        @rtype: Sherlock
+        """
         self.ois_manager.update_tic_csvs()
         self.ois_manager.update_kic_csvs()
         self.ois_manager.update_epic_csvs()
         return self
 
     def load_ois(self):
+        """
+        Loads the csv OIs files into memory
+        @return: the Sherlock object itself
+        @rtype: Sherlock
+        """
         self.ois = self.ois_manager.load_ois()
         return self
 
     def filter_hj_ois(self):
+        """
+        Filters the in-memory OIs given some basic filters associated to hot jupiters properties. This method is added
+        as an example
+        @return: the Sherlock object itself
+        @rtype: Sherlock
+        """
         self.use_ois = True
         self.ois = self.ois[self.ois["Disposition"].notnull()]
         self.ois = self.ois[self.ois["Period (days)"].notnull()]
         self.ois = self.ois[self.ois["Planet Radius (R_Earth)"].notnull()]
         self.ois = self.ois[self.ois["Planet Insolation (Earth Flux)"].notnull()]
         self.ois = self.ois[self.ois["Depth (ppm)"].notnull()]
         self.ois = self.ois[(self.ois["Disposition"] == "KP") | (self.ois["Disposition"] == "CP")]
         self.ois = self.ois[self.ois["Period (days)"] < 10]
         self.ois = self.ois[self.ois["Planet Radius (R_Earth)"] > 5]
         self.ois = self.ois[self.ois["Planet Insolation (Earth Flux)"] > 4]
         self.ois.sort_values(by=['Object Id', 'OI'])
         return self
 
     def filter_ois(self, function):
+        """
+        Applies a function accepting the Sherlock objects of interests dataframe and stores the result into the
+        Sherlock same ois dataframe.
+        @param function: the function to be applied to filter the Sherlock OIs.
+        @return: the Sherlock object itself
+        @rtype: Sherlock
+        """
         self.use_ois = True
         self.ois = function(self.ois)
         return self
 
     def limit_ois(self, offset=0, limit=0):
+        """
+        Limits the in-memory loaded OIs given an offset and a limit (like a pagination)
+        @param offset:
+        @param limit:
+        @return: the Sherlock object itself
+        @rtype: Sherlock
+        """
         if limit == 0:
             limit = len(self.ois.index)
         self.ois = self.ois[offset:limit]
         return self
 
     def run(self):
+        """
+        Entrypoint of Sherlock which launches the main execution for all the input object_infos
+        """
         self.__setup_logging()
         logging.info('SHERLOCK (Searching for Hints of Exoplanets fRom Lightcurves Of spaCe-base seeKers)')
         logging.info('Version %s', self.VERSION)
         if len(self.object_infos) == 0 and self.use_ois:
             self.object_infos = [MissionObjectInfo(object_id, 'all')
                                  for object_id in self.ois["Object Id"].astype('string').unique()]
         for object_info in self.object_infos:
             self.__run_object(object_info)
 
     def __run_object(self, object_info):
+        """
+        Performs the analysis for one object_info
+        @param object_info: The object to be analysed.
+        @type object_info: ObjectInfo
+        """
+        sherlock_id = object_info.sherlock_id()
+        mission_id = object_info.mission_id()
         try:
-            time, flux, star_info, transits_min_count, cadence = self.__prepare(object_info)
-            sherlock_id = object_info.sherlock_id()
-            mission_id = object_info.mission_id()
+            time, flux, star_info, transits_min_count, cadence, sectors = self.__prepare(object_info)
             id_run = 1
             best_signal_score = 1
             self.report[sherlock_id] = []
             logging.info('================================================')
             logging.info('SEARCH RUNS')
             logging.info('================================================')
             while best_signal_score == 1 and id_run <= self.max_runs:
@@ -199,14 +305,24 @@
                 object_report["snr"] = transit_results[signal_selection.curve_index].snr
                 object_report["sde"] = transit_results[signal_selection.curve_index].sde
                 object_report["fap"] = transit_results[signal_selection.curve_index].fap
                 object_report["border_score"] = transit_results[signal_selection.curve_index].border_score
                 object_report["period"] = transit_results[signal_selection.curve_index].period
                 object_report["duration"] = transit_results[signal_selection.curve_index].duration * 60 * 24
                 object_report["t0"] = transit_results[signal_selection.curve_index].t0
+                object_report["depth"] = transit_results[signal_selection.curve_index].depth
+                object_report['rp_rs'] = transit_results[signal_selection.curve_index].results.rp_rs
+                real_transit_args = np.argwhere(~np.isnan(transit_results[signal_selection.curve_index]
+                                                          .results.transit_depths))
+                object_report["transit_times"] = np.array(transit_results[signal_selection.curve_index]
+                                                          .results.transit_times)[real_transit_args.flatten()]
+                object_report["transit_times"] = ','.join(map(str, object_report["transit_times"]))
+                object_report["sectors"] = ','.join(map(str, sectors))
+                object_report["ffi"] = isinstance(object_info, MissionFfiIdObjectInfo) or \
+                                       isinstance(object_info, MissionFfiCoordsObjectInfo)
                 if self.ois is not None:
                     existing_period_in_object = self.ois[(self.ois["Object Id"] == mission_id) &
                                                          (0.95 < self.ois["Period (days)"] / object_report["period"]) &
                                                          (self.ois["Period (days)"] / object_report["period"] < 1.05)]
                     existing_period_in_oi = existing_period_in_object[existing_period_in_object["OI"].notnull()]
                     object_report["oi"] = existing_period_in_oi["OI"].iloc[0] if len(
                         existing_period_in_oi.index) > 0 else np.nan
@@ -217,50 +333,76 @@
                     time, flux = self.__apply_mask_from_transit_results(time, flux, transit_results, signal_selection.curve_index)
                     id_run += 1
                     if id_run > self.max_runs:
                         logging.info("Max runs limit of %.0f is reached. Stopping.", self.max_runs)
                 else:
                     logging.info('New best signal does not look very promising. End')
                 self.report[sherlock_id].append(object_report)
-            sherlock_id = object_info.sherlock_id()
             self.__setup_object_report_logging(sherlock_id)
             object_dir = self.__init_object_dir(object_info.sherlock_id())
             logging.info("Listing most promising candidates for ID %s:", sherlock_id)
-            logging.info("%-12s%-8s%-10s%-8s%-8s%-8s%-10s%-14s%-14s%-18s%-20s", "Detrend no.", "Period", "Duration", "T0", "SNR",
-                         "SDE", "FAP", "Border_score", "Matching OI", "Semi-major axis", "Habitability Zone")
+            logging.info("%-12s%-8s%-10s%-8s%-8s%-8s%-8s%-10s%-14s%-14s%-18s%-18s%-20s", "Detrend no.", "Period",
+                         "Duration", "T0", "Depth", "SNR", "SDE", "FAP", "Border_score", "Matching OI", "Planet radius",
+                         "Semi-major axis", "Habitability Zone")
             if sherlock_id in self.report:
-                candidates_df = pandas.DataFrame(columns=['curve', 'period', 'duration', 't0', 'snr', 'sde', 'fap',
-                                                  'border_score', 'oi', 'a', 'hz'])
+                candidates_df = pandas.DataFrame(columns=['curve', 'period', 'duration', 't0', 'depth', 'snr', 'sde',
+                                                          'fap', 'border_score', 'oi', 'planet_radius', 'a', 'hz'])
+                i = 1
                 for report in self.report[sherlock_id]:
                     a, habitability_zone = HabitabilityCalculator()\
                         .calculate_hz_score(star_info.teff, star_info.mass, star_info.lum, report["period"]) \
                         if star_info.teff is not None and star_info.lum is not None and star_info.mass is not None \
                         else "-"
                     report['a'] = a
                     report['hz'] = habitability_zone
-                    logging.info("%-12s%-8.4f%-10.2f%-8.2f%-8.2f%-8.2f%-10.6f%-14.2f%-14s%-18.5f%-20s",
+                    if star_info.radius_assumed:
+                        report['rad_p'] = "-"
+                        report['rp_rs'] = "-"
+                    else:
+                        report['rad_p'] = star_info.radius * math.sqrt(report["depth"] / 1000) / 0.0091577
+                    logging.info("%-12s%-8.4f%-10.2f%-8.2f%-8.3f%-8.2f%-8.2f%-10.6f%-14.2f%-14s%-18.5f%-18.5f%-20s",
                                  report["curve"], report["period"],
-                                 report["duration"], report["t0"], report["snr"], report["sde"], report["fap"],
-                                 report["border_score"], report["oi"], a, habitability_zone)
+                                 report["duration"], report["t0"], report["depth"], report["snr"], report["sde"],
+                                 report["fap"], report["border_score"], report["oi"], report['rad_p'], a,
+                                 habitability_zone)
                     candidates_df = candidates_df.append(report, ignore_index=True)
+                    latte_input_df = pandas.DataFrame(columns=['TICID', 'sectors', 'transits', 'BLS', 'model', 'FFI'])
+                    latte_input_df = latte_input_df.append({"TICID": report["Object Id"], "sectors": report["sectors"],
+                                           "transits": report["transit_times"], "BLS": False, "model": 0,
+                                           "FFI": report["ffi"]}, ignore_index=True)
+                    run_dir = self.__init_object_run_dir(sherlock_id, i)
+                    latte_input_df.to_csv(run_dir + "best_signal_latte_input.csv", index=False)
+                    i = i + 1
                 candidates_df.to_csv(object_dir + "candidates.csv", index=False)
+        except InvalidNumberOfSectorsError as e:
+            logging.exception(str(e))
+            print(e)
+            self.__remove_object_dir(sherlock_id)
         except Exception as e:
             logging.exception(str(e))
             print(e)
 
     def __init_object_dir(self, object_id, clean_dir=False):
         dir = self.results_dir + str(object_id)
-        if clean_dir and os.path.exists(dir) and os.path.isdir(dir):
-            shutil.rmtree(dir, ignore_errors=True)
+        dir = dir.replace(" ", "_")
+        if clean_dir:
+            self.__remove_object_dir(object_id)
         if not os.path.exists(dir):
             os.makedirs(dir)
         return dir + "/"
 
+    def __remove_object_dir(self, object_id):
+        dir = self.results_dir + str(object_id)
+        dir = dir.replace(" ", "_")
+        if os.path.exists(dir) and os.path.isdir(dir):
+            shutil.rmtree(dir, ignore_errors=True)
+
     def __init_object_run_dir(self, object_id, run_no, clean_dir=False):
         dir = self.results_dir + str(object_id) + "/" + str(run_no)
+        dir = dir.replace(" ", "_")
         if clean_dir and os.path.exists(dir) and os.path.isdir(dir):
             shutil.rmtree(dir, ignore_errors=True)
         if not os.path.exists(dir):
             os.makedirs(dir)
         return dir + "/"
 
     def __setup_logging(self):
@@ -296,87 +438,125 @@
         logger.addHandler(handler)
 
     def __prepare(self, object_info):
         sherlock_id = object_info.sherlock_id()
         object_dir = self.__setup_object_logging(sherlock_id)
         logging.info('ID: %s', sherlock_id)
         lc, star_info, transits_min_count, sectors, quarters = self.lightcurve_builders[type(object_info)].build(object_info)
+        if star_info is not None:
+            logging.info('================================================')
+            logging.info('STELLAR PROPERTIES FOR THE SIGNAL SEARCH')
+            logging.info('================================================')
+            logging.info("Star catalog info downloaded.")
+            if star_info.mass is None or np.isnan(star_info.mass):
+                logging.info("Star catalog doesn't provide mass. Assuming M=0.1Msun")
+                star_info.assume_model_mass()
+            if star_info.radius is None or np.isnan(star_info.radius):
+                logging.info("Star catalog doesn't provide radius. Assuming R=0.1Rsun")
+                star_info.assume_model_radius()
+            logging.info('limb-darkening estimates using quadratic LD (a,b)= %s', star_info.ld_coefficients)
+            logging.info('mass = %.6f', star_info.mass)
+            logging.info('mass_min = %.6f', star_info.mass_min)
+            logging.info('mass_max = %.6f', star_info.mass_max)
+            logging.info('radius = %.6f', star_info.radius)
+            logging.info('radius_min = %.6f', star_info.radius_min)
+            logging.info('radius_max = %.6f', star_info.radius_max)
+        if not star_info.radius_assumed and not star_info.mass_assumed and star_info.teff is not None:
+            star_df = pandas.DataFrame(columns=['R_star', 'R_star_lerr', 'R_star_uerr', 'M_star', 'M_star_lerr',
+                                              'M_star_uerr', 'Teff_star', 'Teff_star_lerr', 'Teff_star_uerr'])
+            star_df = star_df.append({'R_star': star_info.radius, 'R_star_lerr': star_info.radius - star_info.radius_min,
+                            'R_star_uerr': star_info.radius_max - star_info.radius,
+                            'M_star': star_info.mass, 'M_star_lerr': star_info.mass - star_info.mass_min,
+                            'M_star_uerr': star_info.mass_max - star_info.mass,
+                            'Teff_star': star_info.teff, 'Teff_star_lerr': 200, 'Teff_star_uerr': 200},
+                           ignore_index=True)
+            star_df.to_csv(object_dir + "params_star.csv", index=False)
         logging.info('================================================')
         logging.info('USER DEFINITIONS')
         logging.info('================================================')
         if self.detrend_method == "gp":
             logging.info('Detrend method: Gaussian Process Matern 2/3')
         else:
             logging.info('Detrend method: Bi-Weight')
         logging.info('No of detrend models applied: %s', self.n_detrends)
         logging.info('Minimum number of transits: %s', transits_min_count)
         logging.info('Period planet protected: %.1f', self.period_protec)
+        lightcurve_timespan = lc.time[len(lc.time) - 1] - lc.time[0]
+        if self.search_zone is not None and not (star_info.mass_assumed or star_info.radius_assumed):
+            logging.info("Selected search zone: %s. Minimum and maximum periods will be calculated.", self.search_zone)
+            period_min, period_max = self.search_zones_resolvers[self.search_zone].calculate_period_range(star_info)
+            logging.info("Selected search zone periods are [%.2f, %.2f] days", period_min, period_max)
+            if period_min > lightcurve_timespan or period_max > lightcurve_timespan:
+                logging.info("Selected search zone period values are greater than lightcurve dataset. " +
+                             "Defaulting to minimum and maximum input periods.")
+            else:
+                self.period_min = period_min
+                self.period_max = period_max
+        elif self.search_zone is not None:
+            logging.info("Selected search zone was %s but star catalog info was not found or wasn't complete. " +
+                         "Defaulting to minimum and maximum input periods.", self.search_zone)
         logging.info('Minimum Period (d): %.1f', self.period_min)
         logging.info('Maximum Period (d): %.1f', self.period_max)
         logging.info('Binning size (min): %.1f', self.bin_minutes)
         if object_info.initial_mask is not None:
             logging.info('Mask: yes')
         else:
             logging.info('Mask: no')
         logging.info('Threshold limit for SNR: %.1f', self.snr_min)
         logging.info('Threshold limit for SDE: %.1f', self.sde_min)
         logging.info('Threshold limit for FAP: %.1f', self.fap_max)
         logging.info('Signal scoring algorithm: %s', self.best_signal_algorithm)
         if self.best_signal_algorithm == self.VALID_SIGNAL_SELECTORS[2]:
             logging.info('Quorum algorithm vote strength: %.0f',
                          self.signal_score_selectors[self.VALID_SIGNAL_SELECTORS[2]].strength)
-        if star_info is not None:
-            logging.info('================================================')
-            logging.info('STELLAR PROPERTIES FOR THE SIGNAL SEARCH')
-            logging.info('================================================')
-            logging.info("Star catalog info downloaded.")
-            if star_info.mass is None or np.isnan(star_info.mass):
-                logging.info("Star catalog doesn't provide mass. Assuming M=0.1Msun")
-                star_info.assume_model_mass()
-            if star_info.radius is None or np.isnan(star_info.radius):
-                logging.info("Star catalog doesn't provide radius. Assuming R=0.1Rsun")
-                star_info.assume_model_radius()
-            logging.info('limb-darkening estimates using quadratic LD (a,b)= %s', star_info.ld_coefficients)
-            logging.info('mass = %.6f', star_info.mass)
-            logging.info('mass_min = %.6f', star_info.mass_min)
-            logging.info('mass_max = %.6f', star_info.mass_max)
-            logging.info('radius = %.6f', star_info.radius)
-            logging.info('radius_min = %.6f', star_info.radius_min)
-            logging.info('radius_max = %.6f', star_info.radius_max)
         if sectors is not None:
+            sectors_count = len(sectors)
             logging.info('================================================')
             logging.info('SECTORS INFO')
             logging.info('================================================')
             logging.info('Sectors : %s', sectors)
             logging.info('No of sectors available: %s', len(sectors))
+            if sectors_count < self.min_sectors or sectors_count > self.max_sectors:
+                raise InvalidNumberOfSectorsError("The object " + sherlock_id + " contains " + str(sectors_count) +
+                                                  " sectors and the min and max selected are [" +
+                                                  str(self.min_sectors) + ", " + str(self.max_sectors) + "].")
         if quarters is not None:
+            sectors_count = len(quarters)
             logging.info('================================================')
             logging.info('QUARTERS INFO')
             logging.info('================================================')
             logging.info('Quarters : %s', quarters)
+            if sectors_count < self.min_sectors or sectors_count > self.max_sectors:
+                raise InvalidNumberOfSectorsError("The object " + sherlock_id + " contains " + str(sectors_count) +
+                                                  " quarters and the min and max selected are [" +
+                                                  str(self.min_sectors) + ", " + str(self.max_sectors) + "].")
         flux = lc.flux
         flux_err = lc.flux_err
         time = lc.time
         transit_duration = wotan.t14(R_s=star_info.radius, M_s=star_info.mass, P=self.period_protec,
                                      small_planet=True)  # we define the typical duration of a small planet in this star
         if self.detrend_method == 'gp':
             self.wl_min[sherlock_id] = 1
             self.wl_max[sherlock_id] = 12
         else:
             self.wl_min[sherlock_id] = 3 * transit_duration  # minimum transit duration
             self.wl_max[sherlock_id] = 20 * transit_duration  # maximum transit duration
         lc = lk.LightCurve(time=time, flux=flux, flux_err=flux_err)
-        lc_df = pandas.DataFrame(columns=['#TBJD', 'flux', 'flux_err'])
-        lc_df['#TBJD'] = lc.time
+        lc_df = pandas.DataFrame(columns=['#time', 'flux', 'flux_err'])
+        lc_df['#time'] = lc.time
         lc_df['flux'] = lc.flux
         lc_df['flux_err'] = lc.flux_err
         lc_df.to_csv(object_dir + "lc.csv", index=False)
         lc = lc.remove_outliers(sigma_lower=float('inf'), sigma_upper=3)  # remove outliers over 3sigma
+        cadence_array = np.diff(lc.time) * 24 * 60
+        cadence_array = cadence_array[~np.isnan(cadence_array)]
+        cadence_array = cadence_array[cadence_array > 0]
+        cadence = np.nanmedian(cadence_array)
         clean_time, flatten_flux, clean_flux_err = self.__clean_initial_flux(object_info, lc.time, lc.flux, lc.flux_err,
-                                                                             star_info)
+                                                                             star_info, cadence)
         lc = lk.LightCurve(time=clean_time, flux=flatten_flux, flux_err=clean_flux_err)
         period = None
         periodogram = lc.to_periodogram(minimum_period=self.wl_min[sherlock_id], oversample_factor=10)
         periodogram.plot(view='period', scale='log')
         plt.title(str(sherlock_id) + " Lightcurve periodogram")
         plt.savefig(object_dir + "Periodogram_" + str(sherlock_id) + ".png")
         plt.clf()
@@ -404,25 +584,23 @@
             initial_mask = object_info.initial_mask
             logging.info('** Applying ordered masks to the lightcurve **')
             for mask_range in initial_mask:
                 mask = [(clean_time < mask_range[0] if not math.isnan(mask_range[1]) else False) |
                         (clean_time > mask_range[1] if not math.isnan(mask_range[1]) else False)]
                 clean_time = clean_time[mask]
                 flatten_flux = flatten_flux[mask]
-        cadence_array = np.diff(clean_time) * 24 * 60
-        cadence_array = cadence_array[~np.isnan(cadence_array)]
-        cadence_array = cadence_array[cadence_array > 0]
-        cadence = np.nanmedian(cadence_array)
-        return clean_time, flatten_flux, star_info, transits_min_count, cadence
+        return clean_time, flatten_flux, star_info, transits_min_count, cadence, \
+               sectors if sectors is not None else quarters
 
-    def __clean_initial_flux(self, object_info, time, flux, flux_err, star_info):
+    def __clean_initial_flux(self, object_info, time, flux, flux_err, star_info, cadence):
         clean_time = time
         clean_flux = flux
         clean_flux_err = flux_err
-        if self.initial_smooth or (self.initial_rms_mask and object_info.initial_mask is None):
+        is_short_cadence = round(cadence) <= 5
+        if (is_short_cadence and self.initial_smooth) or (self.initial_rms_mask and object_info.initial_mask is None):
             logging.info('================================================')
             logging.info('INITIAL FLUX CLEANING')
             logging.info('================================================')
         if self.initial_rms_mask and object_info.initial_mask is None:
             logging.info('Masking high RMS areas by a factor of %.2f with %.1f hours binning',
                          self.initial_rms_threshold, self.initial_rms_bin_hours)
             bins_per_day = 24 / self.initial_rms_bin_hours
@@ -448,30 +626,29 @@
             axs[1].scatter(time[high_std_mask], before_flux[high_std_mask], linewidth=1, color='red', alpha=1.0, label="High RMS")
             axs[1].legend(loc="upper right")
             axs[1].set_title("Total and masked high RMS flux")
             fig.suptitle(str(star_info.object_id) + " High RMS Mask")
             plot_dir = self.__init_object_dir(star_info.object_id)
             fig.savefig(plot_dir + 'High_RMS_Mask_' + str(star_info.object_id) + '.png', dpi=200)
             fig.clf()
-        if self.initial_smooth:
+        if is_short_cadence and self.initial_smooth:
             logging.info('Applying Savitzky-Golay filter')
             clean_flux = savgol_filter(clean_flux, 11, 3)
         return clean_time, clean_flux, clean_flux_err
 
     def __calculate_max_significant_period(self, lc, periodogram):
-        #TODO improve selection of max period
         #max_accepted_period = (lc.time[len(lc.time) - 1] - lc.time[0]) / 4
         max_accepted_period = np.float64(10)
         accepted_power_indexes = np.transpose(np.argwhere(periodogram.power > 0.0008))[0]
         period_values = [p.value for p in periodogram.period]
         accepted_period_indexes = np.transpose(np.argwhere(period_values < max_accepted_period))[0]
         accepted_indexes = [i for i in accepted_period_indexes if i in accepted_power_indexes]
         local_extrema = argrelextrema(periodogram.power[accepted_indexes], np.greater)[0]
         accepted_indexes = np.array(accepted_indexes)[local_extrema]
-        # TODO check whether this fits better
+        # TODO related to https://github.com/franpoz/SHERLOCK/issues/29 check whether this fits better
         #  periodogram.period[np.argmax(periodogram.power)]
         period = None
         if len(accepted_indexes) > 0:
             relevant_periods = periodogram.period[accepted_indexes]
             period = min(relevant_periods)
             period = period.value
             logging.info("Auto-Detrend found the next important periods: " + str(relevant_periods) + ". Period used " +
@@ -719,15 +896,15 @@
             bin_means, bin_edges, binnumber = stats.binned_statistic(tls_results.folded_phase, tls_results.folded_y,
                                                                      statistic='mean', bins=bins)
             bin_stds, _, _ = stats.binned_statistic(tls_results.folded_phase, tls_results.folded_y, statistic='std', bins=bins)
             bin_width = (bin_edges[1] - bin_edges[0])
             bin_centers = bin_edges[1:] - bin_width / 2
             bin_size = int(round(bin_width * 60 * 24 * transit_result.period))
             ax2.errorbar(bin_centers, bin_means, yerr=bin_stds / 2, xerr=bin_width / 2, marker='o', markersize=4,
-                         color='teal', alpha=1, linestyle='none', label='Bin size: ' + str(bin_size) + "m")
+                         color='darkorange', alpha=1, linestyle='none', label='Bin size: ' + str(bin_size) + "m")
             ax2.legend(loc="upper right")
         ax3 = plt.gca()
         ax3.axvline(transit_result.period, alpha=0.4, lw=3)
         plt.xlim(np.min(tls_results.periods), np.max(tls_results.periods))
         for n in range(2, 10):
             ax3.axvline(n * tls_results.period, alpha=0.4, lw=1, linestyle="dashed")
             ax3.axvline(tls_results.period / n, alpha=0.4, lw=1, linestyle="dashed")
```

### Comparing `sherlockpipe-0.9.6/sherlockpipe/sherlock_tests.py` & `sherlockpipe-0.9.7/sherlockpipe/sherlock_tests.py`

 * *Files identical despite different names*

### Comparing `sherlockpipe-0.9.6/sherlockpipe/transitresult.py` & `sherlockpipe-0.9.7/sherlockpipe/transitresult.py`

 * *Files identical despite different names*

### Comparing `sherlockpipe-0.9.6/sherlockpipe/__main__.py` & `sherlockpipe-0.9.7/sherlockpipe/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sherlockpipe.objectinfo.MissionInputObjectInfo import MissionInputObjectInfo
 from sherlockpipe.objectinfo.MissionObjectInfo import MissionObjectInfo
 from argparse import ArgumentParser
 from os import path
 import yaml
 
 if __name__ == '__main__':
-    ap = ArgumentParser(description='Lightcurve Analysis Tool for Transiting Exoplanets')
+    ap = ArgumentParser(description='Searching for Hints of Exoplanets fRom Lightcurves Of spaCe-based seeKers')
     ap.add_argument('--properties', help="Additional properties to be loaded into Sherlock run ", required=True)
     args = ap.parse_args()
     resources_dir = path.join(path.dirname(__file__))
     sherlock_user_properties = yaml.load(open(resources_dir + "/" + 'properties.yaml'))
     user_properties = yaml.load(open(args.properties))
     sherlock_user_properties.update(user_properties)
 
@@ -115,15 +115,18 @@
                        sherlock_user_properties["INITIAL_HIGH_RMS_MASK"],
                        sherlock_user_properties["INITIAL_HIGH_RMS_THRESHOLD"],
                        sherlock_user_properties["INITIAL_HIGH_RMS_BIN_HOURS"],
                        sherlock_user_properties["DETRENDS_NUMBER"],
                        sherlock_user_properties["DETREND_METHOD"], sherlock_user_properties["DETREND_CORES"],
                        sherlock_user_properties["AUTO_DETREND_ENABLED"], sherlock_user_properties["AUTO_DETREND_RATIO"],
                        sherlock_user_properties["AUTO_DETREND_METHOD"]) \
-        .setup_transit_adjust_params(sherlock_user_properties["MAX_RUNS"], sherlock_user_properties["PERIOD_PROTECT"],
+        .setup_transit_adjust_params(sherlock_user_properties["MAX_RUNS"], sherlock_user_properties["MIN_SECTORS"],
+                                     sherlock_user_properties["MAX_SECTORS"],
+                                     sherlock_user_properties["PERIOD_PROTECT"],
+                                     sherlock_user_properties["SEARCH_ZONE"],
                                      sherlock_user_properties["PERIOD_MIN"], sherlock_user_properties["PERIOD_MAX"],
                                      sherlock_user_properties["BIN_MINUTES"], sherlock_user_properties["CPU_CORES"],
                                      sherlock_user_properties["SNR_MIN"], sherlock_user_properties["SDE_MIN"],
                                      sherlock_user_properties["FAP_MAX"], sherlock_user_properties["MASK_MODE"],
                                      sherlock_user_properties["BEST_SIGNAL_ALGORITHM"],
                                      sherlock_user_properties["QUORUM_STRENGTH"]) \
         .run()
```

### Comparing `sherlockpipe-0.9.6/sherlockpipe.egg-info/PKG-INFO` & `sherlockpipe-0.9.7/sherlockpipe.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherlockpipe
-Version: 0.9.6
+Version: 0.9.7
 Summary: Search for Hints of Exoplanets fRom Lightcurves Of spaCe based seeKers
 Home-page: https://github.com/franpoz/SHERLOCK
 Author: F.J. Pozuelos & M. Dévora
 Author-email: fjpozuelos@uliege.be
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/sherlock3.png?raw=true">
@@ -31,19 +31,30 @@
         You can run SHERLOCK PIPEline as a standalone package by using:
         
         ```python3 -m sherlockpipe --properties my_properties.yaml```
         
         You only need to provide a YAML file with any of the properties contained in the internal 
         [properties.yaml](https://github.com/franpoz/SHERLOCK/blob/master/sherlockpipe/properties.yaml)
         provided by the pipeline. The most important keys to be defined in your YAML file are those under
-        the `GLOBAL OBJECTS RUN SETUP` and `SECTOR OBJECTS RUN SETUP` because they contain the object ids
+        the `GLOBAL OBJECTS RUN SETUP` and `SECTOR OBJECTS RUN SETUP` sections because they contain the object ids
         or files to be analysed in the execution. You'd need to fill at least one of those keys for the
         pipeline to do anything. If you still have any doubts please refer to the 
         [examples/properties](https://github.com/franpoz/SHERLOCK/tree/master/examples/properties.) directory 
         
+        ### WATSON launch
+        SHERLOCK PIPEline comes with a submodule to examine and fit the most promising transit candidates
+        found by any of its executions. By calling:
+        
+        ```python3 sherlockpipe.watson --object_dir $your_sherlock_object_results_dir```
+        
+        you will run the vetting and fitting process for the object. You will be prompted to select which
+        of the found candidates you'd like to vet & fit and then, an automatic (long) task will begin.
+        You could watch the generated results under `$your_sherlock_object_results_dir/$candidate_selection_number`
+        `vetting` and `fit` directories.
+        
         ## SHERLOCK PIPEline Workflow
         It is important to note that SHERLOCK PIPEline uses some csv files with TOIs, KOIs and EPIC IDs
         from the TESS, Kepler and K2 missions. Therefore your first execution of the pipeline might
         take longer because it will download the information.
         
         ### Provisioning of light curve
         The light curve for every input object needs to be obtained from its mission database. For this we 
@@ -122,46 +133,46 @@
         1           0.8111  29.04     1816.10 9.08    5.88    0.068667  0.88          nan           0.01116           I                   
         2           1.0093  32.41     1817.05 8.80    5.59    nan       0.90          nan           0.01291           I                   
         6           3.4035  45.05     1819.35 6.68    5.97    0.059784  1.00          nan           0.02904           I      
         ```
         * Runs directories: Containing png images of the detrended fluxes and their suggested transits.
         Example of one detrended flux transit selection image:
         <p align="center">
-          <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/example_run.png">
+          <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/example_run.png">
         </p>
         
         * Light curve csv file: The original (before pre-processing) PDCSAP signal stored in three columns: 
-        `#TBJD`, `flux` and `flux_err`. Example content:
+        `#time`, `flux` and `flux_err`. Example content:
         ```
-        #TBJD,flux,flux_err
+        #time,flux,flux_err
         1816.0895073542242,0.9916135,0.024114653
         1816.0908962630185,1.0232307,0.024185425
         1816.0922851713472,1.0293404,0.024151148
         1816.0936740796774,1.000998,0.024186047
         1816.0950629880074,1.0168158,0.02415397
         1816.0964518968017,1.0344968,0.024141008
         1816.0978408051305,1.0061758,0.024101004
         ...
         ```
         * Candidates csv file: Containing the same information than the Most Promising Candidates log but
         in a csv format so it can be read by future additions to the pipeline like vetting or fitting
         endpoints.
         * Lomb-Scargle periodogram plot: Showing the period strengths. Example:
         <p align="center">
-          <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/periodogram.png">
+          <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/periodogram.png">
         </p>
         
         * RMS masking plot: In case the High RMS masking pre-processing is enabled. Example:
         <p align="center">
-          <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/rms.png">
+          <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/rms.png">
         </p>
         
         * Phase-folded period plot: In case auto-detrend or manual period detrend is enabled.
         <p align="center">
-          <img width="350" src="https://github.com/franpoz/SHERLOCK/blob/master/images/autodetrend.png">
+          <img width="80%" src="https://github.com/franpoz/SHERLOCK/blob/master/images/autodetrend.png">
         </p>
         
         ### Dependencies
         All the needed dependencies should be included by your `pip` installation of SHERLOCK. 
         These are the Python libraries which are <b>required</b> for <i>SHERLOCK</i> to be run:
         * numpy: If you run into problems by installing numpy, it might be helpful to install 
         the next packages (if you're under an Ubuntu distribution)
```

