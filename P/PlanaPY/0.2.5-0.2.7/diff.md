# Comparing `tmp/PlanaPY-0.2.5.tar.gz` & `tmp/PlanaPY-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlanaPY-0.2.5.tar", last modified: Mon Jun 12 23:16:31 2023, max compression
+gzip compressed data, was "PlanaPY-0.2.7.tar", last modified: Wed Jun 14 21:45:22 2023, max compression
```

## Comparing `PlanaPY-0.2.5.tar` & `PlanaPY-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 23:16:31.076651 PlanaPY-0.2.5/
--rw-rw-rw-   0        0        0      286 2023-06-12 23:16:31.076651 PlanaPY-0.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 23:16:31.070490 PlanaPY-0.2.5/PlanaPY/
--rw-rw-rw-   0        0        0    15821 2023-06-12 23:11:46.000000 PlanaPY-0.2.5/PlanaPY/PlanaPY.py
--rw-rw-rw-   0        0        0       21 2023-06-09 20:22:08.000000 PlanaPY-0.2.5/PlanaPY/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:16:31.075656 PlanaPY-0.2.5/PlanaPY.egg-info/
--rw-rw-rw-   0        0        0      286 2023-06-12 23:16:30.000000 PlanaPY-0.2.5/PlanaPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-12 23:16:31.000000 PlanaPY-0.2.5/PlanaPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 23:16:30.000000 PlanaPY-0.2.5/PlanaPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-12 23:16:30.000000 PlanaPY-0.2.5/PlanaPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 23:16:30.000000 PlanaPY-0.2.5/PlanaPY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 23:16:31.076651 PlanaPY-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      485 2023-06-12 23:16:17.000000 PlanaPY-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 21:45:22.961461 PlanaPY-0.2.7/
+-rw-rw-rw-   0        0        0      286 2023-06-14 21:45:22.960683 PlanaPY-0.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 21:45:22.952093 PlanaPY-0.2.7/PlanaPY/
+-rw-rw-rw-   0        0        0    16725 2023-06-14 21:23:23.000000 PlanaPY-0.2.7/PlanaPY/PlanaPY.py
+-rw-rw-rw-   0        0        0       21 2023-06-09 20:22:08.000000 PlanaPY-0.2.7/PlanaPY/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 21:45:22.959512 PlanaPY-0.2.7/PlanaPY.egg-info/
+-rw-rw-rw-   0        0        0      286 2023-06-14 21:45:22.000000 PlanaPY-0.2.7/PlanaPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-14 21:45:22.000000 PlanaPY-0.2.7/PlanaPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 21:45:22.000000 PlanaPY-0.2.7/PlanaPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 21:45:22.000000 PlanaPY-0.2.7/PlanaPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 21:45:22.000000 PlanaPY-0.2.7/PlanaPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 21:45:22.961461 PlanaPY-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      485 2023-06-14 21:45:16.000000 PlanaPY-0.2.7/setup.py
```

### Comparing `PlanaPY-0.2.5/PlanaPY/PlanaPY.py` & `PlanaPY-0.2.7/PlanaPY/PlanaPY.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,15 +248,29 @@
         
         actions = self.get_request(URL)['exports']
         
         for a in actions:
             exports_dict[a['name']] = a
         
         return exports_dict
+    
+    def get_export_metadata(self, model, workspace, export):
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        export_id = self.get_export_actions(model=model, workspace=workspace)[export]['id']
+        
+        URL = self.api.api_url + "models/{0}/exports/{1}".format(model_id, export_id)
         
+        metadata = self.get_request(URL)['exportMetadata']
+        
+        columns = metadata['headerNames']
+        #export_format = metadata['exportFormat']
+        delimiter = metadata['separator']
+                
+        return columns, delimiter
+    
     def run_export_action(self, model, workspace, export):
         self.api.headers['Content-Type'] = 'application/json'
         model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
         action_id = self.get_export_actions(model=model, workspace=workspace)[export]['id']
         
         URL = self.api.api_url + "models/{0}/exports/{1}/tasks".format(model_id, action_id)
         body = {'localeName': 'en_US'}
@@ -268,30 +282,38 @@
             print("Export action {0} successfully ran in model {1}".format(file, model))
         
         return self.resp 
     
     def export_data(self, model, workspace, export):
         model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
         file_id = self.get_model_files(model=model, workspace = workspace)[export]['id']
+
+        columns, delimiter = self.get_export_metadata(model=model, workspace=workspace, export=export)
         
         URL = self.api.api_url + "models/{0}/files/{1}/chunks".format(model_id, file_id)
-        
+
         chunks = self.get_request(URL)['chunks']
-        
+
         chunk_list = []
         
         for c in chunks:
             chunk_id = c['id']
             chunk_URL = self.api.api_url + "models/{0}/files/{1}/chunks/{2}".format(model_id, file_id, chunk_id)
             chunk = requests.get(chunk_URL, headers = self.api.headers).content
-            df = pd.read_csv(io.StringIO(chunk.decode('utf-8')), header=None)
+            df = pd.read_csv(
+                io.StringIO(chunk.decode('utf-8')), 
+                header=None, 
+                sep=delimiter, 
+                error_bad_lines=False,
+                warn_bad_lines=True)
             chunk_list.append(df)
 
         all_chunks = pd.concat(chunk_list).reset_index()
         all_chunks.columns = all_chunks.iloc[0]
+        #all_chunks.columns = columns
         all_chunks.drop(all_chunks.index[0], inplace=True)
         all_chunks = all_chunks.iloc[:,1:]
         
         return all_chunks       
         
     def change_model_status(self, model, workspace, status):
         model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
```

