# Comparing `tmp/memento-scorecard-0.2.7.tar.gz` & `tmp/memento-scorecard-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memento-scorecard-0.2.7.tar", last modified: Wed Jun  7 21:40:12 2023, max compression
+gzip compressed data, was "memento-scorecard-0.3.3.tar", last modified: Tue Jun 13 23:10:04 2023, max compression
```

## Comparing `memento-scorecard-0.2.7.tar` & `memento-scorecard-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 21:40:12.456616 memento-scorecard-0.2.7/
--rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     1157 2023-06-07 21:40:12.454006 memento-scorecard-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 21:40:12.443029 memento-scorecard-0.2.7/memento/
--rw-rw-rw-   0        0        0     1144 2023-06-07 21:37:46.000000 memento-scorecard-0.2.7/memento/__init__.py
--rw-rw-rw-   0        0        0    20799 2023-06-07 14:51:04.000000 memento-scorecard-0.2.7/memento/bojack.py
--rw-rw-rw-   0        0        0     7612 2023-06-07 14:48:04.000000 memento-scorecard-0.2.7/memento/diane.py
--rw-rw-rw-   0        0        0    15680 2023-06-07 14:48:05.000000 memento-scorecard-0.2.7/memento/mr_peanutbutter.py
--rw-rw-rw-   0        0        0    23651 2023-06-07 14:48:05.000000 memento-scorecard-0.2.7/memento/princess_carolyn.py
--rw-rw-rw-   0        0        0     3241 2023-06-07 14:48:03.000000 memento-scorecard-0.2.7/memento/todd.py
-drwxrwxrwx   0        0        0        0 2023-06-07 21:40:12.452047 memento-scorecard-0.2.7/memento_scorecard.egg-info/
--rw-rw-rw-   0        0        0     1157 2023-06-07 21:40:12.000000 memento-scorecard-0.2.7/memento_scorecard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-07 21:40:12.000000 memento-scorecard-0.2.7/memento_scorecard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 21:40:12.000000 memento-scorecard-0.2.7/memento_scorecard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 21:40:12.000000 memento-scorecard-0.2.7/memento_scorecard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 21:40:12.456616 memento-scorecard-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:10:04.010100 memento-scorecard-0.3.3/
+-rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     1157 2023-06-13 23:10:04.008592 memento-scorecard-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 23:10:03.994713 memento-scorecard-0.3.3/memento/
+-rw-rw-rw-   0        0        0     1314 2023-06-13 23:08:59.000000 memento-scorecard-0.3.3/memento/__init__.py
+-rw-rw-rw-   0        0        0    26294 2023-06-13 22:34:11.000000 memento-scorecard-0.3.3/memento/bojack.py
+-rw-rw-rw-   0        0        0     7624 2023-06-13 22:35:02.000000 memento-scorecard-0.3.3/memento/diane.py
+-rw-rw-rw-   0        0        0    20229 2023-06-13 22:27:44.000000 memento-scorecard-0.3.3/memento/mr_peanutbutter.py
+-rw-rw-rw-   0        0        0    23669 2023-06-13 22:24:33.000000 memento-scorecard-0.3.3/memento/princess_carolyn.py
+-rw-rw-rw-   0        0        0     3251 2023-06-13 22:21:16.000000 memento-scorecard-0.3.3/memento/todd.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:10:04.005599 memento-scorecard-0.3.3/memento_scorecard.egg-info/
+-rw-rw-rw-   0        0        0     1157 2023-06-13 23:10:03.000000 memento-scorecard-0.3.3/memento_scorecard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-13 23:10:03.000000 memento-scorecard-0.3.3/memento_scorecard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 23:10:03.000000 memento-scorecard-0.3.3/memento_scorecard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 23:10:03.000000 memento-scorecard-0.3.3/memento_scorecard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 23:10:04.011268 memento-scorecard-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-0.3.3/setup.py
```

### Comparing `memento-scorecard-0.2.7/LICENSE` & `memento-scorecard-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.2.7/PKG-INFO` & `memento-scorecard-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 0.2.7
+Version: 0.3.3
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
 Platform: UNKNOWN
```

### Comparing `memento-scorecard-0.2.7/memento/__init__.py` & `memento-scorecard-0.3.3/memento/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from memento.todd import (string_categories1, string_categories2, string_to_num,
 breakpoints_to_str, breakpoints_to_num, remapeo_missing, data_convert, adapt_data)
 from memento.diane import (compute_group_names, compute_table, transform_to_woes,
 calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics)
 from memento.princess_carolyn import (compute_final_breakpoints,
 compute_info, features_selection, display_table_ng, reagrupa_var)
-from memento.mr_peanutbutter import pretty_scorecard, parceling, cell_style, proc_freq
+from memento.mr_peanutbutter import (pretty_scorecard, parceling, cell_style, predict_pyspark,
+metrics_pyspark, compute_pyspark_ks, save_model, save_light_model, load_model, proc_freq)
 from memento.bojack import scorecard, autogrouping
 
-__version__ = '0.2.7'
+__version__ = '0.3.3'
 
 __all__ = (
     string_categories1, string_categories2, string_to_num,
     breakpoints_to_str, breakpoints_to_num, remapeo_missing, data_convert, adapt_data,
     compute_group_names, compute_table, transform_to_woes,
     calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics,
     compute_final_breakpoints,
     compute_info, features_selection, display_table_ng, reagrupa_var,
-    pretty_scorecard, parceling, cell_style, proc_freq,
-    scorecard, autogrouping
+    pretty_scorecard, parceling, cell_style, predict_pyspark,
+    metrics_pyspark, compute_pyspark_ks, save_model, save_light_model, load_model, proc_freq
 )
```

### Comparing `memento-scorecard-0.2.7/memento/bojack.py` & `memento-scorecard-0.3.3/memento/bojack.py`

 * *Files 22% similar despite different names*

```diff
@@ -150,15 +150,14 @@
         if self.autogrp_all: variables = X.columns
         else: 
             if self.features != []: variables = self.features
             else: variables = list(set(list(X.columns)) - set(self.excluded_vars))
 
         autogroupings = {}
         variables_no_agrupadas_error = []
-        variables_no_agrupadas_raras = []
 
         for variable in variables:
 
             try:
                 
                 if variable in self.autogrp_dict_max_groups:
                     max_groups = self.autogrp_dict_max_groups[variable]
@@ -167,51 +166,44 @@
                 if variable in self.autogrp_dict_min_pct:
                     min_pct = self.autogrp_dict_min_pct[variable]
                 else: min_pct = self.autogrp_min_pct
 
                 x = X_train[variable].values
                 frenken = autogrouping(max_groups=max_groups, min_pct=min_pct).fit(x, y_train)
 
-                if len(frenken.breakpoints_num) == 0: variables_no_agrupadas_raras.append(variable)
+                if len(frenken.breakpoints_num) == 0: variables_no_agrupadas_error.append(variable)
                 else: autogroupings[variable] = frenken
  
             except:
                 variables_no_agrupadas_error.append(variable)
 
         print('Autogrouping terminado. Máximo número de buckets = {}. Mínimo porcentaje '
         'por bucket = {}'.format(self.autogrp_max_groups, self.autogrp_min_pct))
         print('-' * N)
 
-        if len(variables_no_agrupadas_raras) > 0:
-            print('Variables no agrupadas por algún motivo extraño: {}'\
-            .format(variables_no_agrupadas_raras))
-            print('-' * N)
-
         if len(variables_no_agrupadas_error) > 0:
             print('Variables no agrupadas por algún error, seguramente por excesiva '
             'concentración en algún valor (> 95%) : {}'.format(variables_no_agrupadas_error))
             print('-' * N)
-
-        self.variables_no_agrupadas_raras = variables_no_agrupadas_raras
+            
         self.variables_no_agrupadas_error = variables_no_agrupadas_error
 
         tabla_ivs, contador = pd.DataFrame(columns=['variable', 'iv']), 0
         for variable in autogroupings:
             tabla_ivs.loc[contador] = variable, autogroupings[variable].iv
             contador += 1
         tabla_ivs = tabla_ivs.sort_values('iv', ascending=False).reset_index(drop=True)
 
         self.tabla_ivs = tabla_ivs
-
+        
         variables_filtro_iv = tabla_ivs[tabla_ivs['iv'] >= self.iv_threshold]['variable']
         
         if self.features != []: variables_def = self.features
         else:
-            variables_def = list(set(variables_filtro_iv) - 
-            set(variables_no_agrupadas_raras) - set(variables_no_agrupadas_error))
+            variables_def = list(set(variables_filtro_iv) - set(variables_no_agrupadas_error))
 
         self.final_breakpoints = compute_final_breakpoints(
         variables_def, autogroupings, self.user_breakpoints)
         info = compute_info(X_train, variables_def, self.final_breakpoints)
 
         df_train = adapt_data(X_train, y_train, variables_def, self.final_breakpoints)
         df_test = adapt_data(X_test, y_test, variables_def, self.final_breakpoints)
@@ -266,20 +258,21 @@
 
         for objeto in autogroupings: del autogroupings[objeto].x_final
 
         if self.save_autogroupings == 'all': 
             self.autogroupings = autogroupings
         elif self.save_autogroupings == 'features':
             self.autogroupings = dict((k, autogroupings[k]) for k in features if k in autogroupings)
-
-        # self.pyspark_formula = compute_pyspark_formula(self)
+            
+        try: self.create_pyspark_formula()
+        except: self.pypsark_formula = ['Por algún motivo no se ha podido calcular la fórmula SQL']
 
         return self
-        
 
+        
     def create_excel(self, ruta, color='blue'):
         
         import openpyxl
         from openpyxl.utils.dataframe import dataframe_to_rows
         from openpyxl.styles import PatternFill
         
         scorecard = self.scorecard.copy()
@@ -381,15 +374,142 @@
                     for cell in row:
                         cell.fill = PatternFill(fill_type='solid', fgColor=color)
             contador = new_contador
             moneda += 1
             
         wb.save(ruta)
 
+    
+    def create_pyspark_formula(self):
+    
+        import copy
+
+        pyspark_formula = []
+
+        for i in self.features:
+
+            aux = 'CASE '
+            points = list(self.scorecard[self.scorecard['Variable'] == i]['Aligned score'])
+            groups = copy.deepcopy(list(self.scorecard[self.scorecard['Variable'] == i]['Group']))
+
+            for j in range(len(groups)):
+
+                if self.autogroupings[i].dtype not in ('object', 'bool'):
+                    if 'Missing' in groups[j]:
+                        aux += 'WHEN (isnan({}) OR ({} IS NULL)) THEN {} '.format(i, i, points[j])
+                    if 'inf)' not in groups[j] and groups[j] != 'Missing':
+                        lim = groups[j].split(', ')[1][:-1]
+                        aux += 'WHEN {} < {} THEN {} '.format(i, lim, points[j])
+                    if 'inf)' in groups[j]:
+                        lim = groups[j].split(', ')[0][1:]
+                        aux += 'WHEN {} >= {} THEN {} '.format(i, lim, points[j])
+
+                else:
+                    if 'Missing' in groups[j]:
+                        aux += 'WHEN (isnan({}) OR ({} IS NULL)) THEN {} '.format(i, i, points[j])
+                    try: groups[j].remove('Missing')
+                    except: pass
+                    if groups[j] != []: 
+                        aux += 'WHEN {} IN {} THEN {} '.format(i, groups[j], points[j])
+
+            aux += 'ELSE {} END'.format(min(points))
+            aux = aux.replace('[', '(').replace(']', ')')
+
+            pyspark_formula.append(aux)
+        
+        self.pyspark_formula = pyspark_formula
+
+        
+    def create_pmml(self, nombre_archivo, nombre_modelo='mew', score_name='scorecardpoints'):
+
+        import copy
 
+        texto = '<PMML xmlns="http://www.dmg.org/PMML-4_4" version="4.4">\n'
+        texto += '<DataDictionary>\n'
+
+        for feature in self.features:
+            objeto = self.autogroupings[feature]
+            if 'int' in str(objeto.dtype): 
+                tipo1 = 'integer'
+                tipo2 = 'continuous'
+            elif 'float' in str(objeto.dtype): 
+                tipo1 = 'double'
+                tipo2 = 'continuous'
+            elif 'object' in str(objeto.dtype): 
+                tipo1 = 'string'
+                tipo2 = 'categorical'
+            elif 'bool' in str(objeto.dtype): 
+                tipo1 = 'boolean'
+                tipo2 = 'categorical'
+            else: 
+                raise Exception('WTF, qué tipo de datos tiene {}: '\
+                    .format(feature), str(objeto.dtype))
+            texto += '<DataField name="{}" dataType="{}" optype="{}"/>\n'\
+            .format(feature, tipo1, tipo2)
+        
+        texto += '<DataField name="{}" dataType="double" optype="continuous"/>\n'.format(score_name)
+        texto += '</DataDictionary>\n'
+        texto += '<Scorecard modelName="{}" functionName="regression" '\
+        'useReasonCodes="false" initialScore="0">\n'.format(nombre_modelo)
+        texto += '<MiningSchema>\n'
+
+        for feature in self.features:
+            texto += '<MiningField name="{}" usageType="active" '\
+            'invalidValueTreatment="asMissing"/>\n'.format(feature)
+
+        texto += '<MiningField name="{}" usageType="predicted"/>\n'.format(score_name)
+        texto += '</MiningSchema>\n'
+        texto += '<Characteristics>\n'
+
+        for i in self.features:
+            aux = '<Characteristic name="{}">\n'.format(i)
+            points = list(self.scorecard[self.scorecard['Variable'] == i]['Aligned score'])
+            groups = copy.deepcopy(list(self.scorecard[self.scorecard['Variable'] == i]['Group']))
+
+            for j in range(len(points)):
+                
+                aux += '<Attribute partialScore="{}">\n'.format(points[j])
+                
+                if self.autogroupings[i].dtype not in ('object', 'bool'):
+  
+                    if 'Missing' in groups[j]:
+                        aux += '<CompoundPredicate booleanOperator="or">\n'
+                        aux += '<SimplePredicate field="{}" operator="isMissing"/>\n'.format(i)
+                    if 'inf)' not in groups[j] and groups[j] != 'Missing':
+                        lim = groups[j].split(', ')[1][:-1]
+                        aux += '<SimplePredicate field="{}" operator="lessThan" value="{}"/>\n'\
+                        .format(i, lim)
+                    if 'inf)' in groups[j]:
+                        lim = groups[j].split(', ')[0][1:]
+                        aux += '<SimplePredicate field="{}" operator="greaterOrEqual" '\
+                        'value="{}"/>\n'.format(i, lim)
+                    if 'Missing' in groups[j]:
+                        aux += '</CompoundPredicate>\n'
+        
+                else:
+                
+                    aux += '<CompoundPredicate booleanOperator="or">\n'
+                    for k in groups[j]:
+                        if k != 'Missing':
+                            aux += '<SimplePredicate field="{}" operator="equal" '\
+                            'value="{}"/>\n'.format(i, k)
+                        else:
+                            aux += '<SimplePredicate field="{}" operator="isMissing"/>\n'.format(i)
+                    aux += '</CompoundPredicate>\n'
+                    
+                aux+='</Attribute>\n'
+            aux += '</Characteristic>\n'
+            texto += aux
+        texto += '</Characteristics>\n'
+        texto += '</Scorecard>\n'
+        texto += '</PMML>\n'
+        
+        with open('{}'.format(nombre_archivo), 'w') as f: f.write(texto[1:-1])
+    
+        
     def predict(self, data, target_name='', keep_columns=[], binary_treshold=0.0):
                    
         if target_name != '': X1 = data[keep_columns + self.features + [target_name]].copy()
         else: X1 = data[keep_columns + self.features].copy()
 
         X1_v2, info = X1.copy(), {}
         for feature in self.features:
@@ -405,15 +525,16 @@
 
             else:
                 X1_v2[feature] = remapeo_missing(data_convert(
                 X1[feature].values, string_categories2(bp))[3], bp)
                 info[feature]['breakpoints_num'] = breakpoints_to_num(bp['bp'])
                 info[feature]['group_names'] = compute_group_names(
                 X1[feature].values.dtype, bp['bp'], bp['mg'])
-
+                
+        X1_v2 = X1_v2.reset_index(drop=True)
         X2 = apply_scorecard(X1_v2, self.scorecard, info, 
         target_name=target_name, binary_treshold=binary_treshold)
 
         venga = 0
         for i in X2.columns:
             if 'scr_' in i:
                 break
@@ -555,8 +676,9 @@
 
                 g[i] = np.sum([(y == 0) & (x_groups == i)])
                 b[i] = np.sum([(y == 1) & (x_groups == i)])
 
             error = (g == 0) | (b == 0)
 
         self.breakpoints_num = breakpoints_num
-
+        
+
```

### Comparing `memento-scorecard-0.2.7/memento/diane.py` & `memento-scorecard-0.3.3/memento/diane.py`

 * *Files 11% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         table = compute_table(x, y, breakpoints_num, group_names, False)[0]
         table.insert(0, 'Variable', feature)
         scorecard = pd.concat([scorecard, table])
         features_length = np.append(features_length, len(table))
 
         Xwoes[feature] = transform_to_woes(x, y, breakpoints_num)
 
-    log_reg = sm.Logit(y, sm.add_constant(Xwoes.values)).fit(method='lbfgs')
+    log_reg = sm.Logit(y, sm.add_constant(Xwoes.values)).fit(disp=0)
     coefs, intercept = np.array([log_reg.params[1:]]), np.array([log_reg.params[0]])
 
     scorecard['Raw score'] = scorecard['WoE'] * np.repeat(coefs.ravel(), features_length)
     scorecard['Aligned score'] = calib_score(scorecard['Raw score'], len(features), intercept)
     if redondeo: scorecard['Aligned score'] = scorecard['Aligned score'].round().astype('int')
     scorecard = scorecard.reset_index(drop=True)
 
@@ -165,67 +165,68 @@
 
 
 def transform_to_points(x, breakpoints_num, mapeo_points):
 
     return pd.Series([mapeo_points[i] for i in np.digitize(x, breakpoints_num)])
 
 
-def apply_scorecard(data, scorecard, info, target_name='', binary_treshold=0.0):
+def apply_scorecard(data, scorecard, info, target_name='',
+binary_treshold=0.0, score_name='scorecardpoints'):
 
     features = list(scorecard['Variable'].unique())
     if target_name != '': columnas = features + [target_name]
     else: columnas = features
                  
     data_final = data[columnas].copy()
     data_final = data.copy()
-    data_final['scorecardpoints'] = 0
+    data_final[score_name] = 0
 
     for feature in features:
 
         x = data_final[feature]
         breakpoints_num = info[feature]['breakpoints_num']
 
         mapeo_points = scorecard[scorecard['Variable'] == feature]\
         .reset_index(drop=True)['Aligned score'].to_dict()
 
         data_final['scr_{}'.format(feature)] = \
         transform_to_points(x, breakpoints_num, mapeo_points)
-        data_final['scorecardpoints'] += data_final['scr_{}'.format(feature)]
+        data_final[score_name] += data_final['scr_{}'.format(feature)]
     
     columnas = list(data_final.columns)
-    columnas.remove('scorecardpoints')
-    data_final = data_final[columnas + ['scorecardpoints']]
+    columnas.remove(score_name)
+    data_final = data_final[columnas + [score_name]]
 
     if binary_treshold != 0.0:
-        data_final['prediction'] = np.where(data_final.scorecardpoints >= binary_treshold, 0, 1)
+        data_final['prediction'] = np.where(data_final[score_name] >= binary_treshold, 0, 1)
 
     return data_final
 
-def compute_metrics(data, target_name, metrics, print_log=False):
+def compute_metrics(data, target_name, metrics, print_log=False, score_name='scorecardpoints'):
 
     if metrics not in (['ks'], ['gini'], ['ks', 'gini'], ['gini', 'ks']):
-        raise ValueError("Wrong value for 'metrics'. The values "
-        "allowed are: ['ks'], ['gini'], ['ks', 'gini'], ['gini', 'ks']")
+        raise ValueError("Valor erroneo para 'metrics'. Los valores "
+        "váidos son: ['ks'], ['gini'], ['ks', 'gini'], ['gini', 'ks']")
 
     if 'ks' in metrics:
-        g = data.loc[data[target_name] == 0, 'scorecardpoints']
-        b = data.loc[data[target_name] == 1, 'scorecardpoints']
+        g = data.loc[data[target_name] == 0, score_name]
+        b = data.loc[data[target_name] == 1, score_name]
         ks = ks_2samp(g, b)[0]
 
     if 'gini' in metrics:
-        gini = abs(2*(1 - roc_auc_score(data[target_name], data['scorecardpoints'])) - 1)
+        gini = abs(2*(1 - roc_auc_score(data[target_name], data[score_name])) - 1)
 
     if metrics == ['ks']:
         if print_log:
-            print('The model has a {:.2f}% of KS in this sample'.format(round(ks*100, 2)))
+            print('El modelo tiene un {:.2f}% de KS en esta muestra'.format(round(ks*100, 2)))
         return ks
 
     if metrics == ['gini']:
         if print_log:
-            print('The model has a {:.2f}% of Gini in this sample'.format(round(gini*100, 2), ))
+            print('El modelo tiene un {:.2f}% de Gini en esta muestra'.format(round(gini*100, 2), ))
         return gini
 
     if metrics in (['ks', 'gini'], ['gini', 'ks']):
         if print_log:
             print('El  modelo tiene un {:.2f}% de KS y un {:.2f}% de Gini '
             'en esta muestra'.format(round(ks*100, 2), round(gini*100, 2)))
         return ks, gini
```

### Comparing `memento-scorecard-0.2.7/memento/princess_carolyn.py` & `memento-scorecard-0.3.3/memento/princess_carolyn.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,8 +455,9 @@
     
     display(objeto.table)
     
     if bp != []:
         print('-'*80)
         print('Agrupación propuesta:')
         display_table_ng(modelo, variable, objeto, bp)
-
+        
+
```

### Comparing `memento-scorecard-0.2.7/memento/todd.py` & `memento-scorecard-0.3.3/memento/todd.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,36 +66,37 @@
         else: return v
     else: return v
 
 
 def data_convert(x, categories):
 
     x_original = x
-
+    
     if x.dtype in ('O', 'bool'):
         if categories == {}:
             raise ValueError('En una variable de tipo texto o booleana '
             'es necesario especificar el diccionario de categorias')
         if pd.Series(x).isna().sum() > 0:
             x = pd.Series(x).replace(np.nan, 'Missing').values
         x_initial = x
         x = string_to_num(x, categories)
         x_converted = x
+    
     else:
         x_initial = x
         x_converted = x
 
     if x.dtype not in ('O', 'bool') and np.isnan(x).sum() > 0:
         x_final = np.nan_to_num(x, nan=-12345678)
+
     else: x_final = x_converted
 
     return x_original, x_initial, x_converted, x_final
 
 
-
 def adapt_data(X, y, variables, breakpoints, target_name='target_4815162342'):
     
     df = pd.DataFrame()
     for variable in variables:
         
             bp = breakpoints[variable]
```

### Comparing `memento-scorecard-0.2.7/memento_scorecard.egg-info/PKG-INFO` & `memento-scorecard-0.3.3/memento_scorecard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 0.2.7
+Version: 0.3.3
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
 Platform: UNKNOWN
```

### Comparing `memento-scorecard-0.2.7/setup.py` & `memento-scorecard-0.3.3/setup.py`

 * *Files identical despite different names*

