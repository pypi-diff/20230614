# Comparing `tmp/hydrogibs-0.3.5.tar.gz` & `tmp/hydrogibs-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.3.5.tar", last modified: Tue May 23 16:11:35 2023, max compression
+gzip compressed data, was "hydrogibs-0.3.7.tar", last modified: Tue May 23 16:57:37 2023, max compression
```

## Comparing `hydrogibs-0.3.5.tar` & `hydrogibs-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-23 16:11:35.595618 hydrogibs-0.3.5/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.5/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-23 16:11:35.591618 hydrogibs-0.3.5/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.3.5/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-23 16:11:35.591618 hydrogibs-0.3.5/hydrogibs/
--rwxrwxr-x   0 axel      (1000) axel      (1000)    15307 2023-05-23 16:07:37.000000 hydrogibs-0.3.5/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     5176 2023-05-16 12:38:08.000000 hydrogibs-0.3.5/hydrogibs/ModelApp.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.5/hydrogibs/ModelTemplate.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     9762 2023-05-22 14:18:40.000000 hydrogibs-0.3.5/hydrogibs/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.5/hydrogibs/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.3.5/hydrogibs/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.3.5/hydrogibs/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.5/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-23 16:11:35.591618 hydrogibs-0.3.5/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-23 16:11:35.000000 hydrogibs-0.3.5/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-05-23 16:11:35.000000 hydrogibs-0.3.5/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-05-23 16:11:35.000000 hydrogibs-0.3.5/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-05-23 16:11:35.000000 hydrogibs-0.3.5/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-05-23 16:11:23.000000 hydrogibs-0.3.5/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-05-23 16:11:35.595618 hydrogibs-0.3.5/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-23 16:57:37.954574 hydrogibs-0.3.7/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.7/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1558 2023-05-23 16:57:37.954574 hydrogibs-0.3.7/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1008 2023-05-23 16:56:32.000000 hydrogibs-0.3.7/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-23 16:57:37.954574 hydrogibs-0.3.7/hydrogibs/
+-rwxrwxr-x   0 axel      (1000) axel      (1000)    15081 2023-05-23 16:49:06.000000 hydrogibs-0.3.7/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     5176 2023-05-16 12:38:08.000000 hydrogibs-0.3.7/hydrogibs/ModelApp.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.7/hydrogibs/ModelTemplate.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     9762 2023-05-22 14:18:40.000000 hydrogibs-0.3.7/hydrogibs/QDF.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.7/hydrogibs/RationalMethod.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.3.7/hydrogibs/SoCoSe.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.3.7/hydrogibs/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.7/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-23 16:57:37.954574 hydrogibs-0.3.7/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1558 2023-05-23 16:57:37.000000 hydrogibs-0.3.7/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-05-23 16:57:37.000000 hydrogibs-0.3.7/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-05-23 16:57:37.000000 hydrogibs-0.3.7/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-05-23 16:57:37.000000 hydrogibs-0.3.7/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      535 2023-05-23 16:57:08.000000 hydrogibs-0.3.7/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-05-23 16:57:37.954574 hydrogibs-0.3.7/setup.cfg
```

### Comparing `hydrogibs-0.3.5/LICENSE` & `hydrogibs-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.5/hydrogibs/GR4.py` & `hydrogibs-0.3.7/hydrogibs/GR4.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 
 class Rain(ModelTemplate.Rain):
     """
     Rain object to apply to a Catchment object.
 
     Args:
-        - time        (np.ndarray)       [h]
-        - rain_func   (callable)   -> [mm/h]
+        - time        (numpy.ndarray)  [h]
+        - rainfall    (numpy.ndarray) [mm/h]
 
     Creates a GR4h object when called with a Catchment object:
     >>> gr4h = GR4h(catchment, rain)
     Creates an Event object when applied to a catchment
     >>> event = rain @ catchment
     """
 
@@ -117,29 +117,20 @@
         X1 (float)  [-] : dQ = X1 * dPrecipitations
         X2 (float)  [mm]: Initial abstraction (vegetation interception)
         X3 (float) [1/h]: Sub-surface water volume emptying rate dQs = X3*V*dt
         X4 (float)  [h] : the hydrogram's raising time
     """
 
     def __init__(self,
-                 X1: float = 0,
-                 X2: float = 0,
-                 X3: float = 0,
-                 X4: float = 0,
+                 X1: float,
+                 X2: float,
+                 X3: float,
+                 X4: float,
                  surface: float = 1,
                  initial_volume: float = 0,
-                 model: Literal["Laval",
-                                "Erlenbach",
-                                "Rimbaud",
-                                "Latte",
-                                "Sapine",
-                                "Rietholzbach",
-                                "Lumpenenbach",
-                                "Vogelbach",
-                                "Brusquet"] = None,
                  transfer_function: Callable = None) -> None:
 
         assert 0 <= X1 <= 1, "Runoff coefficient must be within [0 : 1]"
         assert 0 <= X2, "Initial abstraction must be positive"
         assert 0 <= X3 <= 1, "Emptying rate must be within [0 : 1]"
         assert 0 <= X4, "Raising time must be positive"
 
@@ -217,22 +208,24 @@
 class Brusquet(Catchment):
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(13.8/100, 22.4, 0.72/100, 1.63,
                          *args, **kwargs)
 
 
-presets = (
-    Laval, Erlenbach, Rimbaud,
-    Latte,
-    Sapine,
-    Rietholzbach,
-    Lumpenenbach,
-    Vogelbach,
-    Brusquet
+presets = dict(
+    Laval=Laval,
+    Erlenbach=Erlenbach,
+    Rimbaud=Rimbaud,
+    Latte=Latte,
+    Sapine=Sapine,
+    Rietholzbach=Rietholzbach,
+    Lumpenenbach=Lumpenenbach,
+    Vogelbach=Vogelbach,
+    Brusquet=Brusquet
 )
 
 
 class Event(ModelTemplate.Event):
     """
     Stores all relevant results of a GR4h calculation
 
@@ -284,14 +277,19 @@
         time = event.time
         rain = event.rainfall
         V = event.volume
         Qp = event.discharge_rain
         Qv = event.discharge_volume
         Q = event.discharge
 
+        tmax = time.max()
+        Qmax = Q.max()
+        rmax = rain.max()
+        Vmax = V.max()
+
         with plt.style.context(style):
 
             c1, c2, c3, c4, c5 = self.colors
 
             fig, (ax2, ax1) = plt.subplots(
                 figsize=figsize,
                 nrows=2, gridspec_kw=dict(
@@ -329,38 +327,37 @@
                 ls='-.',
                 color=c5,
                 label="Écoulements hypodermiques",
                 zorder=9
             )
             ax1.set_ylabel("$Q$ (m³/s)", color=c1)
             ax1.set_xlabel("Temps (h)")
-            ax1.set_xlim((0, time.max()))
-            ax1.set_ylim((0, Q.max()*1.1))
+            ax1.set_xlim((0, tmax if tmax else 1))
+            ax1.set_ylim((0, Qmax*1.1 if Qmax else 1))
             ax1.tick_params(colors=c1, axis='y')
 
             lineP, = ax2.step(
                 time,
                 rain,
                 lw=1.5,
                 color=c2,
                 label="Précipitations"
             )
-            rmax = rain.max()
             ax2.set_ylim((rmax*1.2 if rmax else 1, -rmax/20))
             ax2.set_ylabel("$P$ (mm)")
 
             lineV, = ax3.plot(
                 time,
                 V,
                 ":",
                 color=c3,
                 label="Volume de stockage",
                 lw=1
             )
-            ax3.set_ylim((0, V.max()*1.1))
+            ax3.set_ylim((0, Vmax*1.1 if Vmax else 1))
             ax3.set_ylabel("$V$ (mm)", color=c3)
             ax3.tick_params(colors=c3, axis='y')
             ax3.grid(False)
 
             ax1.spines[['top', 'right']].set_visible(False)
             ax2.spines['bottom'].set_visible(False)
             ax3.spines[['left', 'bottom', 'top']].set_visible(False)
@@ -445,15 +442,15 @@
         title="Génie rural 4",
         entries=entries,
         *args,
         **kwargs
     )
 
 
-def gr4(catchment, rain, volume_check=True):
+def gr4(catchment, rain, volume_check=False):
 
     # Unpack GR4 parameters
     X1 = catchment.X1  # [-]
     X2 = catchment.X2  # mm
     X3 = catchment.X3  # 1/h
     X4 = catchment.X4  # h
```

### Comparing `hydrogibs-0.3.5/hydrogibs/ModelApp.py` & `hydrogibs-0.3.7/hydrogibs/ModelApp.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.5/hydrogibs/ModelTemplate.py` & `hydrogibs-0.3.7/hydrogibs/ModelTemplate.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.5/hydrogibs/QDF.py` & `hydrogibs-0.3.7/hydrogibs/QDF.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.5/hydrogibs/RationalMethod.py` & `hydrogibs-0.3.7/hydrogibs/RationalMethod.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.5/hydrogibs/SoCoSe.py` & `hydrogibs-0.3.7/hydrogibs/SoCoSe.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.5/hydrogibs/misc.py` & `hydrogibs-0.3.7/hydrogibs/misc.py`

 * *Files identical despite different names*

