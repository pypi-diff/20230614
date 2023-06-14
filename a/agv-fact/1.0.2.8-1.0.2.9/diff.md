# Comparing `tmp/agv-fact-1.0.2.8.tar.gz` & `tmp/agv-fact-1.0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/agv-fact-1.0.2.8.tar", last modified: Thu Sep  8 00:06:45 2022, max compression
+gzip compressed data, was "dist/agv-fact-1.0.2.9.tar", last modified: Mon Sep 12 15:27:34 2022, max compression
```

## Comparing `agv-fact-1.0.2.8.tar` & `agv-fact-1.0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/fact/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/fact/generator/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/fact/generator/cadenaoriginal_3_3_local/
--rw-rw-r--   0 andres    (1000) andres    (1000)        0 2021-07-30 02:38:41.000000 agv-fact-1.0.2.8/fact/generator/cadenaoriginal_3_3_local/__init__.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    37964 2022-07-12 07:02:04.000000 agv-fact-1.0.2.8/fact/generator/generator33.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      397 2021-07-30 02:38:41.000000 agv-fact-1.0.2.8/fact/generator/utils.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    38807 2022-09-08 00:06:16.000000 agv-fact-1.0.2.8/fact/generator/generator40.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      282 2022-07-08 22:32:21.000000 agv-fact-1.0.2.8/fact/generator/contants.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      483 2022-06-09 18:28:53.000000 agv-fact-1.0.2.8/fact/generator/services.py
--rw-rw-r--   0 andres    (1000) andres    (1000)        0 2021-07-30 02:38:41.000000 agv-fact-1.0.2.8/fact/generator/__init__.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     7398 2022-07-08 20:41:51.000000 agv-fact-1.0.2.8/fact/generator/generator_abstract.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/fact/services/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1505 2021-07-30 02:38:41.000000 agv-fact-1.0.2.8/fact/services/factory.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2154 2021-07-30 02:38:41.000000 agv-fact-1.0.2.8/fact/services/exceptions.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    13665 2021-10-06 18:18:09.000000 agv-fact-1.0.2.8/fact/services/services.py
--rw-rw-r--   0 andres    (1000) andres    (1000)        0 2021-07-30 02:38:41.000000 agv-fact-1.0.2.8/fact/services/__init__.py
--rw-rw-r--   0 andres    (1000) andres    (1000)        0 2021-07-30 02:38:41.000000 agv-fact-1.0.2.8/fact/__init__.py
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/agv_fact.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)        5 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/agv_fact.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)      802 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/agv_fact.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/agv_fact.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)      523 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/agv_fact.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)      802 2022-09-08 00:06:45.000000 agv-fact-1.0.2.8/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      815 2022-09-08 00:06:42.000000 agv-fact-1.0.2.8/setup.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      533 2022-06-09 18:28:53.000000 agv-fact-1.0.2.8/README.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-12 15:27:34.000000 agv-fact-1.0.2.9/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-12 15:27:34.000000 agv-fact-1.0.2.9/fact/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-12 15:27:34.000000 agv-fact-1.0.2.9/fact/generator/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-12 15:27:34.000000 agv-fact-1.0.2.9/fact/generator/cadenaoriginal_3_3_local/
+-rw-rw-r--   0 andres    (1000) andres    (1000)        0 2021-07-30 02:38:41.000000 agv-fact-1.0.2.9/fact/generator/cadenaoriginal_3_3_local/__init__.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    37964 2022-07-12 07:02:04.000000 agv-fact-1.0.2.9/fact/generator/generator33.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      397 2021-07-30 02:38:41.000000 agv-fact-1.0.2.9/fact/generator/utils.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    38807 2022-09-12 15:27:29.000000 agv-fact-1.0.2.9/fact/generator/generator40.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      282 2022-07-08 22:32:21.000000 agv-fact-1.0.2.9/fact/generator/contants.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      483 2022-06-09 18:28:53.000000 agv-fact-1.0.2.9/fact/generator/services.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)        0 2021-07-30 02:38:41.000000 agv-fact-1.0.2.9/fact/generator/__init__.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7398 2022-07-08 20:41:51.000000 agv-fact-1.0.2.9/fact/generator/generator_abstract.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-12 15:27:34.000000 agv-fact-1.0.2.9/fact/services/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1505 2021-07-30 02:38:41.000000 agv-fact-1.0.2.9/fact/services/factory.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2154 2021-07-30 02:38:41.000000 agv-fact-1.0.2.9/fact/services/exceptions.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    13665 2021-10-06 18:18:09.000000 agv-fact-1.0.2.9/fact/services/services.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)        0 2021-07-30 02:38:41.000000 agv-fact-1.0.2.9/fact/services/__init__.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)        0 2021-07-30 02:38:41.000000 agv-fact-1.0.2.9/fact/__init__.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2022-09-12 15:27:34.000000 agv-fact-1.0.2.9/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2022-09-12 15:27:34.000000 agv-fact-1.0.2.9/agv_fact.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)        5 2022-09-12 15:27:33.000000 agv-fact-1.0.2.9/agv_fact.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)      802 2022-09-12 15:27:33.000000 agv-fact-1.0.2.9/agv_fact.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2022-09-12 15:27:33.000000 agv-fact-1.0.2.9/agv_fact.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)      523 2022-09-12 15:27:33.000000 agv-fact-1.0.2.9/agv_fact.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)      802 2022-09-12 15:27:34.000000 agv-fact-1.0.2.9/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      815 2022-09-12 15:27:29.000000 agv-fact-1.0.2.9/setup.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      533 2022-06-09 18:28:53.000000 agv-fact-1.0.2.9/README.txt
```

### Comparing `agv-fact-1.0.2.8/fact/generator/generator33.py` & `agv-fact-1.0.2.9/fact/generator/generator33.py`

 * *Files identical despite different names*

### Comparing `agv-fact-1.0.2.8/fact/generator/generator40.py` & `agv-fact-1.0.2.9/fact/generator/generator40.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -443,24 +443,24 @@
                 conceptos.appendChild(cfdi_concepto)
             except Exception as e:
                 raise Exception("Ocurrio un error. Error::: " + str(e))
         return conceptos
 
     def get_impuestos_concepto(self,concepto):
         impuestos = self.dom.createElement('cfdi:Impuestos')
-        if len(concepto.get('retenciones', [])) > 0:
-            retenciones = self.dom.createElement('cfdi:Retenciones')
-            for retencion in concepto.get('retenciones', []):
-                retenciones.appendChild(self.get_retenciones_concepto(retencion))
-            impuestos.appendChild(retenciones)
         if len(concepto.get('traslados', [])) > 0:
             traslados = self.dom.createElement('cfdi:Traslados')
             for traslado in concepto.get('traslados', []):
                 traslados.appendChild(self.get_traslados_concepto(traslado))
             impuestos.appendChild(traslados)
+        if len(concepto.get('retenciones', [])) > 0:
+            retenciones = self.dom.createElement('cfdi:Retenciones')
+            for retencion in concepto.get('retenciones', []):
+                retenciones.appendChild(self.get_retenciones_concepto(retencion))
+            impuestos.appendChild(retenciones)
         return impuestos
 
     def get_traslados_concepto(self, traslado_data):
         traslado = self.dom.createElement('cfdi:Traslado')
         traslado.setAttribute('Base', str(traslado_data.get('base')))  # Importe del concepto
         traslado.setAttribute('Impuesto', traslado_data.get('impuesto', ''))
         traslado.setAttribute('TipoFactor', traslado_data.get('tipo_factor', 'Tasa'))
```

### Comparing `agv-fact-1.0.2.8/fact/generator/generator_abstract.py` & `agv-fact-1.0.2.9/fact/generator/generator_abstract.py`

 * *Files identical despite different names*

### Comparing `agv-fact-1.0.2.8/fact/services/factory.py` & `agv-fact-1.0.2.9/fact/services/factory.py`

 * *Files identical despite different names*

### Comparing `agv-fact-1.0.2.8/fact/services/exceptions.py` & `agv-fact-1.0.2.9/fact/services/exceptions.py`

 * *Files identical despite different names*

### Comparing `agv-fact-1.0.2.8/fact/services/services.py` & `agv-fact-1.0.2.9/fact/services/services.py`

 * *Files identical despite different names*

### Comparing `agv-fact-1.0.2.8/agv_fact.egg-info/PKG-INFO` & `agv-fact-1.0.2.9/agv_fact.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agv-fact
-Version: 1.0.2.8
+Version: 1.0.2.9
 Summary: Libreria para generar xml y realizar el timbrado
 Home-page: https://github.com/pypa/fact
 Author: Andres Alvarado Vazquez
 Author-email: andres@agavesoft.com.mx
 License: UNKNOWN
 Description: # README #
```

### Comparing `agv-fact-1.0.2.8/agv_fact.egg-info/SOURCES.txt` & `agv-fact-1.0.2.9/agv_fact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agv-fact-1.0.2.8/PKG-INFO` & `agv-fact-1.0.2.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agv-fact
-Version: 1.0.2.8
+Version: 1.0.2.9
 Summary: Libreria para generar xml y realizar el timbrado
 Home-page: https://github.com/pypa/fact
 Author: Andres Alvarado Vazquez
 Author-email: andres@agavesoft.com.mx
 License: UNKNOWN
 Description: # README #
```

### Comparing `agv-fact-1.0.2.8/setup.py` & `agv-fact-1.0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="agv-fact",
-    version="1.0.2.8",
+    version="1.0.2.9",
     author="Andres Alvarado Vazquez",
     author_email="andres@agavesoft.com.mx",
     description="Libreria para generar xml y realizar el timbrado",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/fact",
     packages=setuptools.find_packages(),
```

### Comparing `agv-fact-1.0.2.8/README.txt` & `agv-fact-1.0.2.9/README.txt`

 * *Files identical despite different names*

