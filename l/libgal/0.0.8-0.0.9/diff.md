# Comparing `tmp/libgal-0.0.8.tar.gz` & `tmp/libgal-0.0.9.tar.gz`

## Comparing `libgal-0.0.8.tar` & `libgal-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 libgal-0.0.8/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libgal-0.0.8/gitignore
--rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 libgal-0.0.8/libgal.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.8/libgal.py.bak
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 libgal-0.0.8/pyproject.toml.bak
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 libgal-0.0.8/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libgal-0.0.8/libgal_package/libgal/__init__.py.bak
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.8/libgal_package/libgal/libgal.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libgal-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 libgal-0.0.8/README.md
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 libgal-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    13669 2020-02-02 00:00:00.000000 libgal-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 libgal-0.0.9/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libgal-0.0.9/gitignore
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 libgal-0.0.9/libgal.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.9/libgal.py.bak
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 libgal-0.0.9/pyproject.toml.bak
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 libgal-0.0.9/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libgal-0.0.9/libgal_package/libgal/__init__.py.bak
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.9/libgal_package/libgal/libgal.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libgal-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 libgal-0.0.9/README.md
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 libgal-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    13669 2020-02-02 00:00:00.000000 libgal-0.0.9/PKG-INFO
```

### Comparing `libgal-0.0.8/libgal.py` & `libgal-0.0.9/libgal.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,37 +35,29 @@
     from sqlalchemy.orm import sessionmaker
     from sqlalchemy.ext.declarative import declarative_base
     
 except ImportError as imp_err:
     # Freno ejecucion y devuelvo codigo de error
     raise ImportError(f"Error al importar libreria: {imp_err}")
 
-def variables_entorno(path_env_file: str = None):
+def variables_entorno(path_env_file = None):
 
     """
     Descripción: Toma las variables de entorno del archivo .env o del SO
     Parámetro:
     - path_env_file (String): 
     """
     
-    if path_env_file:
+    if path_env_file!=None and Path(path_env_file).exists():
         
-        env_file=Path(path_env_file)
-
-        if env_file.exists():
-            load_dotenv(env_file)
-        else:
-            raise Exception(f"No existe el archivo {env_file} indicado para funcion variables_entorno() de libgal")
+        load_dotenv(path_env_file)
 
     else:
-
-        env_file = Path(os.path.dirname(os.path.abspath(__file__))) / '.env'
-
-        if env_file.exists():
-            load_dotenv(env_file)
+        
+        print(f"No se encontró el archivo {path_env_file} indicado para funcion variables_entorno() de libgal por lo que se toma las variables de entorno de sistema.")
     
     return dict(os.environ)
     
     
 def logger(format_output="JSON", app_name=__name__):
     
     """
```

### Comparing `libgal-0.0.8/libgal.py.bak` & `libgal-0.0.9/libgal.py.bak`

 * *Files identical despite different names*

### Comparing `libgal-0.0.8/pyproject.toml.bak` & `libgal-0.0.9/pyproject.toml.bak`

 * *Files identical despite different names*

### Comparing `libgal-0.0.8/libgal_package/libgal/libgal.py` & `libgal-0.0.9/libgal_package/libgal/libgal.py`

 * *Files identical despite different names*

### Comparing `libgal-0.0.8/LICENSE.txt` & `libgal-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libgal-0.0.8/README.md` & `libgal-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `libgal-0.0.8/pyproject.toml` & `libgal-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "libgal"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Jean Manuel González Mejía", email="ebrainding@gmail.com" },
 ]
 
 license = { file = "LICENSE.txt" }
 
 description = "Librería para agilizar el desarrollo de nuestros programadores en el Banco Galicia"
```

### Comparing `libgal-0.0.8/PKG-INFO` & `libgal-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libgal
-Version: 0.0.8
+Version: 0.0.9
 Summary: Librería para agilizar el desarrollo de nuestros programadores en el Banco Galicia
 Project-URL: Homepage, https://github.com/Banco-Galicia/libgal
 Project-URL: Bug Tracker, https://github.com/Banco-Galicia/libgal/issues
 Author-email: Jean Manuel González Mejía <ebrainding@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 JEAN MANUEL GONZÁLEZ MEJÍA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libgal Version: 0.0.8 Summary: LibrerÃ­a para
+Metadata-Version: 2.1 Name: libgal Version: 0.0.9 Summary: LibrerÃ­a para
 agilizar el desarrollo de nuestros programadores en el Banco Galicia Project-
 URL: Homepage, https://github.com/Banco-Galicia/libgal Project-URL: Bug
 Tracker, https://github.com/Banco-Galicia/libgal/issues Author-email: Jean
 Manuel GonzÃ¡lez MejÃ­a
 gmail.com> License: MIT License Copyright (c) 2022 JEAN MANUEL GONZÃLEZ MEJÃA
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
```

