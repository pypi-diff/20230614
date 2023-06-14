# Comparing `tmp/ohdsi-circe-0.1.0.tar.gz` & `tmp/ohdsi-circe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-circe-0.1.0.tar", last modified: Tue Jun 13 14:53:57 2023, max compression
+gzip compressed data, was "ohdsi-circe-0.2.0.tar", last modified: Wed Jun 14 08:26:50 2023, max compression
```

## Comparing `ohdsi-circe-0.1.0.tar` & `ohdsi-circe-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:57.211874 ohdsi-circe-0.1.0/
--rw-rw-rw-   0        0        0      940 2023-06-13 14:53:57.211874 ohdsi-circe-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:57.162483 ohdsi-circe-0.1.0/ohdsi/
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:57.178107 ohdsi-circe-0.1.0/ohdsi/circe/
--rw-rw-rw-   0        0        0     7681 2023-06-01 13:51:02.000000 ohdsi-circe-0.1.0/ohdsi/circe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:57.180615 ohdsi-circe-0.1.0/ohdsi/circe/data/
--rw-rw-rw-   0        0        0     1157 2023-03-09 15:32:58.000000 ohdsi-circe-0.1.0/ohdsi/circe/data/conceptSet.json
--rw-rw-rw-   0        0        0     1243 2023-03-09 15:32:54.000000 ohdsi-circe-0.1.0/ohdsi/circe/data/conceptSetList.json
--rw-rw-rw-   0        0        0      692 2023-03-09 15:33:05.000000 ohdsi-circe-0.1.0/ohdsi/circe/data/simpleCohort.json
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:57.196258 ohdsi-circe-0.1.0/ohdsi_circe.egg-info/
--rw-rw-rw-   0        0        0      940 2023-06-13 14:53:57.000000 ohdsi-circe-0.1.0/ohdsi_circe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-13 14:53:57.000000 ohdsi-circe-0.1.0/ohdsi_circe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:53:57.000000 ohdsi-circe-0.1.0/ohdsi_circe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-13 14:53:57.000000 ohdsi-circe-0.1.0/ohdsi_circe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 14:53:57.000000 ohdsi-circe-0.1.0/ohdsi_circe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 14:53:57.211874 ohdsi-circe-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1052 2023-06-08 13:18:05.000000 ohdsi-circe-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:50.145492 ohdsi-circe-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-14 08:26:50.145492 ohdsi-circe-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:50.141492 ohdsi-circe-0.2.0/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:50.141492 ohdsi-circe-0.2.0/ohdsi/circe/
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-14 08:26:29.000000 ohdsi-circe-0.2.0/ohdsi/circe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:50.141492 ohdsi-circe-0.2.0/ohdsi/circe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-14 08:26:29.000000 ohdsi-circe-0.2.0/ohdsi/circe/data/conceptSet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-14 08:26:29.000000 ohdsi-circe-0.2.0/ohdsi/circe/data/conceptSetList.json
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 08:26:29.000000 ohdsi-circe-0.2.0/ohdsi/circe/data/simpleCohort.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:50.145492 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-14 08:26:50.000000 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-14 08:26:50.000000 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:26:50.000000 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 08:26:50.000000 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 08:26:50.000000 ohdsi-circe-0.2.0/ohdsi_circe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:26:50.145492 ohdsi-circe-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-14 08:26:29.000000 ohdsi-circe-0.2.0/setup.py
```

### Comparing `ohdsi-circe-0.1.0/PKG-INFO` & `ohdsi-circe-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: ohdsi-circe
-Version: 0.1.0
-Summary: Python wrapper for the OHDSI R packages
-Home-page: https://github.com/vantage6/python-ohdsi
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-# python-ohdsi
-Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
-OMOP data sources in vantage6.
-
-# TODO
-Packages to be wrapped:
-- [ ] [Capr](https://github.com/OHDSI/Capr)
-- [X] [CirceR](https://github.com/OHDSI/CirceR)
-- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
-- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
-- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
-- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
-
-Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
+Metadata-Version: 2.1
+Name: ohdsi-circe
+Version: 0.2.0
+Summary: Python wrapper for the OHDSI R packages
+Home-page: https://github.com/vantage6/python-ohdsi
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
+# python-ohdsi
+Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
+OMOP data sources in vantage6.
+
+# TODO
+Packages to be wrapped:
+- [ ] [Capr](https://github.com/OHDSI/Capr)
+- [X] [CirceR](https://github.com/OHDSI/CirceR)
+- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
+- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
+- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
+- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
+
+Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
```

### Comparing `ohdsi-circe-0.1.0/ohdsi/circe/data/conceptSet.json` & `ohdsi-circe-0.2.0/ohdsi/circe/data/conceptSet.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,70 @@
-00000000: 7b0d 0a20 2020 2022 6964 223a 2030 2c0d  {..    "id": 0,.
-00000010: 0a20 2020 2022 6e61 6d65 223a 2022 5073  .    "name": "Ps
-00000020: 6f72 6961 7369 7322 2c0d 0a20 2020 2022  oriasis",..    "
-00000030: 6578 7072 6573 7369 6f6e 223a 207b 0d0a  expression": {..
-00000040: 2020 2020 2020 2269 7465 6d73 223a 205b        "items": [
-00000050: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-00000060: 2020 2020 2020 2022 636f 6e63 6570 7422         "concept"
-00000070: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00000080: 2022 434f 4e43 4550 545f 4944 223a 2037   "CONCEPT_ID": 7
-00000090: 3536 3134 2c0d 0a20 2020 2020 2020 2020  5614,..         
-000000a0: 2020 2022 434f 4e43 4550 545f 4e41 4d45     "CONCEPT_NAME
-000000b0: 223a 2022 4163 726f 6465 726d 6174 6974  ": "Acrodermatit
-000000c0: 6973 2063 6f6e 7469 6e75 6122 2c0d 0a20  is continua",.. 
-000000d0: 2020 2020 2020 2020 2020 2022 5354 414e             "STAN
-000000e0: 4441 5244 5f43 4f4e 4345 5054 223a 2022  DARD_CONCEPT": "
-000000f0: 5322 2c0d 0a20 2020 2020 2020 2020 2020  S",..           
-00000100: 2022 5354 414e 4441 5244 5f43 4f4e 4345   "STANDARD_CONCE
-00000110: 5054 5f43 4150 5449 4f4e 223a 2022 5374  PT_CAPTION": "St
-00000120: 616e 6461 7264 222c 0d0a 2020 2020 2020  andard",..      
-00000130: 2020 2020 2020 2249 4e56 414c 4944 5f52        "INVALID_R
-00000140: 4541 534f 4e22 3a20 2256 222c 0d0a 2020  EASON": "V",..  
-00000150: 2020 2020 2020 2020 2020 2249 4e56 414c            "INVAL
-00000160: 4944 5f52 4541 534f 4e5f 4341 5054 494f  ID_REASON_CAPTIO
-00000170: 4e22 3a20 2256 616c 6964 222c 0d0a 2020  N": "Valid",..  
-00000180: 2020 2020 2020 2020 2020 2243 4f4e 4345            "CONCE
-00000190: 5054 5f43 4f44 4522 3a20 2232 3030 3937  PT_CODE": "20097
-000001a0: 3630 3038 222c 0d0a 2020 2020 2020 2020  6008",..        
-000001b0: 2020 2020 2244 4f4d 4149 4e5f 4944 223a      "DOMAIN_ID":
-000001c0: 2022 436f 6e64 6974 696f 6e22 2c0d 0a20   "Condition",.. 
-000001d0: 2020 2020 2020 2020 2020 2022 564f 4341             "VOCA
-000001e0: 4255 4c41 5259 5f49 4422 3a20 2253 4e4f  BULARY_ID": "SNO
-000001f0: 4d45 4422 2c0d 0a20 2020 2020 2020 2020  MED",..         
-00000200: 2020 2022 434f 4e43 4550 545f 434c 4153     "CONCEPT_CLAS
-00000210: 535f 4944 223a 2022 436c 696e 6963 616c  S_ID": "Clinical
-00000220: 2046 696e 6469 6e67 220d 0a20 2020 2020   Finding"..     
-00000230: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00000240: 2020 2022 696e 636c 7564 6544 6573 6365     "includeDesce
-00000250: 6e64 616e 7473 223a 2074 7275 650d 0a20  ndants": true.. 
-00000260: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00000270: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00000280: 2263 6f6e 6365 7074 223a 207b 0d0a 2020  "concept": {..  
-00000290: 2020 2020 2020 2020 2020 2243 4f4e 4345            "CONCE
-000002a0: 5054 5f49 4422 3a20 3134 3031 3638 2c0d  PT_ID": 140168,.
-000002b0: 0a20 2020 2020 2020 2020 2020 2022 434f  .            "CO
-000002c0: 4e43 4550 545f 4e41 4d45 223a 2022 5073  NCEPT_NAME": "Ps
-000002d0: 6f72 6961 7369 7322 2c0d 0a20 2020 2020  oriasis",..     
-000002e0: 2020 2020 2020 2022 5354 414e 4441 5244         "STANDARD
-000002f0: 5f43 4f4e 4345 5054 223a 2022 5322 2c0d  _CONCEPT": "S",.
-00000300: 0a20 2020 2020 2020 2020 2020 2022 5354  .            "ST
-00000310: 414e 4441 5244 5f43 4f4e 4345 5054 5f43  ANDARD_CONCEPT_C
-00000320: 4150 5449 4f4e 223a 2022 5374 616e 6461  APTION": "Standa
-00000330: 7264 222c 0d0a 2020 2020 2020 2020 2020  rd",..          
-00000340: 2020 2249 4e56 414c 4944 5f52 4541 534f    "INVALID_REASO
-00000350: 4e22 3a20 2256 222c 0d0a 2020 2020 2020  N": "V",..      
-00000360: 2020 2020 2020 2249 4e56 414c 4944 5f52        "INVALID_R
-00000370: 4541 534f 4e5f 4341 5054 494f 4e22 3a20  EASON_CAPTION": 
-00000380: 2256 616c 6964 222c 0d0a 2020 2020 2020  "Valid",..      
-00000390: 2020 2020 2020 2243 4f4e 4345 5054 5f43        "CONCEPT_C
-000003a0: 4f44 4522 3a20 2239 3031 3430 3032 222c  ODE": "9014002",
-000003b0: 0d0a 2020 2020 2020 2020 2020 2020 2244  ..            "D
-000003c0: 4f4d 4149 4e5f 4944 223a 2022 436f 6e64  OMAIN_ID": "Cond
-000003d0: 6974 696f 6e22 2c0d 0a20 2020 2020 2020  ition",..       
-000003e0: 2020 2020 2022 564f 4341 4255 4c41 5259       "VOCABULARY
-000003f0: 5f49 4422 3a20 2253 4e4f 4d45 4422 2c0d  _ID": "SNOMED",.
-00000400: 0a20 2020 2020 2020 2020 2020 2022 434f  .            "CO
-00000410: 4e43 4550 545f 434c 4153 535f 4944 223a  NCEPT_CLASS_ID":
-00000420: 2022 436c 696e 6963 616c 2046 696e 6469   "Clinical Findi
-00000430: 6e67 220d 0a20 2020 2020 2020 2020 207d  ng"..          }
-00000440: 2c0d 0a20 2020 2020 2020 2020 2022 696e  ,..          "in
-00000450: 636c 7564 6544 6573 6365 6e64 616e 7473  cludeDescendants
-00000460: 223a 2074 7275 650d 0a20 2020 2020 2020  ": true..       
-00000470: 207d 0d0a 2020 2020 2020 5d0d 0a20 2020   }..      ]..   
-00000480: 207d 0d0a 7d                              }..}
+00000000: 7b0a 2020 2020 2269 6422 3a20 302c 0a20  {.    "id": 0,. 
+00000010: 2020 2022 6e61 6d65 223a 2022 5073 6f72     "name": "Psor
+00000020: 6961 7369 7322 2c0a 2020 2020 2265 7870  iasis",.    "exp
+00000030: 7265 7373 696f 6e22 3a20 7b0a 2020 2020  ression": {.    
+00000040: 2020 2269 7465 6d73 223a 205b 0a20 2020    "items": [.   
+00000050: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000060: 2022 636f 6e63 6570 7422 3a20 7b0a 2020   "concept": {.  
+00000070: 2020 2020 2020 2020 2020 2243 4f4e 4345            "CONCE
+00000080: 5054 5f49 4422 3a20 3735 3631 342c 0a20  PT_ID": 75614,. 
+00000090: 2020 2020 2020 2020 2020 2022 434f 4e43             "CONC
+000000a0: 4550 545f 4e41 4d45 223a 2022 4163 726f  EPT_NAME": "Acro
+000000b0: 6465 726d 6174 6974 6973 2063 6f6e 7469  dermatitis conti
+000000c0: 6e75 6122 2c0a 2020 2020 2020 2020 2020  nua",.          
+000000d0: 2020 2253 5441 4e44 4152 445f 434f 4e43    "STANDARD_CONC
+000000e0: 4550 5422 3a20 2253 222c 0a20 2020 2020  EPT": "S",.     
+000000f0: 2020 2020 2020 2022 5354 414e 4441 5244         "STANDARD
+00000100: 5f43 4f4e 4345 5054 5f43 4150 5449 4f4e  _CONCEPT_CAPTION
+00000110: 223a 2022 5374 616e 6461 7264 222c 0a20  ": "Standard",. 
+00000120: 2020 2020 2020 2020 2020 2022 494e 5641             "INVA
+00000130: 4c49 445f 5245 4153 4f4e 223a 2022 5622  LID_REASON": "V"
+00000140: 2c0a 2020 2020 2020 2020 2020 2020 2249  ,.            "I
+00000150: 4e56 414c 4944 5f52 4541 534f 4e5f 4341  NVALID_REASON_CA
+00000160: 5054 494f 4e22 3a20 2256 616c 6964 222c  PTION": "Valid",
+00000170: 0a20 2020 2020 2020 2020 2020 2022 434f  .            "CO
+00000180: 4e43 4550 545f 434f 4445 223a 2022 3230  NCEPT_CODE": "20
+00000190: 3039 3736 3030 3822 2c0a 2020 2020 2020  0976008",.      
+000001a0: 2020 2020 2020 2244 4f4d 4149 4e5f 4944        "DOMAIN_ID
+000001b0: 223a 2022 436f 6e64 6974 696f 6e22 2c0a  ": "Condition",.
+000001c0: 2020 2020 2020 2020 2020 2020 2256 4f43              "VOC
+000001d0: 4142 554c 4152 595f 4944 223a 2022 534e  ABULARY_ID": "SN
+000001e0: 4f4d 4544 222c 0a20 2020 2020 2020 2020  OMED",.         
+000001f0: 2020 2022 434f 4e43 4550 545f 434c 4153     "CONCEPT_CLAS
+00000200: 535f 4944 223a 2022 436c 696e 6963 616c  S_ID": "Clinical
+00000210: 2046 696e 6469 6e67 220a 2020 2020 2020   Finding".      
+00000220: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00000230: 2022 696e 636c 7564 6544 6573 6365 6e64   "includeDescend
+00000240: 616e 7473 223a 2074 7275 650a 2020 2020  ants": true.    
+00000250: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+00000260: 0a20 2020 2020 2020 2020 2022 636f 6e63  .          "conc
+00000270: 6570 7422 3a20 7b0a 2020 2020 2020 2020  ept": {.        
+00000280: 2020 2020 2243 4f4e 4345 5054 5f49 4422      "CONCEPT_ID"
+00000290: 3a20 3134 3031 3638 2c0a 2020 2020 2020  : 140168,.      
+000002a0: 2020 2020 2020 2243 4f4e 4345 5054 5f4e        "CONCEPT_N
+000002b0: 414d 4522 3a20 2250 736f 7269 6173 6973  AME": "Psoriasis
+000002c0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000002d0: 5354 414e 4441 5244 5f43 4f4e 4345 5054  STANDARD_CONCEPT
+000002e0: 223a 2022 5322 2c0a 2020 2020 2020 2020  ": "S",.        
+000002f0: 2020 2020 2253 5441 4e44 4152 445f 434f      "STANDARD_CO
+00000300: 4e43 4550 545f 4341 5054 494f 4e22 3a20  NCEPT_CAPTION": 
+00000310: 2253 7461 6e64 6172 6422 2c0a 2020 2020  "Standard",.    
+00000320: 2020 2020 2020 2020 2249 4e56 414c 4944          "INVALID
+00000330: 5f52 4541 534f 4e22 3a20 2256 222c 0a20  _REASON": "V",. 
+00000340: 2020 2020 2020 2020 2020 2022 494e 5641             "INVA
+00000350: 4c49 445f 5245 4153 4f4e 5f43 4150 5449  LID_REASON_CAPTI
+00000360: 4f4e 223a 2022 5661 6c69 6422 2c0a 2020  ON": "Valid",.  
+00000370: 2020 2020 2020 2020 2020 2243 4f4e 4345            "CONCE
+00000380: 5054 5f43 4f44 4522 3a20 2239 3031 3430  PT_CODE": "90140
+00000390: 3032 222c 0a20 2020 2020 2020 2020 2020  02",.           
+000003a0: 2022 444f 4d41 494e 5f49 4422 3a20 2243   "DOMAIN_ID": "C
+000003b0: 6f6e 6469 7469 6f6e 222c 0a20 2020 2020  ondition",.     
+000003c0: 2020 2020 2020 2022 564f 4341 4255 4c41         "VOCABULA
+000003d0: 5259 5f49 4422 3a20 2253 4e4f 4d45 4422  RY_ID": "SNOMED"
+000003e0: 2c0a 2020 2020 2020 2020 2020 2020 2243  ,.            "C
+000003f0: 4f4e 4345 5054 5f43 4c41 5353 5f49 4422  ONCEPT_CLASS_ID"
+00000400: 3a20 2243 6c69 6e69 6361 6c20 4669 6e64  : "Clinical Find
+00000410: 696e 6722 0a20 2020 2020 2020 2020 207d  ing".          }
+00000420: 2c0a 2020 2020 2020 2020 2020 2269 6e63  ,.          "inc
+00000430: 6c75 6465 4465 7363 656e 6461 6e74 7322  ludeDescendants"
+00000440: 3a20 7472 7565 0a20 2020 2020 2020 207d  : true.        }
+00000450: 0a20 2020 2020 205d 0a20 2020 207d 0a7d  .      ].    }.}
```

### Comparing `ohdsi-circe-0.1.0/ohdsi/circe/data/simpleCohort.json` & `ohdsi-circe-0.2.0/ohdsi/circe/data/simpleCohort.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-00000000: 7b0d 0a20 2022 436f 6e63 6570 7453 6574  {..  "ConceptSet
-00000010: 7322 3a20 5b0d 0a20 2020 207b 0d0a 2020  s": [..    {..  
-00000020: 2020 2020 2269 6422 3a20 302c 0d0a 2020      "id": 0,..  
-00000030: 2020 2020 226e 616d 6522 3a20 2253 6f6d      "name": "Som
-00000040: 6520 436f 6e63 6570 7453 6574 222c 0d0a  e ConceptSet",..
-00000050: 2020 2020 2020 2265 7870 7265 7373 696f        "expressio
-00000060: 6e22 3a20 7b0d 0a20 2020 2020 2020 2022  n": {..        "
-00000070: 6974 656d 7322 3a20 5b5d 0d0a 2020 2020  items": []..    
-00000080: 2020 7d0d 0a20 2020 207d 0d0a 2020 5d2c    }..    }..  ],
-00000090: 0d0a 2020 2250 7269 6d61 7279 4372 6974  ..  "PrimaryCrit
-000000a0: 6572 6961 223a 207b 0d0a 2020 2020 2243  eria": {..    "C
-000000b0: 7269 7465 7269 614c 6973 7422 3a20 5b0d  riteriaList": [.
-000000c0: 0a20 2020 2020 207b 0d0a 2020 2020 2020  .      {..      
-000000d0: 2020 2243 6f6e 6469 7469 6f6e 4f63 6375    "ConditionOccu
-000000e0: 7272 656e 6365 223a 207b 0d0a 2020 2020  rrence": {..    
-000000f0: 2020 2020 2020 2243 6f64 6573 6574 4964        "CodesetId
-00000100: 223a 2030 0d0a 2020 2020 2020 2020 7d0d  ": 0..        }.
-00000110: 0a20 2020 2020 207d 0d0a 2020 2020 5d2c  .      }..    ],
-00000120: 0d0a 2020 2020 224f 6273 6572 7661 7469  ..    "Observati
-00000130: 6f6e 5769 6e64 6f77 223a 207b 0d0a 2020  onWindow": {..  
-00000140: 2020 2020 2250 7269 6f72 4461 7973 223a      "PriorDays":
-00000150: 2030 2c0d 0a20 2020 2020 2022 506f 7374   0,..      "Post
-00000160: 4461 7973 223a 2030 0d0a 2020 2020 7d2c  Days": 0..    },
-00000170: 0d0a 2020 2020 2250 7269 6d61 7279 4372  ..    "PrimaryCr
-00000180: 6974 6572 6961 4c69 6d69 7422 3a20 7b0d  iteriaLimit": {.
-00000190: 0a20 2020 2020 2022 5479 7065 223a 2022  .      "Type": "
-000001a0: 4669 7273 7422 0d0a 2020 2020 7d0d 0a20  First"..    }.. 
-000001b0: 207d 2c0d 0a20 2022 5175 616c 6966 6965   },..  "Qualifie
-000001c0: 644c 696d 6974 223a 207b 0d0a 2020 2020  dLimit": {..    
-000001d0: 2254 7970 6522 3a20 2246 6972 7374 220d  "Type": "First".
-000001e0: 0a20 207d 2c0d 0a20 2022 4578 7072 6573  .  },..  "Expres
-000001f0: 7369 6f6e 4c69 6d69 7422 3a20 7b0d 0a20  sionLimit": {.. 
-00000200: 2020 2022 5479 7065 223a 2022 4669 7273     "Type": "Firs
-00000210: 7422 0d0a 2020 7d2c 0d0a 2020 2249 6e63  t"..  },..  "Inc
-00000220: 6c75 7369 6f6e 5275 6c65 7322 3a20 5b5d  lusionRules": []
-00000230: 2c0d 0a20 2022 4365 6e73 6f72 696e 6743  ,..  "CensoringC
-00000240: 7269 7465 7269 6122 3a20 5b5d 2c0d 0a20  riteria": [],.. 
-00000250: 2022 436f 6c6c 6170 7365 5365 7474 696e   "CollapseSettin
-00000260: 6773 223a 207b 0d0a 2020 2020 2243 6f6c  gs": {..    "Col
-00000270: 6c61 7073 6554 7970 6522 3a20 2245 5241  lapseType": "ERA
-00000280: 222c 0d0a 2020 2020 2245 7261 5061 6422  ",..    "EraPad"
-00000290: 3a20 300d 0a20 207d 2c0d 0a20 2022 4365  : 0..  },..  "Ce
-000002a0: 6e73 6f72 5769 6e64 6f77 223a 207b 7d0d  nsorWindow": {}.
-000002b0: 0a7d 0d0a                                .}..
+00000000: 7b0a 2020 2243 6f6e 6365 7074 5365 7473  {.  "ConceptSets
+00000010: 223a 205b 0a20 2020 207b 0a20 2020 2020  ": [.    {.     
+00000020: 2022 6964 223a 2030 2c0a 2020 2020 2020   "id": 0,.      
+00000030: 226e 616d 6522 3a20 2253 6f6d 6520 436f  "name": "Some Co
+00000040: 6e63 6570 7453 6574 222c 0a20 2020 2020  nceptSet",.     
+00000050: 2022 6578 7072 6573 7369 6f6e 223a 207b   "expression": {
+00000060: 0a20 2020 2020 2020 2022 6974 656d 7322  .        "items"
+00000070: 3a20 5b5d 0a20 2020 2020 207d 0a20 2020  : [].      }.   
+00000080: 207d 0a20 205d 2c0a 2020 2250 7269 6d61   }.  ],.  "Prima
+00000090: 7279 4372 6974 6572 6961 223a 207b 0a20  ryCriteria": {. 
+000000a0: 2020 2022 4372 6974 6572 6961 4c69 7374     "CriteriaList
+000000b0: 223a 205b 0a20 2020 2020 207b 0a20 2020  ": [.      {.   
+000000c0: 2020 2020 2022 436f 6e64 6974 696f 6e4f       "ConditionO
+000000d0: 6363 7572 7265 6e63 6522 3a20 7b0a 2020  ccurrence": {.  
+000000e0: 2020 2020 2020 2020 2243 6f64 6573 6574          "Codeset
+000000f0: 4964 223a 2030 0a20 2020 2020 2020 207d  Id": 0.        }
+00000100: 0a20 2020 2020 207d 0a20 2020 205d 2c0a  .      }.    ],.
+00000110: 2020 2020 224f 6273 6572 7661 7469 6f6e      "Observation
+00000120: 5769 6e64 6f77 223a 207b 0a20 2020 2020  Window": {.     
+00000130: 2022 5072 696f 7244 6179 7322 3a20 302c   "PriorDays": 0,
+00000140: 0a20 2020 2020 2022 506f 7374 4461 7973  .      "PostDays
+00000150: 223a 2030 0a20 2020 207d 2c0a 2020 2020  ": 0.    },.    
+00000160: 2250 7269 6d61 7279 4372 6974 6572 6961  "PrimaryCriteria
+00000170: 4c69 6d69 7422 3a20 7b0a 2020 2020 2020  Limit": {.      
+00000180: 2254 7970 6522 3a20 2246 6972 7374 220a  "Type": "First".
+00000190: 2020 2020 7d0a 2020 7d2c 0a20 2022 5175      }.  },.  "Qu
+000001a0: 616c 6966 6965 644c 696d 6974 223a 207b  alifiedLimit": {
+000001b0: 0a20 2020 2022 5479 7065 223a 2022 4669  .    "Type": "Fi
+000001c0: 7273 7422 0a20 207d 2c0a 2020 2245 7870  rst".  },.  "Exp
+000001d0: 7265 7373 696f 6e4c 696d 6974 223a 207b  ressionLimit": {
+000001e0: 0a20 2020 2022 5479 7065 223a 2022 4669  .    "Type": "Fi
+000001f0: 7273 7422 0a20 207d 2c0a 2020 2249 6e63  rst".  },.  "Inc
+00000200: 6c75 7369 6f6e 5275 6c65 7322 3a20 5b5d  lusionRules": []
+00000210: 2c0a 2020 2243 656e 736f 7269 6e67 4372  ,.  "CensoringCr
+00000220: 6974 6572 6961 223a 205b 5d2c 0a20 2022  iteria": [],.  "
+00000230: 436f 6c6c 6170 7365 5365 7474 696e 6773  CollapseSettings
+00000240: 223a 207b 0a20 2020 2022 436f 6c6c 6170  ": {.    "Collap
+00000250: 7365 5479 7065 223a 2022 4552 4122 2c0a  seType": "ERA",.
+00000260: 2020 2020 2245 7261 5061 6422 3a20 300a      "EraPad": 0.
+00000270: 2020 7d2c 0a20 2022 4365 6e73 6f72 5769    },.  "CensorWi
+00000280: 6e64 6f77 223a 207b 7d0a 7d0a            ndow": {}.}.
```

### Comparing `ohdsi-circe-0.1.0/ohdsi_circe.egg-info/PKG-INFO` & `ohdsi-circe-0.2.0/ohdsi_circe.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: ohdsi-circe
-Version: 0.1.0
-Summary: Python wrapper for the OHDSI R packages
-Home-page: https://github.com/vantage6/python-ohdsi
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-# python-ohdsi
-Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
-OMOP data sources in vantage6.
-
-# TODO
-Packages to be wrapped:
-- [ ] [Capr](https://github.com/OHDSI/Capr)
-- [X] [CirceR](https://github.com/OHDSI/CirceR)
-- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
-- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
-- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
-- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
-
-Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
+Metadata-Version: 2.1
+Name: ohdsi-circe
+Version: 0.2.0
+Summary: Python wrapper for the OHDSI R packages
+Home-page: https://github.com/vantage6/python-ohdsi
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
+# python-ohdsi
+Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
+OMOP data sources in vantage6.
+
+# TODO
+Packages to be wrapped:
+- [ ] [Capr](https://github.com/OHDSI/Capr)
+- [X] [CirceR](https://github.com/OHDSI/CirceR)
+- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
+- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
+- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
+- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
+
+Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
```

