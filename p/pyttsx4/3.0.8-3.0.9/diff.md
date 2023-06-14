# Comparing `tmp/pyttsx4-3.0.8-py3-none-any.whl.zip` & `tmp/pyttsx4-3.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 33631 bytes, number of entries: 16
+Zip file size: 28977 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      814 b- defN 23-Apr-07 13:37 pyttsx4/__init__.py
 -rw-r--r--  2.0 unx     7429 b- defN 23-Apr-07 17:19 pyttsx4/driver.py
 -rw-r--r--  2.0 unx     7224 b- defN 23-Apr-07 13:37 pyttsx4/engine.py
--rw-r--r--  2.0 unx    29524 b- defN 23-Apr-11 03:46 pyttsx4/six.py
 -rw-r--r--  2.0 unx      431 b- defN 23-Apr-07 13:37 pyttsx4/voice.py
--rw-r--r--  2.0 unx      853 b- defN 23-Apr-11 03:47 pyttsx4/drivers/__init__.py
+-rw-r--r--  2.0 unx      845 b- defN 23-Apr-16 10:53 pyttsx4/drivers/__init__.py
 -rw-r--r--  2.0 unx    19495 b- defN 23-Apr-07 13:37 pyttsx4/drivers/_espeak.py
+-rw-r--r--  2.0 unx     5624 b- defN 23-Apr-26 13:58 pyttsx4/drivers/coqui_ai_tts.py
 -rw-r--r--  2.0 unx     6182 b- defN 23-Apr-07 13:37 pyttsx4/drivers/dummy.py
 -rw-r--r--  2.0 unx     7448 b- defN 23-Apr-11 03:43 pyttsx4/drivers/espeak.py
--rw-r--r--  2.0 unx     3895 b- defN 23-Apr-12 08:25 pyttsx4/drivers/nsss.py
+-rw-r--r--  2.0 unx     3919 b- defN 23-May-10 12:29 pyttsx4/drivers/nsss.py
 -rw-r--r--  2.0 unx     6753 b- defN 23-Apr-14 16:02 pyttsx4/drivers/sapi5.py
--rw-r--r--  2.0 unx    17098 b- defN 23-Apr-14 16:04 pyttsx4-3.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2242 b- defN 23-Apr-14 16:04 pyttsx4-3.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 16:04 pyttsx4-3.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-14 16:04 pyttsx4-3.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1244 b- defN 23-Apr-14 16:04 pyttsx4-3.0.8.dist-info/RECORD
-16 files, 110732 bytes uncompressed, 31611 bytes compressed:  71.5%
+-rw-r--r--  2.0 unx    17098 b- defN 23-May-10 12:33 pyttsx4-3.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3595 b- defN 23-May-10 12:33 pyttsx4-3.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 12:33 pyttsx4-3.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-10 12:33 pyttsx4-3.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1260 b- defN 23-May-10 12:33 pyttsx4-3.0.9.dist-info/RECORD
+16 files, 88217 bytes uncompressed, 26923 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,47 +3,47 @@
 
 Filename: pyttsx4/driver.py
 Comment: 
 
 Filename: pyttsx4/engine.py
 Comment: 
 
-Filename: pyttsx4/six.py
-Comment: 
-
 Filename: pyttsx4/voice.py
 Comment: 
 
 Filename: pyttsx4/drivers/__init__.py
 Comment: 
 
 Filename: pyttsx4/drivers/_espeak.py
 Comment: 
 
+Filename: pyttsx4/drivers/coqui_ai_tts.py
+Comment: 
+
 Filename: pyttsx4/drivers/dummy.py
 Comment: 
 
 Filename: pyttsx4/drivers/espeak.py
 Comment: 
 
 Filename: pyttsx4/drivers/nsss.py
 Comment: 
 
 Filename: pyttsx4/drivers/sapi5.py
 Comment: 
 
-Filename: pyttsx4-3.0.8.dist-info/LICENSE
+Filename: pyttsx4-3.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: pyttsx4-3.0.8.dist-info/METADATA
+Filename: pyttsx4-3.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pyttsx4-3.0.8.dist-info/WHEEL
+Filename: pyttsx4-3.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pyttsx4-3.0.8.dist-info/top_level.txt
+Filename: pyttsx4-3.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pyttsx4-3.0.8.dist-info/RECORD
+Filename: pyttsx4-3.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyttsx4/drivers/__init__.py

```diff
@@ -1,12 +1,12 @@
 
 '''
 Utility functions to help with Python 2/3 compatibility
 '''
-from .. import six
+import six
 
 def toUtf8(value):
     '''
     Takes in a value and converts it to a text (unicode) type.  Then decodes that
     type to a byte array encoded in utf-8.  In 2.X the resulting object will be a
     str and in 3.X the resulting object will be bytes.  In both 2.X and 3.X any
     object can be passed in and the object's __str__ will be used (or __repr__ if
```

## pyttsx4/drivers/nsss.py

```diff
@@ -1,11 +1,12 @@
 
 from Foundation import *
 from AppKit import NSSpeechSynthesizer
 from PyObjCTools import AppHelper
+from objc import super
 from ..voice import Voice
 
 
 def buildDriver(proxy):
     return NSSpeechDriver.alloc().initWithProxy(proxy)
```

## Comparing `pyttsx4-3.0.8.dist-info/LICENSE` & `pyttsx4-3.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyttsx4-3.0.8.dist-info/RECORD` & `pyttsx4-3.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 pyttsx4/__init__.py,sha256=pO2FX679OZHgpn2vBVIZDoBQff4uOUMe6yBpNRbaw-4,814
 pyttsx4/driver.py,sha256=uQI4OAbaRRKBEwBeh_cFW5nsev-8btlBP9xEGEaPLs4,7429
 pyttsx4/engine.py,sha256=UJBrPIcN3KXmBCABrb2uY4F_AeAaFlC5h6n_L3V0euA,7224
-pyttsx4/six.py,sha256=yVeu0rLX2Qv1P1UaJtvamDmMrjnxNsJkSuztEvVyGG8,29524
 pyttsx4/voice.py,sha256=GYZLgGtnmjLrg93Wh7_lqDcs6zMaTS_QRr3KZM7RZnY,431
-pyttsx4/drivers/__init__.py,sha256=EFf83iBpSVF4joEh4gQmq5Rl22tngVNuR1zBeWfCdjQ,853
+pyttsx4/drivers/__init__.py,sha256=0mEjYibntVJsqK8f_ZAahupfOCFsF7XkpH3lhjxQ7N4,845
 pyttsx4/drivers/_espeak.py,sha256=Gj0N4aFf3YGZO9fq8K5BFbiwkIExqDu1nBXUn7EZVzY,19495
+pyttsx4/drivers/coqui_ai_tts.py,sha256=o-BElHUvDjBmFFuJQyI49FI2ogtin0do5jENy-XaqPY,5624
 pyttsx4/drivers/dummy.py,sha256=d7K46sijjOxwmAJHbgEALwbYwGcktLfW1FcX1iG5I8E,6182
 pyttsx4/drivers/espeak.py,sha256=5QcaVaCyb3xLKXs6_fjnGv0-mioUXINzendba95mpgs,7448
-pyttsx4/drivers/nsss.py,sha256=n0_ysxWeZhqQuiaxpzZo5RYOIl2Ef0yvX7Kj4du30yo,3895
+pyttsx4/drivers/nsss.py,sha256=Tw5IPC2OTROUmGnbY6TDGzRsnDpvvdpEoFUFDyVt9v8,3919
 pyttsx4/drivers/sapi5.py,sha256=05KrT3qMiv_A3pip6IuNdVX6Gc1rET7HYRM9f6BqNKk,6753
-pyttsx4-3.0.8.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
-pyttsx4-3.0.8.dist-info/METADATA,sha256=LLnPxAB1ETPTXznoUSe1CD-qxO2NQ5jEd4OIg6uDMVo,2242
-pyttsx4-3.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyttsx4-3.0.8.dist-info/top_level.txt,sha256=RZW_EXmaQg7go8T0q583RzqdJUlYm0NeSHGpyq92tiY,8
-pyttsx4-3.0.8.dist-info/RECORD,,
+pyttsx4-3.0.9.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
+pyttsx4-3.0.9.dist-info/METADATA,sha256=mwrZpec6sXrqJx4ac_sfvKTRdwzIyyEWaaHF0atmVRA,3595
+pyttsx4-3.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyttsx4-3.0.9.dist-info/top_level.txt,sha256=RZW_EXmaQg7go8T0q583RzqdJUlYm0NeSHGpyq92tiY,8
+pyttsx4-3.0.9.dist-info/RECORD,,
```

