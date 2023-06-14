# Comparing `tmp/searchlogit-0.3.8.tar.gz` & `tmp/searchlogit-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchlogit-0.3.8.tar", last modified: Mon Apr 24 09:14:28 2023, max compression
+gzip compressed data, was "searchlogit-0.3.9.tar", last modified: Mon May 22 04:49:13 2023, max compression
```

## Comparing `searchlogit-0.3.8.tar` & `searchlogit-0.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:28.718192 searchlogit-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 09:14:15.000000 searchlogit-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-24 09:14:28.718192 searchlogit-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-24 09:14:15.000000 searchlogit-0.3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:28.714192 searchlogit-0.3.8/searchlogit/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/_choice_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/boxcox_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    50811 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/latent_class_mixed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/mixed_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)   169595 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:28.718192 searchlogit-0.3.8/searchlogit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 09:14:28.718192 searchlogit-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-24 09:14:15.000000 searchlogit-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:28.718192 searchlogit-0.3.8/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test__choice_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test__device.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test_latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test_mixed_logit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test_multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:49:13.974191 searchlogit-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 04:49:03.000000 searchlogit-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-05-22 04:49:13.974191 searchlogit-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-05-22 04:49:03.000000 searchlogit-0.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:49:13.974191 searchlogit-0.3.9/searchlogit/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 04:49:03.000000 searchlogit-0.3.9/searchlogit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-05-22 04:49:03.000000 searchlogit-0.3.9/searchlogit/_choice_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-22 04:49:03.000000 searchlogit-0.3.9/searchlogit/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-22 04:49:03.000000 searchlogit-0.3.9/searchlogit/boxcox_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50775 2023-05-22 04:49:03.000000 searchlogit-0.3.9/searchlogit/latent_class_mixed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-05-22 04:49:03.000000 searchlogit-0.3.9/searchlogit/latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60086 2023-05-22 04:49:03.000000 searchlogit-0.3.9/searchlogit/mixed_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-05-22 04:49:03.000000 searchlogit-0.3.9/searchlogit/multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170457 2023-05-22 04:49:03.000000 searchlogit-0.3.9/searchlogit/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:49:13.974191 searchlogit-0.3.9/searchlogit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-05-22 04:49:13.000000 searchlogit-0.3.9/searchlogit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-22 04:49:13.000000 searchlogit-0.3.9/searchlogit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 04:49:13.000000 searchlogit-0.3.9/searchlogit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 04:49:13.000000 searchlogit-0.3.9/searchlogit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 04:49:13.000000 searchlogit-0.3.9/searchlogit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 04:49:13.000000 searchlogit-0.3.9/searchlogit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 04:49:13.974191 searchlogit-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-22 04:49:03.000000 searchlogit-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:49:13.974191 searchlogit-0.3.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-05-22 04:49:03.000000 searchlogit-0.3.9/tests/test__choice_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-22 04:49:03.000000 searchlogit-0.3.9/tests/test__device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 04:49:03.000000 searchlogit-0.3.9/tests/test_latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-22 04:49:03.000000 searchlogit-0.3.9/tests/test_mixed_logit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-05-22 04:49:03.000000 searchlogit-0.3.9/tests/test_multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 04:49:03.000000 searchlogit-0.3.9/tests/test_search.py
```

### Comparing `searchlogit-0.3.8/LICENSE` & `searchlogit-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/PKG-INFO` & `searchlogit-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.8
+Version: 0.3.9
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.8/README.rst` & `searchlogit-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/searchlogit/_choice_model.py` & `searchlogit-0.3.9/searchlogit/_choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/searchlogit/_device.py` & `searchlogit-0.3.9/searchlogit/_device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/searchlogit/boxcox_functions.py` & `searchlogit-0.3.9/searchlogit/boxcox_functions.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/searchlogit/latent_class_mixed_model.py` & `searchlogit-0.3.9/searchlogit/latent_class_mixed_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1144,15 +1144,14 @@
         counter = 0
         for ii, param_spec in enumerate(self.class_params_spec):
             # count + add coeff_
             idx = counter + self._get_betas_length(0)
             class_betas.append(self.coeff_[counter:idx])
             counter = idx
 
-        class_thetas = np.array([])
         counter = 0
         for ii, param_spec in enumerate(self.member_params_spec):
             # count + add coeff_
             idx = counter + len(param_spec)
             class_betas.append(self.coeff_[counter:idx])
             counter = idx
```

### Comparing `searchlogit-0.3.8/searchlogit/latent_class_model.py` & `searchlogit-0.3.9/searchlogit/latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/searchlogit/mixed_logit.py` & `searchlogit-0.3.9/searchlogit/mixed_logit.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,20 +630,14 @@
 
             Xbr_trans = dev.cust_einsum('npjk,nkr -> npjr', Xrtrans_lmda, Brtrans)  # (N, P, J, R)
             # combining utilities
             V += Xbr_trans  # (N, P, J, R)
 
         #  Combine utilities of fixed and random variables
         # V[V > max_exp_val] = max_exp_val
-        # Exponent of the utility function for the logit formula
-        if avail is not None:
-            if self.panels is not None:
-                V = V*avail[:, :, :, None]  # Acommodate availablity of alts with panels
-            else:
-                V = V*avail[:, None, :, None]  # Acommodate availablity of alts.
 
         # max_exp_val = 1400
 
         # V[np.where(V > max_exp_val)] = max_exp_val
         # V[np.where(V < -max_exp_val)] = -max_exp_val
 
         # # if dev.using_gpu:
@@ -656,14 +650,21 @@
         #     V_logsumexp = dev.np.logaddexp.reduce(V, axis=2, keepdims=True)
 
         # p = np.exp(V - V_logsumexp)
         # Thresholds to avoid overflow warnings
         V[np.where(V > max_exp_val)] = max_exp_val
         V[np.where(V < -max_exp_val)] = -max_exp_val
         eV = dev.np.exp(V)
+        # Exponent of the utility function for the logit formula
+        if avail is not None:
+            if self.panels is not None:
+                eV = eV*avail[:, :, :, None]  # Acommodate availablity of alts with panels
+            else:
+                eV = eV*avail[:, None, :, None]  # Acommodate availablity of alts.
+
         sum_eV = dev.np.sum(eV, axis=2, keepdims=True)
         sum_eV[np.where(sum_eV < min_comp_val)] = min_comp_val
         p = np.divide(eV, sum_eV, out=np.zeros_like(eV))
         if self.save_fitted_params:
             self.p = p  # save
         # # temp_p = np.mean(np.mean(np.mean(p, axis=0), axis=0), axis=1)
         # if panel_info is not None:
@@ -1064,14 +1065,15 @@
                 g = np.transpose(np.transpose(g)*weights[:, 0])
             if weights.ndim == 3:  # (3 dim for panel data)
                 g = np.transpose(np.transpose(g)*weights[:, 0, 0])
         g = np.sum(g, axis=0)/n_batches  # (K, )
         # log-lik
         self.gtol_res = np.linalg.norm(g, ord=np.inf)
 
+        # print('g: ', g)
         # print('norm', np.linalg.norm(g, ord=np.inf))  # useful debugging gtol
 
         result = (-loglik)
 
         if self.grad:
             result = (-loglik, -g)
```

### Comparing `searchlogit-0.3.8/searchlogit/multinomial_logit.py` & `searchlogit-0.3.9/searchlogit/multinomial_logit.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
             self.Hinv = Hinv
 
         grad = np.sum(grad, axis=0, dtype=np.float64)
         self.gtol_res = np.linalg.norm(grad, ord=np.inf)
 
         result = (loglik)
         logger.debug('Norm: {}'.format(np.linalg.norm(grad, ord=np.inf)))
-        print('norm', np.linalg.norm(grad, ord=np.inf)) #  this is useful debug gtol
+        # print('norm', np.linalg.norm(grad, ord=np.inf)) #  this is useful debug gtol
 
         if self.grad:
             result = (-loglik, -grad)
             if self.hess:
                 result = (-loglik, -grad, Hinv)
 
         return result
```

### Comparing `searchlogit-0.3.8/searchlogit/search.py` & `searchlogit-0.3.9/searchlogit/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,18 +170,18 @@
 
     p_val : float, default=0.05
         P-value used to test for non-significance of model coefficients.
 
     chosen_alts_test: array-like, default=True
         Array of alts of each choice.
 
-    allow_random : bool, default=True  # TODO? temporary - another prespecified approach?
+    allow_latent_random : bool, default=True  # TODO? temporary - another prespecified approach?
         Allow random variables to be included in the model.
 
-    allow_bcvars : bool, default=True  # TODO? temporary - another prespecified approach?
+    allow_latent_bcvars : bool, default=True  # TODO? temporary - another prespecified approach?
         Allow transformation variables to be included in the model.
 
     base_alt : int, float, or str, default=None
         Base alternative.
     """
     def __init__(self, df, varnames, df_test=None, dist=None, code_name="search",
                  avail=None, test_av=None, avail_latent=None,
@@ -197,15 +197,17 @@
                  ftol_lccmm=1e-4,
                  latent_class=False, num_classes=2, maxiter=200, n_draws=1000,
                  multi_objective=False,
                  multi_objective_variable='BIC',
                  p_val=0.05,
                  chosen_alts_test=None,
                  test_weight_var=None,
-                 allow_random=True, allow_bcvars=True,
+                 allow_latent_random=True,  # TODO: latent only?
+                 allow_latent_bcvars=True,
+                 allow_latent_corvars=True,
                  intercept_opts=None, base_alt=None,
                  val_share=0.25,
                  logger_level=None,
                  seed=None):
         """Initialise the search class.
 
         """
@@ -354,16 +356,17 @@
         self.test_avail_latent = test_avail_latent
         self.test_weight_var = test_weight_var
         self.test_choice_id = test_choice_id
         self.test_ind_id = test_ind_id
         self.test_alt_var = test_alt_var
         self.test_choice_var = test_choice_var
 
-        self.allow_random = allow_random
-        self.allow_bcvars = allow_bcvars
+        self.allow_latent_random = allow_latent_random
+        self.allow_latent_bcvars = allow_latent_bcvars
+        self.allow_latent_corvars = allow_latent_corvars
 
         self.intercept_opts = intercept_opts
         self.base_alt = base_alt
 
         if chosen_alts_test is None and self.multi_objective:
             try:
                 chosen_alts_test = test_alt_var[test_choice_var == 1]
@@ -622,20 +625,20 @@
                 tmp_class_spec = np.array([])
                 for var in class_vars:
                     # NOTE: 0.8 is arbitrary here... kept high...
                     if self.random_state.uniform() < 0.8:  # prob of accepting asvar
                         tmp_class_spec = np.append(tmp_class_spec, var)
                 class_params_spec[i] = np.sort(tmp_class_spec)
 
+            tmp_member_spec = np.array([])
+            for var in member_vars:
+                # NOTE: 0.8 is arbitrary here... kept high...
+                if self.random_state.uniform() < 0.8:  # 0.5 prob of accepting asvar
+                    tmp_member_spec = np.append(tmp_member_spec, var)
             for i in range(self.num_classes-1):
-                tmp_member_spec = np.array([])
-                for var in member_vars:
-                    # NOTE: 0.8 is arbitrary here... kept high...
-                    if self.random_state.uniform() < 0.8:  # 0.5 prob of accepting asvar
-                        tmp_member_spec = np.append(tmp_member_spec, var)
                 member_params_spec[i] = np.sort(tmp_member_spec)
 
         # Determine random coefficient distributions for selected variables
         r_dist = []
         avail_rvar = [var for var in asvars if var in self.avail_rvars]
 
         if class_params_spec is not None:
@@ -651,25 +654,25 @@
         rand_vars = {k: v for k, v in rvars.items() if v != "f" and k in asvars}
         r_dis = [dis for dis in self.dist if dis != "f"]
         for var in self.ps_corvars:
             if var in asvars and var not in rand_vars.keys():
                 rand_vars.update({var: self.random_state.choice(r_dis)})
 
         rand_vars = dict(sorted(rand_vars.items()))  # sort randvars
-        if not self.allow_random:  # additional safety point
+        if not self.avail_rvars:  # additional safety point
             rand_vars = {}
 
         # Determine if the model should include Box-Cox transformations
         if self.ps_bctrans is None:
             bctrans = self.random_state.rand() < 0.5
         else:
             bctrans = self.ps_bctrans
 
         # Randomly select variables for Box-Cox transformations and include prespecified ones
-        if bctrans and self.allow_bcvars:
+        if bctrans and self.allow_latent_bcvars:
             ind_availbcvar = []
             for i in range(len(self.avail_bcvars)):
                 ind_availbcvar.append(self.random_state.randint(2))
             bcvar_select_pos = [i for i, x in enumerate(ind_availbcvar) if x == 1]
             bcvars = [var for var in self.avail_bcvars if self.avail_bcvars.index(var) in bcvar_select_pos]
             bcvars.extend(self.ps_bcvars)
             bc_vars = [var for var in bcvars if var in asvars and var not in self.ps_corvars]
@@ -756,15 +759,15 @@
         """
         Estimates multinomial model for the generated solution.
 
         Parameters
         ----------
         sol : Solution
             Solution object containing the model specification.
-        
+
         Returns
         """
         as_vars = sol['asvars']
         is_vars = sol['isvars']
         asc_ind = sol['asc_ind']
         bcvars = sol['bcvars']
         neg_bcvar = [x for x in bcvars if any(self.df[x].values < 0)]
@@ -1464,20 +1467,31 @@
                                             bcvars = [bc_var for bc_var in bcvars if bc_var not in class_param]
                                         i += 1
                                 tmp_class_params = np.delete(tmp_class_params, delete_idx)
                                 rem_class_params_spec[ii] = tmp_class_params
 
                         if self.latent_class:
                             i = 0
-                            # rem_member_params_spec = member_params_spec.copy()
+                            # pass through to record all significant params
+                            for ii, member_params in enumerate(member_params_spec):
+                                tmp_member_params = member_params.copy()
+                                # delete_idx = []
+                                significant_params = []
+                                for jj, member_param in enumerate(member_params):
+                                    if sig_member[i] < self.p_val:
+                                        significant_params.append(member_param)
+                                    i += 1
+
+                            # delete variables not significant for any class
+                            i = 0
                             for ii, member_params in enumerate(member_params_spec):
                                 tmp_member_params = member_params.copy()
                                 delete_idx = []
-                                for jj, _ in enumerate(member_params):
-                                    if sig_member[i] > self.p_val:
+                                for jj, member_param in enumerate(member_params):
+                                    if member_param not in significant_params:
                                         delete_idx.append(jj)
                                     i += 1
                                 tmp_member_params = np.delete(tmp_member_params, delete_idx)
                                 rem_member_params_spec[ii] = tmp_member_params
 
                         logger.debug("rem_class_params_spec: {}".format(str(rem_class_params_spec)))
                         logger.debug("rem_member_params_spec: {}".format(str(rem_member_params_spec)))
@@ -1835,23 +1849,23 @@
                 if self.ps_intercept is None:
                     opp_sol['asc_ind'] = not sol['asc_ind']
 
             opp_sol['randvars'] = {k: self.random_state.choice(self.dist)
                                    for k in opp_sol['randvars']
                                    if k in opp_sol['asvars']}
 
-            if not self.allow_random:
+            if not self.avail_rvars:
                 opp_sol['randvars'] = {}
 
             opp_sol['corvars'] = [corvar for corvar in opp_sol['corvars'] if corvar in opp_sol['randvars']]
 
             opp_sol['bcvars'] = [bcvar for bcvar in opp_sol['bcvars'] if bcvar in opp_sol['asvars']
                                                                       and bcvar not in opp_sol['corvars']]
 
-            if not self.allow_bcvars:
+            if not self.avail_bcvars:
                 opp_sol['bcvars'] = []
 
             if opp_sol['class_params_spec'] is not None and sol['class_params_spec'] is not None:
                 # remove randvars not in class params
                 for ii, class_param in enumerate(opp_sol['class_params_spec']):
                     opp_sol['class_params_spec'][ii] = np.array([param_i for param_i in class_param
                                                         if param_i not in sol['class_params_spec'][ii]])
@@ -1992,15 +2006,15 @@
                                                        self.trans_asvars,
                                                        self.asvarnames)
             solution['asvars'] = sorted(list(set(solution['asvars'])))
             logger.debug("new sol: {}".format(str(solution['asvars'])))
 
             # randvar logic for selected asvar
             r_vars = {}
-            if self.allow_random:
+            if self.avail_rvars:
                 for i in solution['asvars']:
                     if i in solution['randvars'].keys():
                         r_vars.update({k: v for k, v in solution['randvars'].items()
                                        if k == i})
                         logger.debug("r_vars: {}".format(r_vars))
                     else:
                         if i in self.ps_randvars.keys():
@@ -2042,15 +2056,15 @@
         Inputs: solution list containing all features generated from harmony consideration
         """
         if self.ps_bctrans is None:
             bctrans = bool(self.random_state.randint(2, size=1))
         else:
             bctrans = self.ps_bctrans
 
-        if bctrans and self.allow_bcvars:
+        if bctrans and self.avail_bcvars:
             select_new_bcvars_index = self.random_state.choice([0, 1],
                                                        size=len(solution['asvars']),
                                                        p=[1-PAR_itr, PAR_itr])
             new_bcvar = [i for (i, v) in zip(solution['asvars'],
                                              select_new_bcvars_index) if v]
             solution['bcvars'] = sorted(list(set(solution['bcvars']).union(new_bcvar)))
             solution['bcvars'] = [var for var in solution['bcvars'] if var
@@ -2062,15 +2076,15 @@
                 solution['bcvars'] = [var for var in solution['bcvars']
                                       if var in class_params]
         else:
             solution['bcvars'] = []
 
         if not solution['corvars']:
             solution['corvars'] = []
-        if self.allow_bcvars:
+        if self.avail_bcvars:
             # Remove corvars that are now included in bcvars
             solution['corvars'] = [var for var in solution['corvars'] if var not in solution['bcvars']]
         return solution
 
     def add_new_randfeature(self, solution):
         """
         Randomly selects randvar which is not already in solution
@@ -2145,29 +2159,24 @@
         """
         Randomly selects variables to be added to member_params_spec, which is not already in solution
         Inputs: solution list containing all features generated from harmony consideration
         """
         member_params_spec = solution['member_params_spec']
         member_params_spec_new = copy.deepcopy(member_params_spec)
         all_vars = self.isvarnames + ['_inter']
-        # for ii, class_i in enumerate(member_params_spec):
-        ii = self.random_state.randint(0, len(member_params_spec))
-        member_i = member_params_spec_new[ii]
 
+        curr_member_params = member_params_spec[0]  # now all should be same
+        new_params = np.array([var for var in all_vars if var not in curr_member_params])
         new_param = []
-        if len(member_i) > 0:
-            new_params = np.array([var for var in all_vars if var not in member_i])
-            new_member_spec = member_i
-            if len(new_params) > 0:
-                new_param = self.random_state.choice(new_params, 1)
-                new_member_spec = np.sort(np.append(member_i, new_param))
+        if len(new_params) > 0:
+            new_param = self.random_state.choice(new_params, 1)
+        for ii, member_params in enumerate(member_params_spec):
+            new_member_spec = np.sort(np.append(member_params, new_param))
 
             member_params_spec_new[ii] = new_member_spec
-        else:
-            member_params_spec_new[ii] = member_i
 
         solution['member_params_spec'] = member_params_spec_new
         if new_param not in solution['isvars']:
             solution['isvars'] = sorted(list(set(solution['isvars']).union(new_param)))
 
         return solution
 
@@ -2277,20 +2286,20 @@
         """
         Randomly excludes class_param_spec feature from solution generated from harmony consideration.
         Inputs: solution list containing all features
         """
         member_params_spec = copy.deepcopy(solution['member_params_spec'])
         rem_member_param = []
         if solution['member_params_spec'] is not None:
-            ii = self.random_state.randint(0, len(member_params_spec))
-            member_i = member_params_spec[ii]
-            if len(member_i) > 1:
-                rem_member_param = self.random_state.choice(member_i)
-                tmp_member_i = [var for var in member_i if var not in rem_member_param]
-                member_params_spec[ii] = np.array(tmp_member_i)
+            curr_member_params = member_params_spec[0]
+            if len(curr_member_params) > 1:
+                rem_member_param = self.random_state.choice(curr_member_params)
+                for ii, member_params in enumerate(member_params_spec):
+                    tmp_member_ii = [var for var in member_params if var not in rem_member_param]
+                    member_params_spec[ii] = np.array(tmp_member_ii)
         solution['member_params_spec'] = member_params_spec
         if rem_member_param not in np.concatenate(member_params_spec):
             solution['isvars'] = [var for var in solution['isvars']
                                   if var != rem_member_param]
 
         return solution
 
@@ -2577,15 +2586,15 @@
         best_asvars, best_isvars, best_randvars, best_bcvars, best_corvars, \
             asc_ind, best_class_params_spec, best_member_params_spec = self.best_features(improved_harmony)
         solution = Solution(asvars=best_asvars, isvars=best_isvars,
                             randvars=best_randvars, bcvars=best_bcvars,
                             corvars=best_corvars, asc_ind=asc_ind,
                             class_params_spec=best_class_params_spec,
                             member_params_spec=best_member_params_spec)
-        if self.allow_bcvars:
+        if self.avail_bcvars:
             if self.random_state.rand() < 0.5:
                 solution_6 = self.remove_bcfeature(solution)
             else:
                 solution_6 = self.add_new_bcfeature(solution, PAR_itr)
             improved_harmony, current_sol = self.assess_sol(solution_6,
                                                             improved_harmony)
             logger.debug("sol after local search step 6: {}".format(str(improved_harmony[0])))
@@ -2594,15 +2603,15 @@
             asc_ind, best_class_params_spec, best_member_params_spec = self.best_features(improved_harmony)
         solution = Solution(asvars=best_asvars, isvars=best_isvars,
                             randvars=best_randvars, bcvars=best_bcvars,
                             corvars=best_corvars, asc_ind=asc_ind,
                             class_params_spec=best_class_params_spec,
                             member_params_spec=best_member_params_spec)
 
-        if self.allow_random:
+        if self.avail_rvars:
             if self.random_state.rand() < 0.5:
                 solution_7 = self.remove_corfeature(solution)
             else:
                 solution_7 = self.add_new_corfeature(solution)
 
             improved_harmony, current_sol = self.assess_sol(solution_7,
                                                             improved_harmony)
@@ -2667,15 +2676,15 @@
         improved_harmony, current_sol = self.assess_sol(solution, improved_harmony)
         logger.debug("sol after local search step 9: {}".format(str(improved_harmony[0])))
 
         # check if having all the variables transformed has an improvement in BIC
         best_asvars, best_isvars, best_randvars, best_bcvars, best_corvars, \
             asc_ind, best_class_params_spec, best_member_params_spec = self.best_features(improved_harmony)
         if self.ps_bctrans is None or self.ps_bctrans:
-            best_bcvars = [var for var in best_asvars if var not in self.ps_corvars]
+            best_bcvars = [var for var in best_asvars if var not in self.ps_corvars]  # TODO: DEBUG HERE
         else:
             best_bcvars = []
         if self.ps_cor is None or self.ps_cor:
             best_corvars = [var for var in best_randvars.keys()
                             if var not in best_bcvars]
         else:
             best_corvars = []
@@ -2901,16 +2910,16 @@
         ps_corvar_ind = [0] * len(asvarnames)
 
         # prespecified interactions
         return (psasvar_ind, psisvar_ind, pspecdist_ind, ps_bcvar_ind,
                 ps_corvar_ind)
 
     def run_search(self, HMS=10, HMCR_min=0.6, HMCR_max=0.9, PAR_max=0.85,
-                   PAR_min=0.3, itr_max=30, v=0.8, threshold=15, generate_plots=True,
-                   existing_sols=None):
+                   PAR_min=0.3, itr_max=30, v=0.8, threshold=15,
+                   generate_plots=True, existing_sols=None):
         """Run the IGHS algorithm
 
         Parameters
         ----------
             HMS : int, optional
                 Harmony memory size. The number of models randomly
                 generated when initialising the search. Defaults to 10.
@@ -2948,28 +2957,31 @@
             self.avail_features()
 
         self.avail_asvars = avail_asvars
         self.avail_isvars = avail_isvars
 
         self.generate_plots = generate_plots
 
-        if not self.allow_random:
-            avail_rvars = []
         self.avail_rvars = avail_rvars
-        if not self.allow_bcvars:
-            avail_bcvars = []
         self.avail_bcvars = avail_bcvars
         self.avail_corvars = avail_corvars
 
+        if self.latent_class:
+            if not self.allow_latent_random:
+                self.avail_rvars = []
+            if not self.allow_latent_corvars:
+                self.avail_corvars = []
+            if not self.allow_latent_bcvars:
+                self.avail_bcvars = []
+
         asvars_new = self.df_coeff_col(self.asvarnames)
 
         asvars_new = self.remove_redundant_asvars(asvars_new,
                                                   self.trans_asvars,
                                                   self.asvarnames)
-        # self.generate_sol()
 
         existing_HMS = []
         if existing_sols is not None:
             for sol in existing_sols:
                 new_sol = copy.deepcopy(sol)
                 new_sol = self.increase_sol_by_one_class(new_sol)
                 new_sol.pop('class_num')
```

### Comparing `searchlogit-0.3.8/searchlogit.egg-info/PKG-INFO` & `searchlogit-0.3.9/searchlogit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.8
+Version: 0.3.9
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.8/searchlogit.egg-info/SOURCES.txt` & `searchlogit-0.3.9/searchlogit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/setup.py` & `searchlogit-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 
 with codecs.open("README.rst", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='searchlogit',
-                 version='0.3.8',
+                 version='0.3.9',
                  description='Extensions for a Python package for \
                               GPU-accelerated estimation of mixed logit models.',
                  long_description=long_description,
                  long_description_content_type="text/x-rst",
                  url='https://github.com/RyanJafefKelly/searchlogit',
                  author='Ryan Kelly, Prithvi Beeramoole and Alexander Paz',
                  author_email='ryan@kiiii.com',
```

### Comparing `searchlogit-0.3.8/tests/test__choice_model.py` & `searchlogit-0.3.9/tests/test__choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/tests/test__device.py` & `searchlogit-0.3.9/tests/test__device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/tests/test_latent_class_model.py` & `searchlogit-0.3.9/tests/test_latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/tests/test_mixed_logit.py` & `searchlogit-0.3.9/tests/test_mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.8/tests/test_multinomial_logit.py` & `searchlogit-0.3.9/tests/test_multinomial_logit.py`

 * *Files identical despite different names*

