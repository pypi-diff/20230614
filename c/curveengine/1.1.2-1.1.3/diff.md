# Comparing `tmp/curveengine-1.1.2-py3-none-any.whl.zip` & `tmp/curveengine-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14710 bytes, number of entries: 12
+Zip file size: 14708 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      816 b- defN 23-May-23 20:55 curveengine/__init__.py
--rw-rw-rw-  2.0 fat     7288 b- defN 23-May-30 15:26 curveengine/engine.py
+-rw-rw-rw-  2.0 fat     7198 b- defN 23-Jun-14 14:23 curveengine/engine.py
 -rw-rw-rw-  2.0 fat      272 b- defN 23-May-23 20:55 curveengine/parsing/__init__.py
--rw-rw-rw-  2.0 fat    34375 b- defN 23-May-30 02:19 curveengine/parsing/checks.py
+-rw-rw-rw-  2.0 fat    34649 b- defN 23-Jun-14 14:23 curveengine/parsing/checks.py
 -rw-rw-rw-  2.0 fat     3617 b- defN 23-May-23 20:55 curveengine/parsing/enums.py
--rw-rw-rw-  2.0 fat     4257 b- defN 23-May-23 20:55 curveengine/parsing/others.py
--rw-rw-rw-  2.0 fat     8004 b- defN 23-May-30 02:12 curveengine/parsing/parsers.py
--rw-rw-rw-  2.0 fat    14214 b- defN 23-May-30 15:10 curveengine/parsing/ratehelpers.py
--rw-rw-rw-  2.0 fat      550 b- defN 23-May-30 17:22 curveengine-1.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 17:22 curveengine-1.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-30 17:22 curveengine-1.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      994 b- defN 23-May-30 17:22 curveengine-1.1.2.dist-info/RECORD
-12 files, 74491 bytes uncompressed, 13038 bytes compressed:  82.5%
+-rw-rw-rw-  2.0 fat     4329 b- defN 23-Jun-13 21:22 curveengine/parsing/others.py
+-rw-rw-rw-  2.0 fat     7535 b- defN 23-Jun-14 20:32 curveengine/parsing/parsers.py
+-rw-rw-rw-  2.0 fat    14534 b- defN 23-Jun-14 14:20 curveengine/parsing/ratehelpers.py
+-rw-rw-rw-  2.0 fat      550 b- defN 23-Jun-14 20:57 curveengine-1.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 20:57 curveengine-1.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-14 20:57 curveengine-1.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      994 b- defN 23-Jun-14 20:57 curveengine-1.1.3.dist-info/RECORD
+12 files, 74598 bytes uncompressed, 13036 bytes compressed:  82.5%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: curveengine/parsing/parsers.py
 Comment: 
 
 Filename: curveengine/parsing/ratehelpers.py
 Comment: 
 
-Filename: curveengine-1.1.2.dist-info/METADATA
+Filename: curveengine-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: curveengine-1.1.2.dist-info/WHEEL
+Filename: curveengine-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: curveengine-1.1.2.dist-info/top_level.txt
+Filename: curveengine-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: curveengine-1.1.2.dist-info/RECORD
+Filename: curveengine-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## curveengine/engine.py

```diff
@@ -117,17 +117,15 @@
         self.curves[curveName] = curve
 
     def __buildPiecewiseCurve(self, data):
         rateHelpers = []
         config = data['curveConfig']
         for i, rateHelper in enumerate(config['rateHelpers']):
             helperType = rateHelper['helperType']
-            helperConfig = rateHelper['helperConfig']
-            if 'discountCurve' not in helperConfig.keys():
-                helperConfig['discountCurve'] = None
+            helperConfig = rateHelper['helperConfig']                        
             marketConfig = rateHelper['marketConfig']
         
             if helperType == HelperType.Deposit:
                 helper = createDepositRateHelper(
                     helperConfig, marketConfig, self.curveHandles, self.indexes)
             elif helperType == HelperType.OIS:
                 helper = createOISRateHelper(
```

## curveengine/parsing/checks.py

```diff
@@ -412,32 +412,33 @@
                         "endOfMonth": True,
                         "frequency": "Annual",
                         "settlementDays": 2,
                         "paymentLag": 2,
                         "telescopicValueDates": True,
                         "index": "SOFR",
                         "fixedLegFrequency": "Semiannual",
-                        "fwdStart": "0D"
+                        "fwdStart": "0D",
+                        "discountCurve": "SOFR"
                     }
     ```
     '''
-
     reference = {
         "tenor": checkTenor,
         "dayCounter": checkDayCounter,
         "calendar": checkCalendar,
         "convention": checkConvention,
         "endOfMonth": partial(checkInstance, type=bool),
         "frequency": checkFrequency,
         "settlementDays": partial(checkInstance, type=int),
         "paymentLag": partial(checkInstance, type=int),
         "telescopicValueDates": partial(checkInstance, type=bool),
         "index": partial(checkInstance, type=str),
         "fixedLegFrequency": checkFrequency,
-        "fwdStart": checkTenor
+        "fwdStart": checkTenor,
+        "discountCurve": partial(checkInstance, type=str)
     }
     try:
         checkDictStructure(data, reference)
     except Exception as exc:
         raise RateHelperConfigurationError('Invalid OIS rate helper') from exc
 
 
@@ -680,26 +681,26 @@
         If the rate helper is invalid
 
     Details
     -------
     The cross currency rate helper should have the following example structure:
     ```
     "helperConfig":  {
-                    "tenor": "2Y",
-                    "dayCounter": "Actual360",
-                    "calendar": "NullCalendar",
-                    "convention": "ModifiedFollowing",
-                    "endOfMonth": False,
-                    "settlementDays": 2,
-                    "discountCurve": "CLP_COLLUSD",
-                    "index": "ICP",
-                    "fixedLegCurrency": "CLF",
-                    "fwdStart": "0D",
-                    "fixedLegFrequency": "Semiannual"
-                }
+                "tenor": "2Y",
+                "dayCounter": "Actual360",
+                "calendar": "NullCalendar",
+                "convention": "ModifiedFollowing",
+                "endOfMonth": False,
+                "settlementDays": 2,
+                "discountCurve": "CLP_COLLUSD",
+                "index": "ICP",
+                "fixedLegCurrency": "CLF",
+                "fwdStart": "0D",
+                "fixedLegFrequency": "Semiannual"
+            }
     ```
     '''
 
     reference = {
         "tenor": checkTenor,
         "dayCounter": checkDayCounter,
         "calendar": checkCalendar,
@@ -793,28 +794,32 @@
                     "tenor": "3M",
                     "calendar": "NullCalendar",
                     "settlementDays": 2,
                     "endOfMonth": False,
                     "convention": "ModifiedFollowing",
                     "flatIndex": "LIBOR3M",
                     "spreadIndex": "LIBOR1M",
-                    "discountCurve": "SOFR"
+                    "flatDiscountCurve": "SOFR",
+                    "spreadDiscountCurve": "CLP_COLLUSD",
+                    "flatIsDomestic": True
                 }
     ```
     '''
 
     reference = {
         "tenor": checkTenor,
         "calendar": checkCalendar,
         "settlementDays": partial(checkInstance, type=int),
         "endOfMonth": partial(checkInstance, type=bool),
         "convention": checkConvention,
         "flatIndex": partial(checkInstance, type=str),
         "spreadIndex": partial(checkInstance, type=str),
-        "discountCurve": partial(checkInstance, type=str),
+        "flatDiscountCurve": partial(checkInstance, type=str),
+        "spreadDiscountCurve": partial(checkInstance, type=str),
+        "flatIsDomestic": partial(checkInstance, type=bool)
     }
 
     try:
         checkDictStructure(data, reference)
     except Exception as exc:
         raise RateHelperConfigurationError(
             'Invalid cross currency basis rate helper') from exc
@@ -868,15 +873,15 @@
     |Helper type             | Required fields                  |
     |----------------------- | ---------------------------------|
     |Deposit                 | rate                             |
     |Swap                    | rate, spread                     |    
     |FxSwap                  | fxSpot, fxPoints                 |    
     |Xccy                    | rate, spread, fxSpot             |
     |TenorBasis              | spread                           |
-    |XccyBasis               | spread, fxSpot, fxPoints         |
+    |XccyBasis               | spread, fxSpot                   |
     |OIS                     | spread                           |
     |Bond                    | rate                             |
     '''
 
     def checkPrice(data: dict) -> None:
         if not isinstance(data, dict):
             raise ConfigurationError(
@@ -915,16 +920,15 @@
     elif helperType == HelperType.TenorBasis:
         reference = {
             "spread": checkPrice
         }
     elif helperType == HelperType.XccyBasis:
         reference = {
             "spread": checkPrice,
-            "fxSpot": checkPrice,
-            "fxPoints": checkPrice
+            "fxSpot": checkPrice            
         }
     elif helperType == HelperType.OIS:
         reference = {
             "spread": checkPrice
         }
     elif helperType == HelperType.Bond:
         reference = {
```

## curveengine/parsing/others.py

```diff
@@ -76,18 +76,18 @@
 
     Notes
     -----
     The dependency list is a dictionary with the curve name as key and a set of
     curve names as value. The set contains the names of the curves that the
     curve depends on.
     """
-    # Possible curve related keys
-    pc = ['discountCurve', 'collateralCurve']
+    # Possible curve-related keys
+    pc = ['discountCurve', 'collateralCurve', 'flatDiscountCurve', 'spreadDiscountCurve']
     # Possible index related keys
-    pi = ['index', 'shortIndex', 'longIndex']
+    pi = ['index', 'shortIndex', 'longIndex', 'flatIndex', 'spreadIndex']
 
     dependencies = {}
     for curve in data['curves']:
         curveName = curve['curveName']
         if curveName not in dependencies.keys():
             dependencies[curveName] = set()
```

## curveengine/parsing/parsers.py

```diff
@@ -42,27 +42,15 @@
             results[key] = parseCalendar(value)
 
         elif key == 'convention':
             results[key] = parseBusinessDayConvention(value)
 
         elif key in ['tenor', 'fwdStart', 'shortPayTenor']:
             results[key] = parsePeriod(value)
-
-        elif key in ['endOfMonth', 'telescopicValueDates', 'spreadOnShortIndex', 'baseCurrencyAsCollateral', 'enableExtrapolation']:
-            results[key] = value
-
-        elif key in ['settlementDays', 'paymentLag', 'fixingDays', 'year']:
-            results[key] = value
-
-        elif key in ['discountCurve', 'index', 'shortIndex', 'longIndex', 'curveName']:
-            results[key] = value
-
-        elif key in ['couponRate']:
-            results[key] = value
-
+            
         elif key == 'month':
             results[key] = parseMonth(value)
 
         else:
             results[key] = value
 
     return results
```

## curveengine/parsing/ratehelpers.py

```diff
@@ -490,34 +490,40 @@
     checkCrossCcyBasisSwapRateHelper
     """
     tenor = helperConfig['tenor']
     calendar = helperConfig['calendar']
     settlementDays = helperConfig['settlementDays']
     endOfMonth = helperConfig['endOfMonth']
     convention = helperConfig['convention']
+    flatIsDomestic = helperConfig['flatIsDomestic']
 
     # Discout curveHandles
-    flatDiscountCurve = curveHandles[helperConfig['discountCurve']]
-    spreadDiscountCurve = curveHandles[helperConfig['discountCurve']]
+    flatDiscountCurve: ore.RelinkableYieldTermStructureHandle = curveHandles[helperConfig['flatDiscountCurve']]   
+    spreadDiscountCurve: ore.RelinkableYieldTermStructureHandle = curveHandles[helperConfig['spreadDiscountCurve']]
 
     # Index
-    flatIndex = indexes[helperConfig['flatIndex']]
+    flatIndex: ore.IborIndex = indexes[helperConfig['flatIndex']]
     spreadIndex = indexes[helperConfig['spreadIndex']]
-
+    
     # QuoteHandle
     spread = marketConfig['spread']['value']
     spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
 
+    fxSpot = marketConfig['fxSpot']['value']
+    fxSpotQuote = ore.QuoteHandle(ore.SimpleQuote(fxSpot))
+
     # CrossCcyBasisSwapHelper
     crossCcyBasisSwapHelper = ore.CrossCcyBasisSwapHelper(
         spreadQuote,
-        tenor,
-        calendar,
+        fxSpotQuote,
         settlementDays,
+        calendar,
+        tenor,
+        convention,
         flatIndex,
         spreadIndex,
         flatDiscountCurve,
         spreadDiscountCurve,
         endOfMonth,
-        convention
+        flatIsDomestic
     )
     return crossCcyBasisSwapHelper
```

## Comparing `curveengine-1.1.2.dist-info/METADATA` & `curveengine-1.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curveengine
-Version: 1.1.2
+Version: 1.1.3
 Summary: A simple curve bootstraping tool based on ORE/QuantLib
 Author: Jose Melo
 Author-email: jmelo@live.cl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Requires-Dist: open-source-risk-engine
```

## Comparing `curveengine-1.1.2.dist-info/RECORD` & `curveengine-1.1.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 curveengine/__init__.py,sha256=fG7Ka2v7aTn4pF7lI0zG-neRIZUS8vm6EyF0cxUrCHo,816
-curveengine/engine.py,sha256=HF2MJXybiGHLNIv1OHcfcYdDzlrrsrGCL7tZJF-lVoI,7288
+curveengine/engine.py,sha256=GxLVWn-8Vio4FyiuLpunGusB5o3Vgu61K57eub1OR2M,7198
 curveengine/parsing/__init__.py,sha256=jiYxFpB8cxfRiLTIomE7LguueKAKylTb2vrbrj8j1RU,272
-curveengine/parsing/checks.py,sha256=pJfMKomtCgJEbfUuAQGUNG2O4ErWSTfBR3is-04sMX8,34375
+curveengine/parsing/checks.py,sha256=MpHQYIdz9vJRgsAX5IIKvmZWG35Q3yfYG4PauxGHInM,34649
 curveengine/parsing/enums.py,sha256=nYlnk3PCV4Jax0Tu68Sh-qpBRR3DWFGXX0W3wI9n0xY,3617
-curveengine/parsing/others.py,sha256=2vNml3mjqUnX9D5Yyce9Y15sWv5JmC8RyS4D0EJH4mI,4257
-curveengine/parsing/parsers.py,sha256=61tqPjHveE6Duu1UJjROWwLlk8sFd_UEpjiVbpdj8pc,8004
-curveengine/parsing/ratehelpers.py,sha256=uphByfYCN0na5CzTg4IMerTSKFF3j9kHrxjNNcAKGgc,14214
-curveengine-1.1.2.dist-info/METADATA,sha256=CFLhjwMaEz8Vy9shWRLWPs9O_X6-3VlX3PhhlLv2apI,550
-curveengine-1.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-curveengine-1.1.2.dist-info/top_level.txt,sha256=LK8Ltzj4yLB5cfrjUzMY4Uokv2JNYXqgbUzChD4c92c,12
-curveengine-1.1.2.dist-info/RECORD,,
+curveengine/parsing/others.py,sha256=90e4QnE4mLTKhV1cIy4gGNoURiZSB5IGoW_RETgtd9c,4329
+curveengine/parsing/parsers.py,sha256=YjB4vxOCiTNXOyVcMSLVv_MWtMbPcrzBHDEJOjbmwLo,7535
+curveengine/parsing/ratehelpers.py,sha256=Y4WyEEKFjfLuE_Op9az8NNHjdOv6R1EUGks2LiCu2CM,14534
+curveengine-1.1.3.dist-info/METADATA,sha256=loQlxNIJsSGQVokUgH75T42-2m7ljRZ1aB0ijwzIL2Y,550
+curveengine-1.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+curveengine-1.1.3.dist-info/top_level.txt,sha256=LK8Ltzj4yLB5cfrjUzMY4Uokv2JNYXqgbUzChD4c92c,12
+curveengine-1.1.3.dist-info/RECORD,,
```

