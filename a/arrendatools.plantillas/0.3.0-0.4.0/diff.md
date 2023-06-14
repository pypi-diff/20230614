# Comparing `tmp/arrendatools.plantillas-0.3.0.tar.gz` & `tmp/arrendatools.plantillas-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrendatools.plantillas-0.3.0.tar", last modified: Sun Jun  4 11:50:21 2023, max compression
+gzip compressed data, was "arrendatools.plantillas-0.4.0.tar", last modified: Wed Jun 14 18:56:35 2023, max compression
```

## Comparing `arrendatools.plantillas-0.3.0.tar` & `arrendatools.plantillas-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1201 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/arrendatools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/arrendatools/plantillas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/plantillas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3110 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/fechas.py
--rw-r--r--   0 root         (0) root         (0)     3175 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/numeros.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/plantillas/plantilla.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-04 11:50:21.000000 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-04 11:50:21.000000 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 11:50:21.000000 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-04 11:50:21.000000 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-04 11:50:21.000000 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1355 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.320671 arrendatools.plantillas-0.4.0/arrendatools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/arrendatools/plantillas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/plantillas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/fechas.py
+-rw-r--r--   0 root         (0) root         (0)     3175 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/numeros.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/plantillas/plantilla.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-14 18:56:35.000000 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      538 2023-06-14 18:56:35.000000 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 18:56:35.000000 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-14 18:56:35.000000 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 18:56:35.000000 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-06-14 18:56:32.000000 arrendatools.plantillas-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/test/test_fechas.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/test/test_numeros.py
```

### Comparing `arrendatools.plantillas-0.3.0/LICENSE` & `arrendatools.plantillas-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.3.0/PKG-INFO` & `arrendatools.plantillas-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools.plantillas
-Version: 0.3.0
+Version: 0.4.0
 Summary: Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,....
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT License
         
         Copyright (c) 2023 Jordi
```

### Comparing `arrendatools.plantillas-0.3.0/README.md` & `arrendatools.plantillas-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/fechas.py` & `arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/fechas.py`

 * *Files 16% similar despite different names*

```diff
@@ -77,7 +77,29 @@
     Returns:
         str: Trimestre de la fecha indicada con el formato '<trimeste>T <año>'.
     """
     fecha_trimestre = aplicar_timedelta(fecha, dias=delta * 30 * 3)
     fecha_obj = datetime.fromisoformat(fecha_trimestre)
     num_trimestre = (fecha_obj.month - 1) // 3 + 1
     return str(num_trimestre) + 'T ' + str(fecha_obj.year)
+
+
+def dias_entre(fecha_inicio, fecha_fin):
+    """
+    Calcula los dias transcurridos entre 2 fechas.
+    El cálculo sólo cuenta días enteros, esto significa que si se quiere contar el día final entero hay que sumar 1 día.
+    Por ejemplo:
+        fecha_incio: 2023-12-01
+        fecha_fin: 2023-12-31.
+        Devuelve 30, por lo que para tener en cuenta el día 31/12 hay que usar como fecha fin 2024-01-01.
+
+    Args:
+
+        fecha_inicio (str): fecha inicial en formato ISO8601.
+        fecha_fin (str): fecha final en formato ISO8601.
+
+    Returns:
+        int: Número de días enteros que han transcurrido entre las 2 fechas.
+    """
+    fecha_inicio_obj = datetime.fromisoformat(fecha_inicio)
+    fecha_fin_obj = datetime.fromisoformat(fecha_fin)
+    return (fecha_fin_obj - fecha_inicio_obj).days
```

### Comparing `arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/numeros.py` & `arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/numeros.py`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.3.0/arrendatools/plantillas/plantilla.py` & `arrendatools.plantillas-0.4.0/arrendatools/plantillas/plantilla.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from jinja2 import Environment, FileSystemLoader, BaseLoader
-from arrendatools.plantillas.filters.fechas import dias_del_año, formato_fecha, aplicar_timedelta, trimestre
+from arrendatools.plantillas.filters.fechas import dias_del_año, formato_fecha, aplicar_timedelta, trimestre, dias_entre
 from arrendatools.plantillas.filters.numeros import formato_divisa, formato_porcentaje, numero_a_palabras
 
 
 custom_functions = {
     "aplicar_timedelta": aplicar_timedelta,
     "numero_a_palabras": numero_a_palabras,
     "formato_divisa": formato_divisa,
     "formato_porcentaje": formato_porcentaje,
     "formato_fecha": formato_fecha,
     "dias_del_año": dias_del_año,
-    "trimestre": trimestre
+    "trimestre": trimestre,
+    "dias_entre": dias_entre
 }
 
 custom_filters = {**custom_functions}
 
 
 def aplicar_plantilla(directorio_plantillas, plantilla, datos):
     environment = Environment(loader=FileSystemLoader(directorio_plantillas))
```

### Comparing `arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/PKG-INFO` & `arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools.plantillas
-Version: 0.3.0
+Version: 0.4.0
 Summary: Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,....
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT License
         
         Copyright (c) 2023 Jordi
```

### Comparing `arrendatools.plantillas-0.3.0/setup.py` & `arrendatools.plantillas-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 import pkg_resources
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 with open('LICENSE', encoding='utf-8') as f:
     license = f.read()
```

