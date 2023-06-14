# Comparing `tmp/torchbones-1.2.5.tar.gz` & `tmp/torchbones-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.2.5.tar", last modified: Tue Jun 13 21:35:48 2023, max compression
+gzip compressed data, was "torchbones-1.2.6.tar", last modified: Wed Jun 14 16:04:47 2023, max compression
```

## Comparing `torchbones-1.2.5.tar` & `torchbones-1.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-13 21:35:48.244228 torchbones-1.2.5/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-13 21:35:48.244228 torchbones-1.2.5/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-13 21:35:48.244228 torchbones-1.2.5/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-13 21:35:21.000000 torchbones-1.2.5/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-13 21:35:48.244228 torchbones-1.2.5/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.5/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    20117 2023-06-13 21:35:23.000000 torchbones-1.2.5/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-13 21:35:48.244228 torchbones-1.2.5/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-13 21:35:48.000000 torchbones-1.2.5/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-13 21:35:48.000000 torchbones-1.2.5/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-13 21:35:48.000000 torchbones-1.2.5/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-13 21:35:48.000000 torchbones-1.2.5/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-13 21:35:48.000000 torchbones-1.2.5/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-14 16:04:47.652368 torchbones-1.2.6/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-14 16:04:47.652368 torchbones-1.2.6/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-14 16:04:47.652368 torchbones-1.2.6/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-14 16:04:43.000000 torchbones-1.2.6/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-14 16:04:47.642368 torchbones-1.2.6/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.6/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    21064 2023-06-14 16:04:39.000000 torchbones-1.2.6/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-14 16:04:47.652368 torchbones-1.2.6/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-14 16:04:47.000000 torchbones-1.2.6/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-14 16:04:47.000000 torchbones-1.2.6/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-14 16:04:47.000000 torchbones-1.2.6/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-14 16:04:47.000000 torchbones-1.2.6/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-14 16:04:47.000000 torchbones-1.2.6/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.2.5/torchbones/main.py` & `torchbones-1.2.6/torchbones/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             resnet: (bool, default False) whether to use resnet architecture
 
         Returns:
             None
         """
         sizes, lins, self.activation = args 
         
-
+        
         self.convs = kwargs.get('convs', [])
         csizes = kwargs.get('csizes', [])
         dropout = kwargs.get('dropout', 0)
         self.resnet = kwargs.get('resnet', False)
         if self.resnet:
             pads = ((np.array(csizes)-1)/2).astype(int)
             lsize = self.convs[-1] * sizes[0]*sizes[1]
@@ -139,28 +139,29 @@
             dropout: (float, default 0) the dropout probability
             resnet: (bool, default False) whether to use resnet architecture
             train_frac: (float, default 4/5) the fraction of the data to use for training
             test_set: (list of integers) the indices of the data to use for testing
             cov: (numpy array, default 1) the covariance matrix of the truth values
             max_batch: (int, default all) the maximum number of batches to use per epoch
             check: (bool, default True) whether to check for other runs with the same parameters
+            threads: (int, default 1) the number of threads to use
 
 
 
         Returns:
             None
         """
         self.lins, self.activation, self.optim,  self.batch_size, self.lr, self.indata, self.truth, self.cost =args
         
         keys = ('convs', 'csizes','lr_decay',  'saving', 'run_num', 'new_tar', 'save_weights',
-                'lr_min','dropout', 'resnet', 'train_frac', 'test_set', 'cov', 'max_batch', 'check' )
+                'lr_min','dropout', 'resnet', 'train_frac', 'test_set', 'cov', 'max_batch', 'check', 'threads' )
         for kwarg in kwargs.keys():
             if kwarg not in keys:
                 raise Exception(kwarg + ' is not a valid key. Valid keys: ', keys )
-        
+        torch.set_num_threads(int(kwargs.get('threads', 1)))
         self.cov = kwargs.get('cov', 1)
         self.convs = kwargs.get('convs', [])
         self.csizes = kwargs.get('csizes', [])
         self.resnet = kwargs.get('resnet', False)
         if self.csizes and self.convs :
             if len(self.csizes) != len(self.convs):
                 raise Exception('Number of convolutions does not match the number of convolution sizes')
@@ -217,16 +218,23 @@
 
         self.batches = int(np.floor(self.data[1].shape[0]/self.batch_size))
         self.max_batch = kwargs.get('max_batch', self.batches)
         print(self.max_batch)
   
             
         
-    def params(self, re = True):
-            
+    def params(self, returns = True):
+        """This function returns the parameters of the model.
+        Kwargs:
+            returns: (bool) returns parameters when True, displays when False
+
+        Returns:
+            None        
+        """
+
         if not len(self.testerr):
             trainerr = None
             testerr = None
         else:
             trainerr = round(float(self.trainerr[-1]), 2)
             testerr = round(float(self.testerr[-1]), 2)
             
@@ -236,20 +244,21 @@
         df = pd.DataFrame(columns = ('conv channels', 'conv kernel sizes',  'linear layer sizes', 'activation', 'Dropout', 'ResNet',
                               'training sample size', 'optimizer',  'batch size', 'initial learning rate',   'learning rate decay',
                                      'learning rate',  'epochs',  'train loss', 'test loss', ))
         vals = ( self.convs, self.csizes,  self.lins, str(self.activation).split('.')[-1][:-2],  self.dropout,  self.resnet ,
                     self.data[3].shape[0],  str(self.optimizer).split()[0], 
                 self.batch_size,  self.init_lr,  self.lr_decay, self.lr, self.epoch,  trainerr, testerr,)
         df.loc[self.loc] = vals
-        if re == True:
+        if returns == True:
             return df
         else: display(df)
             
             
     def check(self):
+        """This function checks if the current parameters match any previous runs. """
         
         df = self.params()
         if os.path.exists(val_file):
             vals = pickle.load(open(val_file, 'rb'))
         else:
             vals = df
             pickle.dump(vals, open(val_file, 'wb'))
@@ -282,14 +291,18 @@
         if not self.save_tar:
             self.save_file = None
         else: 
             self.save_file = weight_path + '/' + str(self.loc)+'.tar'
             print(f'saving weights to {self.save_file}')
             
     def save(self): 
+
+        """This function saves the model parameters."""
+        
+
         if self.save_tar:
             torch.save(self.net.state_dict(), open(self.save_file, 'wb'))
         vals = pickle.load(open(val_file, 'rb'))
         df = self.params()
         if self.loc in vals.index.tolist():
             vals.loc[self.loc] = df.loc[self.loc]
         else:
@@ -371,14 +384,23 @@
                 self.checkpoint(t)
                 
             if self.saving:
                 self.save()
             self.epoch += 1
     
     def checkpoint(self, t = 10): 
+        """ This function checks if the training is going well.
+         If the current train loss is nan, inf, or >5x the loss at the previous checkpoint, 
+         it reverts to the last checkpoint.
+
+         Kwargs:
+            t: (int) the number of epochs between checkpoints
+
+        """
+
         if len(self.trainerr) < t +1:
             return 0
         if not self.epoch>t:
             #create a checkpoint
             self.oldmodel = copy.deepcopy(self.net.state_dict())#create a checkpoint to return to if training goes off the rails
             self.oldlr = 1*self.lr
             self.countcheck = 0
@@ -400,14 +422,15 @@
             self.countcheck = 0 
             
 
 
 
             
     def plot(self):
+        """ This function plots the results of the training and testing. """
         testtruth = self.data[5]
         output = self.testout
         if len(self.testerr) > 1:
             fig, ax = plt.subplots(1,3, figsize = (15,4))
             xs = np.arange(len(self.trainerr))
             ax[2].plot(xs, self.trainerr, label = 'Train loss')
             ax[2].plot(xs, self.testerr, label = 'Test loss')
@@ -449,14 +472,15 @@
             ax[0].hist2d(xt, np.squeeze(yt), bins = 30)
             ax[1].hist2d(x, np.squeeze(y), bins = 30)
             
         fig.tight_layout()
         plt.show()
     
     def data_prep(self):
+        """ This function prepares the data for training and testing. """
         data = torch.tensor(self.indata).double()
         
         if len(data.shape) == 1:
             data = torch.unsqueeze(data, 0)
         if len(data.shape) >= 2:
             data = torch.unsqueeze(data, 1)
```

