# Comparing `tmp/gtst-0.0.5.tar.gz` & `tmp/GTST-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "GTST-0.0.6.tar", last modified: Wed Jun 14 10:07:40 2023, max compression
```

## Comparing `gtst-0.0.5.tar` & `GTST-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0   130033 2020-02-02 00:00:00.000000 gtst-0.0.5/README.ipynb
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 gtst-0.0.5/requirements.txt
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 gtst-0.0.5/test.ipynb
--rw-r--r--   0        0        0    23546 2020-02-02 00:00:00.000000 gtst-0.0.5/GTST/MMD.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 gtst-0.0.5/GTST/MONK.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 gtst-0.0.5/GTST/__init__.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 gtst-0.0.5/GTST/glasso.py
--rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 gtst-0.0.5/GTST/kernels/DeepKernel.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 gtst-0.0.5/GTST/kernels/GNTK.py
--rw-r--r--   0        0        0    25851 2020-02-02 00:00:00.000000 gtst-0.0.5/GTST/kernels/RandomWalk.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 gtst-0.0.5/GTST/kernels/WL.py
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 gtst-0.0.5/GTST/kernels/WWL.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtst-0.0.5/GTST/kernels/__init__.py
--rw-r--r--   0        0        0    78301 2020-02-02 00:00:00.000000 gtst-0.0.5/README_files/README_29_1.png
--rw-r--r--   0        0        0    79660 2020-02-02 00:00:00.000000 gtst-0.0.5/README_files/README_31_1.png
--rw-r--r--   0        0        0    77505 2020-02-02 00:00:00.000000 gtst-0.0.5/README_files/README_32_1.png
--rw-r--r--   0        0        0    87192 2020-02-02 00:00:00.000000 gtst-0.0.5/README_files/README_34_1.png
--rw-r--r--   0        0        0    78093 2020-02-02 00:00:00.000000 gtst-0.0.5/README_files/README_41_1.png
--rw-r--r--   0        0        0    72039 2020-02-02 00:00:00.000000 gtst-0.0.5/README_files/README_46_1.png
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 gtst-0.0.5/.gitignore
--rw-r--r--   0        0        0    25160 2020-02-02 00:00:00.000000 gtst-0.0.5/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 gtst-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    25028 2020-02-02 00:00:00.000000 gtst-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 10:07:40.327576 GTST-0.0.6/
+-rw-rw-rw-   0        0        0     1102 2023-04-14 21:26:45.000000 GTST-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    26519 2023-06-14 10:07:40.327576 GTST-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    25552 2023-06-14 09:39:21.000000 GTST-0.0.6/README.md
+-rw-rw-rw-   0        0        0      227 2023-04-18 23:57:55.000000 GTST-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1290 2023-06-14 10:07:40.328576 GTST-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-04-18 23:19:33.000000 GTST-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 10:07:40.284566 GTST-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 10:07:40.301571 GTST-0.0.6/src/GTST/
+-rw-rw-rw-   0        0        0    23589 2023-04-19 12:24:41.000000 GTST-0.0.6/src/GTST/MMD.py
+-rw-rw-rw-   0        0        0     4810 2023-04-18 15:04:29.000000 GTST-0.0.6/src/GTST/MONK.py
+-rw-rw-rw-   0        0        0      176 2023-04-19 12:12:37.000000 GTST-0.0.6/src/GTST/__init__.py
+-rw-rw-rw-   0        0        0     3876 2023-04-02 21:45:10.000000 GTST-0.0.6/src/GTST/glasso.py
+drwxrwxrwx   0        0        0        0 2023-06-14 10:07:40.325576 GTST-0.0.6/src/GTST/kernels/
+-rw-rw-rw-   0        0        0     9216 2023-04-19 16:53:27.000000 GTST-0.0.6/src/GTST/kernels/DeepKernel.py
+-rw-rw-rw-   0        0        0    10692 2023-04-17 21:54:26.000000 GTST-0.0.6/src/GTST/kernels/GNTK.py
+-rw-rw-rw-   0        0        0    22303 2023-04-19 20:09:21.000000 GTST-0.0.6/src/GTST/kernels/RandomWalk.py
+-rw-rw-rw-   0        0        0     9069 2023-04-17 22:17:00.000000 GTST-0.0.6/src/GTST/kernels/WWL.py
+-rw-rw-rw-   0        0        0      156 2023-04-18 23:02:29.000000 GTST-0.0.6/src/GTST/kernels/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 10:07:40.321575 GTST-0.0.6/src/GTST.egg-info/
+-rw-rw-rw-   0        0        0    26519 2023-06-14 10:07:40.000000 GTST-0.0.6/src/GTST.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-06-14 10:07:40.000000 GTST-0.0.6/src/GTST.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 10:07:40.000000 GTST-0.0.6/src/GTST.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 09:50:51.000000 GTST-0.0.6/src/GTST.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      164 2023-06-14 10:07:40.000000 GTST-0.0.6/src/GTST.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-14 10:07:40.000000 GTST-0.0.6/src/GTST.egg-info/top_level.txt
```

### Comparing `gtst-0.0.5/GTST/MMD.py` & `GTST-0.0.6/src/GTST/MMD.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-
-
-
-
 import numpy as np
 import warnings
 import networkx as nx
 from GTST.MONK import MMD_MONK
 import tqdm
 
-from GTST.kernels import RandomWalk, WWL, GNTK, DeepKernel
-import GTST.glasso as glasso
+import GTST
 
 # Biased empirical maximum mean discrepancy
 def MMD_b(K: np.array, n1: int, n2: int):
     '''
     Biased empirical maximum mean discrepancy
 
     Parameters
@@ -143,15 +138,15 @@
 class BoostrapMethods():
     """
     Various Bootstrap/Permutation Functions
 
     Class for permutation testing
     """
 
-    def __init__(self, list_of_functions:list,function_arguments:dict,) -> None:
+    def __init__(self, list_of_functions:list,function_arguments:dict) -> None:
         """
 
         Parameters
         ---------------------------
         list_of_functions: list,
             list containing function that represent a MMD calculation
 
@@ -237,15 +232,15 @@
 
         if verbose:
             pbar = tqdm.tqdm(total = B)
         # Now Perform Bootstraping
         for boot in range(B):
             K_i = evaluation_method(K)
             if check_symmetry:
-                if self.issymmetric(K_i):
+                if not self.issymmetric(K_i):
                     warnings.warn("Not a Symmetric matrix", Warning)
 
             # apply each test defined in list_if_functions, and keep the bootstraped/permutated value
             for i in range(len(self.list_of_functions)):
                 key = self.list_of_functions[i].__name__
                 boot_statistic[key][boot] = self.list_of_functions[i](K_i, **self.function_arguments[key])
 
@@ -374,15 +369,15 @@
         for i in range(window_size,X1.shape[0]+1,window_size):
             # Extract data points used to estimate a precision matrix
             tmp_X1= X1[(i-window_size):(i)].copy()
 
             if tmp_X1.shape[0] != window_size:
                 break
         
-            info_G1 = glasso.glasso_wrapper(alpha =self.alpha, beta = self.beta, nonparanormal=self.nonparanormal, scale = self.scale ).fit(tmp_X1)
+            info_G1 = GTST.glasso.glasso_wrapper(alpha =self.alpha, beta = self.beta, nonparanormal=self.nonparanormal, scale = self.scale ).fit(tmp_X1)
             precision1 = info_G1.precision_.copy()
             np.fill_diagonal(precision1,0)
             G1i = nx.from_numpy_array(precision1)
             if callable(set_attributes):
                 attributes_i = set_attributes(tmp_X1)
                 nx.set_node_attributes(G1i, {k:attributes_i[k] for k in range(len(attributes_i))}, 'attr')
             if set_labels is not None:
@@ -402,15 +397,15 @@
         for i in range(window_size,X2.shape[0]+1,window_size):
             # Extract data points used to estimate a precision matrix
             tmp_X2= X2[(i-window_size):(i)].copy()
 
             if tmp_X2.shape[0] != window_size:
                 break
              # Estimate precision2
-            info_G2 = glasso.glasso_wrapper(alpha =self.alpha, beta = self.beta, nonparanormal=self.nonparanormal, scale = self.scale ).fit(tmp_X2)
+            info_G2 = GTST.glasso_wrapper(alpha =self.alpha, beta = self.beta, nonparanormal=self.nonparanormal, scale = self.scale ).fit(tmp_X2)
             precision2 = info_G2.precision_.copy()
             np.fill_diagonal(precision2,0)
             G2i = nx.from_numpy_array(precision2)
             if callable(set_attributes):
                 attributes_i = set_attributes(tmp_X2)
                 nx.set_node_attributes(G2i, {k:attributes_i[k] for k in range(X2.shape[1])}, 'attr')
             if set_labels is not None:
@@ -507,74 +502,74 @@
             function_arguments[estimator] = fun_args[estimator]
 
 
         pval = BoostrapMethods(list_of_functions=list_of_functions, function_arguments=function_arguments)
 
         # Caluclate kernel
         if kernel == "RW_ARKU_plus":
-            rw_kernel = RandomWalk.RandomWalk(self.G1+self.G2, r = kwargs['r'],c = kwargs['c'], 
+            rw_kernel = GTST.RandomWalk(self.G1+self.G2, r = kwargs['r'],c = kwargs['c'], 
                                                 edge_attr=getattr(self, 'edge_attr', None), 
                                                 normalize=kwargs.get('normalize',False), 
                                                 node_attr= getattr(self, 'node_attr', None))
             rw_kernel.fit(calc_type = "ARKU_plus",  
                             verbose = kwargs.get('verbose',False), 
                             check_psd = kwargs.get('check_psd',True))
 
             self.K = rw_kernel.K
             del rw_kernel
         elif kernel == "RW_ARKU":
-            rw_kernel = RandomWalk.RandomWalk(self.G1+self.G2, r = kwargs['r'],c = kwargs['c'], 
+            rw_kernel = GTST.RandomWalk(self.G1+self.G2, r = kwargs['r'],c = kwargs['c'], 
                                                 edge_attr=getattr(self, 'edge_attr', None), 
                                                 normalize=kwargs.get('normalize',False), 
                                                 node_attr= getattr(self, 'node_attr', None))
             rw_kernel.fit(calc_type = "ARKU",  
                             verbose = kwargs.get('verbose',False), 
                             check_psd = kwargs.get('check_psd',True))
 
             self.K = rw_kernel.K
             del rw_kernel
         elif kernel == "RW_ARKU_edge":
-            rw_kernel = RandomWalk.RandomWalk(self.G1+self.G2, r = kwargs['r'],c = kwargs['c'], 
+            rw_kernel = GTST.RandomWalk(self.G1+self.G2, r = kwargs['r'],c = kwargs['c'], 
                                     edge_attr=getattr(self, 'edge_attr', None), 
                                     normalize=kwargs.get('normalize',False), 
                                     edge_label = kwargs['edge_label'],
                                     unique_edge_labels=kwargs['unique_edge_labels'])
             rw_kernel.fit(calc_type = "ARKU_edge",  
                             verbose = kwargs.get('verbose',False), 
                             check_psd = kwargs.get('check_psd',True))
 
             self.K = rw_kernel.K
             del rw_kernel
         elif kernel == "RW_ARKL":
-            rw_kernel = RandomWalk.RandomWalk(self.G1+self.G2, r = kwargs['r'],c = kwargs['c'], 
+            rw_kernel = GTST.RandomWalk(self.G1+self.G2, r = kwargs['r'],c = kwargs['c'], 
                                     edge_attr=getattr(self, 'edge_attr', None), 
                                     normalize=kwargs.get('normalize',False), 
                                     node_label = kwargs['node_label'],
                                     unique_node_labels=kwargs['unique_node_labels'])
             rw_kernel.fit(calc_type = "ARKL",  
                             verbose = kwargs.get('verbose',False), 
                             check_psd = kwargs.get('check_psd',True))
 
             self.K = rw_kernel.K
             del rw_kernel
         elif kernel == "GNTK":
-            gntk_kernel = GNTK.GNTK(num_layers= kwargs['num_layers'], num_mlp_layers = kwargs['num_layers'], 
+            gntk_kernel = GTST.GNTK(num_layers= kwargs['num_layers'], num_mlp_layers = kwargs['num_layers'], 
                                         jk = kwargs['jk'], scale = kwargs['scale'], normalize=kwargs.get('normalize',False))
             
-            gntk_kernel.fit_all(self.G1+self.G2,degree_as_tag=kwargs.get('degree_as_tag',True),features= getattr(self, 'node_attr', None))
+            gntk_kernel.fit_all(self.G1+self.G2,degree_as_tag=kwargs.get('degree_as_tag',True),features= getattr(self, 'node_attr', None), verbose = kwargs.get('verbose',False))
             self.K = gntk_kernel.K
             del gntk_kernel
         elif kernel == "WWL":
-            wwl_kernel = WWL.WWL( param =dict(discount=kwargs['discount'], h=kwargs['h'], sinkhorn=kwargs.get('sinkhorn', False), 
+            wwl_kernel = GTST.WWL( param =dict(discount=kwargs['discount'], h=kwargs['h'], sinkhorn=kwargs.get('sinkhorn', False), 
                                     sinkhorn_lambda = kwargs.get('sinkhorn_lambda', 1), normalize = kwargs.get('normalize',False)),
                                     label_name=self.node_label)
             self.K = wwl_kernel.fit_transform(self.G1+self.G2)
             del wwl_kernel
         elif kernel == 'DK':
-            dk_kernel = DeepKernel.DK(type = kwargs['type'], wl_it = kwargs.get('wl_it',2),opt_type= kwargs.get('opt_type',None),
+            dk_kernel = GTST.DK(type = kwargs['type'], wl_it = kwargs.get('wl_it',2),opt_type= kwargs.get('opt_type',None),
                                       vector_size= kwargs.get('vector_size',2), window=kwargs.get('window',2), min_count=kwargs.get('min_count',0), 
                                       normalize = kwargs.get('normalize',False), nodel_label=self.node_label)
             self.K = dk_kernel.fit_transform(self.G1+self.G2)
             del dk_kernel
         elif type(kernel) == list:
             import grakel as gk
             # Grakel kernels
@@ -596,16 +591,15 @@
 
         elif type(kernel) == np.ndarray:
             self.K = kernel
         else: 
             raise ValueError(f'{kernel} not defined ')
 
 
-
-        pval.Bootstrap(self.K, kwargs.get('B',1000))
+        pval.Bootstrap(self.K, kwargs.get('B',1000), method = kwargs.get('bootstrap_method', 'PermutationScheme'), check_symmetry=kwargs.get('check_symmetry', False))
         self.p_values = pval.p_values
         self.sample_mmd = pval.sample_test_statistic
```

### Comparing `gtst-0.0.5/GTST/MONK.py` & `GTST-0.0.6/src/GTST/MONK.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     
 
 
     def __init__(self,Q=11,K=None,maxiter=100,epsilon=1e-5,perte=False,beta=0.001, solver = 'BCD'):
 
         # Even so that the median can be calculated by picking the middle point
         if Q % 2 == 0:
-            raise ValueError('Q should be even')
+            raise ValueError('Q should be odd')
         args, _, _, values = inspect.getargvalues(inspect.currentframe())
         values.pop("self")
         for arg, val in values.items():
             setattr(self, arg, val)
 
     def estimate(self,y1,y2):
         if self.solver == 'BCD' :
```

### Comparing `gtst-0.0.5/GTST/glasso.py` & `GTST-0.0.6/src/GTST/glasso.py`

 * *Files identical despite different names*

### Comparing `gtst-0.0.5/GTST/kernels/DeepKernel.py` & `GTST-0.0.6/src/GTST/kernels/DeepKernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 """
-# Most of the original code:
 Author: Pinar Yanardag (ypinar@purdue.edu)
 Please refer to: http://web.ics.purdue.edu/~ypinar/kdd for more details.
 """
 
 from collections.abc import Iterable
 import networkx as nx
 import numpy as np
@@ -227,14 +226,16 @@
                     P[i][jdx] = prob_map[i].get(j,0)
             K = P.dot(P.T)
 
     
         if self.normalize:
             K = self.normalize_kernel_matrix(K)
 
+        self.K = K
+
         return K
```

### Comparing `gtst-0.0.5/GTST/kernels/GNTK.py` & `GTST-0.0.6/src/GTST/kernels/GNTK.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+### Most of the code is from Simon S. Du, Kangcheng Hou, Barnabás Póczos, Ruslan Salakhutdinov, Ruosong Wang, Keyulu Xu. Graph Neural Tangent Kernel: Fusing Graph Neural Networks with Graph Kernels. NeurIPS 2019
+## Adjusted so the class can work on networkx graphs
+
+
+
+
 import math
 import numpy as np
 import scipy as sp
 import tqdm
 
 
 class GNTK(object):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gtst-0.0.5/GTST/kernels/RandomWalk.py` & `GTST-0.0.6/src/GTST/kernels/RandomWalk.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             self.all_A = [[None] * len(self.unique_edge_labels)] * self.N
 
 
         if calc_type == "ARKL":
             self.Ls = [None] * self.N
             for i in range(self.N):
                 self.Ls[i] = self._get_node_label_vectors(self.X[i], self.unique_node_labels, self.node_label)
-        
+                
         # Calculate kernel
         for i in range(self.N):
             for j in range(i,self.N):
                 if calc_type == "ARKU":
                     (i,j,value) = self.fit_arku_ij(i,j,pbar)
 
                 elif calc_type == "ARKU_plus":
@@ -389,93 +389,14 @@
                             self.r, self.Ls[i], self.Ls[j], self.p[i], self.p[j], self.q[i], self.q[j])
 
         if pbar is not None:
             pbar.update()
 
         return (i,j,value)
 
-    def fit_ARKL(self, r, label_list, normalize_adj = False, row_normalize_adj = False, edge_attr =None, verbose = True, label_name = 'label'):
-        """
-        Fit approximate label node random walk kernel.
-
-        Parameters
-        ----------------------------
-        r - int, number of eigenvalues
-        label_list - array with labels
-        normalize_adj - bool, Should the adj matrix normalized? D^{-1/2}AD^{-1/2} where A is adj matrix and D is degree matrix.
-        row_normalize_adj - bool, Should the adj matrix be row normalized? AD^{-1/2} where A is adj matrix and D is degree matrix.
-        verbose - bool, print progress bar?
-        label_name - str, what is the name of labels
-
-        Returns 
-        ------------------
-        K - np.array, N x N, kernel matrix, N number of graphs
-        
-        """
-
-        if normalize_adj and row_normalize_adj:
-            raise ValueError("Can not have both row normalized and normalized adj") 
-
-        
-        all_A = [None] * self.N
-        U_list = [None] * self.N  # left SVD matrix of each adj matrix
-        Lamda_list = [None] * self.N  # eigenvalues of each adj matrix
-        Vt_list = [None] * self.N  # Right transposed SVD matrix of each adj matrix
-        K = np.zeros((self.N, self.N))
-
-        if verbose:
-            pbar = tqdm.tqdm(disable=(verbose is False), total=self.N*(self.N+1)/2)
-
-        # get label matrix/vector of all graphs
-        Ls = [None] * self.N
-        for i in range(self.N):
-            Ls[i] = self._get_node_label_vectors(self.X[i], label_list, label_name)
-
-        for i in range(self.N):
-            for j in range(i,self.N):
-
-
-                if row_normalize_adj:
-                    if all_A[i] is None:
-                        all_A[i] = self._row_normalized_adj(self.X[i], edge_attr = edge_attr)
-                        U_list[i], Lamda_list[i], Vt_list[i] = randomized_svd(all_A[i].T, n_components= r)
-                    if all_A[j] is None:
-                        all_A[j] = self._row_normalized_adj(self.X[j], edge_attr = edge_attr)
-                        U_list[j], Lamda_list[j], Vt_list[j] = randomized_svd(all_A[j].T, n_components= r)
-                else:
-                    if all_A[i] is None:
-                        all_A[i] = self._get_adj_matrix(self.X[i], edge_attr = edge_attr)
-                        U_list[i], Lamda_list[i], Vt_list[i] = randomized_svd(all_A[i].T, n_components= r)
-                    if all_A[j] is None:
-                        all_A[j] = self._get_adj_matrix(self.X[j], edge_attr = edge_attr)
-                        U_list[j], Lamda_list[j], Vt_list[j] = randomized_svd(all_A[j].T, n_components= r)
-                
-
-
-                p1 = np.ones((self.X[i].number_of_nodes())) / float(self.X[i].number_of_nodes())
-                p2 = np.ones((self.X[j].number_of_nodes())) / float(self.X[j].number_of_nodes())
-                q1 = np.ones((self.X[i].number_of_nodes())) / float(self.X[i].number_of_nodes())
-                q2 = np.ones((self.X[j].number_of_nodes())) / float(self.X[j].number_of_nodes())
-    
-
-                K[i,j] = self.ARKL(U_list[i], Lamda_list[i], Vt_list[i], U_list[j], Lamda_list[j], Vt_list[j], r, Ls[i], Ls[j], p1, p2, q1, q2)
-
-                if verbose:
-                    pbar.update()
-
-        if verbose:
-            pbar.close()
-            
-        K = np.triu(K) + np.triu(K, 1).T
-
-        if self.normalize:
-            K = self.normalize_gram_matrix(K)
-
-        return K
-
 
     def ARKU_plus(self, u1, w1, u2, w2, r, p1, p2, q1, q2):
         """
         Fast Random walk kernel for symmetric (weight) matrices
 
         Parameters
         ----------------
```

### Comparing `gtst-0.0.5/GTST/kernels/WWL.py` & `GTST-0.0.6/src/GTST/kernels/WWL.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,15 @@
         M = (M + M.T)
 
         K = np.exp(-self.param['discount']*M)
 
         if self.param.get('normalize', False):
             K = self.normalize_gram_matrix(K)
 
+        self.K = K
         return  K
 
     @staticmethod
     def normalize_gram_matrix(x):
         k = np.reciprocal(np.sqrt(np.diag(x)))
         k = np.resize(k, (len(k), 1))
         return np.multiply(x, k.dot(k.T))
```

### Comparing `gtst-0.0.5/README.md` & `GTST-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-# MMDGraph
+![Tests](https://github.com/ragnarlevi/GTST/actions/workflows/tests.yml/badge.svg)
+[![Coverage Status](https://coveralls.io/repos/github/ragnarlevi/GTST/badge.svg?branch=test)](https://coveralls.io/github/ragnarlevi/GTST?branch=test)
+
+# GTST
+
 
 ## What is this package for?
 
-This package contains code to perform kernel two-sample hypothesis testing on samples of graphs. The code additionally allows for estimation of graphs from a real data matrix.
+This package contains code to perform kernel two-sample hypothesis testing on samples of graphs. The code additionally allows for the estimation of graphs from a real data matrix. Below one can find a description of the various function inputs available and examples of different use cases this package offers.
 
 
 ## How to install
 
 <code>pip install GTST</code>
 
-Note that if one wants to use the WWL kernel then the pot package has to be installed via  <code>pip install pot</code>.
+Note that if one wants to use Grakel kernels then the Grakel package has to be installed via  <code>pip install grakel</code>.
 
 
 ## Function Inputs
 
 <code>GTST.MMD</code> is the main function used. If the user already has samples of graphs where each sample is a list of networkx graph objects then the user can use the <code>fit</code> method to perform the hypothesis test.
 
-* **kernel**: list, str, np.array. If str then one of kernels provided by the MMDGraph: RW_ARKU_plus, RW_ARKU, RW_ARKU_edge, RW_ARKL, GNTK, WWL, DK. If list then a GraKel kernel is used meaning the list should be formatted as one would do for the GraKel package. If np.array then a pre-calculated kernel is used.
+* **kernel**: list, str, np.array. If str then one of the kernels provided by the MMDGraph: RW_ARKU_plus, RW_ARKU, RW_ARKU_edge, RW_ARKL, GNTK, WWL, DK. If list then a GraKel kernel is used meaning the list should be formatted as one would do for the GraKel package. If np.array then a pre-calculated kernel is used.
 * **mmd_estimators**:str or list of strings, example MMD_u, MMD_b, MONK, MMD_l.
 
 The fit method additionally takes in additional parameters that are used by the kernel functions or the bootstrap function, such as:
 
 * **edge_attr**: Edge attribute name, if any.
 * **node_attr**: Node attribute name, if any.
 * **node_label**: Node label name, if any.
-* **edge_label**: Edge label  name, if any.
+* **edge_label**: Edge label name, if any.
 * **Q**: int, number of partitions for the MONK estimator.
 * **B**: int, number of bootstraps for p-value estimation.
 * **B**: int, number of bootstraps for p-value estimation.
 
 The RW kernels take:
 * **r**: int, number of eigenvalues.
 * **c**: float, discount constant.
@@ -47,58 +51,58 @@
 * **sinkhorn**:bool, should the Wasserstein calculation be sped up and approximated?
 * **sinkhorn_lambda**: float, regularization term >0.
 * **normalize**: bool, normalize kernel?
 
 The DK kernel uses:
 * **type**: str, 'wl', 'sp'. 
 * **wl_it**: int, number of WL iterations (only used if type = wl)
-* **opt_type**: str, if opt_type = 'word2vec' then a similarity matrix is estimated using gensim which needs to be installed, If None the similiarity matrix is just the frequency.
+* **opt_type**: str, if opt_type = 'word2vec' then a similarity matrix is estimated using gensim which needs to be installed, If None the similarity matrix is just the frequency.
 * **vector_size**: int, the dimensionality of the word vectors. Only used if opt\_type = 'word2vec'.
 * **window**: int, the maximum distance between the current and predicted word within a sentence.  Only used if opt\_type = 'word2vec'.
 * **min_count**: int, Ignores all words with total frequency lower than this. Might have to be set to zero for the estimation to work.  Only used if opt\_type = 'word2vec'.
 * **node_label**: str, name of node labels.
 * **workers**: int, Use these many worker threads to train the model (=faster training with multicore machines).  Only used if opt\_type = 'word2vec'.
 * **normalize**: bool, normalize kernel?
 
 
-
 If the user has data matrices then the method <code>estimate_graphs</code> can be used beforehand to estimate graph samples using sklearn graphical lasso the inputs are:
 
 * **X1,X2**: two numpy arrays.
-* **window\_size**: integer that controls how many samples are used to estimate each graph. That is window_size = 50, means that the first 50 samples are used to estimate the first graph, the next 50 graphs are used to estimate the second and so on. If the window size is not divisible by the total length of the data arrays then the remainder will be skipped.
-* **alpha**: float, Regularization parameters in a list or a single float. If list then EBIC will be used to select best graph.
+* **window\_size**: an integer that controls how many samples are used to estimate each graph. That is window_size = 50, which means that the first 50 samples are used to estimate the first graph, the next 50 graphs are used to estimate the second and so on. If the window size is not divisible by the total length of the data arrays then the remainder will be skipped.
+* **alpha**: float, Regularization parameters in a list or a single float. If a list then EBIC will be used to select the best graph.
 * **beta**: float. EBIC hyperparameter.
 * **nonparanormal**: bool, should data be nonparanormally transformed?
 * **scale** bool , should data be scaled?
 * **set_attributes**: function or None, set attribute of nodes. The function should take numpy array  (which will be a submatrix of X1,X2) as input and output attributes for each node/parameter, used as an attribute for a graph kernel. See an example in usage below.
 * **set_labels**: function, str, dict or None. If a function should take networkx graph as input and output labels for each node/parameter.  Should return a dict {node_i:label,..}. 
 If dict, then should be: dict['1'] = dictionary with label for each node in sample 1 ({node:label}),dict['2'] = dictionary with label for each node in sample 2 ({node:label})
 If string = 'degree' then nodes will be labelled with degree. If None no labelling.
 
 After the estimate_graphs procedure has been run then the user should run <code>fit</code> to perform the hypothesis test, but be sure to leave G1 = None and G2= None.
 
 
 
+
 ## Usage
 
-We will go through multiple scenarios: The case when the user has it own networkx graphs, when they are estimated from data matrices, using different kernels and using different MMD estimators.
+We will go through multiple scenarios: The case when the user has its own networkx graphs, when they are estimated from data matrices, using different kernels and using different MMD estimators.
 
 
 ```python
 import numpy as np
 import networkx as nx
 import matplotlib.pyplot as plt
 import GTST
 ```
 
 ### Fit when H1 true, different edge probability
 
-In this example, we simulate binomial graphs assuming that the two samples have different edge probabilities. There will be 50 graphs in each sample and the number of nodes is 30 for all graphs. Sample 1 has an edge probabilty of 0.3 and sample 2 has an edge probability of 0.4. We will label each node with its corresponding degree so that graph kernels that assume labels can be used.
+In this example, we simulate binomial graphs assuming that the two samples have different edge probabilities. There will be 50 graphs in each sample and the number of nodes is 30 for all graphs. Sample 1 has an edge probability of 0.3 and sample 2 has an edge probability of 0.4. We will label each node with its corresponding degree so that graph kernels that assume labels can be used.
 
-Start by creating two samples of graphs
+Start by creating two samples of graphs:
 
 
 ```python
 
 n1 = n2 = 50  # sample sizes
 # generate two samples
 g1 = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n1)]
@@ -609,15 +613,15 @@
 X2 = np.random.multivariate_normal(np.ones(11),np.linalg.inv(A), size = 10000)
 ```
 
     
 
 
 ```python
-# Random Walk, with attributes, should reject. , the class will use the node label name 'attr'
+# Random Walk, with attributes, should reject. The class will use the node label name 'attr'
 # Define attribute function that sets the mean as the node attribute. 
 # Note the window size is 400 so there will be 400 observations that are used to estimate each graph/node attribute.
 def attr_function(X):
     return np.expand_dims(np.mean(X,axis = 0),axis=1)
 
 MMD_out = GTST.MMD()
 MMD_out.estimate_graphs(X1,X2,window_size=400, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False, set_attributes = attr_function)
@@ -630,15 +634,15 @@
         
 
     {'MMD_u': 0.0}
     
 
 
 ```python
-# If we do not give attributes, the test should not be rejected reject as underlying the precision matrices are the same
+# If we do not give attributes, the test should not be rejected as the underlying the precision matrices are the same
 MMD_out_no_attr = GTST.MMD()
 MMD_out_no_attr.fit(G1= MMD_out.G1, G2 = MMD_out.G2, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 5, c = 0.1, edge_attr = 'weight')
 print(MMD_out_no_attr.p_values)
 ```
 
     Using weight as edge attributes
     {'MMD_u': 0.993}
```

### Comparing `gtst-0.0.5/PKG-INFO` & `GTST-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,702 +1,717 @@
-Metadata-Version: 2.1
-Name: GTST
-Version: 0.0.5
-Summary: A package for comparing two-sample of graphs
-Author: Gareth W. Peters
-Author-email: "Ragnar L. Gudmundarson" <ragnarlevigud@gmail.com>
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: networkx>=2.7.1
-Requires-Dist: numpy>=1.24.0
-Requires-Dist: scikit-learn>=1.0.2
-Requires-Dist: scipy>=1.8.0
-Requires-Dist: tqdm>=4.63.1
-Description-Content-Type: text/markdown
-
-# MMDGraph
-
-## What is this package for?
-
-This package contains code to perform kernel two-sample hypothesis testing on samples of graphs. The code additionally allows for estimation of graphs from a real data matrix.
-
-
-## How to install
-
-<code>pip install GTST</code>
-
-Note that if one wants to use the WWL kernel then the pot package has to be installed via  <code>pip install pot</code>.
-
-
-## Function Inputs
-
-<code>GTST.MMD</code> is the main function used. If the user already has samples of graphs where each sample is a list of networkx graph objects then the user can use the <code>fit</code> method to perform the hypothesis test.
-
-* **kernel**: list, str, np.array. If str then one of kernels provided by the MMDGraph: RW_ARKU_plus, RW_ARKU, RW_ARKU_edge, RW_ARKL, GNTK, WWL, DK. If list then a GraKel kernel is used meaning the list should be formatted as one would do for the GraKel package. If np.array then a pre-calculated kernel is used.
-* **mmd_estimators**:str or list of strings, example MMD_u, MMD_b, MONK, MMD_l.
-
-The fit method additionally takes in additional parameters that are used by the kernel functions or the bootstrap function, such as:
-
-* **edge_attr**: Edge attribute name, if any.
-* **node_attr**: Node attribute name, if any.
-* **node_label**: Node label name, if any.
-* **edge_label**: Edge label  name, if any.
-* **Q**: int, number of partitions for the MONK estimator.
-* **B**: int, number of bootstraps for p-value estimation.
-* **B**: int, number of bootstraps for p-value estimation.
-
-The RW kernels take:
-* **r**: int, number of eigenvalues.
-* **c**: float, discount constant.
-* **normalize**:bool, normalize kernel matrix?
-
-The GNTK kernel takes:
-* **num_layers**: int, number of layers in the neural networks (including the input layer)
-* **num_mlp_layers**:int, number of MLP layers
-* **jk**: a bool variable indicating whether to add jumping knowledge
-* **scale**:str, the scale used aggregate neighbours [uniform, degree]
-* **normalize**:bool, normalize kernel matrix?
-
-The WWL kernel uses:
-* **discount**: float, discount
-* **h**: int, number of WL iterations:
-* **sinkhorn**:bool, should the Wasserstein calculation be sped up and approximated?
-* **sinkhorn_lambda**: float, regularization term >0.
-* **normalize**: bool, normalize kernel?
-
-The DK kernel uses:
-* **type**: str, 'wl', 'sp'. 
-* **wl_it**: int, number of WL iterations (only used if type = wl)
-* **opt_type**: str, if opt_type = 'word2vec' then a similarity matrix is estimated using gensim which needs to be installed, If None the similiarity matrix is just the frequency.
-* **vector_size**: int, the dimensionality of the word vectors. Only used if opt\_type = 'word2vec'.
-* **window**: int, the maximum distance between the current and predicted word within a sentence.  Only used if opt\_type = 'word2vec'.
-* **min_count**: int, Ignores all words with total frequency lower than this. Might have to be set to zero for the estimation to work.  Only used if opt\_type = 'word2vec'.
-* **node_label**: str, name of node labels.
-* **workers**: int, Use these many worker threads to train the model (=faster training with multicore machines).  Only used if opt\_type = 'word2vec'.
-* **normalize**: bool, normalize kernel?
-
-
-
-If the user has data matrices then the method <code>estimate_graphs</code> can be used beforehand to estimate graph samples using sklearn graphical lasso the inputs are:
-
-* **X1,X2**: two numpy arrays.
-* **window\_size**: integer that controls how many samples are used to estimate each graph. That is window_size = 50, means that the first 50 samples are used to estimate the first graph, the next 50 graphs are used to estimate the second and so on. If the window size is not divisible by the total length of the data arrays then the remainder will be skipped.
-* **alpha**: float, Regularization parameters in a list or a single float. If list then EBIC will be used to select best graph.
-* **beta**: float. EBIC hyperparameter.
-* **nonparanormal**: bool, should data be nonparanormally transformed?
-* **scale** bool , should data be scaled?
-* **set_attributes**: function or None, set attribute of nodes. The function should take numpy array  (which will be a submatrix of X1,X2) as input and output attributes for each node/parameter, used as an attribute for a graph kernel. See an example in usage below.
-* **set_labels**: function, str, dict or None. If a function should take networkx graph as input and output labels for each node/parameter.  Should return a dict {node_i:label,..}. 
-If dict, then should be: dict['1'] = dictionary with label for each node in sample 1 ({node:label}),dict['2'] = dictionary with label for each node in sample 2 ({node:label})
-If string = 'degree' then nodes will be labelled with degree. If None no labelling.
-
-After the estimate_graphs procedure has been run then the user should run <code>fit</code> to perform the hypothesis test, but be sure to leave G1 = None and G2= None.
-
-
-
-## Usage
-
-We will go through multiple scenarios: The case when the user has it own networkx graphs, when they are estimated from data matrices, using different kernels and using different MMD estimators.
-
-
-```python
-import numpy as np
-import networkx as nx
-import matplotlib.pyplot as plt
-import GTST
-```
-
-### Fit when H1 true, different edge probability
-
-In this example, we simulate binomial graphs assuming that the two samples have different edge probabilities. There will be 50 graphs in each sample and the number of nodes is 30 for all graphs. Sample 1 has an edge probabilty of 0.3 and sample 2 has an edge probability of 0.4. We will label each node with its corresponding degree so that graph kernels that assume labels can be used.
-
-Start by creating two samples of graphs
-
-
-```python
-
-n1 = n2 = 50  # sample sizes
-# generate two samples
-g1 = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n1)]
-g2 = [nx.fast_gnp_random_graph(30,0.4) for _ in range(n2)]
-
-# Set node labels as the degree
-for j in range(len(g1)):
-    nx.set_node_attributes(g1[j],  {key: str(value) for key, value in dict(g1[j].degree).items()} , 'label')
-for j in range(len(g2)):
-    nx.set_node_attributes(g2[j], {key: str(value) for key, value in dict(g2[j].degree).items()}, 'label')
-
-```
-
-Perform the MMD test using various kernels. Note that the unbiases MMD estimator is used
-
-
-```python
-# Random Walk, r is number of eigen-pairs, c is the discount constant
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1, G2 = g2, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 6, c = 0.001)  
-print(f" RW_ARKU_plus {MMD_out.p_values}")
-```
-
-     RW_ARKU_plus {'MMD_u': 0.0}
-    
-
-
-```python
-# RW kernel with labels, Note that we input the label list (all node labels encountered in both graph samples)
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1, G2 = g2, kernel = 'RW_ARKL', mmd_estimators = 'MMD_u', r = 4, c = 1e-3,node_label = 'label',
-                                    unique_node_labels= set(np.concatenate([list(nx.get_node_attributes(g, 'label').values())for g in g1+g2])))
-print(f" RW_ARKL {MMD_out.p_values}")
-
-```
-
-    Using label as node labels
-     RW_ARKL {'MMD_u': 0.0}
-    
-
-
-```python
-# GNTK kernel,
-# num_layers is the number of layers in the neural network,
-# num_mlp_layers is the number of multi-layer perceptron layers
-# jk indicate whether to add jumping knowledge
-# scale how to aggregate neighbours uniform or degree.
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1, G2 = g2, kernel = 'GNTK', mmd_estimators = 'MMD_u', num_layers = 2, num_mlp_lauers = 2, jk = True, scale = 'uniform')
-print(f" GNTK {MMD_out.p_values}")
-```
-
-    100%|██████████| 5050/5050.0 [00:11<00:00, 438.12it/s]
-
-     GNTK {'MMD_u': 0.0}
-    
-
-    
-    
-
-
-```python
-# WWL kernel
-# discount is discount
-# h is the number of WL iterations
-# node_label is the name of node labels
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1, G2 = g2, kernel = 'WWL', mmd_estimators = 'MMD_u', discount = 0.1, h = 2, node_label = 'label')
-print(f" WWL {MMD_out.p_values}")
-```
-
-    Using label as node labels
-     WWL {'MMD_u': 0.0}
-    
-
-
-```python
-# Deep Kernel without the deepness
-# type is wl= wl closeness or sp: shortest path closeness
-# wl_it is the number of wl iterations, only applicable for wl.
-# no deepness in this case only a frequency similarity
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1, G2 = g2, kernel = 'DK', mmd_estimators = 'MMD_u', type = 'wl', wl_it = 4, node_label = 'label')
-print(f" ML DK {MMD_out.p_values}")
-```
-
-    Using label as node labels
-     ML DK {'MMD_u': 0.0}
-    
-
-
-```python
-
-# Deep kernel with deepness, the user has to install gensim, this might take some time, can try to increase the number of workers
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1, G2 = g2, kernel = 'DK', mmd_estimators = 'MMD_u', type = 'wl', wl_it = 4, opt_type = 'word2vec', node_label = 'label', workers = 10)
-print(f" Deep DK {MMD_out.p_values}")
-```
-
-    Using label as node labels
-     Deep DK {'MMD_u': 0.0}
-    
-
-
-```python
-# It is also possible to use the Grakel library
-kernel = [{"name": "weisfeiler_lehman", "n_iter": 1}, {"name": "vertex_histogram"}]
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1, G2 = g2, kernel = kernel, mmd_estimators = 'MMD_u', node_label = 'label')
-print(f" WL {MMD_out.p_values}")
-```
-
-    Using label as node labels
-    label
-     WL {'MMD_u': 0.0}
-    
-
-
-```python
-# Grakel propagation
-kernel = [ {"name":"propagation", 't_max':5, 'w':0.1, 'M':"TV"}]
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1, G2 = g2, kernel = kernel, mmd_estimators = 'MMD_u', node_label = 'label')
-print(f" propagation {MMD_out.p_values}")
-
-```
-
-    Using label as node labels
-    label
-     propagation {'MMD_u': 0.0}
-    
-
-### Using different MMD estimators
-
-It is also possible  to use other MMD estimators such as the biases, linear and robust.
-
-
-```python
-# Q is the number of partitions in the MONK estimator
-
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1, G2 = g2, kernel = 'RW_ARKU_plus', mmd_estimators = ['MMD_u', 'MMD_b', 'MMD_l', 'MONK_EST'], r = 2, c = 0.001, Q = 5)
-print(f" RW_ARKU_plus {MMD_out.p_values}")
-```
-   
-
-     RW_ARKU_plus {'MMD_u': 0.0, 'MMD_b': 0.0, 'MMD_l': 0.0, 'MONK_EST': 0.0}
-    
-
-### H1 true, Graphs with different weights
-
-It is possible to test graphs which are topologically the same but have different edge weights. Here there are 50 graphs in each sample and the number of nodes is 30 for all graphs. The edge probability is 0.3. We will label each node with its corresponding degree so that graph kernels that assume labels can be used.
-
-
-```python
-n1 = n2 = 100
-g1_weights = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n1)]  # sample 1
-g2_weights = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n2)]  # sample 2
-
-# For loops to label each node accoriding to its degree for the two samples.
-for j in range(len(g1_weights)):
-    nx.set_node_attributes(g1_weights[j],  {key: str(value) for key, value in dict(g1_weights[j].degree).items()} , 'label')
-for j in range(len(g2_weights)):
-    nx.set_node_attributes(g2_weights[j], {key: str(value) for key, value in dict(g2_weights[j].degree).items()}, 'label')
-
-
-# For loops to label each node according to its degree for the two samples.
-def edge_dist(loc, scale ):
-    from scipy.stats import uniform
-    return np.random.normal(loc = loc, scale = scale)# uniform.rvs(size=1,  loc = loc , scale = scale)[0]
-def add_weight(G, loc, scale ):
-    edge_w = dict()
-    for e in G.edges():
-        edge_w[e] = edge_dist(loc, scale)
-    return edge_w
-
-
-for G in g1_weights:
-    nx.set_edge_attributes(G, add_weight(G, loc = 0.5, scale = 1), "weight")
-for G in g2_weights:
-    nx.set_edge_attributes(G, add_weight(G, loc = 0.5, scale = 2), "weight")
-
-```
-
-
-```python
-# Random Walk
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1_weights, G2 = g2_weights, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 2, c = 0.001, edge_attr = 'weight')
-print(f" RW_ARKU_plus {MMD_out.p_values}")
-```
-
-    Using weight as edge attributes
-     RW_ARKU_plus {'MMD_u': 0.0}
-    
-
-Note that if we use a graph kernel that does not take edge weights into account, the test will not be rejected.
-
-
-```python
-# Random Walk weights ignored, should not reject
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1_weights, G2 = g2_weights, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 2, c = 0.001)
-print(f" RW_ARKU_plus no labels {MMD_out.p_values}")
-```
-
-     RW_ARKU_plus no labels {'MMD_u': 0.462}
-    
-
-
-```python
-# Grakel pyramid match kernel
-kernel = [{"name": "pyramid_match", "L": 6, "d":6, 'with_labels':False}]
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1_weights, G2 = g2_weights, kernel = kernel, mmd_estimators = 'MMD_u', edge_attr = 'weight')
-print(f" pyramid_match {MMD_out.p_values}")
-```
-
-    Using weight as edge attributes
-    None
-     pyramid_match {'MMD_u': 0.0}
-    
-
-
-```python
-# propagation, needs node attribute or label 
-kernel = [ {"name":"propagation", 't_max':5, 'w':0.05, 'M':"TV"}]
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1_weights, G2 = g2_weights, kernel = kernel, mmd_estimators = 'MMD_u', edge_attr = 'weight', node_label = 'label')
-print(f" propagation {MMD_out.p_values}")
-```
-
-    Using weight as edge attributes
-    Using label as node labels
-    label
-     propagation {'MMD_u': 0.0}
-    
-
- ### H1 true different attributes
-
-Some kernels can be used to compare graphs with node attributes.
-
-
-```python
-
-n1 = n2 = 50
-g1_attr = [nx.fast_gnp_random_graph(30,0.2) for _ in range(n1)]  # sample 1
-g2_attr = [nx.fast_gnp_random_graph(30,0.2) for _ in range(n2)]  # sample 2
-# For loop for the two samples to add node attributes for each graph which have different normal distributions
-for j in range(len(g1_attr)):
-    nx.set_node_attributes(g1_attr[j], dict( ( (i, np.random.normal(loc = 0, scale = 0.1, size = (1,))) for i in range(len(g1_attr[j])) ) ), 'attr')
-for j in range(len(g2_attr)):
-    nx.set_node_attributes(g2_attr[j], dict( ( (i, np.random.normal(loc = 0.1, scale = 0.1, size = (1,))) for i in range(len(g2_attr[j])) ) ), 'attr')
-
-```
-
-
-```python
-# Random Walk with weights and node attributes
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1_attr, G2 = g2_attr, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 4, c = 0.01, node_attr = 'attr')
-print(f" RW_ARKU_plus {MMD_out.p_values}")
-```
-
-    Using attr as node attributes
-       
-
-     RW_ARKU_plus {'MMD_u': 0.0}
-    
-
-
-```python
-# GNTK with node attributes
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1_attr, G2 = g2_attr, kernel = 'GNTK', mmd_estimators = 'MMD_u', num_layers = 2, num_mlp_lauers = 2, jk = True, scale = 'uniform', node_attr = 'attr')
-print(f" GNTK {MMD_out.p_values}")
-```
-
-    Using attr as node attributes
-    
-
-    100%|██████████| 5050/5050.0 [00:04<00:00, 1246.33it/s]
-    
-
-     GNTK {'MMD_u': 0.0}
-    
-
-
-```python
-# Grakel propagation
-kernel = [ {"name":"propagation", 't_max':5, 'w':0.1, 'M':"L1",'with_attributes':True}]
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1_attr, G2 = g2_attr, kernel = kernel, mmd_estimators = 'MMD_u', discount = 0.1, h = 2, node_attr = 'attr')
-print(f" Propagation {MMD_out.p_values}")
-```
-
-    Using attr as node attributes
-    attr
-       
-
-     Propagation {'MMD_u': 0.0}
-    
-
-### Different edge labels
-
-The RW kernel can take different edge labels.
-
-
-```python
-n1 = n2 = 50
-g1_edge = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n1)]  # sample 1
-g2_edge = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n2)]  # sample 2
-
-# For loop to label each edge either 'a' or 'b' the labelling probabilities are different for the two samples
-for j in range(len(g1_edge)):
-    nx.set_edge_attributes(g1_edge[j], {(i,k):np.random.choice(['a','b'], p = [0.6,0.4]) for i,k in g1_edge[j].edges }, 'edge_label')
-for j in range(len(g2_edge)):
-    nx.set_edge_attributes(g2_edge[j], {(i,k):np.random.choice(['a','b'], p = [0.7,0.3]) for i,k in g2_edge[j].edges }, 'edge_label')
-
-
-
-```
-
-
-```python
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1_edge, G2 = g2_edge, kernel = 'RW_ARKU_edge', mmd_estimators = 'MMD_u', r = 6, c = 0.0001,edge_label = 'edge_label',unique_edge_labels= ['a', 'b'])
-print(f" RW_ARKU_edge {MMD_out.p_values}")
-
-```
-
-    Using edge_label as edge labels
-     RW_ARKU_edge {'MMD_u': 0.0}
-    
-
-# Directed Graphs
-
-The RW kernel can take directed graphs
-
-
-```python
-n1 = n2 = 50
-g1_di = [nx.fast_gnp_random_graph(30,0.2) for _ in range(n1)]  # sample 1
-g2_di = [nx.fast_gnp_random_graph(30,0.2) for _ in range(n2)]  # sample 2
-
-# for loop for both samples to convert the networkx graph to a networkx directed graph object
-for j in range(len(g1_di)):
-    g1_di[j] = nx.DiGraph(g1_di[j])
-for j in range(len(g2_di)):
-    g2_di[j] = nx.DiGraph(g2_di[j])
-
-# for loop for both samples that removes edges with different removal probabilties between the two samples
-for j in range(len(g1_di)):
-    edges= list(g1_di[j].edges())
-    for e,u in edges:
-        if np.random.uniform() <0.3:
-            g1_di[j].remove_edge(e,u)
-for j in range(len(g2_di)):
-    edges= list(g2_di[j].edges())
-    for e,u in edges:
-        if np.random.uniform() <0.5:
-            g2_di[j].remove_edge(e,u)
-
-
-
-
-
-```
-
-
-```python
-MMD_out = GTST.MMD()
-MMD_out.fit(G1 = g1_di, G2 = g2_di, kernel = 'RW_ARKU', mmd_estimators = 'MMD_u', r = 4, c = 1e-3)
-print(f" RW_ARKU_edge {MMD_out.p_values}")
-
-```
-
-     RW_ARKU_edge {'MMD_u': 0.0}
-    
-
-### Two data matrices with different structure
-It is possible to estimate graphs from data matrices.
-
-
-```python
-G = nx.fast_gnp_random_graph(11, 0.25, seed=42)  # generate a random graph
-assert nx.is_connected(G)
-
-#  Add random weights to the graphs, either positive or negative
-for e in G.edges():
-    if np.random.uniform() <0.1:
-        w = np.random.uniform(low = 0.1, high = 0.3)
-        G.edges[e[0], e[1]]['weight'] = -w
-    else:
-        w = np.random.uniform(low = 0.1, high = 0.3)
-        G.edges[e[0], e[1]]['weight'] = w
-
-# Extract the adjacency matrix and fill the diagonal so that the resulting matrix will be positive definite.
-A = np.array(nx.adjacency_matrix(G).todense())
-np.fill_diagonal(A, np.sum(np.abs(A), axis = 1)+0.1)
-
-# Copy the adjacency matrix, and remove some edges for that graph, note that the seed is assumed to be 42 when G was constructed
-A_s = A.copy()
-A_s[7,4] = 0
-A_s[4,7] = 0
-A_s[5,2] = 0
-A_s[2,5] = 0
-
-
-# Simulate random variables one has A as its precision and one has A_s (the sparse copy of A) as its precision matrix.
-# Note the precision matrix is the inverse covariance.
-X1 = np.random.multivariate_normal(np.zeros(11),np.linalg.inv(A), size = 10000)
-X2 = np.random.multivariate_normal(np.zeros(11),np.linalg.inv(A_s), size = 10000)
-```
-    
-
-Input the two samples X1 and X2 to the class method estimate_graphs. Which estimates graphs according to a window size. The best estimation is selected via the EBIC criterion.
-
-
-```python
-# window size = 200 so 10000/200 = 50 graphs in each sample. (200 observations were used to estimate each graph.)
-# Nonparanormal, should the nonparanormal transformation be performed on the data matrices?
-# Scale should the data be scaled.
-# Random Walk
-MMD_out = GTST.MMD()
-MMD_out.estimate_graphs(X1,X2,window_size=200, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False)
-MMD_out.fit( kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 5, c = 0.1, edge_attr = 'weight')
-print(MMD_out.p_values)
-
-
-```
-
-    Using weight as edge attributes
-       
-
-    {'MMD_u': 0.001}
-    
-
-
-```python
-# We can set node labels as degree (or define our own labelling, see below)
-MMD_out = GTST.MMD()
-kernel = [{"name": "weisfeiler_lehman", "n_iter": 4}, {"name": "vertex_histogram"}]
-MMD_out.estimate_graphs(X1,X2,window_size=200, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False, set_labels="degree")
-MMD_out.fit( kernel = kernel, mmd_estimators = 'MMD_u',  edge_attr = 'weight')
-print(MMD_out.p_values)
-```
-
-    Using weight as edge attributes
-    Using label as node labels
-    label
-    {'MMD_u': 0.002}
-    
-
-Plot some estimated graphs and compare to the true graphs.
-
-
-```python
-np.fill_diagonal(A_s,0)
-fig, ax = plt.subplots(2,2,figsize = (10,10))
-pos = nx.kamada_kawai_layout(G, weight = None)
-nx.draw(G, pos = pos, ax = ax[0,0])
-nx.draw(nx.from_numpy_array(A_s), pos = pos, ax = ax[0,1])
-nx.draw(MMD_out.G1[3], pos = pos, ax = ax[1,0])  # select graph number 3 in sample 1
-nx.draw(MMD_out.G2[3], pos = pos, ax = ax[1,1])  # select graph number 3 in sample 2
-ax[0,0].set_title("Sample 1 true precision structure")
-ax[0,1].set_title("Sample 2 true precision structure")
-ax[1,0].set_title("One estimated precision structure from sample 1")
-ax[1,1].set_title("One estimated precision structure from sample 2")
-```
-
-
-
-
-    Text(0.5, 1.0, 'One estimated precision structure from sample 2')
-
-
-
-
-    
-![png](README_files/README_46_1.png)
-    
-
-
-### Two data matrices same structure with different attributes
-It is possible to estimate the graphs beforehand and apply a function to get node attributes
-
-
-```python
-# Generate random samples that have the same underlying precision matrix/graph, but the node has different mean.
-
-G = nx.fast_gnp_random_graph(11, 0.25, seed = 42)
-assert nx.is_connected(G)
-
-for e in G.edges():
-    if np.random.uniform() <0.1:
-        w = np.random.uniform(low = 0.1, high = 0.3)
-        G.edges[e[0], e[1]]['weight'] = -w
-    else:
-        w = np.random.uniform(low = 0.1, high = 0.3)
-        G.edges[e[0], e[1]]['weight'] = w
-
-A = np.array(nx.adjacency_matrix(G).todense())
-np.fill_diagonal(A, np.sum(np.abs(A), axis = 1)+0.1)
-
-
-X1 = np.random.multivariate_normal(np.zeros(11),np.linalg.inv(A), size = 10000)
-X2 = np.random.multivariate_normal(np.ones(11),np.linalg.inv(A), size = 10000)
-```
-
-    
-
-
-```python
-# Random Walk, with attributes, should reject. , the class will use the node label name 'attr'
-# Define attribute function that sets the mean as the node attribute. 
-# Note the window size is 400 so there will be 400 observations that are used to estimate each graph/node attribute.
-def attr_function(X):
-    return np.expand_dims(np.mean(X,axis = 0),axis=1)
-
-MMD_out = GTST.MMD()
-MMD_out.estimate_graphs(X1,X2,window_size=400, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False, set_attributes = attr_function)
-MMD_out.fit( kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 5, c = 0.1, edge_attr = 'weight', node_attr = 'attr')
-print(MMD_out.p_values)
-```
-
-    Using weight as edge attributes
-    Using attr as node attributes
-        
-
-    {'MMD_u': 0.0}
-    
-
-
-```python
-# If we do not give attributes, the test should not be rejected reject as underlying the precision matrices are the same
-MMD_out_no_attr = GTST.MMD()
-MMD_out_no_attr.fit(G1= MMD_out.G1, G2 = MMD_out.G2, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 5, c = 0.1, edge_attr = 'weight')
-print(MMD_out_no_attr.p_values)
-```
-
-    Using weight as edge attributes
-    {'MMD_u': 0.993}
-    
-
-
-```python
-# We can also try to make a label function, which has to be a dictionary, the class will use the node label name 'label'
-# Note we label the nodes with the rounded mean
-def label_function(X):
-    m = np.mean(X,axis = 0)
-    return {i:str(np.round(m[i],1)) for i in range(len(m))}
-
-kernel = [{"name": "weisfeiler_lehman", "n_iter": 2}, {"name": "vertex_histogram"}]
-MMD_out = GTST.MMD()
-MMD_out.estimate_graphs(X1,X2,window_size=400, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False, set_labels= label_function)
-MMD_out.fit(kernel = kernel, mmd_estimators = 'MMD_u', node_label = 'label')
-print(MMD_out.p_values)
-```
-
-    Using label as node labels
-    label
-    {'MMD_u': 0.0}
-    
-
-
-```python
-# We can also define labels using a dict
-# '1' for sample 1, '2' for sample 2. Graph nr. j gets the list ['a']*6 + ['b']*5
-# meaning the first 6 nodes will be labelled 'a' and the last 5 nodes will be labelled 'b' for sample 1 but
-# the first 4 nodes will be labelled 'a' and the last 7 nodes will be labelled 'b' for sample 2
-label_dict = {'1':{j:i for j,i in enumerate(['a']*6 + ['b']*5)}, 
-              '2':{j:i for j,i in enumerate(['a']*4 + ['b']*7)}}
-kernel = [{"name": "weisfeiler_lehman", "n_iter": 2}, {"name": "vertex_histogram"}]
-MMD_out = GTST.MMD()
-MMD_out.estimate_graphs(X1,X2,window_size=400, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False, set_labels= label_dict)
-MMD_out.fit(kernel = kernel, mmd_estimators = 'MMD_u', node_label = 'label')
-print(MMD_out.p_values)
-```
-
-    Using label as node labels
-    label
-    {'MMD_u': 0.0}
-    
+Metadata-Version: 2.1
+Name: GTST
+Version: 0.0.6
+Summary: A package for comparing two samples of graphs
+Home-page: https://github.com/ragnarlevi/GTST
+Author: Ragnar Leví Guðmundarson
+Author-email: rlg2000@hw.ac.uk
+License: MIT
+Project-URL: Bug Tracker, https://github.com/ragnarlevi/GTST/issues
+Keywords: graph two sample testing,MMD,graph kernel
+Platform: unix
+Platform: linux
+Platform: osx
+Platform: cygwin
+Platform: win32
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
+![Tests](https://github.com/ragnarlevi/GTST/actions/workflows/tests.yml/badge.svg)
+[![Coverage Status](https://coveralls.io/repos/github/ragnarlevi/GTST/badge.svg?branch=test)](https://coveralls.io/github/ragnarlevi/GTST?branch=test)
+
+# GTST
+
+
+## What is this package for?
+
+This package contains code to perform kernel two-sample hypothesis testing on samples of graphs. The code additionally allows for the estimation of graphs from a real data matrix. Below one can find a description of the various function inputs available and examples of different use cases this package offers.
+
+
+## How to install
+
+<code>pip install GTST</code>
+
+Note that if one wants to use Grakel kernels then the Grakel package has to be installed via  <code>pip install grakel</code>.
+
+
+## Function Inputs
+
+<code>GTST.MMD</code> is the main function used. If the user already has samples of graphs where each sample is a list of networkx graph objects then the user can use the <code>fit</code> method to perform the hypothesis test.
+
+* **kernel**: list, str, np.array. If str then one of the kernels provided by the MMDGraph: RW_ARKU_plus, RW_ARKU, RW_ARKU_edge, RW_ARKL, GNTK, WWL, DK. If list then a GraKel kernel is used meaning the list should be formatted as one would do for the GraKel package. If np.array then a pre-calculated kernel is used.
+* **mmd_estimators**:str or list of strings, example MMD_u, MMD_b, MONK, MMD_l.
+
+The fit method additionally takes in additional parameters that are used by the kernel functions or the bootstrap function, such as:
+
+* **edge_attr**: Edge attribute name, if any.
+* **node_attr**: Node attribute name, if any.
+* **node_label**: Node label name, if any.
+* **edge_label**: Edge label name, if any.
+* **Q**: int, number of partitions for the MONK estimator.
+* **B**: int, number of bootstraps for p-value estimation.
+* **B**: int, number of bootstraps for p-value estimation.
+
+The RW kernels take:
+* **r**: int, number of eigenvalues.
+* **c**: float, discount constant.
+* **normalize**:bool, normalize kernel matrix?
+
+The GNTK kernel takes:
+* **num_layers**: int, number of layers in the neural networks (including the input layer)
+* **num_mlp_layers**:int, number of MLP layers
+* **jk**: a bool variable indicating whether to add jumping knowledge
+* **scale**:str, the scale used aggregate neighbours [uniform, degree]
+* **normalize**:bool, normalize kernel matrix?
+
+The WWL kernel uses:
+* **discount**: float, discount
+* **h**: int, number of WL iterations:
+* **sinkhorn**:bool, should the Wasserstein calculation be sped up and approximated?
+* **sinkhorn_lambda**: float, regularization term >0.
+* **normalize**: bool, normalize kernel?
+
+The DK kernel uses:
+* **type**: str, 'wl', 'sp'. 
+* **wl_it**: int, number of WL iterations (only used if type = wl)
+* **opt_type**: str, if opt_type = 'word2vec' then a similarity matrix is estimated using gensim which needs to be installed, If None the similarity matrix is just the frequency.
+* **vector_size**: int, the dimensionality of the word vectors. Only used if opt\_type = 'word2vec'.
+* **window**: int, the maximum distance between the current and predicted word within a sentence.  Only used if opt\_type = 'word2vec'.
+* **min_count**: int, Ignores all words with total frequency lower than this. Might have to be set to zero for the estimation to work.  Only used if opt\_type = 'word2vec'.
+* **node_label**: str, name of node labels.
+* **workers**: int, Use these many worker threads to train the model (=faster training with multicore machines).  Only used if opt\_type = 'word2vec'.
+* **normalize**: bool, normalize kernel?
+
+
+If the user has data matrices then the method <code>estimate_graphs</code> can be used beforehand to estimate graph samples using sklearn graphical lasso the inputs are:
+
+* **X1,X2**: two numpy arrays.
+* **window\_size**: an integer that controls how many samples are used to estimate each graph. That is window_size = 50, which means that the first 50 samples are used to estimate the first graph, the next 50 graphs are used to estimate the second and so on. If the window size is not divisible by the total length of the data arrays then the remainder will be skipped.
+* **alpha**: float, Regularization parameters in a list or a single float. If a list then EBIC will be used to select the best graph.
+* **beta**: float. EBIC hyperparameter.
+* **nonparanormal**: bool, should data be nonparanormally transformed?
+* **scale** bool , should data be scaled?
+* **set_attributes**: function or None, set attribute of nodes. The function should take numpy array  (which will be a submatrix of X1,X2) as input and output attributes for each node/parameter, used as an attribute for a graph kernel. See an example in usage below.
+* **set_labels**: function, str, dict or None. If a function should take networkx graph as input and output labels for each node/parameter.  Should return a dict {node_i:label,..}. 
+If dict, then should be: dict['1'] = dictionary with label for each node in sample 1 ({node:label}),dict['2'] = dictionary with label for each node in sample 2 ({node:label})
+If string = 'degree' then nodes will be labelled with degree. If None no labelling.
+
+After the estimate_graphs procedure has been run then the user should run <code>fit</code> to perform the hypothesis test, but be sure to leave G1 = None and G2= None.
+
+
+
+
+## Usage
+
+We will go through multiple scenarios: The case when the user has its own networkx graphs, when they are estimated from data matrices, using different kernels and using different MMD estimators.
+
+
+```python
+import numpy as np
+import networkx as nx
+import matplotlib.pyplot as plt
+import GTST
+```
+
+### Fit when H1 true, different edge probability
+
+In this example, we simulate binomial graphs assuming that the two samples have different edge probabilities. There will be 50 graphs in each sample and the number of nodes is 30 for all graphs. Sample 1 has an edge probability of 0.3 and sample 2 has an edge probability of 0.4. We will label each node with its corresponding degree so that graph kernels that assume labels can be used.
+
+Start by creating two samples of graphs:
+
+
+```python
+
+n1 = n2 = 50  # sample sizes
+# generate two samples
+g1 = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n1)]
+g2 = [nx.fast_gnp_random_graph(30,0.4) for _ in range(n2)]
+
+# Set node labels as the degree
+for j in range(len(g1)):
+    nx.set_node_attributes(g1[j],  {key: str(value) for key, value in dict(g1[j].degree).items()} , 'label')
+for j in range(len(g2)):
+    nx.set_node_attributes(g2[j], {key: str(value) for key, value in dict(g2[j].degree).items()}, 'label')
+
+```
+
+Perform the MMD test using various kernels. Note that the unbiases MMD estimator is used
+
+
+```python
+# Random Walk, r is number of eigen-pairs, c is the discount constant
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1, G2 = g2, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 6, c = 0.001)  
+print(f" RW_ARKU_plus {MMD_out.p_values}")
+```
+
+     RW_ARKU_plus {'MMD_u': 0.0}
+    
+
+
+```python
+# RW kernel with labels, Note that we input the label list (all node labels encountered in both graph samples)
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1, G2 = g2, kernel = 'RW_ARKL', mmd_estimators = 'MMD_u', r = 4, c = 1e-3,node_label = 'label',
+                                    unique_node_labels= set(np.concatenate([list(nx.get_node_attributes(g, 'label').values())for g in g1+g2])))
+print(f" RW_ARKL {MMD_out.p_values}")
+
+```
+
+    Using label as node labels
+     RW_ARKL {'MMD_u': 0.0}
+    
+
+
+```python
+# GNTK kernel,
+# num_layers is the number of layers in the neural network,
+# num_mlp_layers is the number of multi-layer perceptron layers
+# jk indicate whether to add jumping knowledge
+# scale how to aggregate neighbours uniform or degree.
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1, G2 = g2, kernel = 'GNTK', mmd_estimators = 'MMD_u', num_layers = 2, num_mlp_lauers = 2, jk = True, scale = 'uniform')
+print(f" GNTK {MMD_out.p_values}")
+```
+
+    100%|██████████| 5050/5050.0 [00:11<00:00, 438.12it/s]
+
+     GNTK {'MMD_u': 0.0}
+    
+
+    
+    
+
+
+```python
+# WWL kernel
+# discount is discount
+# h is the number of WL iterations
+# node_label is the name of node labels
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1, G2 = g2, kernel = 'WWL', mmd_estimators = 'MMD_u', discount = 0.1, h = 2, node_label = 'label')
+print(f" WWL {MMD_out.p_values}")
+```
+
+    Using label as node labels
+     WWL {'MMD_u': 0.0}
+    
+
+
+```python
+# Deep Kernel without the deepness
+# type is wl= wl closeness or sp: shortest path closeness
+# wl_it is the number of wl iterations, only applicable for wl.
+# no deepness in this case only a frequency similarity
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1, G2 = g2, kernel = 'DK', mmd_estimators = 'MMD_u', type = 'wl', wl_it = 4, node_label = 'label')
+print(f" ML DK {MMD_out.p_values}")
+```
+
+    Using label as node labels
+     ML DK {'MMD_u': 0.0}
+    
+
+
+```python
+
+# Deep kernel with deepness, the user has to install gensim, this might take some time, can try to increase the number of workers
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1, G2 = g2, kernel = 'DK', mmd_estimators = 'MMD_u', type = 'wl', wl_it = 4, opt_type = 'word2vec', node_label = 'label', workers = 10)
+print(f" Deep DK {MMD_out.p_values}")
+```
+
+    Using label as node labels
+     Deep DK {'MMD_u': 0.0}
+    
+
+
+```python
+# It is also possible to use the Grakel library
+kernel = [{"name": "weisfeiler_lehman", "n_iter": 1}, {"name": "vertex_histogram"}]
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1, G2 = g2, kernel = kernel, mmd_estimators = 'MMD_u', node_label = 'label')
+print(f" WL {MMD_out.p_values}")
+```
+
+    Using label as node labels
+    label
+     WL {'MMD_u': 0.0}
+    
+
+
+```python
+# Grakel propagation
+kernel = [ {"name":"propagation", 't_max':5, 'w':0.1, 'M':"TV"}]
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1, G2 = g2, kernel = kernel, mmd_estimators = 'MMD_u', node_label = 'label')
+print(f" propagation {MMD_out.p_values}")
+
+```
+
+    Using label as node labels
+    label
+     propagation {'MMD_u': 0.0}
+    
+
+### Using different MMD estimators
+
+It is also possible  to use other MMD estimators such as the biases, linear and robust.
+
+
+```python
+# Q is the number of partitions in the MONK estimator
+
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1, G2 = g2, kernel = 'RW_ARKU_plus', mmd_estimators = ['MMD_u', 'MMD_b', 'MMD_l', 'MONK_EST'], r = 2, c = 0.001, Q = 5)
+print(f" RW_ARKU_plus {MMD_out.p_values}")
+```
+   
+
+     RW_ARKU_plus {'MMD_u': 0.0, 'MMD_b': 0.0, 'MMD_l': 0.0, 'MONK_EST': 0.0}
+    
+
+### H1 true, Graphs with different weights
+
+It is possible to test graphs which are topologically the same but have different edge weights. Here there are 50 graphs in each sample and the number of nodes is 30 for all graphs. The edge probability is 0.3. We will label each node with its corresponding degree so that graph kernels that assume labels can be used.
+
+
+```python
+n1 = n2 = 100
+g1_weights = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n1)]  # sample 1
+g2_weights = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n2)]  # sample 2
+
+# For loops to label each node accoriding to its degree for the two samples.
+for j in range(len(g1_weights)):
+    nx.set_node_attributes(g1_weights[j],  {key: str(value) for key, value in dict(g1_weights[j].degree).items()} , 'label')
+for j in range(len(g2_weights)):
+    nx.set_node_attributes(g2_weights[j], {key: str(value) for key, value in dict(g2_weights[j].degree).items()}, 'label')
+
+
+# For loops to label each node according to its degree for the two samples.
+def edge_dist(loc, scale ):
+    from scipy.stats import uniform
+    return np.random.normal(loc = loc, scale = scale)# uniform.rvs(size=1,  loc = loc , scale = scale)[0]
+def add_weight(G, loc, scale ):
+    edge_w = dict()
+    for e in G.edges():
+        edge_w[e] = edge_dist(loc, scale)
+    return edge_w
+
+
+for G in g1_weights:
+    nx.set_edge_attributes(G, add_weight(G, loc = 0.5, scale = 1), "weight")
+for G in g2_weights:
+    nx.set_edge_attributes(G, add_weight(G, loc = 0.5, scale = 2), "weight")
+
+```
+
+
+```python
+# Random Walk
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1_weights, G2 = g2_weights, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 2, c = 0.001, edge_attr = 'weight')
+print(f" RW_ARKU_plus {MMD_out.p_values}")
+```
+
+    Using weight as edge attributes
+     RW_ARKU_plus {'MMD_u': 0.0}
+    
+
+Note that if we use a graph kernel that does not take edge weights into account, the test will not be rejected.
+
+
+```python
+# Random Walk weights ignored, should not reject
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1_weights, G2 = g2_weights, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 2, c = 0.001)
+print(f" RW_ARKU_plus no labels {MMD_out.p_values}")
+```
+
+     RW_ARKU_plus no labels {'MMD_u': 0.462}
+    
+
+
+```python
+# Grakel pyramid match kernel
+kernel = [{"name": "pyramid_match", "L": 6, "d":6, 'with_labels':False}]
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1_weights, G2 = g2_weights, kernel = kernel, mmd_estimators = 'MMD_u', edge_attr = 'weight')
+print(f" pyramid_match {MMD_out.p_values}")
+```
+
+    Using weight as edge attributes
+    None
+     pyramid_match {'MMD_u': 0.0}
+    
+
+
+```python
+# propagation, needs node attribute or label 
+kernel = [ {"name":"propagation", 't_max':5, 'w':0.05, 'M':"TV"}]
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1_weights, G2 = g2_weights, kernel = kernel, mmd_estimators = 'MMD_u', edge_attr = 'weight', node_label = 'label')
+print(f" propagation {MMD_out.p_values}")
+```
+
+    Using weight as edge attributes
+    Using label as node labels
+    label
+     propagation {'MMD_u': 0.0}
+    
+
+ ### H1 true different attributes
+
+Some kernels can be used to compare graphs with node attributes.
+
+
+```python
+
+n1 = n2 = 50
+g1_attr = [nx.fast_gnp_random_graph(30,0.2) for _ in range(n1)]  # sample 1
+g2_attr = [nx.fast_gnp_random_graph(30,0.2) for _ in range(n2)]  # sample 2
+# For loop for the two samples to add node attributes for each graph which have different normal distributions
+for j in range(len(g1_attr)):
+    nx.set_node_attributes(g1_attr[j], dict( ( (i, np.random.normal(loc = 0, scale = 0.1, size = (1,))) for i in range(len(g1_attr[j])) ) ), 'attr')
+for j in range(len(g2_attr)):
+    nx.set_node_attributes(g2_attr[j], dict( ( (i, np.random.normal(loc = 0.1, scale = 0.1, size = (1,))) for i in range(len(g2_attr[j])) ) ), 'attr')
+
+```
+
+
+```python
+# Random Walk with weights and node attributes
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1_attr, G2 = g2_attr, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 4, c = 0.01, node_attr = 'attr')
+print(f" RW_ARKU_plus {MMD_out.p_values}")
+```
+
+    Using attr as node attributes
+       
+
+     RW_ARKU_plus {'MMD_u': 0.0}
+    
+
+
+```python
+# GNTK with node attributes
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1_attr, G2 = g2_attr, kernel = 'GNTK', mmd_estimators = 'MMD_u', num_layers = 2, num_mlp_lauers = 2, jk = True, scale = 'uniform', node_attr = 'attr')
+print(f" GNTK {MMD_out.p_values}")
+```
+
+    Using attr as node attributes
+    
+
+    100%|██████████| 5050/5050.0 [00:04<00:00, 1246.33it/s]
+    
+
+     GNTK {'MMD_u': 0.0}
+    
+
+
+```python
+# Grakel propagation
+kernel = [ {"name":"propagation", 't_max':5, 'w':0.1, 'M':"L1",'with_attributes':True}]
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1_attr, G2 = g2_attr, kernel = kernel, mmd_estimators = 'MMD_u', discount = 0.1, h = 2, node_attr = 'attr')
+print(f" Propagation {MMD_out.p_values}")
+```
+
+    Using attr as node attributes
+    attr
+       
+
+     Propagation {'MMD_u': 0.0}
+    
+
+### Different edge labels
+
+The RW kernel can take different edge labels.
+
+
+```python
+n1 = n2 = 50
+g1_edge = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n1)]  # sample 1
+g2_edge = [nx.fast_gnp_random_graph(30,0.3) for _ in range(n2)]  # sample 2
+
+# For loop to label each edge either 'a' or 'b' the labelling probabilities are different for the two samples
+for j in range(len(g1_edge)):
+    nx.set_edge_attributes(g1_edge[j], {(i,k):np.random.choice(['a','b'], p = [0.6,0.4]) for i,k in g1_edge[j].edges }, 'edge_label')
+for j in range(len(g2_edge)):
+    nx.set_edge_attributes(g2_edge[j], {(i,k):np.random.choice(['a','b'], p = [0.7,0.3]) for i,k in g2_edge[j].edges }, 'edge_label')
+
+
+
+```
+
+
+```python
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1_edge, G2 = g2_edge, kernel = 'RW_ARKU_edge', mmd_estimators = 'MMD_u', r = 6, c = 0.0001,edge_label = 'edge_label',unique_edge_labels= ['a', 'b'])
+print(f" RW_ARKU_edge {MMD_out.p_values}")
+
+```
+
+    Using edge_label as edge labels
+     RW_ARKU_edge {'MMD_u': 0.0}
+    
+
+# Directed Graphs
+
+The RW kernel can take directed graphs
+
+
+```python
+n1 = n2 = 50
+g1_di = [nx.fast_gnp_random_graph(30,0.2) for _ in range(n1)]  # sample 1
+g2_di = [nx.fast_gnp_random_graph(30,0.2) for _ in range(n2)]  # sample 2
+
+# for loop for both samples to convert the networkx graph to a networkx directed graph object
+for j in range(len(g1_di)):
+    g1_di[j] = nx.DiGraph(g1_di[j])
+for j in range(len(g2_di)):
+    g2_di[j] = nx.DiGraph(g2_di[j])
+
+# for loop for both samples that removes edges with different removal probabilties between the two samples
+for j in range(len(g1_di)):
+    edges= list(g1_di[j].edges())
+    for e,u in edges:
+        if np.random.uniform() <0.3:
+            g1_di[j].remove_edge(e,u)
+for j in range(len(g2_di)):
+    edges= list(g2_di[j].edges())
+    for e,u in edges:
+        if np.random.uniform() <0.5:
+            g2_di[j].remove_edge(e,u)
+
+
+
+
+
+```
+
+
+```python
+MMD_out = GTST.MMD()
+MMD_out.fit(G1 = g1_di, G2 = g2_di, kernel = 'RW_ARKU', mmd_estimators = 'MMD_u', r = 4, c = 1e-3)
+print(f" RW_ARKU_edge {MMD_out.p_values}")
+
+```
+
+     RW_ARKU_edge {'MMD_u': 0.0}
+    
+
+### Two data matrices with different structure
+It is possible to estimate graphs from data matrices.
+
+
+```python
+G = nx.fast_gnp_random_graph(11, 0.25, seed=42)  # generate a random graph
+assert nx.is_connected(G)
+
+#  Add random weights to the graphs, either positive or negative
+for e in G.edges():
+    if np.random.uniform() <0.1:
+        w = np.random.uniform(low = 0.1, high = 0.3)
+        G.edges[e[0], e[1]]['weight'] = -w
+    else:
+        w = np.random.uniform(low = 0.1, high = 0.3)
+        G.edges[e[0], e[1]]['weight'] = w
+
+# Extract the adjacency matrix and fill the diagonal so that the resulting matrix will be positive definite.
+A = np.array(nx.adjacency_matrix(G).todense())
+np.fill_diagonal(A, np.sum(np.abs(A), axis = 1)+0.1)
+
+# Copy the adjacency matrix, and remove some edges for that graph, note that the seed is assumed to be 42 when G was constructed
+A_s = A.copy()
+A_s[7,4] = 0
+A_s[4,7] = 0
+A_s[5,2] = 0
+A_s[2,5] = 0
+
+
+# Simulate random variables one has A as its precision and one has A_s (the sparse copy of A) as its precision matrix.
+# Note the precision matrix is the inverse covariance.
+X1 = np.random.multivariate_normal(np.zeros(11),np.linalg.inv(A), size = 10000)
+X2 = np.random.multivariate_normal(np.zeros(11),np.linalg.inv(A_s), size = 10000)
+```
+    
+
+Input the two samples X1 and X2 to the class method estimate_graphs. Which estimates graphs according to a window size. The best estimation is selected via the EBIC criterion.
+
+
+```python
+# window size = 200 so 10000/200 = 50 graphs in each sample. (200 observations were used to estimate each graph.)
+# Nonparanormal, should the nonparanormal transformation be performed on the data matrices?
+# Scale should the data be scaled.
+# Random Walk
+MMD_out = GTST.MMD()
+MMD_out.estimate_graphs(X1,X2,window_size=200, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False)
+MMD_out.fit( kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 5, c = 0.1, edge_attr = 'weight')
+print(MMD_out.p_values)
+
+
+```
+
+    Using weight as edge attributes
+       
+
+    {'MMD_u': 0.001}
+    
+
+
+```python
+# We can set node labels as degree (or define our own labelling, see below)
+MMD_out = GTST.MMD()
+kernel = [{"name": "weisfeiler_lehman", "n_iter": 4}, {"name": "vertex_histogram"}]
+MMD_out.estimate_graphs(X1,X2,window_size=200, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False, set_labels="degree")
+MMD_out.fit( kernel = kernel, mmd_estimators = 'MMD_u',  edge_attr = 'weight')
+print(MMD_out.p_values)
+```
+
+    Using weight as edge attributes
+    Using label as node labels
+    label
+    {'MMD_u': 0.002}
+    
+
+Plot some estimated graphs and compare to the true graphs.
+
+
+```python
+np.fill_diagonal(A_s,0)
+fig, ax = plt.subplots(2,2,figsize = (10,10))
+pos = nx.kamada_kawai_layout(G, weight = None)
+nx.draw(G, pos = pos, ax = ax[0,0])
+nx.draw(nx.from_numpy_array(A_s), pos = pos, ax = ax[0,1])
+nx.draw(MMD_out.G1[3], pos = pos, ax = ax[1,0])  # select graph number 3 in sample 1
+nx.draw(MMD_out.G2[3], pos = pos, ax = ax[1,1])  # select graph number 3 in sample 2
+ax[0,0].set_title("Sample 1 true precision structure")
+ax[0,1].set_title("Sample 2 true precision structure")
+ax[1,0].set_title("One estimated precision structure from sample 1")
+ax[1,1].set_title("One estimated precision structure from sample 2")
+```
+
+
+
+
+    Text(0.5, 1.0, 'One estimated precision structure from sample 2')
+
+
+
+
+    
+![png](README_files/README_46_1.png)
+    
+
+
+### Two data matrices same structure with different attributes
+It is possible to estimate the graphs beforehand and apply a function to get node attributes
+
+
+```python
+# Generate random samples that have the same underlying precision matrix/graph, but the node has different mean.
+
+G = nx.fast_gnp_random_graph(11, 0.25, seed = 42)
+assert nx.is_connected(G)
+
+for e in G.edges():
+    if np.random.uniform() <0.1:
+        w = np.random.uniform(low = 0.1, high = 0.3)
+        G.edges[e[0], e[1]]['weight'] = -w
+    else:
+        w = np.random.uniform(low = 0.1, high = 0.3)
+        G.edges[e[0], e[1]]['weight'] = w
+
+A = np.array(nx.adjacency_matrix(G).todense())
+np.fill_diagonal(A, np.sum(np.abs(A), axis = 1)+0.1)
+
+
+X1 = np.random.multivariate_normal(np.zeros(11),np.linalg.inv(A), size = 10000)
+X2 = np.random.multivariate_normal(np.ones(11),np.linalg.inv(A), size = 10000)
+```
+
+    
+
+
+```python
+# Random Walk, with attributes, should reject. The class will use the node label name 'attr'
+# Define attribute function that sets the mean as the node attribute. 
+# Note the window size is 400 so there will be 400 observations that are used to estimate each graph/node attribute.
+def attr_function(X):
+    return np.expand_dims(np.mean(X,axis = 0),axis=1)
+
+MMD_out = GTST.MMD()
+MMD_out.estimate_graphs(X1,X2,window_size=400, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False, set_attributes = attr_function)
+MMD_out.fit( kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 5, c = 0.1, edge_attr = 'weight', node_attr = 'attr')
+print(MMD_out.p_values)
+```
+
+    Using weight as edge attributes
+    Using attr as node attributes
+        
+
+    {'MMD_u': 0.0}
+    
+
+
+```python
+# If we do not give attributes, the test should not be rejected as the underlying the precision matrices are the same
+MMD_out_no_attr = GTST.MMD()
+MMD_out_no_attr.fit(G1= MMD_out.G1, G2 = MMD_out.G2, kernel = 'RW_ARKU_plus', mmd_estimators = 'MMD_u', r = 5, c = 0.1, edge_attr = 'weight')
+print(MMD_out_no_attr.p_values)
+```
+
+    Using weight as edge attributes
+    {'MMD_u': 0.993}
+    
+
+
+```python
+# We can also try to make a label function, which has to be a dictionary, the class will use the node label name 'label'
+# Note we label the nodes with the rounded mean
+def label_function(X):
+    m = np.mean(X,axis = 0)
+    return {i:str(np.round(m[i],1)) for i in range(len(m))}
+
+kernel = [{"name": "weisfeiler_lehman", "n_iter": 2}, {"name": "vertex_histogram"}]
+MMD_out = GTST.MMD()
+MMD_out.estimate_graphs(X1,X2,window_size=400, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False, set_labels= label_function)
+MMD_out.fit(kernel = kernel, mmd_estimators = 'MMD_u', node_label = 'label')
+print(MMD_out.p_values)
+```
+
+    Using label as node labels
+    label
+    {'MMD_u': 0.0}
+    
+
+
+```python
+# We can also define labels using a dict
+# '1' for sample 1, '2' for sample 2. Graph nr. j gets the list ['a']*6 + ['b']*5
+# meaning the first 6 nodes will be labelled 'a' and the last 5 nodes will be labelled 'b' for sample 1 but
+# the first 4 nodes will be labelled 'a' and the last 7 nodes will be labelled 'b' for sample 2
+label_dict = {'1':{j:i for j,i in enumerate(['a']*6 + ['b']*5)}, 
+              '2':{j:i for j,i in enumerate(['a']*4 + ['b']*7)}}
+kernel = [{"name": "weisfeiler_lehman", "n_iter": 2}, {"name": "vertex_histogram"}]
+MMD_out = GTST.MMD()
+MMD_out.estimate_graphs(X1,X2,window_size=400, alpha = np.exp(np.linspace(-5,-2,100)),beta = 0.5, nonparanormal=False,scale = False, set_labels= label_dict)
+MMD_out.fit(kernel = kernel, mmd_estimators = 'MMD_u', node_label = 'label')
+print(MMD_out.p_values)
+```
+
+    Using label as node labels
+    label
+    {'MMD_u': 0.0}
+
```

