# Comparing `tmp/bludwig-0.0.2.tar.gz` & `tmp/bludwig-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bludwig-0.0.2.tar", last modified: Tue Jun 13 06:28:30 2023, max compression
+gzip compressed data, was "bludwig-0.0.4.tar", last modified: Wed Jun 14 04:33:37 2023, max compression
```

## Comparing `bludwig-0.0.2.tar` & `bludwig-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 06:28:30.092600 bludwig-0.0.2/
--rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 bludwig-0.0.2/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)      485 2023-06-13 06:28:30.092600 bludwig-0.0.2/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)       58 2023-06-13 06:27:25.000000 bludwig-0.0.2/README.md
--rw-r--r--   0 me        (1000) me        (1000)     1114 2023-06-13 06:26:55.000000 bludwig-0.0.2/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-13 06:28:30.092600 bludwig-0.0.2/setup.cfg
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 06:28:30.084600 bludwig-0.0.2/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 06:28:30.088600 bludwig-0.0.2/src/bludwig/
--rw-rw-r--   0 me        (1000) me        (1000)    13992 2023-06-12 20:12:05.000000 bludwig-0.0.2/src/bludwig/LudwigJob.py
--rw-r--r--   0 me        (1000) me        (1000)       82 2023-06-11 18:48:52.000000 bludwig-0.0.2/src/bludwig/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      197 2023-06-10 09:59:04.000000 bludwig-0.0.2/src/bludwig/__main__.py
--rw-r--r--   0 me        (1000) me        (1000)     3798 2023-06-11 20:20:52.000000 bludwig-0.0.2/src/bludwig/helper.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 06:28:30.092600 bludwig-0.0.2/src/bludwig.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      485 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      339 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       50 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       11 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:33:37.167999 bludwig-0.0.4/
+-rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 bludwig-0.0.4/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)      488 2023-06-14 04:33:37.167999 bludwig-0.0.4/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)       58 2023-06-14 04:32:55.000000 bludwig-0.0.4/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     1124 2023-06-14 04:32:40.000000 bludwig-0.0.4/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-14 04:33:37.167999 bludwig-0.0.4/setup.cfg
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:33:37.163999 bludwig-0.0.4/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:33:37.167999 bludwig-0.0.4/src/bludwig/
+-rw-r--r--   0 me        (1000) me        (1000)    13727 2023-06-13 20:10:46.000000 bludwig-0.0.4/src/bludwig/LudwigJob.py
+-rw-r--r--   0 me        (1000) me        (1000)       82 2023-06-11 18:48:52.000000 bludwig-0.0.4/src/bludwig/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      197 2023-06-10 09:59:04.000000 bludwig-0.0.4/src/bludwig/__main__.py
+-rw-r--r--   0 me        (1000) me        (1000)     3798 2023-06-11 20:20:52.000000 bludwig-0.0.4/src/bludwig/helper.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:33:37.167999 bludwig-0.0.4/src/bludwig.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)      488 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      339 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)       50 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)       17 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)        8 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/top_level.txt
```

### Comparing `bludwig-0.0.2/LICENSE` & `bludwig-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bludwig-0.0.2/pyproject.toml` & `bludwig-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # pyproject.toml
 
 
 [project]
 name            = "bludwig"
-version         = "0.0.2"        
+version         = "0.0.4"        
 
 requires-python = ">=3.9"
-dependencies    = ['pandasklar',]
+dependencies    = ['pandasklar','munch']
 
 authors        = [{ name = "djekra", email = "hopsalla@gmail.com" }]
-description     = "Some helper for Ludwig"
+description     = "Some helper for Ludwig AI"
 readme          = "README.md"
 license         = {text = "MIT"}
 classifiers     = [
                   "Programming Language :: Python :: 3",
                   "License :: OSI Approved :: MIT License",
                   "Operating System :: OS Independent",
 ]
```

### Comparing `bludwig-0.0.2/src/bludwig/LudwigJob.py` & `bludwig-0.0.4/src/bludwig/LudwigJob.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 
         # gpu_info
         if verbose:
             gpu_info()
 
         # aktuelles model
         self.model = None
+        self.model_no = None
+        self.cuda = None
         self.output_feature_name = ''
 
         # job
         self.train_jobs = []
         self.model_names = []
         self.model_paths = []
 
@@ -90,14 +92,16 @@
         result = f'''LudwigJob object
         experiment_name:     {self.experiment_name}
         output_feature_name: {self.output_feature_name}
         train_jobs:          {self.train_jobs}
         model_names:         {self.model_names}
         model_paths:         {self.model_paths}        
         output_dirs:         {self.output_dirs}
+        model_no:            {self.model_no}   
+        cuda:                {self.cuda}             
         '''
         return result
 
 
     
     def load_from_results(self):    
         '''
@@ -124,32 +128,46 @@
         # nochmal gegenprüfen
         b = list(self.train_stats[0]['test'].keys())
         b.remove('combined')
         assert self.output_feature_name in b
 
 
     
-    def load_model(self, model_no):
+    def load_model(self, model_no, cuda=True):
         '''
-        Loads a model identified by model number
+        Loads a model identified by model number.
+        * cuda: Use cuda, if available
         '''
+        if model_no == self.model_no and cuda == self.cuda:
+            return
+            
         self.model = LudwigModel.load( self.model_paths[model_no] )
+        if cuda and torch.cuda.is_available():
+            self.model.model.to('cuda')
+            self.cuda = True
+        else:
+            self.model.model.to('cpu')   
+            self.cuda = False
+        self.model_no = model_no
+
+
 
 
         
 #####################################################################################################
 # print_models
 #
 
-    def print_model(self, model_no=0):
+    def print_model(self, model_no=None):
         '''
         Uses torchinfo.summary to print a model
         '''
-        self.load_model(model_no)
-        _ = self.model.model.to('cpu')
+        if model_no is None:
+            model_no = self.model_no
+        self.load_model(model_no, cuda=False)
         print( '### {} ###'.format(self.model_names[model_no]))
         print( summary(self.model.model, 
                        input_data=[self.model.model.get_model_inputs()], 
                        depth=20, 
                        col_names=['input_size','output_size','num_params','trainable'] 
                       ) )
         print('\n'*3)   
@@ -186,23 +204,26 @@
             except:
                 pass
 
             logging_level = 20 if self.verbose else 30
 
             # lade model
             self.model               = LudwigModel(config=self.configs[config_no], logging_level=logging_level)   
+            self.model_no            = config_no
+            self.cuda                = torch.cuda.is_available()
             self.output_feature_name = self.model.config['output_features'][0]['name']
             self.output_feature_type = self.model.config['output_features'][0]['type']
 
             # trainiere
             start_time = time.time()     
             test_stat, train_stat, _, output_dir = self.model.experiment( dataset=dataset, experiment_name=experiment_subname)
             self.test_stats  += [test_stat]
             self.train_stats += [train_stat]
             self.output_dirs += [output_dir]
+            self.model_paths += [output_dir + '/model']
 
             # logge config
             train_secs        = round( time.time() - start_time )
             train_time        = bpy.human_readable_seconds( train_secs )
             epochs            = len(train_stat.test['combined']['loss']) 
             validation_metric = self.model.config['trainer']['validation_metric']
             log = pak.dataframe([
@@ -224,14 +245,31 @@
         # logge Gesamtprozess
         self.train_log_raw = pak.add_rows( self.train_log_raw, entwirre_test_stat(self.test_stats))            
 
 
 
         
 #####################################################################################################
+# predict
+#
+
+    def predict(self, data, merge=True):
+        pred, _ = self.model.predict(data)
+        if not merge:
+            return pred
+            
+        pred.index = data.index
+        result = pd.merge( data, pred, left_index=True, right_index=True)
+        result = pak.move_cols( result, [self.output_feature_name, self.output_feature_name + '_predictions'])
+        result.rename(columns=lambda x: x.replace('_predictions', '_pred').replace('probabilities', 'prob').replace('probability', 'prob'), inplace=True)
+        return result        
+
+
+        
+#####################################################################################################
 # train_log
 #
 
     def train_log(self):
         ''' returns small log'''
         if self.train_log_raw.shape[0] > 0:
             result = prepare_train_log(self.train_log_raw, size='small')
@@ -329,31 +367,29 @@
                               model_names=self.model_names, 
                               normalize=True )
 
 
     
     def roc_curves(self, output_feature_name=None):
         '''
-Die ROC-Kurve (Receiver Operating Characteristic) ist ein grafisches Maß zur Bewertung der Leistung eines Klassifikators, wie z.B. eines neuronalen Netzwerks, insbesondere bei binären Klassifikationsproblemen. Die ROC-Kurve stellt die True Positive Rate (TPR) gegen die False Positive Rate (FPR) dar.
-
-Der Verlauf der ROC-Kurve wird durch den Schwellenwert bestimmt, der festlegt, ab welchem Ausgabewert des neuronalen Netzwerks eine Instanz als positiv oder negativ klassifiziert wird. Die Schwellenwertänderung ermöglicht es, die TPR und FPR zu variieren und somit die Leistung des Klassifikators zu analysieren.
-
-Zu Beginn, wenn der Schwellenwert sehr niedrig ist, werden viele Instanzen als positiv klassifiziert, was zu einer hohen FPR und TPR führt. Mit zunehmendem Schwellenwert werden einige wahre positive Instanzen fälschlicherweise als negativ klassifiziert, was zu einem Anstieg der FPR und einem möglichen Abfall der TPR führen kann. Wenn der Schwellenwert sehr hoch ist, werden die meisten Instanzen als negativ klassifiziert, was zu einer niedrigen FPR und TPR führt.
-
-Idealerweise strebt man bei der ROC-Analyse eine Kurve an, die möglichst nahe am linken oberen Rand des Diagramms liegt. Ein Punkt in diesem Bereich repräsentiert einen hohen TPR bei einer niedrigen FPR und deutet auf eine gute Leistung des Klassifikators hin. Ein zufälliger Klassifikator würde eine diagonal verlaufende Linie (45-Grad-Linie) erzeugen, da seine FPR und TPR gleich wären.
-
-Die Leistung des Klassifikators kann anhand des Bereichs unter der ROC-Kurve (AUC, Area Under the Curve) quantifiziert werden. Ein AUC-Wert von 1.0 bedeutet perfekte Vorhersage, während ein Wert von 0.5 einem zufälligen Klassifikator entspricht.
-
-Daher ermöglicht die ROC-Kurve die Beurteilung und Vergleich der Leistung eines neuronalen Netzwerks für verschiedene Schwellenwerte und unterstützt bei der Auswahl des optimalen Schwellenwerts, abhängig von den Anforderungen des Anwendungsfalls.        
+    
         '''
         # Kein bestimmer output_feature_name angefragt >> Default
         if output_feature_name is None:
             output_feature_name = self.output_feature_name  
             
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
-            roc_curves_from_test_statistics(self.test_stats, output_feature_name=output_feature_name)   
-        
-        
+            try:
+                roc_curves_from_test_statistics(self.test_stats, output_feature_name=output_feature_name)   
+            except KeyError:
+                print('No roc_curve found')
+                pass
+            except TypeError:
+                print('No roc_curve found')
+                pass                
+            except:
+                raise  # Löst die Ausnahme erneut aus        
+
```

### Comparing `bludwig-0.0.2/src/bludwig/helper.py` & `bludwig-0.0.4/src/bludwig/helper.py`

 * *Files identical despite different names*

