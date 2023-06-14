# Comparing `tmp/FlyBaseDownloads-1.0.0.tar.gz` & `tmp/FlyBaseDownloads-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyBaseDownloads-1.0.0.tar", last modified: Tue Jun 13 21:46:32 2023, max compression
+gzip compressed data, was "FlyBaseDownloads-1.0.1.tar", last modified: Wed Jun 14 01:01:29 2023, max compression
```

## Comparing `FlyBaseDownloads-1.0.0.tar` & `FlyBaseDownloads-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-13 21:46:32.252022 FlyBaseDownloads-1.0.0/
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-13 21:46:32.252022 FlyBaseDownloads-1.0.0/FlyBaseDownloads/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    12357 2023-06-13 21:02:15.000000 FlyBaseDownloads-1.0.0/FlyBaseDownloads/FBD.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      480 2023-06-13 21:24:44.000000 FlyBaseDownloads-1.0.0/FlyBaseDownloads/__init__.py
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-13 21:46:32.252022 FlyBaseDownloads-1.0.0/FlyBaseDownloads.egg-info/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      600 2023-06-13 21:46:32.000000 FlyBaseDownloads-1.0.0/FlyBaseDownloads.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      231 2023-06-13 21:46:32.000000 FlyBaseDownloads-1.0.0/FlyBaseDownloads.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-13 21:46:32.000000 FlyBaseDownloads-1.0.0/FlyBaseDownloads.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-13 21:46:32.000000 FlyBaseDownloads-1.0.0/FlyBaseDownloads.egg-info/top_level.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      600 2023-06-13 21:46:32.252022 FlyBaseDownloads-1.0.0/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       77 2023-06-13 21:44:04.000000 FlyBaseDownloads-1.0.0/README.md
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       38 2023-06-13 21:46:32.252022 FlyBaseDownloads-1.0.0/setup.cfg
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      865 2023-06-13 21:46:24.000000 FlyBaseDownloads-1.0.0/setup.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 01:01:29.020763 FlyBaseDownloads-1.0.1/
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 01:01:29.020763 FlyBaseDownloads-1.0.1/FlyBaseDownloads/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    12920 2023-06-14 00:43:17.000000 FlyBaseDownloads-1.0.1/FlyBaseDownloads/FBD.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      480 2023-06-13 21:24:44.000000 FlyBaseDownloads-1.0.1/FlyBaseDownloads/__init__.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 01:01:29.020763 FlyBaseDownloads-1.0.1/FlyBaseDownloads.egg-info/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      600 2023-06-14 01:01:28.000000 FlyBaseDownloads-1.0.1/FlyBaseDownloads.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      241 2023-06-14 01:01:28.000000 FlyBaseDownloads-1.0.1/FlyBaseDownloads.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-14 01:01:28.000000 FlyBaseDownloads-1.0.1/FlyBaseDownloads.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-14 01:01:28.000000 FlyBaseDownloads-1.0.1/FlyBaseDownloads.egg-info/top_level.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      600 2023-06-14 01:01:29.020763 FlyBaseDownloads-1.0.1/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)     4709 2023-06-14 01:00:42.000000 FlyBaseDownloads-1.0.1/README.md
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-14 01:01:29.020763 FlyBaseDownloads-1.0.1/setup.cfg
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      865 2023-06-13 23:01:58.000000 FlyBaseDownloads-1.0.1/setup.py
```

### Comparing `FlyBaseDownloads-1.0.0/FlyBaseDownloads/FBD.py` & `FlyBaseDownloads-1.0.1/FlyBaseDownloads/FBD.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,27 +53,41 @@
 
             ftp.quit()
             if len(archivos) > 0:
                 return archivos
             else:
                 print('Failed to download the file')
                 return []
+            
         
         
         
         def open_file(self, ruta_archivo, header):
+            def df_r(df):
+                if re.search(r"FB\w{9}", df.columns[0]):
+                    df_columns = pd.DataFrame(df.columns).T
+
+                    df.columns = range(len(df.columns))
+                    
+                    # Unir la fila de columnas con el resto del DataFrame
+                    df = pd.concat([df_columns, df], ignore_index=True, axis = 0)
+                
+                if re.search('## Finished', df.iloc[-1,0]):
+                    df = df.iloc[:-1, :]
+                
+                return df
             a = []
 
             if re.search(r'gz', ruta_archivo):
                 
                 try: 
                     with gzip.open('../' + ruta_archivo, 'rt') as archivo:
                        df = pd.read_csv(archivo, sep='\t', header=header)
                        a.append(df)
-                    return a[0]
+                    return df_r(a[0])
                 
                 except: 
                     try:
                         with gzip.open('../' + ruta_archivo, 'rt') as archivo:
                             df = csv.reader(archivo, delimiter='\t')
                             a.append(pd.DataFrame(df))
                     
@@ -84,15 +98,15 @@
                         df = df.iloc[header + 1:, :]
                         
                         # Asigna los nuevos nombres de columna al DataFrame
                         df.columns = columns
                         df = df.dropna(axis='columns')
                       
       
-                        return df
+                        return df_r(df)
                     except:
                         print('Failed to download the file') 
             
                     
     
     class Synonyms():
```

### Comparing `FlyBaseDownloads-1.0.0/FlyBaseDownloads.egg-info/PKG-INFO` & `FlyBaseDownloads-1.0.1/FlyBaseDownloads.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `FlyBaseDownloads-1.0.0/PKG-INFO` & `FlyBaseDownloads-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `FlyBaseDownloads-1.0.0/setup.py` & `FlyBaseDownloads-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: javiera.quiroz
 """
 
 from setuptools import setup
 
 setup(
     name='FlyBaseDownloads',
-    version='1.0.0',
+    version='1.0.1',
     license='MIT',
     author='Javiera Quiroz Olave',
     url= 'https://github.com/JavieraQuirozO/FlyBaseDownloads',
     author_email='javiera.quiroz@biomedica.udec.cl',
     long_description_content_type='text/x-rst',
     long_description= 'The non-official FlyBaseDownload Packege',
     description='Package to download Flybase data in Python, easily and quickly.',
```

