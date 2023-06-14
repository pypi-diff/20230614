# Comparing `tmp/challengerteco-0.1.8.tar.gz` & `tmp/challengerteco-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "challengerteco-0.1.8.tar", max compression
+gzip compressed data, was "challengerteco-0.1.9.tar", max compression
```

## Comparing `challengerteco-0.1.8.tar` & `challengerteco-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.8/README.md
--rw-r--r--   0        0        0    83013 2023-05-23 15:03:49.708078 challengerteco-0.1.8/challengerteco/Challenger.py
--rw-r--r--   0        0        0       86 2023-04-20 16:51:54.029080 challengerteco-0.1.8/challengerteco/__init__.py
--rw-r--r--   0        0        0      357 2023-05-23 15:05:14.517929 challengerteco-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 challengerteco-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.9/README.md
+-rw-r--r--   0        0        0    83013 2023-05-30 14:10:29.671227 challengerteco-0.1.9/challengerteco/Challenger.py
+-rw-r--r--   0        0        0       86 2023-04-20 16:51:54.029080 challengerteco-0.1.9/challengerteco/__init__.py
+-rw-r--r--   0        0        0      357 2023-05-30 14:10:36.104495 challengerteco-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 challengerteco-0.1.9/PKG-INFO
```

### Comparing `challengerteco-0.1.8/challengerteco/Challenger.py` & `challengerteco-0.1.9/challengerteco/Challenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
             query=f"DROP TABLE IF EXISTS   " + self.qm.getNombreTabla(f"tmp_challenger_{self.modelo}_0")
             self.qm.execute_query(query)
             print("INFORMACION DE SEGUIMIENTO: DROP TABLA _0")
         except:
             pass
 
         try:
-            query=f"DROP TABLE IF EXISTS   " + self.qm.getNombreTabla(f"tmp_challenger_{self.modelo}_Q")
+            query=f"DROP TABLE IF EXISTS   " + self.qm.getNombreTabla(f"tmp_challenger_{self.modelo}_1")
             self.qm.execute_query(query)
             print("INFORMACION DE SEGUIMIENTO: DROP TABLA _1")
         except:
             pass
 
         try:
             query=f"DROP TABLE IF EXISTS   " + self.qm.getNombreTabla(f"tmp_challenger_{self.modelo}_2")
```

### Comparing `challengerteco-0.1.8/PKG-INFO` & `challengerteco-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: challengerteco
-Version: 0.1.8
+Version: 0.1.9
 Summary: Clase para manejo de challenger en la nube
 Author: Eduardo Pagnone
 Author-email: mlopsaa@teco.com.ar
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

