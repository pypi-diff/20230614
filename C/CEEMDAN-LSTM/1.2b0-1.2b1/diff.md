# Comparing `tmp/CEEMDAN_LSTM-1.2b0.tar.gz` & `tmp/CEEMDAN_LSTM-1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CEEMDAN_LSTM-1.2b0.tar", last modified: Fri Nov 18 02:00:27 2022, max compression
+gzip compressed data, was "CEEMDAN_LSTM-1.2b1.tar", last modified: Wed Jun 14 11:00:12 2023, max compression
```

## Comparing `CEEMDAN_LSTM-1.2b0.tar` & `CEEMDAN_LSTM-1.2b1.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-11-18 02:00:27.276956 CEEMDAN_LSTM-1.2b0/
-drwxrwxrwx   0        0        0        0 2022-11-18 02:00:27.268446 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/
--rw-rw-rw-   0        0        0      916 2022-11-18 01:34:52.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/__init__.py
--rw-rw-rw-   0        0        0    25552 2022-10-10 06:38:57.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/core.py
--rw-rw-rw-   0        0        0    39871 2022-11-04 11:42:55.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/data_preprocessor.py
-drwxrwxrwx   0        0        0        0 2022-11-18 02:00:27.274966 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/
--rw-rw-rw-   0        0        0    30846 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/beijing_ets.csv
--rw-rw-rw-   0        0        0    97722 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/guangzhou_ets.csv
--rw-rw-rw-   0        0        0    60602 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/hubei_ets.csv
--rw-rw-rw-   0        0        0   536253 2022-08-31 07:05:12.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/sse_index.csv
--rw-rw-rw-   0        0        0    26696 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/tianjin_ets.csv
--rw-rw-rw-   0        0        0    57127 2022-11-18 01:53:35.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/keras_predictor.py
--rw-rw-rw-   0        0        0    16689 2022-10-07 07:34:33.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/sklearn_predictor.py
-drwxrwxrwx   0        0        0        0 2022-11-18 02:00:27.271455 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM.egg-info/
--rw-rw-rw-   0        0        0     9923 2022-11-18 02:00:27.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2022-11-18 02:00:27.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-18 02:00:27.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2022-11-18 02:00:27.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-18 02:00:27.000000 CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b0/LICENSE
--rw-rw-rw-   0        0        0     9923 2022-11-18 02:00:27.276511 CEEMDAN_LSTM-1.2b0/PKG-INFO
--rw-rw-rw-   0        0        0     9088 2022-11-18 01:55:56.000000 CEEMDAN_LSTM-1.2b0/README.md
--rw-rw-rw-   0        0        0       42 2022-11-18 02:00:27.276956 CEEMDAN_LSTM-1.2b0/setup.cfg
--rw-rw-rw-   0        0        0     1364 2022-11-18 01:35:06.000000 CEEMDAN_LSTM-1.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:00:12.070623 CEEMDAN_LSTM-1.2b1/
+drwxrwxrwx   0        0        0        0 2023-06-14 11:00:12.037078 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/
+-rw-rw-rw-   0        0        0      916 2022-11-18 01:34:52.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/__init__.py
+-rw-rw-rw-   0        0        0    25551 2023-06-14 08:47:20.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/core.py
+-rw-rw-rw-   0        0        0    41297 2023-06-11 07:33:07.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/data_preprocessor.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:00:12.067625 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/
+-rw-rw-rw-   0        0        0    30846 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/beijing_ets.csv
+-rw-rw-rw-   0        0        0    56764 2023-03-15 06:59:29.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/ftse.csv
+-rw-rw-rw-   0        0        0    97722 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/guangzhou_ets.csv
+-rw-rw-rw-   0        0        0    59837 2023-03-15 06:59:12.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/hsi.csv
+-rw-rw-rw-   0        0        0    60602 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/hubei_ets.csv
+-rw-rw-rw-   0        0        0    57605 2023-06-08 11:49:39.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/n225.csv
+-rw-rw-rw-   0        0        0    61006 2023-06-08 11:48:36.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/nasdaq.csv
+-rw-rw-rw-   0        0        0    60683 2023-03-15 06:59:00.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/sp500.csv
+-rw-rw-rw-   0        0        0   536253 2022-08-31 07:05:12.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/sse_index.csv
+-rw-rw-rw-   0        0        0    55845 2023-03-15 06:57:54.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/ssec.csv
+-rw-rw-rw-   0        0        0    26696 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/tianjin_ets.csv
+-rw-rw-rw-   0        0        0    56152 2023-06-14 07:23:48.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/keras_predictor.py
+-rw-rw-rw-   0        0        0    16724 2023-04-19 06:45:48.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/sklearn_predictor.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:00:12.041596 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/
+-rw-rw-rw-   0        0        0     9923 2023-06-14 11:00:11.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-06-14 11:00:12.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 11:00:11.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-06-14 11:00:11.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-14 11:00:11.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b1/LICENSE
+-rw-rw-rw-   0        0        0     9923 2023-06-14 11:00:12.069627 CEEMDAN_LSTM-1.2b1/PKG-INFO
+-rw-rw-rw-   0        0        0     9088 2022-11-18 01:55:56.000000 CEEMDAN_LSTM-1.2b1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 11:00:12.070623 CEEMDAN_LSTM-1.2b1/setup.cfg
+-rw-rw-rw-   0        0        0     1374 2023-06-14 05:52:12.000000 CEEMDAN_LSTM-1.2b1/setup.py
```

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/__init__.py` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/__init__.py`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/core.py` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Email: jupiterzhou@foxmail.com
 # URL: 'http://github.com/FateMurphy/CEEMDAN_LSTM'
 # Feel free to email me if you have any questions or error reports.
 
 import os
 import pandas as pd
 import matplotlib.pyplot as plt
-
+from datetime import datetime
 
 
 # 0.Guideline
 # ------------------------------------------------------
 def help():
     print('CEEMDAN_LSTM is a module that helps you make a quick decomposition-integration time series forecasting.')
     print('===============================')
@@ -111,14 +111,15 @@
     print("\nprint('\\n4.K-Means Cluster by Sample Entropy')")
     print("print('-------------------------------')")
     print("df_integrate_form = cl.inte_kmeans(df_sampen)")
     print("print(df_integrate_form) # show")
     print("\nprint('\\n5.Integrate IMFs and Residue to be 3 Co-IMFs')")
     print("print('-------------------------------')")
     print("df_integrate_result = cl.inte(df_ceemdan, df_integrate_form)")
+    print("df_integrate_result = df_integrate_result[0]")
     print("df_integrate_result.plot(title='Integrated IMFs (Co-IMFs) of CEEMDAN', subplots=True, figsize=(6,3)) # plot")
     print("plt.show() # plot")
     print("\nprint('\\n6.Secondary Decompose the high-frequency Co-IMF0 by OVMD')")
     print("print('-------------------------------')")
     print("df_vmd_co_imf0 = cl.decom(df_integrate_result['co-imf0'], decom_mode='ovmd')")
     print("df_vmd_co_imf0.plot(title='OVMD Decomposition of Co-IMF0', subplots=True, figsize=(6,11)) # plot")
     print("plt.show() # plot")
@@ -321,16 +322,16 @@
     path         - the saving path
     """
     
     PATH, FIG_PATH, LOG_PATH = check_path(path)
 
     # Check Name
     if name is None: 
-        name = pd.datetime.now().strftime('%Y%m%d_%H%M%S_')
-    elif isinstance(name, pd.datetime):
+        name = datetime.now().strftime('%Y%m%d_%H%M%S_')
+    elif isinstance(name, datetime):
         name = name.strftime('%Y%m%d_%H%M%S_')
     else: name = ''
     if PATH is None: save = False
 
     # Default output function
     def default_output(df): 
         if 'Evaluation' not in df.name:
@@ -378,15 +379,15 @@
         print('Load the sample dataset of the SSE index. Check it by cl.load_dataset()')
         dataset = load_dataset()
         data = pd.Series(dataset['close'].values, index=dataset.index)
     try: data = pd.Series(data) # 1.Load raw data
     except: raise ValueError('Sorry! %s is not supported, please input pd.DataFrame, pd.Series, nd.array(<=2D)'%type(data))
 
     kr = keras_predictor(**kwargs)
-    df_result = kr.hybrid_keras_predict(data=data, show_data=True, show_model=True, plot_result=True, save_result=True)
+    df_result = kr.hybrid_keras_predict(data=data, show=True, plot=True, save=True)
     
     return df_result
 
 
 # Run the details forecasting
 def details_keras_predict(data=None, fitting=False, **kwargs):
     """
@@ -406,17 +407,16 @@
     # 1.Load raw data
     print("\n1.Load raw data")
     print("-------------------------------")
     if data is None: 
         print('Load the sample dataset of the SSE index. Check it by cl.load_dataset()')
         dataset = load_dataset()
         data = pd.Series(dataset['close'].values, index=dataset.index)
-    try: data = pd.Series(data)
-    except: raise ValueError('Sorry! %s is not supported, please input pd.DataFrame, pd.Series, nd.array(<=2D)'%type(data))
     data = check_dataset(data, False, 'vmd')
+    data = pd.Series(data.values.ravel(), index=data.index)
     data.plot(title='Original Data')
     plt.show()
 
     # 2.CEEMDAN decompose
     print("\n2.CEEMDAN decompose")
     print("-------------------------------")
     start = time.time()
@@ -437,14 +437,15 @@
     df_integrate_form = inte_kmeans(df_sampen)
     print(df_integrate_form)
 
     # 5.Integrate IMFs and Residue to be 3 Co-IMFs
     print("\n5.Integrate IMFs and Residue to be 3 Co-IMFs")
     print("-------------------------------")
     df_integrate_result = inte(df_ceemdan, df_integrate_form)
+    df_integrate_result = df_integrate_result[0]
     df_integrate_result.plot(title='Integrated IMFs (Co-IMFs) of CEEMDAN', subplots=True, figsize=(6, 3))
     plt.show()
 
     # 6.Secondary Decompose the high-frequency Co-IMF0 by VMD (cl.redecom cna finish step 2 to 6)
     print("\n6.Secondary Decompose the high-frequency Co-IMF0 by OVMD")
     print("-------------------------------")
     df_vmd_co_imf0 = decom(df_integrate_result['co-imf0'], decom_mode='ovmd')
```

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/data_preprocessor.py` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/data_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,17 @@
     elif decom_mode == 'vmd': 
         df_decom, imfs_hat, omega = decom_vmd(series, **kwargs)
     elif decom_mode == 'ovmd': 
         df_decom, best_params = decom_ovmd(series, vmd_params=vmd_params, **kwargs)
     elif decom_mode == 'svmd': 
         df_decom = decom_svmd(series, vmd_params=vmd_params, FORECAST_LENGTH=FORECAST_LENGTH, **kwargs)
     else: raise ValueError('%s is not a supported decomposition method!'%(decom_mode))
-    if isinstance(series, pd.Series): df_decom.index = series.index # change index
+    if isinstance(series, pd.Series): 
+        if 'vmd' in decom_mode and len(series)%2: df_decom.index = series[1:].index # change index
+        else: df_decom.index = series.index # change index
     df_decom['target'] = series
     df_decom.name = decom_mode.lower()+'_'+str(best_params)
     return df_decom
 
 # 1.1 VMD
 def decom_vmd(series=None, alpha=2000, tau=0, K=10, DC=0, init=1, tol=1e-7, **kwargs): # VMD Decomposition
     """
@@ -137,31 +139,35 @@
     ---------------------
     df_vmd     - the collection of decomposed modes in pd.Dataframe 
     """
     
     if series is None: raise ValueError('Please input pd.Series, or pd.DataFrame(1D), nd.array(1D).')
     try: series = pd.Series(series)
     except: raise ValueError('Sorry! %s is not supported to decompose, please input pd.Series, or pd.DataFrame(1D), nd.array(1D)'%type(series))
+    if len(series)%2: 
+        print('Warning! The vmdpy module will delete the last one data point of series before decomposition')
+        series = series[1:]
     if vmd_params is None:
         try: import optuna
         except: raise ImportError('Cannot import optuna, run: pip install optuna!')
         def objective(trial):
             K = trial.suggest_int('K', 1, 10) # set hyperparameter range
+            alpha = trial.suggest_int('alpha', 1, 10000)
             tau = trial.suggest_float('tau', 0, 1) 
-            df_vmd, imfs_hat, imfs_omega = decom_vmd(series, K=K, tau=tau)
+            df_vmd, imfs_hat, imfs_omega = decom_vmd(series, K=K, alpha=alpha, tau=tau)
             return abs((df_vmd.sum(axis=1).values - series.values).sum()) # residual of decomposed and original series 
         study = optuna.create_study(study_name='OVMD Method', direction='minimize') # TPESampler is used
         optuna.logging.set_verbosity(optuna.logging.WARNING) # not to print
         study.optimize(objective, n_trials=trials, n_jobs=-1, gc_after_trial=True)  # number of iterations
         vmd_params = study.best_params
-    df_vmd, imfs_hat, imfs_omega = decom_vmd(series, K=vmd_params['K'], tau=vmd_params['tau'])
+    df_vmd, imfs_hat, imfs_omega = decom_vmd(series, K=vmd_params['K'], alpha=vmd_params['alpha'], tau=vmd_params['tau'])
     return df_vmd, vmd_params
 
 # 1.2 Separated VMD (SVMD)
-def decom_svmd(series=None, FORECAST_LENGTH=None, optimize=True, vmd_params=None, trials=100, ): # VMD Decomposition
+def decom_svmd(series=None, FORECAST_LENGTH=None, optimize=True, vmd_params=None, trials=100): # VMD Decomposition
     """
     Decompose time series by VMD separatey for traning and test set,
     and use Bayesian Optimization to find the best K and tau.
     Example: df_vmd = cl.decom_svmd(series)
     Plot by pandas: df_vmd.plot(title='VMD Decomposition Results', subplots=True)
 
     Input and Parameters:
@@ -175,68 +181,74 @@
     ---------------------
     df_vmd     - the collection of decomposed modes in pd.Dataframe 
     """
     
     if series is None: raise ValueError('Please input pd.Series, or pd.DataFrame(1D), nd.array(1D).')
     try: series = pd.Series(series)
     except: raise ValueError('Sorry! %s is not supported to decompose, please input pd.Series, or pd.DataFrame(1D), nd.array(1D)'%type(series))
+    if len(series)%2: 
+        print('Warning! The vmdpy module will delete the last one data point of series before decomposition')
+        series = series[1:]
     if FORECAST_LENGTH is None: raise ValueError('Please input FORECAST_LENGTH.')
     if vmd_params is None and optimize == False: vmd_params = {'K':10, 'tau':0}
 
     series_train = series[:-FORECAST_LENGTH]
     series_test = series[-FORECAST_LENGTH:]
     if vmd_params is None and optimize:
         try: import optuna
         except: raise ImportError('Cannot import optuna, run: pip install optuna!')
         def objective(trial):
             K = trial.suggest_int('K', 1, 10) # set hyperparameter range
+            alpha = trial.suggest_int('alpha', 1, 10000)
             tau = trial.suggest_float('tau', 0, 1) 
-            df_vmd, imfs_hat, imfs_omega = decom_vmd(series_train, K=K, tau=tau)
+            df_vmd, imfs_hat, imfs_omega = decom_vmd(series_train, K=K, alpha=alpha, tau=tau)
             return abs((df_vmd.sum(axis=1).values - series_train.values).sum()) # residual of decomposed and original training set series 
         study = optuna.create_study(study_name='SVMD Method for training set', direction='minimize') # TPESampler is used
         optuna.logging.set_verbosity(optuna.logging.WARNING) # not to print
         study.optimize(objective, n_trials=trials, n_jobs=-1, gc_after_trial=True)  # number of iterations
         vmd_params = study.best_params
-    df_vmd_train, imfs_hat, imfs_omega = decom_vmd(series_train, K=vmd_params['K'], tau=vmd_params['tau'])
-    df_vmd_test, imfs_hat, imfs_omega = decom_vmd(series_test, K=vmd_params['K'], tau=vmd_params['tau'])
+    df_vmd_train, imfs_hat, imfs_omega = decom_vmd(series_train, K=vmd_params['K'], alpha=vmd_params['alpha'], tau=vmd_params['tau'])
+    df_vmd_test, imfs_hat, imfs_omega = decom_vmd(series_test, K=vmd_params['K'], alpha=vmd_params['alpha'], tau=vmd_params['tau'])
     df_vmd = pd.concat((df_vmd_train, df_vmd_test))
     df_vmd.index = series.index
     return df_vmd
 
 # 2.Integrate
 # ------------------------------------------------------
 # 2.Main. Integrate
 def inte(df_decom=None, inte_list='auto', num_clusters=3):
     """
     Integrate IMFs to be CO-IMFs by sampen.sampen2 and sklearn.cluster.
-    Example: df_inte = cl.inte(df_decom)
+    Example: df_inte, df_inte_list = cl.inte(df_decom)
     Plot by pandas: df_inte.plot(title='Integrated IMFs (Co-IMFs) Results', subplots=True)
     Custom integration: please use cl.inte_sampen() and cl.inte_kmeans()
 
     Input and Parameters:
     ---------------------
     df_decom       - the decomposing results in pd.Dataframe, or a group of series
     inte_list      - the integration list, eg. pd.Dataframe, (int) 3, (str) '233', (list) [0,0,1,1,1,2,2,2], ...
     num_clusters   - number of categories/clusters eg. num_clusters = 3
 
     Output:
     ---------------------
     df_inte        - the integrating form of each time series
+    df_inte_list   - the integrating set of each co-imf
     """
     
     # Check input
     try: df_decom = pd.DataFrame(df_decom)
     except: raise ValueError('Invalid input of df_decom!')
     if 'target' in df_decom.columns: 
         tmp_target = df_decom['target']
         df_decom = df_decom.drop('target', axis=1, inplace=False)
     else: tmp_target = None
     df_decom.columns = ['imf'+str(i) for i in range(df_decom.columns.size)]
 
     # Check inte_list
+    df_inte_list = []
     if inte_list is not None:
         if str(inte_list).lower() == 'auto': # Without 
             df_sampen = inte_sampen(df_decom)
             inte_list = inte_kmeans(df_sampen, num_clusters)
         elif isinstance(inte_list, pd.DataFrame):
             if len(inte_list) == 1: inte_list = inte_list.T
         elif type(inte_list) == str and len(inte_list) < df_decom.columns.size:
@@ -258,26 +270,37 @@
             try: inte_list = pd.DataFrame(inte_list, columns=['Cluster'], index=['imf'+str(x) for x in range(len(inte_list))])
             except: raise ValueError('Invalid inte_list of %s with type %s. Check your input or length.'%(inte_list, type(inte_list)))
 
         # Integrate, name, and resort
         df_tmp = pd.DataFrame()
         for i in range(inte_list.values.max()+1):
             df_tmp['imf'+str(i)] = df_decom[inte_list[(inte_list['Cluster']==i)].index].sum(axis=1)
+            df_tmp_list = pd.DataFrame(df_tmp['imf'+str(i)])
+            df_tmp_list.columns = ['target']
+            df_inte_list.append(pd.concat((df_tmp_list, df_decom[inte_list[(inte_list['Cluster']==i)].index]), axis=1))
         df_inte = df_tmp.T # Use Sample Entropy sorting the Co-IMFs
         df_inte['sampen'] = inte_sampen(df_tmp).values
         df_inte.sort_values(by=['sampen'], ascending=False, inplace=True)
         df_inte.index = ['co-imf'+str(i) for i in range(inte_list.values.max()+1)]
         df_inte = df_inte.drop('sampen', axis=1, inplace=False).T
 
+        # Rename df_inte_list
+        for i in range(len(df_inte.columns)):
+            for j in range(len(df_inte.columns)):
+                try:
+                    if df_inte_list[i]['target'].sum() == df_inte['co-imf'+str(j)].sum():
+                        df_inte_list[i].columns = ['co-imf'+str(j)] + list(df_inte_list[i].columns)[1:]
+                except: break
+
         # Output
         df_inte.name = 'df_inte_list_is_'+''.join(str(x) for x in inte_list.values.ravel()) # record integrate list
         df_inte.index = df_decom.index
     else: df_inte = df_decom
     if tmp_target is not None: df_inte['target'] = tmp_target # add tmp target column
-    return df_inte
+    return df_inte, df_inte_list
     
 
 # 2.1 Sample Entropy
 def inte_sampen(df_decom=None, max_len=1, tol=0.1, nor=True, **kwargs):
     """
     Calculate Sample Entropy for each IMF or series by sampen.sampen2.
     Example: df_sampen = cl.inte_sampen(df_decom)
@@ -364,15 +387,15 @@
 
     from CEEMDAN_LSTM.core import check_dataset
     data = check_dataset(data, show_data, decom_mode, redecom_list)
     if vmd_params is not None and type(vmd_params) != dict: raise ValueError('Invalid input of vmd_params!') 
     if len(data.columns) == 1: 
         df_decom = decom(data[data.columns[0]], decom_mode=decom_mode, FORECAST_LENGTH=FORECAST_LENGTH)
     else: df_decom = data # pd.DataFrame
-    df_inte = inte(df_decom, inte_list=inte_list)
+    df_inte, df_inte_list = inte(df_decom, inte_list=inte_list)
 
     # Re-decompose 
     df_redecom_list, best_params_dict, inte_columns = [], {}, str(df_inte.columns.to_list())
     if redecom_list is not None:
         try: redecom_list = pd.DataFrame(redecom_list, index=range(1))
         except: raise ValueError("Invalid input for redecom_list! Please input eg. None, '{'co-imf0':'vmd', 'co-imf1':'emd'}'.")
         for i in redecom_list.columns:
@@ -598,18 +621,18 @@
     Make Ljung-Box Test to evaluate autocorrelation.
     Input: series     - the time series (1D)
     """
     from statsmodels.stats.diagnostic import acorr_ljungbox as lb_test # LB_test
     series = check_series(series)
     lb_ans = lb_test(series,lags=None,boxpierce=False) # The default lags=40 for long series.
     print('\n==========Ljung-Box Test==========')
-    pd.Series(lb_ans[1]).plot(title='Ljung-Box Test p-values') # Plot p-values in a figure
+    pd.Series(lb_ans['lb_pvalue']).plot(title='Ljung-Box Test p-values') # Plot p-values in a figure
     plt.show()
-    if np.sum(lb_ans[1])<=0.05: # Brief review
-        print('The sum of p-value is '+str(np.sum(lb_ans[1]))+'<=0.05, rejecting the null hypothesis that the series has very strong autocorrelation.')
+    if np.sum(lb_ans['lb_pvalue'])<=0.05: # Brief review
+        print('The sum of p-value is '+str(np.sum(lb_ans['lb_pvalue']))+'<=0.05, rejecting the null hypothesis that the series has very strong autocorrelation.')
     else: print('Please view with the line chart, the autocorrelation of the series may be not strong.')
     # print(pd.DataFrame(lb_ans)) # Show outcomes with test value at line 0, and p-value at line 1.
 
 # 4.3 Jarque-Bera Test 
 def jb_test(series=None):
     """
     Make Jarque-Bera Test to evaluate normality (whether conforms to a normal distribution).
```

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/beijing_ets.csv` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/beijing_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/guangzhou_ets.csv` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/guangzhou_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/hubei_ets.csv` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/hubei_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/sse_index.csv` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/sse_index.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/datasets/tianjin_ets.csv` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/tianjin_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/keras_predictor.py` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/keras_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,24 @@
 # Import modules for keras_predictor
 import os
 import sys
 import time
 import pandas as pd
 import numpy as np
 import warnings
+from datetime import datetime
 warnings.filterwarnings("ignore") # Ignore some annoying warnings
 # CEEMDAN_LSTM
 from CEEMDAN_LSTM.core import check_dataset, check_path, plot_save_result, name_predictor, change_name
 # Keras
 try: from tensorflow.python.keras.models import Sequential, load_model
 except: raise ImportError('Cannot import tensorflow, install or check your tensorflow verison!')
 from tensorflow import constant
 # from tcn import TCN # pip install keras-tcn
-from tensorflow.python.keras.layers import Dense, Activation, Dropout, LSTM, GRU, Flatten, CuDNNGRU, CuDNNLSTM
+from tensorflow.python.keras.layers import Dense, Activation, Dropout, LSTM, GRU, Flatten
 from tensorflow.python.keras.optimizer_v2.adam import Adam
 from tensorflow.python.keras.callbacks import ReduceLROnPlateau, EarlyStopping, ModelCheckpoint
 
 
 
 class keras_predictor:
     # 0.Initialize
@@ -54,15 +55,15 @@
         ---------------------
         PATH               - the saving path of figures and logs
         FORECAST_HORIZONS  - also called Timestep or Forecast_horizons or sliding_windows_length in some papers
                            - the length of each input row(x_train.shape), which means the number of previous days related to today
         FORECAST_LENGTH    - the length of the days to forecast (test set)
         KERAS_MODEL        - the Keras model, eg. 'GRU', 'LSTM', 'DNN', 'BPNN', model = Sequential(), h5 file, dict, pd.DataFrame.
                            - eg. {'co-imf0':'co_imf0_model.h5', 'co-imf1':'co_imf1_model.h5'}
-        DECOM_MODE         - the decomposition method, eg.'EMD', 'VMD', 'CEEMDAN'
+        DECOM_MODE         - the decomposition method, eg.'EMD', 'EEMD', 'CEEMDAN', 'VMD', 'OVDM', 'SMVD'
         INTE_LIST          - the integration list, eg. pd.Dataframe, (int) 3, (str) '233', (list) [0,0,1,1,1,2,2,2], ...
         REDECOM_LIST       - the re-decomposition list eg. '{'co-imf0':'vmd', 'co-imf1':'emd'}', pd.DataFrame
         NEXT_DAY           - set True to only predict next out-of-sample value
         DAY_AHEAD          - define to forecast n days' ahead eg. 0, 1 (default int 1)
         NOR_METHOD         - the normalizing method, eg. 'minmax'-MinMaxScaler, 'std'-StandardScaler, otherwise without normalization
         FIT_METHOD         - the fitting method to stablize the forecasting result (not necessarily useful), eg. 'add', 'ensemble'
         USE_TPU            - change Keras model to TPU model (for google Colab)
@@ -198,19 +199,22 @@
             model.add(LSTM(self.units, activation=self.activation, return_sequences=False))
             model.add(Dropout(self.dropout))
             model.add(Dense(1, activation=self.activation))
             model.compile(loss=self.opt_loss, optimizer=self.opt)
             return model
         elif self.KERAS_MODEL == 'GRU':
             model = Sequential(name=model_name)
-            model.add(GRU(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), activation=self.activation, return_sequences=True))
+            model.add(GRU(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), recurrent_activation = 'sigmoid', reset_after = True,
+                          activation=self.activation, return_sequences=True))
             model.add(Dropout(self.dropout))
-            model.add(GRU(self.units*2, activation=self.activation, return_sequences=True))
+            model.add(GRU(self.units*2, recurrent_activation = 'sigmoid', reset_after = True,
+                          activation=self.activation, return_sequences=True))
             model.add(Dropout(self.dropout))
-            model.add(GRU(self.units, activation=self.activation, return_sequences=False))
+            model.add(GRU(self.units, recurrent_activation = 'sigmoid', reset_after = True,
+                          activation=self.activation, return_sequences=False))
             model.add(Dropout(self.dropout))
             model.add(Dense(1, activation=self.activation))
             model.compile(loss=self.opt_loss, optimizer=self.opt)
             return model
         elif self.KERAS_MODEL == 'DNN':
             model = Sequential(name=model_name)
             model.add(Dense(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), activation=self.activation))
@@ -227,36 +231,14 @@
             model = Sequential(name=model_name)
             model.add(Dense(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), activation=self.activation))
             model.add(Dropout(self.dropout))
             model.add(Flatten())
             model.add(Dense(1, activation=self.activation))
             model.compile(loss=self.opt_loss, optimizer=self.opt)
             return model
-        elif self.KERAS_MODEL == 'CUDNNLSTM':
-            model = Sequential(name=model_name)
-            model.add(CuDNNLSTM(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]),return_sequences=True))
-            model.add(Dropout(self.dropout))
-            model.add(CuDNNLSTM(self.units*2, return_sequences=True))
-            model.add(Dropout(self.dropout))
-            model.add(CuDNNLSTM(self.units, return_sequences=False))
-            model.add(Dropout(self.dropout))
-            model.add(Dense(1, activation=self.activation))
-            model.compile(loss=self.opt_loss, optimizer=self.opt)
-            return model
-        elif self.KERAS_MODEL == 'CUDNNGRU':
-            model = Sequential(name=model_name)
-            model.add(CuDNNGRU(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), return_sequences=True))
-            model.add(Dropout(self.dropout))
-            model.add(CuDNNGRU(self.units*2, return_sequences=True))
-            model.add(Dropout(self.dropout))
-            model.add(CuDNNGRU(self.units, return_sequences=False))
-            model.add(Dropout(self.dropout))
-            model.add(Dense(1, activation=self.activation))
-            model.compile(loss=self.opt_loss, optimizer=self.opt)
-            return model
         else: raise ValueError("%s is an invalid input for KERAS_MODEL! eg. 'GRU', 'LSTM', or model = Sequential()"%self.KERAS_MODEL)
 
     # 1.2 Change Keras model to TPU model (for google Colab)
     def tpu_model(self, shape, model_name, model_file):
         """
         Change Keras model to TPU model (for google Colab)
         """
@@ -308,16 +290,17 @@
         # Set callbacks
         Reduce = ReduceLROnPlateau(monitor=self.callbacks_monitor, patience=self.opt_patience, verbose=self.verbose, mode='auto') # Adaptive learning rate
         EarlyStop = EarlyStopping(monitor=self.callbacks_monitor, patience=self.stop_patience, verbose=self.verbose, mode='auto') # Early stop at small learning rate 
         callbacks_list = [Reduce, EarlyStop]
 
         # Load and save model
         try: 
-            if '.h5' not in str(data.name): data.name = data.name + '.h5'
-        except: data.name = 'Keras model.h5'
+            if '.h5' and '\'' and ':' not in str(data.name): data.name = data.name + '.h5'
+            else: data.name = 'Keras_model.h5'
+        except: data.name = 'Keras_model.h5'
         model_file = None
         if self.PATH is not None:
             if not isinstance(self.KERAS_MODEL, Sequential): # set model_file to load model
                 if isinstance(self.KERAS_MODEL, pd.DataFrame):
                     for x in self.KERAS_MODEL.columns:
                         if change_name(x) in data.name: model_file = x # change to be key value
                     if model_file is not None: model_file = self.PATH + self.KERAS_MODEL[model_file][0]
@@ -406,15 +389,15 @@
         df_predict_real - forecasting results and the original real series set
         df_eval         - evaluating results of forecasting 
         df_train_loss   - training loss log
         next_y          - forecasting result of the next day when NEXT_DAY=Ture
         """
 
         # Name and set 
-        now = pd.datetime.now()
+        now = datetime.now()
         predictor_name = name_predictor(now, 'Single', 'Keras', self.KERAS_MODEL, None, None, self.NEXT_DAY)
         data = check_dataset(data, show, self.DECOM_MODE, self.REDECOM_LIST)
         data.name = change_name(predictor_name+'_model.h5')
         
         # set target and model
         try: 
             if 'Keras_Forecasting' in data.name: predictor_name = data.name
@@ -469,15 +452,15 @@
         df_predict_real - forecasting results and the original real series set
         df_eval         - evaluating results of forecasting 
         df_train_loss   - training loss log
         next_y          - forecasting result of the next day when NEXT_DAY=Ture
         """
 
         # Name
-        now = pd.datetime.now()
+        now = datetime.now()
         predictor_name = name_predictor(now, 'Ensemble', 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)
 
         # Decompose, integrate, re-decompose
         start = time.time()
         from CEEMDAN_LSTM.data_preprocessor import redecom
         df_redecom, df_redecom_list = redecom(data, show, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.VMD_PARAMS, self.FORECAST_LENGTH)
         df_redecom.name = change_name(predictor_name+'_model.h5')
@@ -535,15 +518,15 @@
         df_predict_real - forecasting results and the original real series set
         df_eval         - evaluating results of forecasting 
         df_train_loss   - training loss log
         next_y          - forecasting result of the next day when NEXT_DAY=Ture
         """
 
         # Name
-        now = pd.datetime.now()
+        now = datetime.now()
         predictor_name = name_predictor(now, 'Respective', 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)
 
         # Decompose, integrate, re-decompose
         start = time.time()
         from CEEMDAN_LSTM.data_preprocessor import redecom
         df_redecom, df_redecom_list = redecom(data, show, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.VMD_PARAMS, self.FORECAST_LENGTH)
         
@@ -637,15 +620,15 @@
         df_predict_real - forecasting results and the original real series set
         df_eval         - evaluating results of forecasting 
         df_train_loss   - training loss log
         next_y          - forecasting result of the next day when NEXT_DAY=Ture
         """
 
         # Name
-        now = pd.datetime.now()
+        now = datetime.now()
         predictor_name = name_predictor(now, 'Hybrid', 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)
 
         # Decompose, integrate, re-decompose
         start = time.time()
         from CEEMDAN_LSTM.data_preprocessor import redecom
         df_redecom, df_redecom_list = redecom(data, show, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.VMD_PARAMS, self.FORECAST_LENGTH)
         df_rest_columns, df_rest_list = [], []
@@ -799,15 +782,15 @@
 
         Output
         ---------------------
         df_eval_result     - evaluating forecasting results of each run
         """
 
         # Initialize 
-        now = pd.datetime.now()
+        now = datetime.now()
         data = check_dataset(data, False, self.DECOM_MODE, self.REDECOM_LIST)
         self.TARGET = data['target']
         
         if self.PATH is None: print('Do not set a PATH! It is recommended to set a PATH to prevent the loss of running results')
         if predict_method is None: raise ValueError("Please input a predict method! eg. 'single', 'ensemble', 'respective', 'hybrid'.")
         else: predict_method = predict_method.capitalize()
         if predict_method == 'Single': predictor_name = name_predictor(now, 'Multiple Single', 'Keras', self.KERAS_MODEL, None, None, self.NEXT_DAY)
@@ -866,15 +849,15 @@
         Output
         ---------------------
         df_eval_result     - evaluating forecasting results of each run
         """
 
         # Initialize 
         self.NEXT_DAY = True
-        now = pd.datetime.now()
+        now = datetime.now()
         start = time.time()
         data = check_dataset(data, False, self.DECOM_MODE, self.REDECOM_LIST)
         if self.PATH is None: 
             if transfer_learning: raise ValueError('Do not set a PATH! Please set a PATH to start transfer Learning.')
             print('Do not set a PATH! It is recommended to set a PATH to prevent the loss of running results')
         if predict_method is None: raise ValueError("Please input a predict method! eg. 'single', 'ensemble', 'respective', 'hybrid'.")
         else: predict_method = predict_method.capitalize()
```

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM/sklearn_predictor.py` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/sklearn_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 
 # Import modules for sklearn_predictor
 import os
 import sys
 import time
 import numpy as np
 import pandas as pd
+from datetime import datetime
 import warnings
 warnings.filterwarnings("ignore") # Ignore some annoying warnings
 # CEEMDAN_LSTM
 from CEEMDAN_LSTM.core import check_dataset, check_path, plot_save_result, name_predictor
 # Sklearn
-import matplotlib as plt
+import matplotlib.pyplot as plt
 from sklearn.svm import SVR
 from sklearn.linear_model import Lasso
 from sklearn.model_selection import cross_val_score, GridSearchCV
 
 class sklearn_predictor:
     # 0.Initialize
     # ------------------------------------------------------
@@ -113,15 +114,15 @@
     # SVM (Support Vector Machine Regression)
     def svm_predict(self, data=None, grid_search_times=5, show_data=False, plot_result=False, save_result=False):
         """
         Single Method (directly forecast)
         Use keras model to directly forecast wiht vector input
         Example: 
         sr = cl.sklearn_predictor()
-        df_result = kr.svm_predict(data, show_data=True, plot_result=True)
+        df_result = sr.svm_predict(data, show_data=True, plot_result=True)
 
         Input and Parameters:
         ---------------------
         Note important hyperarameters of class cl.sklearn_predictor()
         data               - data set (include training set and test set)
         grid_search_times  - grid search times
         show_data          - show the inputting data set
@@ -134,15 +135,15 @@
         df_predict_real   - forecasting results and the original real series set
         df_eval           - evaluating results of forecasting 
         next_y            - forecasting result of the next day when NEXT_DAY=Ture
         """
 
         # Name and set target
         self.SKLEARN_MODEL = 'SVM'
-        now = pd.datetime.now()
+        now = datetime.now()
         predictor_name = name_predictor(now, '', 'Sklearn', self.SKLEARN_MODEL, None, None, False)
         data = check_dataset(data, show_data)
         self.TARGET = data['target']
 
         # Divide the training and test set
         from CEEMDAN_LSTM.data_preprocessor import normalize_dataset, eval_result
         start = time.time()
```

### Comparing `CEEMDAN_LSTM-1.2b0/CEEMDAN_LSTM.egg-info/PKG-INFO` & `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CEEMDAN-LSTM
-Version: 1.2b0
+Version: 1.2b1
 Summary: CEEMDAN_LSTM is a Python project for decomposition-integration forecasting models based on EMD methods and LSTM.
 Home-page: http://github.com/FateMurphy/CEEMDAN_LSTM
 Author: Feite Zhou
 Author-email: jupiterzhou@foxmail.com
 Keywords: CEEMDAN,VMD,LSTM,decomposition,forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `CEEMDAN_LSTM-1.2b0/LICENSE` & `CEEMDAN_LSTM-1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b0/PKG-INFO` & `CEEMDAN_LSTM-1.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CEEMDAN_LSTM
-Version: 1.2b0
+Version: 1.2b1
 Summary: CEEMDAN_LSTM is a Python project for decomposition-integration forecasting models based on EMD methods and LSTM.
 Home-page: http://github.com/FateMurphy/CEEMDAN_LSTM
 Author: Feite Zhou
 Author-email: jupiterzhou@foxmail.com
 Keywords: CEEMDAN,VMD,LSTM,decomposition,forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `CEEMDAN_LSTM-1.2b0/README.md` & `CEEMDAN_LSTM-1.2b1/README.md`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b0/setup.py` & `CEEMDAN_LSTM-1.2b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='CEEMDAN_LSTM',
-    version='1.2b',
+    version='1.2b1',
     packages=setuptools.find_packages(),
     install_requires=['numpy >= 1.17.3',
                       'pandas >= 1.2.0',
                       'EMD-signal >= 1.2.3',
                       'optuna >= 3.0.0',
                       'vmdpy',
                       'sampen',
                       'matplotlib',
                       'sklearn',
-                      'tensorflow',
+                      'tensorflow >= 2.5.0',
                       ],
     package_data={'CEEMDAN_LSTM': ['datasets/*']},
     description='CEEMDAN_LSTM is a Python project for decomposition-integration forecasting models based on EMD methods and LSTM.',
     url='http://github.com/FateMurphy/CEEMDAN_LSTM',
 
     author='Feite Zhou',
     author_email='jupiterzhou@foxmail.com',
```

