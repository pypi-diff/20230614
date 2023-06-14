# Comparing `tmp/CLEMENTDNA-1.0.2.tar.gz` & `tmp/CLEMENTDNA-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CLEMENTDNA-1.0.2.tar", last modified: Tue Jun 13 05:26:43 2023, max compression
+gzip compressed data, was "dist/CLEMENTDNA-1.0.4.tar", last modified: Wed Jun 14 08:37:29 2023, max compression
```

## Comparing `CLEMENTDNA-1.0.2.tar` & `CLEMENTDNA-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 goldpm1   (1311) goldpm1   (1315)        0 2023-06-13 05:26:43.000000 CLEMENTDNA-1.0.2/
-drwxrwxrwx   0 goldpm1   (1311) goldpm1   (1315)        0 2023-06-13 05:26:43.000000 CLEMENTDNA-1.0.2/CLEMENT/
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    10330 2023-06-12 08:19:40.000000 CLEMENTDNA-1.0.2/CLEMENT/Bunch.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    27642 2023-06-13 05:22:12.000000 CLEMENTDNA-1.0.2/CLEMENT/CLEMENT.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    11903 2023-06-12 10:13:06.000000 CLEMENTDNA-1.0.2/CLEMENT/EMhard.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     4277 2023-06-12 09:23:54.000000 CLEMENTDNA-1.0.2/CLEMENT/EMsoft.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     5952 2023-06-12 09:11:09.000000 CLEMENTDNA-1.0.2/CLEMENT/Estep.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     7854 2023-06-12 09:28:52.000000 CLEMENTDNA-1.0.2/CLEMENT/Mstep.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)        7 2023-05-30 07:50:32.000000 CLEMENTDNA-1.0.2/CLEMENT/__init__.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     1244 2023-06-12 08:40:02.000000 CLEMENTDNA-1.0.2/CLEMENT/comb.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     6209 2023-06-12 08:45:36.000000 CLEMENTDNA-1.0.2/CLEMENT/datapreparation.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)      524 2023-06-12 08:56:28.000000 CLEMENTDNA-1.0.2/CLEMENT/extract.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)      809 2023-06-12 09:06:46.000000 CLEMENTDNA-1.0.2/CLEMENT/filetype.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     2935 2023-05-30 07:50:28.000000 CLEMENTDNA-1.0.2/CLEMENT/graph.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    19712 2023-06-12 10:20:43.000000 CLEMENTDNA-1.0.2/CLEMENT/isparent.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    30544 2023-06-12 09:22:08.000000 CLEMENTDNA-1.0.2/CLEMENT/miscellaneous.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     3353 2023-06-12 09:06:25.000000 CLEMENTDNA-1.0.2/CLEMENT/phylogeny.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    14518 2023-06-12 08:59:50.000000 CLEMENTDNA-1.0.2/CLEMENT/visualizationeachstep.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     9388 2023-06-12 09:05:53.000000 CLEMENTDNA-1.0.2/CLEMENT/visualizationpair.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     6841 2023-06-12 09:29:57.000000 CLEMENTDNA-1.0.2/CLEMENT/visualizationsingle.py
--rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     7007 2023-06-12 09:30:39.000000 CLEMENTDNA-1.0.2/CLEMENT/visualizationsinglesoft.py
-drwxrwxrwx   0 goldpm1   (1311) goldpm1   (1315)        0 2023-06-13 05:26:43.000000 CLEMENTDNA-1.0.2/CLEMENTDNA.egg-info/
--rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)      529 2023-06-13 05:26:42.000000 CLEMENTDNA-1.0.2/CLEMENTDNA.egg-info/PKG-INFO
--rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)      653 2023-06-13 05:26:42.000000 CLEMENTDNA-1.0.2/CLEMENTDNA.egg-info/SOURCES.txt
--rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)        1 2023-06-13 05:26:42.000000 CLEMENTDNA-1.0.2/CLEMENTDNA.egg-info/dependency_links.txt
--rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)       49 2023-06-13 05:26:42.000000 CLEMENTDNA-1.0.2/CLEMENTDNA.egg-info/entry_points.txt
--rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)      113 2023-06-13 05:26:42.000000 CLEMENTDNA-1.0.2/CLEMENTDNA.egg-info/requires.txt
--rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)        8 2023-06-13 05:26:42.000000 CLEMENTDNA-1.0.2/CLEMENTDNA.egg-info/top_level.txt
--rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)      529 2023-06-13 05:26:43.000000 CLEMENTDNA-1.0.2/PKG-INFO
--rwxrwxrwx   0 goldpm1   (1311) goldpm1   (1315)     4277 2023-06-13 05:26:17.000000 CLEMENTDNA-1.0.2/README.md
--rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)       79 2023-06-13 05:26:43.000000 CLEMENTDNA-1.0.2/setup.cfg
--rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)     1141 2023-06-13 05:26:11.000000 CLEMENTDNA-1.0.2/setup.py
+drwxrwxrwx   0 goldpm1   (1311) goldpm1   (1315)        0 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/
+drwxrwxrwx   0 goldpm1   (1311) goldpm1   (1315)        0 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/CLEMENT/
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    10330 2023-06-12 08:19:40.000000 CLEMENTDNA-1.0.4/CLEMENT/Bunch.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    29749 2023-06-14 08:18:53.000000 CLEMENTDNA-1.0.4/CLEMENT/CLEMENT.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    11933 2023-06-14 07:36:28.000000 CLEMENTDNA-1.0.4/CLEMENT/EMhard.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     4277 2023-06-12 09:23:54.000000 CLEMENTDNA-1.0.4/CLEMENT/EMsoft.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     5952 2023-06-12 09:11:09.000000 CLEMENTDNA-1.0.4/CLEMENT/Estep.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     7854 2023-06-12 09:28:52.000000 CLEMENTDNA-1.0.4/CLEMENT/Mstep.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)        7 2023-05-30 07:50:32.000000 CLEMENTDNA-1.0.4/CLEMENT/__init__.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     1244 2023-06-12 08:40:02.000000 CLEMENTDNA-1.0.4/CLEMENT/comb.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     6209 2023-06-12 08:45:36.000000 CLEMENTDNA-1.0.4/CLEMENT/datapreparation.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)      524 2023-06-12 08:56:28.000000 CLEMENTDNA-1.0.4/CLEMENT/extract.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)      809 2023-06-12 09:06:46.000000 CLEMENTDNA-1.0.4/CLEMENT/filetype.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     2825 2023-06-14 07:29:30.000000 CLEMENTDNA-1.0.4/CLEMENT/graph.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    19712 2023-06-12 10:20:43.000000 CLEMENTDNA-1.0.4/CLEMENT/isparent.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    30629 2023-06-14 08:20:09.000000 CLEMENTDNA-1.0.4/CLEMENT/miscellaneous.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     3425 2023-06-14 07:38:39.000000 CLEMENTDNA-1.0.4/CLEMENT/phylogeny.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)    14598 2023-06-14 08:16:10.000000 CLEMENTDNA-1.0.4/CLEMENT/visualizationeachstep.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     9420 2023-06-14 08:16:55.000000 CLEMENTDNA-1.0.4/CLEMENT/visualizationpair.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     6908 2023-06-14 08:18:01.000000 CLEMENTDNA-1.0.4/CLEMENT/visualizationsingle.py
+-rwxrwxr--   0 goldpm1   (1311) goldpm1   (1315)     7007 2023-06-12 09:30:39.000000 CLEMENTDNA-1.0.4/CLEMENT/visualizationsinglesoft.py
+drwxrwxrwx   0 goldpm1   (1311) goldpm1   (1315)        0 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/CLEMENTDNA.egg-info/
+-rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)      529 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/CLEMENTDNA.egg-info/PKG-INFO
+-rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)      653 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/CLEMENTDNA.egg-info/SOURCES.txt
+-rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)        1 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/CLEMENTDNA.egg-info/dependency_links.txt
+-rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)       49 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/CLEMENTDNA.egg-info/entry_points.txt
+-rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)      113 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/CLEMENTDNA.egg-info/requires.txt
+-rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)        8 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/CLEMENTDNA.egg-info/top_level.txt
+-rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)      529 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/PKG-INFO
+-rwxrwxrwx   0 goldpm1   (1311) goldpm1   (1315)     4470 2023-06-14 08:36:59.000000 CLEMENTDNA-1.0.4/README.md
+-rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)      103 2023-06-14 08:37:29.000000 CLEMENTDNA-1.0.4/setup.cfg
+-rw-rw-rw-   0 goldpm1   (1311) goldpm1   (1315)     1174 2023-06-14 08:37:04.000000 CLEMENTDNA-1.0.4/setup.py
```

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/Bunch.py` & `CLEMENTDNA-1.0.4/CLEMENT/Bunch.py`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/CLEMENT.py` & `CLEMENTDNA-1.0.4/CLEMENT/CLEMENT.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 
 def main():
     import os, subprocess, sys, datetime, time, io, contextlib, argparse
     import numpy as np
     import pandas as pd
 
-    print ( "Package directory : {}".format (  os.path.dirname(__file__) ) )
+    print ( "Package directory : {}\n".format (  os.path.dirname(__file__) ) )
     if os.path.dirname(__file__) not in sys.path:
        sys.path.append  ( os.path.dirname(__file__) )
        
     import EMhard, EMsoft, Estep, Mstep, Bunch, miscellaneous, datapreparation, phylogeny, visualizationsingle, visualizationsinglesoft, filetype
+    
+    #python3 CLEMENT.py	--INPUT_TSV "/data/project/Alzheimer/YSscript/EM_MRS/Packaging/CLEMENT/example/2.CellData/MRS_2D/M1-5_M1-7/M1-5_M1-7_input.txt"  --CLEMENT_DIR "/data/project/Alzheimer/YSscript/EM_MRS/Packaging/CLEMENT/example/2.CellData/MRS_2D/M1-5_M1-7"  		--NUM_CLONE_TRIAL_START 2 		--NUM_CLONE_TRIAL_END 6  --RANDOM_PICK 500
 
 
     pd.options.mode.chained_assignment = None
 
     kwargs = {}
 
     parser = argparse.ArgumentParser(description='The below is usage direction.')
-    parser.add_argument('--INPUT_TSV', type=str, default="/data/project/Alzheimer/YSscript/EM_MRS/CLEMENT/example/2.CellData/MRS_2D/M1-3_M1-8/M1-3_M1-8_input.txt",  help="Path where TSV format file locate. (Important : DIRECTORY (X), File path (O) )")
-    parser.add_argument('--CLEMENT_DIR', default="/data/project/Alzheimer/YSscript/EM_MRS/CLEMENT/example/2.CellData/MRS_2D/M1-3_M1-8",   help="Directory where input and output of CLEMENT deposits (Important : DIRECTORY (O), File path (X) )")
+    parser.add_argument('--INPUT_TSV', type=str, default="",  help="Path where TSV format file locate. (Important : DIRECTORY (X), File path (O) )")
+    parser.add_argument('--CLEMENT_DIR', default="",   help="Directory where input and output of CLEMENT deposits (Important : DIRECTORY (O), File path (X) )")
     parser.add_argument('--MODE', type=str, choices=["Hard", "Both"], default="Both", help="Selection of clustering method. Default : Both")
     parser.add_argument('--RANDOM_PICK', type=int, default=-1,  help="The number of mutations to alleviate the computational load. Default : -1 (load the whole data)")
     parser.add_argument('--KMEANS_CLUSTERNO',  type=int, default=8,  choices=range(5, 20), help="Number of initial K-means cluster. Recommendation : 5~8 for one-sample, 8-15 for larger-sample. Default : 8")
     parser.add_argument('--NUM_CLONE_TRIAL_START', type=int, default=3,  help="Minimum number of expected cluster_hards (initation of K). Default : 3")
     parser.add_argument('--NUM_CLONE_TRIAL_END', type=int, default=5, choices=range(1, 11), help="Maximum number of expected cluster_hards (termination of K). Default : 5")
     parser.add_argument('--TRIAL_NO', default=5, type=int, choices=range(1, 21),  help="The number of trials in each candidate clone number. DO NOT recommend over 20. Default : 5")
     parser.add_argument('--MAXIMUM_NUM_PARENT',  default=1, type=int,  help="The maximum number of parents in the given samples. Recommendation : 0-2. Default : 1")
     parser.add_argument('--MIN_CLUSTER_SIZE', type=int, default=9, help="The minimum number of membersip in single cluster. Default : 9")
     parser.add_argument('--RANDOM_SEED', type=int, default=1,  help="random_seed for regular random sampling")
     parser.add_argument('--MAKEONE_STRICT', type=int,  choices=[1, 2], default = 1, help="1:strict, 2:lenient. Default : 1")
     parser.add_argument('--TN_CONFIDENTIALITY', default=0.995, type=float, help="Confidentiality that negative being negative (TN). Recommendation : > 0.99. Default : 0.995")
+    parser.add_argument('--FONT_FAMILY', type=str, default="arial", help="Font family that displayed in the plots")
     parser.add_argument('--VERBOSE', type=int, choices=[0, 1, 2, 3], default=2, help="0: Verbose, 3: Concise. Default : 2")
 
 
     args = parser.parse_args()
     kwargs["INPUT_TSV"] = args.INPUT_TSV
     kwargs["INPUT_FILETYPE"], kwargs["NUM_BLOCK"] = filetype.main( kwargs["INPUT_TSV"] )
     kwargs["NUM_BLOCK_INPUT"] =  kwargs["NUM_BLOCK"]
@@ -45,14 +48,15 @@
     kwargs["TRIAL_NO"] = int(args.TRIAL_NO)
     kwargs["VERBOSE"] = int(args.VERBOSE)
     kwargs["MIN_CLUSTER_SIZE"] = int(args.MIN_CLUSTER_SIZE)
     kwargs["KMEANS_CLUSTERNO"] = args.KMEANS_CLUSTERNO
     kwargs["RANDOM_SEED"] = int(args.RANDOM_SEED)
     kwargs["SCORING"] = False
     kwargs["MAKEONE_STRICT"] = int(args.MAKEONE_STRICT)
+    kwargs["FONT_FAMILY"] = str(args.FONT_FAMILY)
     kwargs["CLEMENT_DIR"] = args.CLEMENT_DIR
     if kwargs["CLEMENT_DIR"][-1] == "/":
         kwargs["CLEMENT_DIR"] = kwargs["CLEMENT_DIR"][0:-1]
     kwargs["method"] = "gap+normal"
     kwargs["adjustment"] = "half"
     kwargs["STEP_NO"] = 30
     kwargs["DECISION_STANDARD"]= 0.8 + (0.03 * kwargs ["NUM_BLOCK"])
@@ -77,33 +81,31 @@
 
 
     # membership_answer: ['V1', 'V2', 'FP', 'S0', 'V2', 'S0', 'V2', ....
     # membership_answer_numerical : [0 1 2 3 1 3 1 ...
 
     inputdf, df, np_vaf, np_BQ, membership_answer, mutation_id, samplename_dict_CharacterToNum, kwargs  = datapreparation.main( **kwargs)
 
-    print (kwargs["RANDOM_PICK"])
-
     membership_answer_numerical = np.zeros( kwargs["RANDOM_PICK"], dtype="int")
     membership_answer_numerical_nofp_index = []
 
 
 
     if type(inputdf) != type(False):
         samplename_dict_NumToCharacter = {v: k for k, v in samplename_dict_CharacterToNum.items()}   # {0: 'FP', 1: 'V2', 2: 'S0', 3: 'V1'}
 
         print ("samplename_dict_CharacterToNum = {}\nsamplename_dict_NumToCharacter = {}".format( samplename_dict_CharacterToNum, samplename_dict_NumToCharacter ))
 
         if kwargs["NUM_BLOCK"] == 1:
             x_median = miscellaneous.VAFdensitogram(np_vaf, "INPUT DATA", kwargs["CLEMENT_DIR"] + "/0.inputdata.pdf", **kwargs)
-            visualizationsingle.drawfigure_1d(membership_answer_numerical, "ANSWER_SET (n={})".format(kwargs["RANDOM_PICK"]), kwargs["CLEMENT_DIR"] + "/0.inputdata.pdf", np_vaf, samplename_dict_NumToCharacter, False, -1, list (set (membership_answer_numerical)))
+            visualizationsingle.drawfigure_1d(membership_answer_numerical, "ANSWER_SET (n={})".format(kwargs["RANDOM_PICK"]), kwargs["CLEMENT_DIR"] + "/0.inputdata.pdf", np_vaf, samplename_dict_NumToCharacter, False, -1, list (set (membership_answer_numerical)), **kwargs)
         elif kwargs["NUM_BLOCK"] == 2:
-            visualizationsingle.drawfigure_2d(membership_answer, "ANSWER_SET (n={})".format(kwargs["RANDOM_PICK"]), kwargs["CLEMENT_DIR"] + "/0.inputdata.pdf", np_vaf, samplename_dict_CharacterToNum, False, -1)
+            visualizationsingle.drawfigure_2d(membership_answer, "ANSWER_SET (n={})".format(kwargs["RANDOM_PICK"]), kwargs["CLEMENT_DIR"] + "/0.inputdata.pdf", np_vaf, samplename_dict_CharacterToNum, False, -1, "None", **kwargs)
         elif kwargs["NUM_BLOCK"] >= 3:
-            visualizationsingle.drawfigure_2d(membership_answer, "ANSWER_SET (n={})".format(kwargs["RANDOM_PICK"]), kwargs["CLEMENT_DIR"] + "/0.inputdata.pdf", np_vaf, samplename_dict_CharacterToNum, False, -1, "SVD")
+            visualizationsingle.drawfigure_2d(membership_answer, "ANSWER_SET (n={})".format(kwargs["RANDOM_PICK"]), kwargs["CLEMENT_DIR"] + "/0.inputdata.pdf", np_vaf, samplename_dict_CharacterToNum, False, -1, "SVD", **kwargs)
         subprocess.run(["cp " + kwargs["CLEMENT_DIR"] + "/0.inputdata.pdf  " +  kwargs["CLEMENT_DIR"] + "/candidate/0.inputdata.pdf"], shell=True)
         subprocess.run(["cp " + kwargs["CLEMENT_DIR"] + "/0.inputdata.pdf  " +  kwargs["CLEMENT_DIR"] + "/trial/0.inputdata.pdf"], shell=True)
 
 
     START_TIME = datetime.datetime.now()
 
 
@@ -138,15 +140,16 @@
                 for step_index in range(1, kwargs["STEP_NO"]): 
                     kwargs["STEP"], kwargs["TRIAL"] = step_index, cluster_hard.trialindex_record[ NUM_CLONE ]
                     kwargs["STEP_TOTAL"] = step_index + cluster_hard.stepindex_record [ NUM_CLONE ] - 1
                     
                     print("\t\tstep #{} ( = TOTAL step #{})".format(kwargs["STEP"], kwargs["STEP_TOTAL"]) )
 
                     step_soft = Estep.main(df, np_vaf, np_BQ, step_soft, **kwargs)               # E step
-                    print ( "\t\t\tAfter the E step: {}\tmakeone_index : {}".format( np.unique(step_soft.membership  , return_counts=True), step_soft.makeone_index ) )
+                    #print ( "\t\t\tAfter the E step : {}\tmakeone_index : {}".format( np.unique(step_soft.membership  , return_counts=True), step_soft.makeone_index ) )
+                    print ( "\t\t\tAfter the E step : fp_index {}\tmakeone_index : {}".format( step_soft.fp_index, step_soft.makeone_index ) )
                     step_soft = Mstep.main(df, np_vaf, np_BQ, step_soft, "Soft", **kwargs)     # M step
                     print("\t\t\tAfter the M step : fp_index {}\tmakeone_index {}\tlikelihood : {}".format( step_soft.fp_index, step_soft.makeone_index, round (step_soft.likelihood, 1), step_soft.mixture ))
 
 
                     step_soft.acc(step_soft.mixture, step_soft.membership, step_soft.likelihood, step_soft.membership_p, step_soft.membership_p_normalize, step_soft.makeone_index, step_soft.fp_index, step_index + 1, step_soft.fp_member_index, step_soft.includefp, step_soft.fp_involuntary, step_soft.makeone_prenormalization, step_index, step_index)
 
                     if (miscellaneous.GoStop(step_soft, **kwargs) == "Stop")  :
@@ -238,21 +241,22 @@
 
         for i, priority in enumerate(["1st"]):
             if i >= len (NUM_CLONE_hard):
                 break
             
             print ( "NUM_CLONE_hard (by order): {}".format(NUM_CLONE_hard))
 
-            if cluster_soft.mixture_record [ NUM_CLONE_hard[i] ] == []:
+            if cluster_soft.mixture_record [ NUM_CLONE_hard[i] ] == []: # When soft clustering was unavailable
                 if (priority == "1st") & (kwargs["MODE"] in ["Both"]):
+                    DECISION = "hard_1st"
                     print ("DECISION\t{}".format(DECISION))
                     with open (kwargs["CLEMENT_DIR"] + "/result/CLEMENT_hard_vs_fuzzy.txt", "w", encoding = "utf8") as output_hard_vs_fuzzy:
                         print ("DECISION\t{}".format(DECISION) , file = output_hard_vs_fuzzy )            
                 
-            else:
+            else: # Most of the case
                 if (priority == "1st") &  (kwargs["MODE"] in ["Both"]):
                     moved_col_list = miscellaneous.movedcolumn ( cluster_hard, cluster_soft,  NUM_CLONE_hard[i]  )
                     hard_std = np.std(  cluster_hard.mixture_record [ NUM_CLONE_hard[i] ] [ : , moved_col_list ]   )
                     soft_std = np.std(  cluster_soft.mixture_record [ NUM_CLONE_hard[i] ] [ : , moved_col_list ]   )
                     if ( len (moved_col_list) == 1 )  & (  kwargs["NUM_BLOCK"] == 1 ) :  # Incalculable std in this condition
                         not_moved_col_list = [i for i in list(range ( NUM_CLONE_hard[i] )) if i not in moved_col_list]
                         print ( "moved_col_list = {}\nnot_moved_col_list = {}\ncluster_hard.mixture_record = {}".format (moved_col_list, not_moved_col_list, cluster_hard.mixture_record [ NUM_CLONE_hard[i] ] ))
@@ -273,14 +277,31 @@
                     with open (kwargs["CLEMENT_DIR"] + "/result/CLEMENT_hard_vs_fuzzy.txt", "w", encoding = "utf8") as output_hard_vs_fuzzy:
                         print ( "Moved column : {}".format(moved_col_list), file = output_hard_vs_fuzzy)
                         print ( "Hard (n = {}) : std = {}\tstep = {}\nhard_mixture = {}\n".format( cluster_hard.mixture_record [NUM_CLONE_hard[i]].shape[1],  round( hard_std, 3) ,  cluster_hard.stepindex_record [ NUM_CLONE_hard[i] ],  cluster_hard.mixture_record [ NUM_CLONE_hard[i] ]   ) , file = output_hard_vs_fuzzy  )
                         print ( "Soft (n = {}) : std = {}\tstep = {}\nhard_mixture = {}".format( cluster_soft.mixture_record [NUM_CLONE_hard[i]].shape[1],  round( soft_std, 3) ,  cluster_soft.stepindex_record [ NUM_CLONE_hard[i] ],  cluster_soft.mixture_record [ NUM_CLONE_hard[i] ]   )  , file = output_hard_vs_fuzzy )
                         print ( "ratio : {}".format ( round(soft_std, 3) / round(hard_std, 3) ), file = output_hard_vs_fuzzy )
                         print ("\nsoft 선택 기준 :  < {}\nDECISION\t{}".format(kwargs["DECISION_STANDARD"], DECISION) , file = output_hard_vs_fuzzy )
 
+                
+                ###################################### PHYLOGENY RECONSTRUCTION #######################################
+                if len (cluster_hard.makeone_index_record [NUM_CLONE_hard[i]]) + int ( cluster_hard.includefp_record [NUM_CLONE_hard[i]])  < NUM_CLONE_hard[i]:    # ISPARENT == TRUE
+                    print ("\n\n\t▶▶▶  PHYLOGENY RECONSTRUCTION IN HARD CLUSTERING ◀◀◀")
+                    kwargs["PHYLOGENY_DIR"] = kwargs["CLEMENT_DIR"] + "/CLEMENT_hard_" + priority + ".phylogeny.txt"
+                    f = io.StringIO()
+                    with contextlib.redirect_stdout(f):
+                        membership_child = set ( cluster_hard.makeone_index_record[ NUM_CLONE_hard[i] ] )            # Pick child index only ( e.g.  0, 1, 3)
+                        membership_outside = set (range (0, NUM_CLONE_hard [i] )) - membership_child - set ( [cluster_hard.fp_index_record[ NUM_CLONE_hard[i] ] ] )   # Pick possible parent index only (e.g. 2)
+
+                        g = phylogeny.main(membership_child, membership_outside, cluster_hard.mixture_record[ NUM_CLONE_hard[i] ],  **kwargs)
+
+                    print ( f.getvalue() )    # Print in command line
+                    with open ( kwargs["PHYLOGENY_DIR"] , "w", encoding = "utf8") as phylogeny_file:   # Print in separate file
+                        print (f.getvalue(), file = phylogeny_file)
+                    #########################################################################################################
+
 
 
             with open (kwargs["CLEMENT_DIR"] + "/result/CLEMENT_hard_" + priority + ".results.txt", "w", encoding = "utf8") as output_myEM:
                 print ("NUM_CLONE\t{}\nNUM_CHILD\t{}\nrunningtime\t{}\nFPexistence\t{}\nFPindex\t{}\nmakeone_index\t{}".
                         format(cluster_hard.mixture_record [NUM_CLONE_hard[i]].shape[1] - int (cluster_hard.includefp_record [ NUM_CLONE_hard[i] ]) , len (cluster_hard.makeone_index_record [NUM_CLONE_hard[i]]),   round((datetime.datetime.now() - START_TIME).total_seconds()), cluster_hard.includefp_record [NUM_CLONE_hard[i]], cluster_hard.fp_index_record [NUM_CLONE_hard[i]] , cluster_hard.makeone_index_record [NUM_CLONE_hard[i]]  ), file = output_myEM)
```

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/EMhard.py` & `CLEMENTDNA-1.0.4/CLEMENT/EMhard.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         if kwargs["KMEANS_CLUSTERNO"] < kwargs["NUM_CLONE"]:  
             continue
 
         else:  # Most of the cases
             trial_index, failure_num = 0, 0
             while trial_index < kwargs["TRIAL_NO"]:
                 kwargs["TRIAL"] = trial_index
-                print("\t#Trial #{0}".format(trial_index))
+                print("\tTrial #{0}".format(trial_index))
 
                 step = Bunch.Bunch1(NUM_MUTATION , NUM_BLOCK, NUM_CLONE, kwargs["STEP_NO"])
 
                 step.mixture = miscellaneous.set_initial_parameter(np_vaf, mixture_kmeans, 
                                                                 kwargs["CLEMENT_DIR"] + "/trial/clone" + str(kwargs["NUM_CLONE_NOMINAL"]) + "." + str(kwargs["TRIAL"]) + "-0.initial_kmeans(hard).pdf"  , **kwargs)
                 
                 if np.any(step.mixture < 0) == True: 
@@ -77,15 +77,15 @@
                     #print(",".join(str(row) for row in step.mixture ))
 
 
 
                 for step_index in range(0, kwargs["STEP_NO"]):
                     kwargs["STEP"], kwargs["STEP_TOTAL"] = step_index, step_index
                     kwargs["OPTION"] = "hard"
-                    print ("\t\t# Step #{}".format(step_index))
+                    print ("\t\tStep #{}".format(step_index))
 
                     step = Estep.main(df, np_vaf, np_BQ, step, **kwargs)  
                     
                     
                     ################################ Early terminating condition  (NUM_PARENT, MIN_CLUSTER_SIZE) ################################################
                     if (  NUM_CLONE -  len (step.makeone_index) - int(step.includefp)  > kwargs["MAXIMUM_NUM_PARENT"] ):     #  1st early terminating condition
                         failure_num = failure_num + 1
@@ -144,15 +144,15 @@
                     if kwargs["VERBOSE"] >= 3:
                         print ("\t\t\t failure_num = 1  → Give up and pass to the next trial")
                     
                     failure_num = 0
                     trial_index = trial_index + 1
                 
             i =  trial.find_max_likelihood(0, kwargs["TRIAL_NO"]) 
-            print ("\n\n\tChose {}th trial, {}th step\n\t(trial.likelihood_record : {})\n\tFP_index : {}\n\tlen(fp_member_index) : {}".format(i, trial.max_step_index_record[i], np.round ( trial.likelihood_record ), trial.fp_index_record[i],  len (trial.fp_member_index_record[i] ) ) )
+            print ("\n\n\tIn NUM_CLONE = {}, we chose {}th trial, {}th step\n\t(trial.likelihood_record : {})\n\tFP_index : {}\n\tlen(fp_member_index) : {}".format(NUM_CLONE, i, trial.max_step_index_record[i], np.round ( trial.likelihood_record ), trial.fp_index_record[i],  len (trial.fp_member_index_record[i] ) ) )
 
             if trial.max_step_index_record [i]  != -1:   # If unavailable in this trial
                 os.system ("cp " + kwargs["CLEMENT_DIR"] + "/trial/clone" + str (kwargs["NUM_CLONE"]) + "." + str( i ) + "-"  + str(  trial.max_step_index_record [i]  ) + "\(hard\).pdf" + " " + 
                     kwargs["CLEMENT_DIR"] + "/candidate/clone" + str (kwargs["NUM_CLONE"]) + ".\(hard\).pdf"  ) 
             
             cluster.acc ( trial.mixture_record [i], trial.membership_record [i], trial.likelihood_record [i], trial.membership_p_record [i], trial.membership_p_normalize_record [i], trial.stepindex_record [i], i, trial.max_step_index_record [i], trial.makeone_index_record[i], trial.fp_index_record[i], trial.includefp_record[i], trial.fp_involuntary_record[i], trial.fp_member_index_record [i], **kwargs )
```

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/EMsoft.py` & `CLEMENTDNA-1.0.4/CLEMENT/EMsoft.py`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/Estep.py` & `CLEMENTDNA-1.0.4/CLEMENT/Estep.py`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/Mstep.py` & `CLEMENTDNA-1.0.4/CLEMENT/Mstep.py`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/comb.py` & `CLEMENTDNA-1.0.4/CLEMENT/comb.py`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/datapreparation.py` & `CLEMENTDNA-1.0.4/CLEMENT/datapreparation.py`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/extract.py` & `CLEMENTDNA-1.0.4/CLEMENT/extract.py`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/filetype.py` & `CLEMENTDNA-1.0.4/CLEMENT/filetype.py`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/isparent.py` & `CLEMENTDNA-1.0.4/CLEMENT/isparent.py`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/miscellaneous.py` & `CLEMENTDNA-1.0.4/CLEMENT/miscellaneous.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,20 +319,22 @@
     if output_filename != "NotSave":
         matplotlib.pyplot.savefig(output_filename)
     
     return x_median
 
 
 
-def drawfigure (np_vaf, membership, output_filename):
+def drawfigure (np_vaf, membership, output_filename, **kwargs):
     import palettable
     import matplotlib
     import numpy as np
     import seaborn as sns
 
+    matplotlib.rcParams["font.family"] =  kwargs["FONT_FAMILY"]
+
     tabl = palettable.tableau.Tableau_20.mpl_colors
     colorlist = [i for i in tabl]
 
     if np_vaf.shape[1] == 2:
         matplotlib.pyplot.figure(figsize=(6, 6))
         #matplotlib.pyplot.axis([0,  1,  0,  1])
         for k in set (membership):
@@ -457,15 +459,15 @@
                 if (kwargs["NUM_BLOCK"] == 1) | (cluster.includefp_record [NUM_CLONE] == False): 
                     kmeans = KMeans(n_clusters=NUM_CLONE, init = cluster.mixture_record [NUM_CLONE].transpose() , max_iter=3, random_state=0)  
                 else: 
                     kmeans = KMeans(n_clusters=NUM_CLONE - 1, init = np.delete(cluster.mixture_record [NUM_CLONE].transpose(), cluster.fp_index_record [NUM_CLONE], axis = 0), max_iter=3, random_state=0)  
 
                 kmeans.fit(reference_np)  # nparray
                 Wkb_list.append ( round (math.log10(kmeans.inertia_), 3) )
-                drawfigure (reference_np, kmeans.labels_,  kwargs["CLEMENT_DIR"] + "/Kmeans/Kmeans.clone"  +   str (NUM_CLONE) + "." + str(b) + ".jpg")
+                drawfigure (reference_np, kmeans.labels_,  kwargs["CLEMENT_DIR"] + "/Kmeans/Kmeans.clone"  +   str (NUM_CLONE) + "." + str(b) + ".jpg", **kwargs)
 
             Gap_list [NUM_CLONE] = round ( np.mean(Wkb_list) - Wk, 3)
             Std_list [NUM_CLONE] = round ( np.std (Wkb_list), 3)
             S_list [NUM_CLONE] = round (Std_list[NUM_CLONE] * math.sqrt(1 + Input_B) , 3 )
             
 
             if (kwargs["VERBOSE"] in ["True", "T"]) | (kwargs["VERBOSE"] >= 1):
```

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/phylogeny.py` & `CLEMENTDNA-1.0.4/CLEMENT/phylogeny.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,24 +60,24 @@
 
         # Now, exclude from the list
         completed_parent.append (j_maxmax)
         subset_list_acc.remove(subset_list_maxmax)
         subset_mixture_acc.remove(subset_mixture_maxmax)
         sum_mixture_acc.remove(sum_mixture_maxmax)
 
-        print ("parent No = {0}, parent_mixture = {1}, sum_mixture = {2}, subset_list = {3},  p = {4}".format(j_maxmax,  mixture_total[:,j_maxmax], sum_mixture_maxmax, subset_list_maxmax, p_maxmax ), file = output_file )
-        print ("parent No = {0}, parent_mixture = {1}, sum_mixture = {2}, subset_list = {3},  p = {4}".format(j_maxmax,  mixture_total[:,j_maxmax], sum_mixture_maxmax, subset_list_maxmax, p_maxmax ) )
+        print ("\t\tparent No = {0}, parent_mixture = {1}, sum_mixture = {2}, subset_list = {3},  p = {4}".format(j_maxmax,  mixture_total[:,j_maxmax], np.round(sum_mixture_maxmax, 2), subset_list_maxmax, round (p_maxmax, 2) ), file = output_file )
+        print ("\t\tparent No = {0}, parent_mixture = {1}, sum_mixture = {2}, subset_list = {3},  p = {4}".format(j_maxmax,  mixture_total[:,j_maxmax], np.round(sum_mixture_maxmax, 2), subset_list_maxmax, round (p_maxmax, 2) ) )
         g.intervene (j_maxmax, subset_list_maxmax)           
         for proband_clone_index in subset_list_maxmax:      # 4 -6,  4- 7
             g.addEdge(j_maxmax, proband_clone_index)
 
-    print ("", file = output_file)
-    print ("")
+    print ("\t\t", file = output_file)
+    print ("\t\t")
     for root in completed_parent:
         if g.findparent(root) == "None":   # Run only if root node
             g.dfs(root, kwargs["PHYLOGENY_DIR"])
-        print ("", file = output_file)
-        print ("")
+        print ("\t\t", file = output_file)
+        print ("\t\t")
 
 
     output_file.close()
     return g
```

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/visualizationeachstep.py` & `CLEMENTDNA-1.0.4/CLEMENT/visualizationeachstep.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
     tabl = palettable.tableau.Tableau_20.mpl_colors
     Gr_10 = palettable.scientific.sequential.GrayC_20.mpl_colors
     colorlist = [i for i in tabl]
     if (bunch.includefp == True) & (bunch.fp_index != -1):
         colorlist[bunch.fp_index] = Gr_10[8]
 
-    font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
-    font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
-    for font in font_dirs:
-        matplotlib.font_manager.fontManager.addfont(font)
-    matplotlib.rcParams["font.family"] = 'arial'
+    # font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
+    # font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
+    # for font in font_dirs:
+    #     matplotlib.font_manager.fontManager.addfont(font)
+    matplotlib.rcParams["font.family"] = kwargs["FONT_FAMILY"]
 
     matplotlib.pyplot.figure(figsize=(6, 6))
 
     max_y = 0
 
     x = np.linspace(0, 2, 200)
 
@@ -89,20 +89,19 @@
 
     tabl = palettable.tableau.Tableau_20.mpl_colors
     Gr_10 = palettable.scientific.sequential.GrayC_20.mpl_colors
     colorlist = [i for i in tabl]
     if (bunch.includefp == True) & (bunch.fp_index != -1):
         colorlist[bunch.fp_index] = Gr_10[8]
 
-    font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
-    font_dirs = matplotlib.font_manager.findSystemFonts(
-        fontpaths=font_dir, fontext='ttf')
-    for font in font_dirs:
-        matplotlib.font_manager.fontManager.addfont(font)
-    matplotlib.rcParams["font.family"] = 'arial'
+    # font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
+    # font_dirs = matplotlib.font_manager.findSystemFonts( fontpaths=font_dir, fontext='ttf')
+    # for font in font_dirs:
+    #     matplotlib.font_manager.fontManager.addfont(font)
+    matplotlib.rcParams["font.family"] = kwargs["FONT_FAMILY"]
 
     matplotlib.pyplot.figure(figsize=(6, 6))
     matplotlib.pyplot.xlim(0, 1)
     matplotlib.pyplot.xlabel("VAF x 2 (= Mixture)")
     matplotlib.pyplot.ylabel("count (weighted)")
 
     matplotlib.pyplot.suptitle("clone{}.{}-{},  Total prob = {}".format(kwargs["NUM_CLONE"], kwargs["TRIAL"], kwargs["STEP_TOTAL"], round(bunch.likelihood)), fontsize=20)
@@ -142,19 +141,19 @@
 
     samplename_dict = {k: k for k in range(0, bunch.mixture.shape[1])}
 
     tabl = palettable.tableau.Tableau_20.mpl_colors
     Gr_10 = palettable.scientific.sequential.GrayC_20.mpl_colors
     colorlist = [i for i in tabl]
 
-    font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
-    font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
-    for font in font_dirs:
-        matplotlib.font_manager.fontManager.addfont(font)
-    matplotlib.rcParams["font.family"] = 'arial'
+    # font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
+    # font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
+    # for font in font_dirs:
+    #     matplotlib.font_manager.fontManager.addfont(font)
+    matplotlib.rcParams["font.family"] = kwargs["FONT_FAMILY"]
 
     matplotlib.pyplot.figure(figsize=(6, 6))
     matplotlib.pyplot.axis( [0,  np.max(np_vaf[:, :]) * 2.1, 0,  np.max(np_vaf[:, :]) * 2.1])
     matplotlib.pyplot.xlabel("VAF x 2 of the Sample 1", fontdict={"fontsize": 14})
     matplotlib.pyplot.ylabel("VAF x 2 of the Sample 2", fontdict={"fontsize": 14})
 
     matplotlib.pyplot.suptitle("clone{}.{}-{},  Total prob = {}".format(kwargs["NUM_CLONE"], kwargs["TRIAL"], kwargs["STEP"], round(bunch.likelihood)), fontsize=20)
@@ -206,19 +205,19 @@
 
     samplename_dict = {k: k for k in range(0, bunch.mixture.shape[1])}
 
     tabl = palettable.tableau.Tableau_20.mpl_colors
     Gr_10 = palettable.scientific.sequential.GrayC_20.mpl_colors
     colorlist = [i for i in tabl]
 
-    font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
-    font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
-    for font in font_dirs:
-        matplotlib.font_manager.fontManager.addfont(font)
-    matplotlib.rcParams["font.family"] = 'arial'
+    # font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
+    # font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
+    # for font in font_dirs:
+    #     matplotlib.font_manager.fontManager.addfont(font)
+    matplotlib.rcParams["font.family"] = kwargs["FONT_FAMILY"]
 
     if bunch.includefp == True:
         fp_color_num = samplename_dict[bunch.fp_index]
         colorlist[fp_color_num] = Gr_10[10]
 
     matplotlib.pyplot.figure(figsize=(6, 6))
```

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/visualizationpair.py` & `CLEMENTDNA-1.0.4/CLEMENT/visualizationpair.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import seaborn as sns
 import numpy as np
 from scipy.stats import kde
 import extract
 from sklearn.decomposition import TruncatedSVD, PCA
 
 
-def drawfigure_1d(membership1, sample_dict_rev, membership2, mixture2, output_filename, np_vaf):
+def drawfigure_1d(membership1, sample_dict_rev, membership2, mixture2, output_filename, np_vaf, **kwargs):
     vivid_10 = palettable.cartocolors.qualitative.Vivid_10.mpl_colors
     bdo = palettable.lightbartlein.diverging.BlueDarkOrange18_18.mpl_colors
     tabl = palettable.tableau.Tableau_20.mpl_colors
     Gr_10 = palettable.scientific.sequential.GrayC_20.mpl_colors
     colorlist = [i for i in tabl]
 
-    font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
-    font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
-    for font in font_dirs:
-        matplotlib.font_manager.fontManager.addfont(font)
+    # font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
+    # font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
+    # for font in font_dirs:
+    #     matplotlib.font_manager.fontManager.addfont(font)
     
-    matplotlib.rcParams["font.family"] = 'arial'
+    matplotlib.rcParams["font.family"] = kwargs["FONT_FAMILY"]
 
 
     maxmaxmax_NUM_CLONE = np.max(membership2) + 1
     fig, ax = matplotlib.pyplot.subplots(ncols=2, figsize=(15, 6))
 
     ax[0].set_title("ANSWER FIGURE OF MRS (n = {0})".format(len(membership1)), fontdict = {"fontsize" : 20})
     ax[1].set_title("MYANSWER_NUM_CLONE : {0} (n = {1})".format(maxmaxmax_NUM_CLONE, len(membership2)) , fontdict = {"fontsize" : 20})
```

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/visualizationsingle.py` & `CLEMENTDNA-1.0.4/CLEMENT/visualizationsingle.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 import numpy as np
 from scipy.stats import kde
 import extract
 from sklearn.decomposition import TruncatedSVD, PCA
 from mpl_toolkits import mplot3d
 
 
-def drawfigure_1d(membership, output_suptitle, output_filename, np_vaf, samplename_dict, includefp, fp_index, makeone_index):
+def drawfigure_1d(membership, output_suptitle, output_filename, np_vaf, samplename_dict, includefp, fp_index, makeone_index, **kwargs):
     vivid_10 = palettable.cartocolors.qualitative.Vivid_10.mpl_colors
     bdo = palettable.lightbartlein.diverging.BlueDarkOrange18_18.mpl_colors
     tabl = palettable.tableau.Tableau_20.mpl_colors
     Gr_10 = palettable.scientific.sequential.GrayC_20.mpl_colors
     colorlist = [i for i in tabl]
 
-    font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
-    font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
-    for font in font_dirs:
-        matplotlib.font_manager.fontManager.addfont(font)
+    # font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
+    # font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
+    # for font in font_dirs:
+    #     matplotlib.font_manager.fontManager.addfont(font)
     #print (matplotlib.font_manager.FontProperties(fname = font).get_name())
 
-    matplotlib.rcParams["font.family"] = 'arial'
+    matplotlib.rcParams["font.family"] =  kwargs["FONT_FAMILY"]
     matplotlib.pyplot.style.use("seaborn-white")
 
     if includefp == True:
         colorlist[ fp_index ] = Gr_10[8]       
     
     fig, ax = matplotlib.pyplot.subplots (figsize = (6, 6))
     matplotlib.pyplot.suptitle(output_suptitle, fontsize = 20)
@@ -68,28 +68,28 @@
     if output_filename != "NotSave":
         matplotlib.pyplot.savefig(output_filename)
     matplotlib.pyplot.show()
 
 
 
 
-def drawfigure_2d(membership, output_suptitle, output_filename, np_vaf, samplename_dict, includefp, fp_index, dimensionreduction="None"):
+def drawfigure_2d(membership, output_suptitle, output_filename, np_vaf, samplename_dict, includefp, fp_index, dimensionreduction="None",  **kwargs):
     vivid_10 = palettable.cartocolors.qualitative.Vivid_10.mpl_colors
     bdo = palettable.lightbartlein.diverging.BlueDarkOrange18_18.mpl_colors
     tabl = palettable.tableau.Tableau_20.mpl_colors
     Gr_10 = palettable.scientific.sequential.GrayC_20.mpl_colors
     colorlist = [i for i in tabl]
     
-    font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
-    font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
-    for font in font_dirs:
-        matplotlib.font_manager.fontManager.addfont(font)
+    # font_dir = "/home/goldpm1/miniconda3/envs/cnvpytor/lib/python3.7/site-packages/matplotlib/mpl-data/fonts/ttf/"
+    # font_dirs = matplotlib.font_manager.findSystemFonts(fontpaths=font_dir, fontext='ttf')
+    # for font in font_dirs:
+    #     matplotlib.font_manager.fontManager.addfont(font)
     #print (matplotlib.font_manager.FontProperties(fname = font).get_name())
 
-    matplotlib.rcParams["font.family"] = 'arial'
+    matplotlib.rcParams["font.family"] =  kwargs["FONT_FAMILY"]
     matplotlib.pyplot.style.use("seaborn-white")
 
     fig, ax = matplotlib.pyplot.subplots (figsize = (6, 6))
     
     if dimensionreduction == "SVD":
         print("SVD → 2D")
         tsvd = TruncatedSVD(n_components=2)
```

### Comparing `CLEMENTDNA-1.0.2/CLEMENT/visualizationsinglesoft.py` & `CLEMENTDNA-1.0.4/CLEMENT/visualizationsinglesoft.py`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/CLEMENTDNA.egg-info/PKG-INFO` & `CLEMENTDNA-1.0.4/CLEMENTDNA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CLEMENTDNA
-Version: 1.0.2
+Version: 1.0.4
 Summary: Genomic decomposition and reconstruction of non-tumor diploid subclones
 Home-page: https://github.com/Yonsei-TGIL/CLEMENT
 Download-URL: https://github.com/Yonsei-TGIL/CLEMENT.git
 Author: Young-soo Chung, M.D.
 Author-email: goldpm1@yuhs.ac
 License: GPL v3
 Keywords: CLEMENT,genomic decomposition
```

### Comparing `CLEMENTDNA-1.0.2/CLEMENTDNA.egg-info/SOURCES.txt` & `CLEMENTDNA-1.0.4/CLEMENTDNA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CLEMENTDNA-1.0.2/PKG-INFO` & `CLEMENTDNA-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CLEMENTDNA
-Version: 1.0.2
+Version: 1.0.4
 Summary: Genomic decomposition and reconstruction of non-tumor diploid subclones
 Home-page: https://github.com/Yonsei-TGIL/CLEMENT
 Download-URL: https://github.com/Yonsei-TGIL/CLEMENT.git
 Author: Young-soo Chung, M.D.
 Author-email: goldpm1@yuhs.ac
 License: GPL v3
 Keywords: CLEMENT,genomic decomposition
```

### Comparing `CLEMENTDNA-1.0.2/README.md` & `CLEMENTDNA-1.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # CLEMENT
 - Genomic decomposition and reconstruction of **non-tumor** diploid subclones (2022)
 - CLonal decomposition via Expectation-Maximization algorithm established in Non-Tumor setting
 - Support multiple diploid sample
+- Biallelic variants (Homo, 1/1) can degrade the performance of CLEMENT.
 
 ## Overview of CLEMENT workflow and core algorithms
 <br/>
 
 ![Figure1 overview](https://user-images.githubusercontent.com/56012432/195979886-cd29df09-8291-4150-9001-db7dde5e7567.png)
 <br/>
 
@@ -16,85 +17,98 @@
 - seaborn 0.11.2
 - numpy 1.21.5
 - pandas 1.3.4
 - scikit-learn 1.0.2
 - scipy 1.7.3
 - palettable 3.3.0
 
-### Install from github (requires Python 3.6.* or newer)
+### Install from github
 1. git clone https://github.com/Yonsei-TGIL/CLEMENT.git   
     cd CLEMENT   
     pip3 install .   
-*or*   
+
 2. pip3 install git+https://github.com/Yonsei-TGIL/CLEMENT.git    
 
 ### Install from PyPi
 3. pip3 install CLEMENTDNA   
 
-### Install from Conda
-4. conda install CLEMENTDNA (to be updated)   
-
 ## Version update
-1.0.2 (June 13rd, 2023)
+1.0.4 (June 14h, 2023)
 
 ## Input format
-As now of 1.0.2, CLEMENT only supports standardized TSV input. Examples of input file is shown in "example" directory.
+As now of 1.0.4, CLEMENT only supports standardized TSV input. Examples of input file is shown in _"example"_ directory.
 - 1st column: mutation ID (CHR_POS is recommended)
-- 2nd column: label  (answer), if possible. If user don't know the label (answer), just set 0
+- 2nd column: label (answer), if possible. If user don't know the label (answer), just set 0
 - 3rd column: **Depth1,Alt1,Depth2,Alt2....,Depth_n,Alt_n**    * should be comma-separated, and no space permitted
 - 4th column: **BQ1,BQ2....,BQ_n**    * should be comma-separated, and no space permitted. If absent, CLEMENT set default BQ as 20.
 
 ## Running
-python3 CLEMENT.py [OPTIONS]   
-*or*   
-CLEMENT [OPTIONS]   
+### command line interface
+	CLEMENT [OPTIONS]   
 
 
-**options**
+### options
 
-	These options are regarding User's input and output format.
-		--INPUT_TSV	Input data whether TSV. The tool automatically detects the number of samples. (mandatory)
-		--CLEMENT_DIR Directory where the outputs of CLEMENT be saved. (mandatory)
+	(Mandatory) These options are regarding User's input and output format
+		--INPUT_TSV		Input data whether TSV. The tool automatically detects the number of samples
+		--CLEMENT_DIR 		Directory where the outputs of CLEMENT be saved
 
 	These options are regarding downsizing User's input or not
-		--RANDOM_PICK Set this variable to user want to downsize the sample. If user don't want to downsize, set -1 (default).
+		--RANDOM_PICK 		Set this variable to user want to downsize the sample. If user don't want to downsize, set -1. (default : -1).
 	
 	These options are adjusting E-M algorithm parameter
-		--NUM_CLONE_TRIAL_START Minimum number of expected cluster_hards (initation of K) (default: 3)
-		--NUM_CLONE_TRIAL_END Maximum number of expected cluster_hards (termination of K) (default: 5)
-		--TRIAL_NO Trial number in each candidate cluster_hard number. DO NOT recommend over 15 (default: 5)
-		--KMEANS_CLUSTERNO	Number of initial K-means cluster. Recommendation : 5~8 for one-sample, 8-15 for larger-sample (default: 8)
-		--MIN_CLUSTER_SIZE	The minimum cluster size that is acceptable (default: 9)
+		--NUM_CLONE_TRIAL_START 	Minimum number of expected cluster_hards (initation of K) 	(default: 3)
+		--NUM_CLONE_TRIAL_END 		Maximum number of expected cluster_hards (termination of K)	 (default: 5)
+		--TRIAL_NO 			Trial number in each candidate cluster_hard number. DO NOT recommend over 15 (default: 5)
+		--KMEANS_CLUSTERNO		Number of initial K-means cluster. Recommendation : 5~8 for one-sample, 8-15 for larger-sample (default: 8)
+		--MIN_CLUSTER_SIZE		The minimum cluster size that is acceptable. Recommendation : 1-3% of total variants number 	(default: 9)
 
 	Other options
-		--MODE	Selection of clustering method  "Hard" : hard clustering only,  "Both" : both hard and soft (fuzzy) clustering (default: "Both")
-		--MAKEONE_STRICT  1:strict, 2:lenient. (default : 1)
-		--TN_CONFIDENTIALITY  Confidentiality that negative being negative (TN). Recommendation : > 0.99. (default : 0.995)
+		--MODE			Selection of clustering method.
+					"Hard": hard clustering only,  "Both": both hard and soft (fuzzy) clustering (default: "Both")
+		--MAKEONE_STRICT  	1: strict, 2: lenient (default : 1)
+		--TN_CONFIDENTIALITY  	Confidentiality that negative being negative (TN). Recommendation : > 0.99. (default : 0.995)
 
 	Miscelleneous
-		--VERBOSE	Print process →  0: no record,  1: simplified record,  2: verbose record (default: 2)
+		--FONT_FAMILY		Font family that displayed in the plots (default : "arial")
+		--VERBOSE			0: no record,  1: simplified record,  2: verbose record (default: 2)
 
 
-**output**
+### output
 
 **${CLEMENT_DIR}"/result"**
-- **CLEMENT_decision**	CLEMENT's best recommendation among hard and soft clustering.
-- **CLEMENT_hard_1st** CLEMENT's best decomposition by hard clustering.
-- **CLEMENT_hard.gapstatistics.txt** Selecting the optimal K in hard clustering based on gap* stastics.
-- **CLEMENT_soft_1st** CLEMENT's best decomposition by soft (fuzzy) clustering.
-- **membership.txt** Membership assignment of all variants to each clusters. 
-- **membership_count.txt** Count matrix of the membership assignment to each clusters.
-- **mixture.txt** Centroid of each clusters
+- **CLEMENT_decision**		_CLEMENT's best recommendation among hard and soft clustering._
+- **CLEMENT_hard_1st**  	_CLEMENT's best decomposition by hard clustering._
+- **CLEMENT_hard.gapstatistics.txt** 	_Selecting the optimal K in hard clustering based on gap* stastics._
+- **CLEMENT_soft_1st** 	_CLEMENT's best decomposition by soft (fuzzy) clustering._
+- **membership.txt** 	_Membership assignment of all variants to each clusters._
+- **membership_count.txt** 	_Count matrix of the membership assignment to each clusters._
+- **mixture.txt** 	_Centroid of each clusters_
 
 ## Example
-	[Installation through git clone]
-	python3 CLEMENT.py --INPUT_TSV "../example/2.CellData/MRS_2D/M1-5_M1-6/M1-5_M1-6_input.txt" --CLEMENT_DIR "../example/2.CellData/MRS_2D/M1-5_M1-6"  --NUM_CLONE_TRIAL_START 2 --NUM_CLONE_TRIAL_END 6 --RANDOM_PICK 500   
-	or   
-	[Installation through PyPi]
-	CLEMENT --INPUT_TSV "../example/2.CellData/MRS_2D/M1-5_M1-6/M1-5_M1-6_input.txt" --CLEMENT_DIR "../example/2.CellData/MRS_2D/M1-5_M1-6"  --NUM_CLONE_TRIAL_START 2 --NUM_CLONE_TRIAL_END 6 --RANDOM_PICK 500
+	DIR=[YOUR_DIRECTORY]
 
-<br/>
-![CLEMENT_example](https://github.com/Yonsei-TGIL/CLEMENT/assets/56012432/36dbbd01-0926-4802-8b3e-d91b9fbc7d57)
+	# Example 1
+	CLEMENT \
+		--INPUT_TSV ${DIR}"/example/2.CellData/MRS_2D/M1-5_M1-6/M1-5_M1-6_input.txt" \
+		--CLEMENT_DIR ${DIR}"/example/2.CellData/MRS_2D/M1-5_M1-6"  \
+		--NUM_CLONE_TRIAL_START 2 \
+		--NUM_CLONE_TRIAL_END 6 \
+		--RANDOM_PICK 500
+	
+	# Example 2
+	CLEMENT \
+		--INPUT_TSV ${DIR}"/example/2.CellData/MRS_2D/M1-5_M1-7/M1-5_M1-7_input.txt" \
+		--CLEMENT_DIR ${DIR}"/example/2.CellData/MRS_2D/M1-5_M1-7"  \
+		--NUM_CLONE_TRIAL_START 2 \
+		--NUM_CLONE_TRIAL_END 6
+		
+
+
+![example1](https://github.com/Yonsei-TGIL/CLEMENT/assets/56012432/a5a6beb2-e0ac-44ad-8a5a-1b9aa4480010)
+![example2](https://github.com/Yonsei-TGIL/CLEMENT/assets/56012432/3ee2c4a3-4627-40a3-80e6-666a981a6c20)
 <br/>
 
 ## Contact
 	goldpm1@yuhs.ac
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `CLEMENTDNA-1.0.2/setup.py` & `CLEMENTDNA-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # print(aa)
 # aa = setuptools.find_packages(where="scripts")
 # print(aa)
 
 
 setuptools.setup(
     name             = 'CLEMENTDNA',
-    version          = '1.0.2',
+    version          = '1.0.4',
     description      = 'Genomic decomposition and reconstruction of non-tumor diploid subclones',
     author           = 'Young-soo Chung, M.D.',
     author_email     = 'goldpm1@yuhs.ac',
     url              = 'https://github.com/Yonsei-TGIL/CLEMENT',
     download_url     = 'https://github.com/Yonsei-TGIL/CLEMENT.git',
     install_requires = ['matplotlib>=3.5.2','seaborn>=0.11.2', 'numpy>=1.21.5', 'pandas>=1.3.4', 'scikit-learn>=1.0.2', 'scipy>=1.7.3', 'palettable>=3.3.0' ],
     keywords         = ['CLEMENT', 'genomic decomposition'],
     python_requires  = '>=3.6',
     packages = setuptools.find_packages(),
     license='GPL v3',
+    license_files="LICENSE.txt",
     classifiers      = [
         'Programming Language :: Python :: 3.6', 
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     entry_points={
         'console_scripts': [
```

