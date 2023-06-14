# Comparing `tmp/QuNet-0.0.87-py3-none-any.whl.zip` & `tmp/QuNet-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,14 @@
-Zip file size: 66880 bytes, number of entries: 28
--rw-rw-rw-  2.0 fat      519 b- defN 23-Jun-12 07:32 qunet/__init__.py
--rw-rw-rw-  2.0 fat      616 b- defN 23-Apr-27 07:47 qunet/batch.py
--rw-rw-rw-  2.0 fat     5703 b- defN 23-May-05 12:11 qunet/callback.py
--rw-rw-rw-  2.0 fat     8843 b- defN 23-May-25 11:08 qunet/data.py
--rw-rw-rw-  2.0 fat     2955 b- defN 23-May-28 11:12 qunet/losses.py
--rw-rw-rw-  2.0 fat    21586 b- defN 23-Jun-13 19:00 qunet/modelstate.py
+Zip file size: 31279 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-22 07:06 qunet/__init__.py
+-rw-rw-rw-  2.0 fat     6484 b- defN 23-Apr-21 07:06 qunet/data.py
+-rw-rw-rw-  2.0 fat    21899 b- defN 23-Apr-22 20:00 qunet/models.py
 -rw-rw-rw-  2.0 fat    16977 b- defN 23-Apr-20 12:40 qunet/old.py
--rw-rw-rw-  2.0 fat    10491 b- defN 23-May-21 20:52 qunet/plots.py
--rw-rw-rw-  2.0 fat    52035 b- defN 23-Jun-14 07:39 qunet/trainer.py
--rw-rw-rw-  2.0 fat     6545 b- defN 23-Jun-06 08:41 qunet/utils.py
--rw-rw-rw-  2.0 fat        3 b- defN 23-Apr-26 10:17 qunet/modules/__init__.py
--rw-rw-rw-  2.0 fat    25379 b- defN 23-Jun-11 13:06 qunet/modules/cnn.py
--rw-rw-rw-  2.0 fat     7964 b- defN 23-May-20 06:54 qunet/modules/cnn3D.py
--rw-rw-rw-  2.0 fat     6302 b- defN 23-Apr-27 12:45 qunet/modules/gnn.py
--rw-rw-rw-  2.0 fat     4470 b- defN 23-May-20 06:52 qunet/modules/mlp.py
--rw-rw-rw-  2.0 fat     2897 b- defN 23-Apr-28 13:35 qunet/modules/points.py
--rw-rw-rw-  2.0 fat     1594 b- defN 23-Jun-13 17:44 qunet/modules/total.py
--rw-rw-rw-  2.0 fat    20312 b- defN 23-May-12 12:52 qunet/modules/transformer.py
--rw-rw-rw-  2.0 fat        3 b- defN 23-Apr-26 10:17 qunet/optim/__init__.py
--rw-rw-rw-  2.0 fat     8517 b- defN 23-Jun-07 15:24 qunet/optim/adams.py
--rw-rw-rw-  2.0 fat    14092 b- defN 23-Apr-25 10:33 qunet/optim/scheduler.py
--rw-rw-rw-  2.0 fat        3 b- defN 23-Apr-26 10:17 qunet/rl/__init__.py
--rw-rw-rw-  2.0 fat    15969 b- defN 23-Jun-05 12:31 qunet/rl/dqn.py
--rw-rw-rw-  2.0 fat     1068 b- defN 23-Jun-14 07:40 QuNet-0.0.87.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    16131 b- defN 23-Jun-14 07:40 QuNet-0.0.87.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 07:40 QuNet-0.0.87.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-14 07:40 QuNet-0.0.87.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2122 b- defN 23-Jun-14 07:40 QuNet-0.0.87.dist-info/RECORD
-28 files, 253194 bytes uncompressed, 63556 bytes compressed:  74.9%
+-rw-rw-rw-  2.0 fat    10435 b- defN 23-Apr-22 11:36 qunet/optim.py
+-rw-rw-rw-  2.0 fat     7131 b- defN 23-Apr-22 14:25 qunet/plots.py
+-rw-rw-rw-  2.0 fat    26998 b- defN 23-Apr-23 11:26 qunet/trainer.py
+-rw-rw-rw-  2.0 fat     1068 b- defN 23-Apr-23 11:32 QuNet-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13877 b- defN 23-Apr-23 11:32 QuNet-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-23 11:32 QuNet-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-23 11:32 QuNet-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      879 b- defN 23-Apr-23 11:32 QuNet-0.0.9.dist-info/RECORD
+12 files, 105969 bytes uncompressed, 29845 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -1,85 +1,37 @@
 Filename: qunet/__init__.py
 Comment: 
 
-Filename: qunet/batch.py
-Comment: 
-
-Filename: qunet/callback.py
-Comment: 
-
 Filename: qunet/data.py
 Comment: 
 
-Filename: qunet/losses.py
+Filename: qunet/models.py
 Comment: 
 
-Filename: qunet/modelstate.py
+Filename: qunet/old.py
 Comment: 
 
-Filename: qunet/old.py
+Filename: qunet/optim.py
 Comment: 
 
 Filename: qunet/plots.py
 Comment: 
 
 Filename: qunet/trainer.py
 Comment: 
 
-Filename: qunet/utils.py
-Comment: 
-
-Filename: qunet/modules/__init__.py
-Comment: 
-
-Filename: qunet/modules/cnn.py
-Comment: 
-
-Filename: qunet/modules/cnn3D.py
-Comment: 
-
-Filename: qunet/modules/gnn.py
-Comment: 
-
-Filename: qunet/modules/mlp.py
-Comment: 
-
-Filename: qunet/modules/points.py
-Comment: 
-
-Filename: qunet/modules/total.py
-Comment: 
-
-Filename: qunet/modules/transformer.py
-Comment: 
-
-Filename: qunet/optim/__init__.py
-Comment: 
-
-Filename: qunet/optim/adams.py
-Comment: 
-
-Filename: qunet/optim/scheduler.py
-Comment: 
-
-Filename: qunet/rl/__init__.py
-Comment: 
-
-Filename: qunet/rl/dqn.py
-Comment: 
-
-Filename: QuNet-0.0.87.dist-info/LICENSE
+Filename: QuNet-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: QuNet-0.0.87.dist-info/METADATA
+Filename: QuNet-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: QuNet-0.0.87.dist-info/WHEEL
+Filename: QuNet-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: QuNet-0.0.87.dist-info/top_level.txt
+Filename: QuNet-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: QuNet-0.0.87.dist-info/RECORD
+Filename: QuNet-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qunet/__init__.py

```diff
@@ -1,18 +1,5 @@
-﻿from .utils               import *
-from .data                import *
-from .trainer             import *
-from .plots               import *
-from .callback            import *
-from .losses              import *
-from .modelstate          import *
-
-from .modules.mlp         import *
-from .modules.cnn         import *
-from .modules.cnn3D       import *
-from .modules.transformer import *
-from .modules.points      import *
-
-from .optim.scheduler     import *
-from .optim.adams         import Adams
-
-
+﻿from .models  import *
+from .data    import *
+from .trainer import *
+from .optim   import *
+from .plots   import *
```

## qunet/data.py

```diff
@@ -1,233 +1,131 @@
-﻿import copy
-import numpy as np
-import torch
+﻿import os, gc, math, copy, time, datetime
+import numpy as np, matplotlib.pyplot as plt
+import torch, torch.nn as nn
+from   tqdm.auto import tqdm
 
 class Data:
     """
-    Data class. Its iterator gives out data in batches of batch_size examples in each.
-    """
-    def __init__(self, dataset=None, shuffle=False, batch_size=64,  whole_batch=False, n_packs=1, n_batches=-1) -> None:
-        """
-        Data class. Its iterator gives out data in batches of batch_size examples in each.
-
-        Args
-        ------------
-            dataset (tensor or list of tensors):
-                data for batches formation - it can be a torch tensor or a list (tuple) of tensors of the same length
-            shuffle (bool = False):
-                shuffle or not data
-            batch_size (int = 64):
-                minibatch size; then you can change
-            whole_batch (bool = False):
-                take only batches of size batch_size (if the number of examples is not divisible by batch_size)
-            n_packs (int = 1)
-                split the dataset into n_packs packs; the iterator terminates on the first pack and the next time it is called, it starts at the second pack, and so on.
-            n_batches (int = -1)
-                print only n_batches of the first batches (if n_batches < 0, then all)
-
-        Example:
-        ------------        
-        ```
-        X, Y = torch.rand(1000,2),  torch.rand(1000,)
-        data = Data( (X,Y),  batch_size=128)
-        for x,y in data:
-            print(x.shape, y.shape)
-        ```
-        """
-        assert dataset is None or torch.is_tensor(dataset) or type(dataset) is list or type(dataset) is tuple, f"dataset = tensor or  list (tuple) of tensors; got: {type(dataset)}"
-
-        self.data = self.set_data(dataset)
-        self.check_data(self.data)
-
-        self.shuffle     = shuffle      # перемешивать или нет данные
-        self.batch_size  = batch_size   # размер минибатча
-        self.start       = 0            # индекс начала текущего батча
-        self.n_packs     = n_packs      # разбить датасет на n_packs паков
-        self.pack_id     = 0            # номер текущего пака
-        self.whole_batch = whole_batch  # брать только батчи размера batch_size
-        self.n_batches   = n_batches    # выдать только n_batches первых батчей
-
-    #---------------------------------------------------------------------------
-
-    def set_data(self, data):
-        """
-        Dataset will be list of tensors
-        """
-        if data is None:
-            return data
-
-        if   torch.is_tensor(data) or type(data) is list:  
-            return data
-        elif type(data) is tuple:
-            return list(data)        # в mix надо менять тензоры в списке
-
-        assert True, "dataset should be tensor or tuple (list) of tensors"
-
-    #---------------------------------------------------------------------------
-
-    def check_data(self, data):
-        """ 
-        Check data in list of tensors 
-        """
-        if data is None:
-            return True
-        
-        if torch.is_tensor(data):
-            return True
-
-        for i,d in enumerate(data): # check data
-            if type(d).__module__ == np.__name__:  # from numpy to torch
-                data[i] = d = torch.tensor(d)
-
-            assert torch.is_tensor(d), "all data in dataset should be torch tensors"
-            if i==0:
-                count_first = len(d)
-            else:
-                assert len(d) == count_first, "all tensors must have the same length (number of examples)"
-        return True
-    #---------------------------------------------------------------------------
-
-    def reset(self):
-        """
-        Reset batch and pack number indexes to zero
-        """
-        self.start   = 0
-        self.pack_id = 0
-
-    #---------------------------------------------------------------------------
-
-    def copy(self):
-        """
-        Get a copy of the data class
-        """
-        return copy.deepcopy(self)
-
-    #---------------------------------------------------------------------------
-
-    def add(self, data):
-        """
-        Adding a dataset with the same data structure
-
-        Args:
-        ------------
-            data (Data) - an instance of the Data class
-        """
-        if self.data is None:
-            self.data = data.data
-            return self
-
-        if torch.is_tensor(data.data):
-            assert torch.is_tensor(self.data), "Data.add:data is tensor, but current dataset not is tensor"
-            self.data = torch.cat([self.data, data.data], dim=0)
-
-        for i, (cur, new) in enumerate(zip(self.data, data.data)):
-            assert torch.is_tensor(cur) and torch.is_tensor(new), "Data.add: method add works only with simple list of tensors"
-            assert cur.shape[1:] == new.shape[1:], "Data.add: data should have the same shape (except first index)"
-            self.data[i] = torch.cat([cur, new], dim=0)
+    Класс даных. Может в задаче переопределяется.
+    Для работы тренера Trainer в итераторе __next__ экземпляр Data должен возвращать кортеж X,Y где 
+        X - тензор или кортеж тензоров для входа модели,
+        Y - тензор или кортеж тензоров для целевых значений модели.
+    Модель - это класс (наследник nn.Module) с методом forward и metrics.
+    Первый даёт тензор или список (кортеж) тензоров на выходе модели
+    Второй вычсляет ошибку (скаляр) и метрики качества (тензор для каждого примера)
+
+    Кортеж батча данных используется в тренере следуюшим образом:
+        for X,Y in data:  # при обучении
+            y = model(X)
+            loss, score = model.metrics(y, Y)
+
+        y = model(X) # в продакшене
+
+    необходимых для модели данных (батча), отправленных на нужное устройство device.
+
+    Таким образом, dataset это список или кортеж из двух элементов (ввод и цель).
+    Каждый элемент может быть тензором или списком (кортежем) тензоров.    
+        Data(dataset = (X,Y) )               # 2 тензора (ввод и цель)
+        Data(dataset = ( (X1,X2), Y) )       # ввод список тензоров, цель -тензор
+        Data(dataset = ( (X1,X2), (Y1,Y2)) ) # ввод список тензоров, цель -список тензоров
+    Предполагается, что все тензоры в dataset имеют одинаковую длину (по первому индексу).
+
+    С Trainer можно также  использовать стандартный DataLoader:
+        from torchvision            import datasets
+        from torchvision.transforms import ToTensor 
+        from torch.utils.data       import DataLoader
+
+        mnist = datasets.MNIST(root='data', train=True,  transform=ToTensor(), download=True)
+        print(mnist.data.shape, mnist.targets.shape, mnist.classes)
+        plt.imshow(255-mnist.data[0], cmap='gray');
 
-        return self
-    #---------------------------------------------------------------------------
-
-    def count(self):
-        """ Number of samples in the dataset """
-        if self.data is None:
-            return 0
-        
-        if torch.is_tensor(self.data):
-            return len(self.data)
-        
-        return len(self.data[0])
-
-    #---------------------------------------------------------------------------
-
-    def mix(self, data):
-        """ Shuffle data. """
-        if data is None:
-            print("Data warning: data is None in function mix")
-            return data
-
-        idx = torch.randperm(  self.count() )
-
-        if torch.is_tensor(data):
-            return data[idx]
-
-        for i in range(len(data)):
-            data[i] = data[i][idx]
-        return data
+        data_trn  = DataLoader(dataset=mnist, batch_size=1024, shuffle=True)
+    """
+    def __init__(self, dataset, shuffle=True, batch_size=64,  whole_batch=False, n_packs=1) -> None:
+        assert type(dataset) is list or type(dataset) is tuple, f"data = [X, Y, ...] <- list or tuple; got: {type(dataset)}"
+        assert len(dataset) == 2,      "dataset must be (X,Y)"
+        self.X = dataset[0]             
+        self.Y = dataset[1]
+
+        self.shuffle    = shuffle      # перемешивать или нет данные        
+        self.batch_size = batch_size   # размер батча        
+        self.start = 0                 # индекс начала текущего батча
+        self.n_packs = n_packs         # разбить весть датасет на packs паков
+        self.pack_id = 0               # номер текущего пака
+        self.whole_batch = whole_batch # брать только батчи размера batch_size
+
+        # число примеров todo: проверь, что одинаковое для всех в списках
+        self.X_list = type(self.X) is list or type(self.X) is tuple
+        self.Y_list = type(self.Y) is list or type(self.Y) is tuple
+
+        self.N = len(self.X[0]) if self.Y_list else len(self.X)
+        assert self.N == len(self.Y[0]) if self.Y_list else len(self.Y), "X, Y must have the same number of examples"        
 
     #---------------------------------------------------------------------------
 
-    def get_batch(self, data, s, B):
-        """ Get batch size B starting from sample s. """        
-        if torch.is_tensor(data):
-            return data[s: s+B]
-        return [ d[s: s+B] for d in data ]
+    def mix(self):
+        """ Перемешать данные. С list по памяти эффективнее, чем с tuple."""
+        idx = torch.randperm( self.N )
+
+        if self.X_list:
+            for i in range(len(self.X)):
+                self.X[i] = self.X[i][idx]        
+        else:
+            self.X = self.X[idx]        
+
+        if self.Y_list:
+            for i in range(len(self.Y)):
+                self.Y[i] = self.Y[i][idx]        
+        else:
+            self.Y = self.Y[idx]        
 
     #---------------------------------------------------------------------------
 
-    def __next__(self):
-        """The iterator to get the next minibatch. """
-        assert self.data is not None, "Data: data is None in iterator"            
-
-        if (self.start >= self.count() )                                             \
-        or                                                                           \
-           (self.whole_batch and self.start + self.batch_size > self.count() )       \
-        or                                                                           \
-           (self.n_batches > 0 and self.start >= self.n_batches * self.batch_size ):
-                self.start = self.pack_id = 0
-                if self.data_is_over():
-                    if self.shuffle:
-                        self.data = self.mix(self.data)                
-                    raise StopIteration
+    def __next__(self):        
+        if (self.start >= self.N ) \
+           or                      \
+           (self.whole_batch and self.start + self.batch_size > self.N ):
+                self.start = self.pack_id = 0                
+                if self.shuffle:
+                    self.mix()
+                raise StopIteration
 
-        n = self.count() // self.n_packs
+        n = self.N // self.n_packs
         if self.start > self.pack_id * n + n:
             self.pack_id += 1
             raise StopIteration
 
-        batch = self.get_batch(self.data, self.start, self.batch_size)
+        s, B = self.start, self.batch_size
         self.start += self.batch_size
-        return batch
 
+        if self.X_list:
+            X = [d[s: s+B] for d in self.X]
+        else:
+            X = self.X[s: s+B]
+
+        if self.Y_list:
+            Y = [d[s: s+B] for d in self.Y]
+        else:
+            Y = self.Y[s: s+B]
 
-    #---------------------------------------------------------------------------
 
-    def data_is_over(self):
-        """
-        Overridden if part of the data needs to be retrieved from disk.
-        """
-        return True
-    #---------------------------------------------------------------------------
+        return (X, Y)                
 
     def __iter__(self):
         return self
-    
-    #---------------------------------------------------------------------------
 
     def __len__(self):
-        nb = (self.count() // self.n_packs) // self.batch_size
-        if not self.whole_batch and self.count()  % self.batch_size:
+        nb = self.N  // self.batch_size
+        if not self.whole_batch and self.N  % self.batch_size:
             nb += 1
         return nb
 
-    #---------------------------------------------------------------------------
-
-    def unit_test():
-        X = torch.rand(1000,)
-        data = Data( X,  batch_size=128)
-
-        X, Y = torch.rand(1000,2),  torch.rand(1000,)
-        data = Data( (X,Y),  batch_size=128)
-
-        print("ok Data")
-        return True
 
 #===============================================================================
 #                                   Main
 #===============================================================================
 if __name__ == '__main__':
-    X = torch.rand((100,))
-    data = Data(X, batch_size=7, n_packs=10)    
-    print(data.count(), len(data))
-    
-
+    X = torch.rand((1000, 2))
+    Y = (X[:,0] * X[:,1]).view(-1,1)     # (B,1)  !!!
+    n_trn = int(len(X)*0.80)
+    data_trn = Data((X[:n_trn], Y[:n_trn]), batch_size=40, whole_batch=True)
+    data_val = Data((X[n_trn:], Y[n_trn:]), batch_size=40, whole_batch=False, n_packs=4)
```

## qunet/plots.py

```diff
@@ -1,201 +1,126 @@
-﻿import os, math, copy, time, datetime
-import numpy as np, matplotlib.pyplot as plt
-import torch, torch.nn as nn
-from   tqdm.auto import tqdm
-
-#---------------------------------------------------------------------------
-
-def plot_histogram( x, x_sub=None, pref="", digits=1, w=12, h=3, bins=50, bins_sub=100, xlim=None, fname=""):
-    """ 
-    Distribution of values of x and its subset x_sub (in a narrower range) 
-    """
-    r = lambda x: '{x:.{digits}f}'.format(x=round(x,digits), digits=digits)
-    if x_sub is not None:
-        _, (ax1, ax2) = plt.subplots(1,2, figsize=(w, h), facecolor ='w')    
-        plt.suptitle(f"{pref}median={r(np.median(x))}; mean={r(x.mean())} ± {r(x.std())}  [min,max]=[{r(x.min())}, {r(x.max())}]; cnt={len(x)} ({100*len(x_sub)/len(x):.0f}%)", fontsize=14)    
-        ax1.hist(x, bins=bins, log=True, color="lightblue", ec="black");  plt.grid(ls=":",alpha=1); plt.ylabel("log10(N)")    
-        ax2.hist(x_sub, bins=bins_sub, density=True, color="lightblue", ec="black");    plt.grid(ls=":",alpha=1); plt.ylabel("Density")
-    else:
-        _, ax = plt.subplots(1,1, figsize=(w, h), facecolor ='w')    
-        plt.title(f"{pref}median={r(np.median(x))}; mean={r(x.mean())} ± {r(x.std())} [{r(x.min())}, {r(x.max())}]; cnt={len(x)}", fontsize=14)    
-        ax.hist(x, bins=bins, density=True, color="lightblue", ec="black");    plt.grid(ls=":",alpha=1); plt.ylabel("Density")
-        if xlim is not None:
-            ax.set_xlim(xlim)
-    
-    if fname:
-        plt.savefig(fname, bbox_inches='tight')
-    else:
-        plt.show()
-
-
-#---------------------------------------------------------------------------
-
-def plot_history(hist, view, fname=""):
-    """
-    """    
-    samples, steps             = hist.samples, hist.steps
-    if samples == 0:
-        print("plot_history warning: empty history")
-        return
-    val, trn, labels = hist.val, hist.trn, hist.labels
-    
-    t_unit = view.units.time  if  view.units.time in ['ms','s','m','h']  else 's'
-    t_unit_scale = dict(ms=1e-3, s=1, m=60, h=3600)[t_unit]
-    c_unit = view.units.count if view.units.count > 0  else 1
-    c_unit_power = round(np.log10(c_unit), 0)
-            
-    plt.figure(figsize=(view.w,  view.h), facecolor ='w')
-    
-    lr     = f"{trn.lr[-1]:.1e}" if len(trn.lr) else '?'
-    bs_trn = f"{trn.batch_size[-1]}" if len(trn.batch_size) else '?'
-    bs_val = f"{val.batch_size[-1]}" if len(val.batch_size) else '?'
-    tm_trn = f"{c_unit * trn.times[-1]/(t_unit_scale*trn.samples_epoch[-1]):.2f}" if len(trn.times) and trn.samples_epoch[-1] > 0 else '?'
-    tm_val = f"{c_unit * val.times[-1]/(t_unit_scale*val.samples_epoch[-1]):.2f}" if len(val.times) and val.samples_epoch[-1] > 0 else '?'
-
-    plt.suptitle(fr"samples={samples}, steps:{steps}; lr={lr}; batch=(trn:{bs_trn}, val:{bs_val}); time=(trn:{tm_trn}, val:{tm_val}){t_unit}/$10^{c_unit_power:.0f}$; params={hist.params/1e3:.0f}k", fontsize = 10)
-
-    if  not view.loss.show:
-        subplot_history(111, val, trn, view=view.score, view_tot=view, c_unit=c_unit, c_unit_power=c_unit_power, unit=view.units.unit, labels=labels, kind='score')
-    elif not view.score.show:
-        subplot_history(111, val, trn, view=view.loss,  view_tot=view, c_unit=c_unit, c_unit_power=c_unit_power, unit=view.units.unit, labels=labels, kind='loss')
-    else:
-        subplot_history(121, val, trn, view=view.score, view_tot=view, c_unit=c_unit, c_unit_power=c_unit_power, unit=view.units.unit, labels=labels, kind='score')
-        subplot_history(122, val, trn, view=view.loss,  view_tot=view, c_unit=c_unit, c_unit_power=c_unit_power, unit=view.units.unit, labels=labels, kind='loss')            
-    if fname:
-        plt.savefig(fname, bbox_inches='tight')
-    else:
-        plt.show()
-
-    #---------------------------------------------------------------------------    
-
-def subplot_history(sub, val, trn, view, view_tot, c_unit, c_unit_power, unit, labels, kind):                
-    
-    ax1 = plt.subplot(sub); ax1.grid(ls=':')                           
-    if len(val.samples) > 0 and len(trn.samples) > 0:        
-        if unit == 'samples':
-            x_max = max(val.samples[-1], trn.samples[-1]) if view_tot.x_max is None else view_tot.x_max        
-            ax1.set_xlim(view_tot.x_min/c_unit, x_max/c_unit)
-        else:
-            x_max = max(val.epochs[-1], trn.epochs[-1]) if view_tot.x_max is None else view_tot.x_max        
-            ax1.set_xlim(view_tot.x_min, x_max)
-
-    if kind == 'loss':
-        
-        best_loss  = f"{val.best.loss:.4f}"    if val.best.loss is not None  else "?"
-        loss_val   = f"{val.losses[-1]:.4f}"   if len(val.losses)  else "?"
-        loss_trn   = f"{trn.losses[-1]:.4f}"   if len(trn.losses)  else "?"
-        plt.title(f"loss = (min: {best_loss} [{val.best.loss_epochs}], val: {loss_val}, trn: {loss_trn})", fontsize=12, pad=-2)
-
-    if kind == 'score':        
-        best_score = f"{val.best.score:.4f}"   if val.best.score is not None else "?"
-        score_val  = f"{val.scores[-1]:.4f}"   if len(val.scores) else "?"
-        score_trn  = f"{trn.scores[-1]:.4f}"   if len(trn.scores) else "?"
-        plt.title(f"score = (bst: {best_score} [{val.best.score_epochs}], val: {score_val},  trn: {score_trn})", fontsize=12, pad=-2)
-
-    y_min, y_max = view.y_min, view.y_max
-    ax1.set_xlabel(fr"$10^{c_unit_power:.0f}$ samples" if unit=='samples' else 'epochs'); ax1.set_ylabel(kind);                     
-    if y_min is not None  and y_max is not None:            
-        ax1.set_ylim(y_min, y_max)
-        if view.ticks:
-            ax1.set_yticks(np.linspace(y_min, y_max, view.ticks))  
-
-    text = view.cfg.get_jaml(exclude=view.exclude)
-    if text:                
-        ax1.text(0.02, 0.02, text[:-1],  ha='left', va='bottom', transform = ax1.transAxes, fontsize=view.fontsize, family="monospace")
-
-    if len(trn.samples):                      # trn
-        x = np.array(trn.samples)/c_unit if unit=='sample' else np.array(trn.epochs)
-        y = trn.losses if kind=='loss' else trn.scores    
-        plot_smooth_line(ax1, x,y, 'darkblue', label=kind+'_trn', **view_tot.smooth.get_dict())            
-
-    if len(val.samples):                      # val
-        x = np.array(val.samples)/c_unit if unit=='sample' else np.array(val.epochs)
-        y = val.losses if kind=='loss' else val.scores        
-        plot_smooth_line(ax1, x,y, 'g', label=kind+'_val', **view_tot.smooth.get_dict())
-
-
-    ax1.legend(loc='upper left', frameon = False)
-    ax1.tick_params(axis='y', colors='darkgreen')
-
-    if view.labels:
-        y_min,y_max = ax1.get_ylim()
-        for lb in labels:  
-            x = lb[2]/c_unit if unit=='sample' else lb[1]               
-            ax1.vlines(x, y_min,y_max, linestyles=':', color='gray', linewidths=1.5 if len(lb[0]) else 1)
-            ax1.text  (x, y_min+(y_max-y_min)*0.01,    lb[0])
-
-    checks = trn.best.losses if kind=='loss' else trn.best.scores
-    if view.trn_checks:        
-        if view.last_checks > 0:
-            checks = checks[-view.last_checks :]
-        for c in checks:            
-            x = c[2]/c_unit if unit=='sample' else c[1]               
-            ax1.scatter(x, c[0],  s=3, c='darkblue', edgecolors='black', linewidths=0.5)                                
-
-    checks = val.best.losses if kind=='loss' else val.best.scores
-    if view.val_checks:        
-        if view.last_checks > 0:
-            checks = checks[-view.last_checks :]
-        for c in checks:            
-            x = c[2]/c_unit if unit=='sample' else c[1]               
-            ax1.scatter(x, c[0], s=7, c='g', edgecolors='black', linewidths=0.5)                                
-
-    if view.lr and len(trn.samples):
-        ax2 = ax1.twinx();                                     # lr
-        ax2.set_yscale('log')                
-        lr1, lr2 = np.min(trn.lr), np.max(trn.lr)
-        if lr1 > 0 and lr2 > 0:
-            lr1, lr2 = math.floor(np.log10(lr1)), math.ceil(np.log10(lr2))
-            if lr1 == lr2:
-                lr1 -= 1; lr2 +=1
-            lr1, lr2 = 10**lr1, 10**lr2
-            ax2.set_ylim(lr1, lr2)
-
-        x = np.array(trn.samples)/c_unit if unit=='sample' else np.array(trn.epochs)
-        y = trn.lr
-        if len(x) != len(y):        
-            print(f"Plot warning: {kind}: lr {len(x)} != {len(y)}")
-            x, y = x[:min(len(x),len(y))], y[:min(len(x),len(y))]
-        ax2.plot(x, y, ":", color='darkred')                 
-        ax2.legend(['lr'], loc='upper right', frameon = False)
-        ax2.tick_params(axis='y', colors='darkred')
-        if sub == 121:
-            ax2.set_yticklabels([])   
-            ax2.minorticks_off() # for log scale         
-
-
-def plot_smooth_line(ax=None, x=[],y=[], color="black", label="", count=200, kern=51, stride=1, width=1.5, alpha=0.5, num=10):    
-    if len(x) != len(y):        
-        print(f"Plot warning: {len(x)} != {len(y)}")
-        x, y = x[:min(len(x),len(y))], y[:min(len(x),len(y))]
-
-    lw = 1.5 if len(x) < 100 else (1 if len(x) < 200 else 0.5)        
-    if len(x) <  count:
-        ax.plot(x, y, color, linewidth=lw, label=label)
-    else:
-        if alpha > 0:
-            ax.plot(x, y, color, linewidth=lw, alpha=alpha)
-        pool = nn.AvgPool1d(kern, stride=stride, padding=kern // 2, count_include_pad=False)
-        avg_y = pool(torch.Tensor(y).view(1,-1)).flatten().numpy()
-        avg_x = pool(torch.Tensor(x).view(1,-1)).flatten().numpy()
-        
-        sx, sxx = avg_x[-num:].sum(), (avg_x[-num:]*avg_x[-num:]).sum()
-        sy, sxy = avg_y[-num:].sum(), (avg_x[-num:]*avg_y[-num:]).sum()
-        d = num*sxx - sx*sx
-        if d > 0:
-            b = (num*sxy - sx*sy) / d                                 # экстраполируем вперёд
-            a = (sy - b*sx) / num                                     # даже при stride=1 график отстаёт                  
-            avg_x = np.append(avg_x, [ x[-1] ])                       # из-за усреднения x            
-            avg_y = np.append(avg_y, [a + b*x[-1]])
-                
-        ax.plot(avg_x, avg_y, color, linewidth=width, label=label)    
-        
-
-
-#===============================================================================
-#                                   Main
-#===============================================================================
-
-if __name__ == '__main__':
-    x = np.random.normal(size=(1000,))
-    plot_histogram(x, w=8, digits=3)
+﻿import os, math, copy, time, datetime
+import numpy as np, matplotlib.pyplot as plt
+import torch, torch.nn as nn
+from   tqdm.auto import tqdm
+
+#---------------------------------------------------------------------------
+
+def plot_histogram( x, x_sub, pref="", digits=1, w=12, h=3, bins=50, bins_sub=100):
+    """ 
+    Distribution of values of x and its subset x_sub (in a narrower range) 
+    """
+    r = lambda x: '{x:.{digits}f}'.format(x=round(x,digits), digits=digits)
+    plt.figure(figsize=(w,h), facecolor ='w')         
+    plt.suptitle(f"{pref}median={r(x.median())}; mean={r(x.mean())} ± {r(x.std())}  [min,max]=[{r(x.min())}, {r(x.max())}]; cnt={len(x)} ({100*len(x_sub)/len(x):.0f}%)", fontsize=14)
+    plt.subplot(1,2,1)
+    plt.hist(x, bins=bins, log=True, color="lightblue", ec="black");  plt.grid(ls=":",alpha=1); plt.ylabel("log10(N)")
+    plt.subplot(1,2,2)
+    plt.hist(x_sub, bins=bins_sub, density=True, color="lightblue", ec="black");    plt.grid(ls=":",alpha=1); plt.ylabel("Density")
+    plt.show()
+
+#---------------------------------------------------------------------------
+
+def plot_history(hist, view):
+    """
+    """    
+    val, trn, labels = hist.get('val', []), hist.get('trn', []), hist.get('labels, []')
+    samples, steps             = hist.get('samples', 0), hist.get('steps', 0)    
+
+    t_unit = view.get('time_units','s') 
+    t_unit_scale = dict(ms=1e-3, s=1, m=60, h=3600).get(t_unit, 1)
+    c_unit = view.get('count_units', 1)
+    c_unit_power = round(np.log10(c_unit), 0)
+    
+    plt.figure(figsize=(view.get('w', 12),  view.get('h', 5)), facecolor ='w')
+    
+    lr     = f"{trn['lr'][-1]:.1e}" if len(trn['lr']) else '?'
+    bs_trn = f"{trn['batch_size'][-1]}" if len(trn['batch_size']) else '?'
+    bs_val = f"{val['batch_size'][-1]}" if len(val['batch_size']) else '?'
+    tm_trn = f"{c_unit * trn['time'][-1]/(t_unit_scale*trn['samples_epoch'][-1]):.2f}" if len(trn['time']) and trn['samples_epoch'][-1] > 0 else '?'
+    tm_val = f"{c_unit * val['time'][-1]/(t_unit_scale*val['samples_epoch'][-1]):.2f}" if len(val['time']) and val['samples_epoch'][-1] > 0 else '?'
+
+    plt.suptitle(fr"samples={samples}, steps:{steps}; lr={lr}; batch=(trn:{bs_trn}, val:{bs_val}); time=(trn:{tm_trn}, val:{tm_val}){t_unit}/$10^{c_unit_power:.0f}$; params={hist.get('parms',0)/1e3:.0f}k", fontsize = 10)
+
+    if  not view['loss'].get('show', True):
+        subplot_history(111, val, trn, view=view.get('score',{}), x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, labels=hist.get('labels',[]), kind='score')
+    elif not view['score'].get('show', True):
+        subplot_history(111, val, trn, view=view.get('loss',{}),  x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, labels=hist.get('labels',[]), kind='loss')
+    else:
+        subplot_history(121, val, trn, view=view.get('score',{}), x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, labels=hist.get('labels',[]), kind='score')
+        subplot_history(122, val, trn, view=view.get('loss',{}),  x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, labels=hist.get('labels',[]), kind='loss')            
+    plt.show()
+
+    #---------------------------------------------------------------------------    
+
+def subplot_history(sub, val, trn, view, x_min, x_max, c_unit, c_unit_power, labels, kind):                
+    
+    ax1 = plt.subplot(sub); ax1.grid(ls=':')                           
+    if len(val['samples']) > 0 and len(trn['samples']) > 0:        
+        x_max = max(val['samples'][-1], trn['samples'][-1]) if x_max is None else x_max        
+        ax1.set_xlim(x_min/c_unit, x_max/c_unit)
+
+    if kind == 'loss':
+        best_loss  = f"{val['best_loss'] [-1][-1]:.4f}" if len(val['best_loss'])  else "?"
+        loss_val   = f"{val['loss'] [-1]:.4f}"      if len(val['loss'])  else "?"
+        loss_trn   = f"{trn['loss'] [-1]:.4f}"      if len(trn['loss'])  else "?"
+        plt.title(f"loss = (min: {best_loss}, val: {loss_val}, trn: {loss_trn})")
+
+    if kind == 'score':
+        best_score = f"{val['best_score'][-1][-1]:.4f}" if len(val['best_score']) else "?"
+        score_val  = f"{val['score'][-1]:.4f}"      if len(val['score']) else "?"
+        score_trn  = f"{trn['score'][-1]:.4f}"      if len(trn['score']) else "?"
+        plt.title(f"score = (bst: {best_score}, val: {score_val},  trn: {score_trn})")
+
+    y_min, y_max = view.get('y_min'), view.get('y_max')
+    ax1.set_xlabel(fr"$10^{c_unit_power:.0f}$ samples"); ax1.set_ylabel(kind);                     
+    if y_min is not None  and y_max is not None:            
+        ax1.set_ylim(y_min, y_max)
+        if view.get('ticks', False):
+            ax1.set_yticks(np.linspace(y_min, y_max, view['ticks']))  
+
+    if len(trn['samples']):                      # trn
+        ax1.plot(np.array(trn['samples'])/c_unit, trn[kind], 'darkblue', linewidth=0.5)
+
+    if len(val['samples']):                      # val
+        ax1.plot(np.array(val['samples'])/c_unit, val[kind], 'g', linewidth=1.5)
+
+    ax1.legend([kind+'_trn',  kind+'_val'], loc='upper left', frameon = False)
+    ax1.tick_params(axis='y', colors='darkgreen')
+
+    if view.get('labels', False):
+        y_min,y_max = ax1.get_ylim()
+        for lb in labels:                 
+            ax1.vlines(lb[1]/c_unit, y_min,y_max, linestyles=':', color='gray')
+            ax1.text  (lb[1]/c_unit, y_min+(y_max-y_min)*0.01,    lb[0])
+
+
+    if view.get('trn_checks', False) and len(trn['best_'+kind]):        
+        for c in trn['best_'+kind]:
+            if True:
+                ax1.scatter(c[0]/c_unit, c[2], s=3, c='darkblue', edgecolors='black', linewidths=0.5)                                
+
+    if view.get('val_checks', False) and  len(val['best_'+kind]):        
+        for c in val['best_'+kind]:
+            if True:
+                ax1.scatter(c[0]/c_unit, c[2], s=7, c='g', edgecolors='black', linewidths=0.5)                                
+
+    if view.get('lr', False):
+        ax2 = ax1.twinx();                                     # lr
+        ax2.set_yscale('log')        
+        if len(trn['samples']):        
+            lr1, lr2 = np.min(trn['lr']), np.max(trn['lr'])
+            if lr1 > 0 and lr2 > 0:
+                lr1, lr2 = math.floor(np.log10(lr1)), math.ceil(np.log10(lr2))
+                if lr1 == lr2:
+                    lr1 -= 1; lr2 +=1
+                lr1, lr2 = 10**lr1, 10**lr2
+                ax2.set_ylim(lr1, lr2)
+            ax2.plot(np.array(trn['samples'])/c_unit, trn['lr'], ":", color='darkred')                 
+        ax2.legend(['lr'], loc='upper right', frameon = False)
+        ax2.tick_params(axis='y', colors='darkred')
+        if sub == 121:
+            ax2.set_yticklabels([])   
+            ax2.minorticks_off() # for log scale         
+
+#---------------------------------------------------------------------------
+
```

## qunet/trainer.py

```diff
@@ -1,1073 +1,491 @@
-﻿import os, glob, math, copy, time, datetime
-from pathlib import Path
-from   tqdm.auto import tqdm
-import numpy as np, matplotlib.pyplot as plt
-import torch, torch.nn as nn
-
-from .utils    import Config
-from .utils    import ModelEma
-from .callback import Callback
-from .batch    import Batch
-from .optim.scheduler    import Scheduler
-from .plots    import plot_history
-
-class Trainer:
-    """
-    Generic model training class.
-    Any method can, of course, be overridden by inheritance or by an instance.
-    """
-    def __init__(self, model=None, data_trn=None, data_val=None, callbacks=[], score_max=True, wandb_cfg=None, ema=False, ema_decay=0.9999, ema_start_epoch=1) -> None:
-        """
-        Trainer
-
-        Args:
-        ------------
-            model   (nn.Module):
-                model for traininig; must have a training_step method
-            data_trn (Data or DataLoader):
-                training data
-            data_val  (Data or DataLoader):
-                data for validatio; may be missing;
-            callbacks (Callback):
-                list of Callback instances to be called on events
-            score_max (bool):
-                consider that the metric (the first column of the second tensor returned by the function `metrics` of the model ); should strive to become the maximum (for example, so for accuracy).
-            wandb_cfg (Config):
-                wandb params to external data tracking. You have to specify next:
-                    api_key(str)
-                        WANDB API key
-                    project_name(str)
-                        WANDB project name
-                    run_name(str, optional)
-                        WANDB run name
-            ema (bool)
-                enable EMA (Exponential Moving Average) support
-            ema_decay (float)
-                average decay for EMA
-            ema_start_epoch (int)
-                first epoch to average weights (avoid first random values impact)
-        """
-        self.model     = model
-        self.score_max = score_max       # метрика должна быть максимальной (например accuracy)
-
-        self.device     = "cuda" if torch.cuda.is_available() else "cpu"
-        self.dtype      = torch.float32 # see training large models;
-        self.optim      = None
-
-        self.schedulers = []             # список шедулеров для управления обучением
-        self.scheduler  = Scheduler()    # текущий шедулер
-
-        self.epoch      = 0              # текущая эпоха за всё время
-        self.fit_epoch  = 0              # текущая эпоха после вызова fit
-
-        self.callbacks  = callbacks      # list of Callback instances to be called on events
-        self.wandb_cfg  = wandb_cfg      # wandb configuration
-
-        self.data = Config(trn = data_trn,  val = data_val)
-
-        self.ema = ema                              # enable EMA (Exponential Moving Average) support
-        self.ema_decay = ema_decay                  # average decay for EMA
-        self.ema_start_epoch = ema_start_epoch      # first epoch to average weights (avoid first random values impact)
-        self.model_ema = None                       # reference to ema model
-
-        self.best = Config(
-            score = None,               # best val score
-            loss = None,                # best val loss
-            score_model = None,         # copy of the best model by val score
-            loss_model  = None,         # copy of the best model by val loss
-            score_ema_model = None,     # copy of the best EMA model by val score
-            loss_ema_model  = None,     # copy of the best EMA model by val loss
-            copy = False                # should copy loss or score model if is in monitor
-        )
-
-        self.folders = Config(
-            loss   = None,              # folder to save the best val loss models
-            score  = None,              # folder to save the best val score models
-            loss_ema = None,            # folder to save the best val loss EMA models
-            score_ema = None,           # folder to save the best val score EMA models
-            point  = None,              # folder to save checkpoints
-            prefix = "",                # add prefix to file name
-        )
-
-        # -------------------------------- настройки для построения графиков ошибок и метрик
-        self.view = Config(
-            w  = 12,                   # plt-plot width
-            h  =  5,                   # plt-plot height
-            units = Config(
-                unit  = 'epoch',       # 'epoch' | 'sample'
-                count = 1e6,           # units for number of samples
-                time  = 's'            # time units: ms, s, m, h
-            ),
-
-            x_min = 0,                 # minimum value in samples on the x-axis (if < 0 last x_min samples)
-            x_max = None,              # maximum value in samples on the x-axis (if None - last)
-            smooth = Config(
-                count  = 200,          # if the number of points exceeds count - draw a smooth line
-                kern   = 51,           # averaging kernel (how many points are averaged)
-                stride = 1,            # averaging step
-                width  = 1.5,          # line thickness
-                alpha  = 0.5,          # source data transparency
-                num    = 10,           # number of last points for "extrapolation"
-            ),
-            loss = Config(
-                show  = True,          # show loss subplot
-                y_min = None,          # fixing the minimum value on the y-axis
-                y_max = None,          # fixing the maximum value on the y-axis
-                ticks = None,          # how many labels on the y-axis
-                lr    = True,          # show learning rate
-                labels= True,          # show labels (training events)
-                trn_checks = False,    # show the achievement of the minimum training loss (dots)
-                val_checks = True,     # show the achievement of the minimum validation loss (dots)
-                last_checks = 100,     # how many last best points to display (if -1 then all)
-                cfg   =  Config(),
-                exclude = [],
-                fontsize = 8,
-            ),
-            score = Config(
-                show  = True,          # show score subplot
-                y_min = None,          # fixing the minimum value on the y-axis
-                y_max = None,          # fixing the maximum value on the y-axis
-                ticks = None,          # how many labels on the y-axis
-                lr    = True,          # show learning rate
-                labels = True,         # show labels (training events)
-                trn_checks = False,    # show the achievement of the optimum training score (dots)
-                val_checks = True,     # show the achievement of the optimum validation score (dots)
-                last_checks = 100,     # how many last best points to display (if -1 then all)
-                cfg =  Config(),
-                exclude = [],
-                fontsize = 8,
-            ),
-        )
-
-        # -------------------------------- история и текущие метрики процесса обучения модели
-        self.hist = Config(            # история обучения и валидации:
-            epochs  = 0,               # число эпох в режиме обучения (same self.epoch)
-            samples = 0,               # число примеров в режиме обучения
-            steps   = 0,               # число шагов градиентного спуска
-
-            time = Config(
-                trn  = 0,              # общее время тренировки
-                val =  0               # общее время валидациии
-            ),
-
-            labels = [],
-            trn  = Config(
-                        best = Config(  loss = None,       # лучшее значение тренировочная ошибки
-                                        score = None,      # лучшее значение тенировочной метрики (первой)
-                                        loss_samples  = 0, # когда была лучшая тренировочная ошибка
-                                        loss_epochs   = 0, # когда была лучшая тренировочная ошибка
-                                        score_samples = 0, # когда была лучшая тренировочная метрика
-                                        score_epochs  = 0, # когда была лучшая тренировочная метрика
-                                        losses=[],         # точки достижения лучшей ошибки  (loss,epochs,samples,steps)
-                                        scores=[]          # точки достижения лучшей метрики (score,epochs,samples,steps)
-                                      ),
-                        epochs=[], samples=[], steps=[],   # история заначений после вызова training_step
-                        batch_size=[], lr=[],
-                        samples_epoch=[], steps_epoch=[],
-                        times=[], losses=[], scores=[]
-                    ),
-            val  = Config(
-                        best = Config(  loss = None,       # лучшее значение валиадционная ошибки
-                                        score = None,      # лучшее значение валиадционная метрики (первой)
-                                        loss_ema = None,   # лучшее значение валиадционная ошибки EMA модели
-                                        score_ema = None,  # лучшее значение валиадционная метрики (первой) EMA модели
-                                        loss_samples  = 0, # когда была лучшая валиадционная ошибка
-                                        loss_epochs   = 0, # когда была лучшая валиадционная ошибка
-                                        score_samples = 0, # когда была лучшая валиадционная метрика
-                                        score_epochs  = 0, # когда была лучшая валиадционная метрика
-                                        losses=[],         # точки достижения лучшей ошибки  (loss,epochs,samples,steps)
-                                        scores=[]          # точки достижения лучшей метрики (score,epochs,samples,steps)
-                                    ),
-                        epochs=[], samples=[], steps=[],    # история заначений после вызова validation_step
-                        batch_size=[], lr=[], samples_epoch=[],
-                        steps_epoch=[], times=[],
-                        losses=[], scores=[]
-                    ),
-
-            params = 0
-        )
-        if model is not None:
-            self.hist.params = sum(p.numel() for p in model.parameters() if p.requires_grad)
-
-        if self.wandb_cfg:
-            self.wandb_init()
-        else:
-            self.wandb = None
-
-
-    #---------------------------------------------------------------------------
-
-    def add_label(self, text):
-        """ Добавить пометку для графиков обучения """
-        h = self.hist
-        h.labels.append( [ text, h.epochs, h.samples, h.steps, h.time.trn, h.time.val ] )
-
-    #---------------------------------------------------------------------------
-
-    def set_optimizer(self, optim):
-        """ Установить текущий оптимизатор """
-        self.optim = optim
-        self.set_optim_schedulers()
-
-    def set_optim_schedulers(self):
-        self.scheduler.optim = self.optim
-        for sch in self.schedulers:
-            sch.optim = self.optim
-
-    #---------------------------------------------------------------------------
-
-    def set_scheduler(self, scheduler):
-        self.schedulers = []
-        self.add_scheduler(scheduler)
-        if scheduler.lr1 is not None:
-            scheduler.set_lr(scheduler.lr1)
-
-    def add_scheduler(self, scheduler):
-        scheduler.optim = self.optim
-        self.schedulers.append(scheduler)
-
-    def del_scheduler(self, i):
-        self.schedulers.pop(i)
-
-    def clear_schedulers(self):
-        self.scheduler = Scheduler(self.optim)
-        self.schedulers = []
-
-    def reset_schedulers(self):
-        for sch in self.schedulers:
-            sch.enable = True
-            sch.done   = 0
-
-    def stop_schedulers(self):
-        for sch in self.schedulers:
-            sch.enable = False
-
-    def step_schedulers(self, epochs, samples):
-        for sch in self.schedulers:
-            if sch.enable:
-                sch.step(epochs, samples)
-                if not sch.enable:
-                    self.add_label("")
-                self.scheduler = sch
-                break
-
-    def plot_schedulers(self):
-        self.scheduler.plot_list(self.schedulers)
-
-    #---------------------------------------------------------------------------
-
-    def to_device(self, batch):
-        """ send mini-batch to device """
-        if torch.is_tensor(batch) or Batch in batch.__class__.__bases__:
-            return batch.to(self.device)
-        batch = list(batch)
-        for i in range(len(batch)):
-            batch[i] = self.to_device(batch[i])
-        return batch
-
-    #---------------------------------------------------------------------------
-
-    def get_fun_step(self, model, train):
-        """ Получить функцию шага тренировки или валидации """
-        fun_step = None
-        if train:
-            if hasattr(model, "training_step"):
-                fun_step = model.training_step
-        else:
-            if hasattr(model, "validation_step"):
-                fun_step = model.validation_step
-            elif hasattr(model, "training_step"):
-                fun_step = model.training_step
-
-        assert fun_step is not None, "model must has training_step function"
-        return fun_step
-
-    #---------------------------------------------------------------------------
-
-    def get_metrics(self, step):
-        """ из результатов шага обучения вделить ошибку и метрику"""
-        if torch.is_tensor(step):
-            loss   = step
-            scores = None
-        elif type(step) is dict:
-            loss  = step.get('loss')
-            scores = step.get('score')
-        if torch.is_tensor(scores) and scores.ndim == 0:
-            scores = scores.view(1)
-        return loss, scores
-
-    #---------------------------------------------------------------------------
-
-    def samples_in_batch(self, batch):
-        """ сколько примров в батче """
-        if torch.is_tensor(batch):
-            return len(batch)
-        if type(batch) is list or type(batch) is tuple:
-            return self.samples_in_batch(batch[0])
-        if Batch in batch.__class__.__bases__:
-            return len(batch)
-        assert False, "wrong type of the fist element in batch"
-
-    #---------------------------------------------------------------------------
-
-    def fit_one_epoch(self, model, data,  train=True, accumulate=1, state=None, verbose=1):
-        """
-        Args
-        ------------
-        train (bool=True):
-            режим тренировки, иначе валидации
-        accumulate:
-            аккумулировать градиент для accumulate батчей перед сдвигом оптимизатора; используем, когда большой батч или граф не помещаются в GPU
-            https://kozodoi.me/blog/20210219/gradient-accumulation
-        
-        float16:
-        https://pytorch.org/blog/what-every-user-should-know-about-mixed-precision-training-in-pytorch/
-        """
-        self.model.train(train)                     # режим обучение или тестирование
-        torch.set_grad_enabled(train)               # строить или нет вычислительный граф
-
-        scaler = None                               # используется для float16
-        if torch.cuda.is_available() and self.dtype != torch.float32:
-            scaler = torch.cuda.amp.GradScaler()
-
-        if train:                                   # в режиме обучения
-            self.hist.epochs  += 1                  # эпох за всё время (а если packs > 1 ?)
-            self.epoch += 1                         # the same !!!
-            self.optim.zero_grad()                  # обнуляем градиенты
-
-        fun_step = self.get_fun_step(model, train)  # функция шага тренировки или валидации
-
-        samples, steps, beg, lst = 0, 0, time.time(), time.time()
-        counts_all, losses_all,  scores_all = torch.empty(0,1), None,  None
-        batch_id = 0  # может и раньше итератор прерваться (enumerate - плохо)
-        for batch in data:
-            num   = self.samples_in_batch(batch)
-
-            if train:
-                for callback in self.callbacks:
-                    batch = callback.on_train_before_batch_transfer(self, self.model, batch, batch_id)
-
-                batch = self.to_device(batch)
-
-                for callback in self.callbacks:
-                    batch = callback.on_train_after_batch_transfer(self, self.model, batch, batch_id)
-            else:
-                for callback in self.callbacks:
-                    batch = callback.on_validation_before_batch_transfer(self, self.model, batch, batch_id)
-
-                batch = self.to_device(batch)
-
-                for callback in self.callbacks:
-                    batch = callback.on_validation_after_batch_transfer(self, self.model, batch, batch_id)
-
-            if scaler is None:
-                step = fun_step(batch, batch_id)
-            else:
-                with torch.autocast(device_type=self.device, dtype=self.dtype):
-                    step = fun_step(batch, batch_id)
-            loss, scores = self.get_metrics(step)
-
-            if train:
-                if accumulate > 1:                  # normalize loss to account for batch accumulation (!)
-                    loss = loss / accumulate
-
-                if scaler is None:
-                    loss.backward()                 # вычисляем градиенты
-                else:
-                    scaler.scale(loss).backward()   # вычисляем градиенты
-
-                if (batch_id+1) % accumulate == 0 or (batch_id + 1 == len(data)):
-                    if scaler is None:
-                        self.optim.step()
-                    else:
-                        scaler.step(self.optim)     # подправляем параметры
-                        scaler.update()             # Updates the scale for next iteration
-
-                    if state is not None:
-                        state.update()
-
-                    self.optim.zero_grad()          # обнуляем градиенты
-
-                    steps      += 1                 # шагов за эпоху
-                    self.hist.steps += 1            # шагов за всё время
-                self.hist.samples += num            # примеров за всё время
-
-            samples += num                          # просмотренных примеров за эпоху
-            losses_all = loss.detach() if losses_all is None else torch.vstack([losses_all, loss.detach()])
-            if scores is not None:
-                scores = scores.detach()            # just in case
-                assert scores.ndim == 1, f"scores should be averaged over the batch, but got shape:{scores.shape}"
-                scores_all = scores if scores_all is None else torch.vstack([scores_all, scores])
-            counts_all = torch.vstack([counts_all, torch.Tensor([num])])
-
-            if verbose and (time.time()-lst > 1 or batch_id+1 == len(data) ):
-                lst = time.time()
-                self.fit_progress(train, batch_id+1, len(data),
-                                  losses_all, scores_all, counts_all, samples, steps, time.time()-beg)
-            
-            batch_id += 1  
-
-        if train: self.hist.time.trn += (time.time()-beg)
-        else:     self.hist.time.val += (time.time()-beg)
-
-        if scores_all is not None:
-            scores_all = scores_all.cpu()
-        if losses_all is not None:
-            self.fit_progress(train, len(data), len(data), losses_all, scores_all, counts_all, samples, steps, time.time()-beg)
-            losses_all = losses_all.cpu()
-
-        return losses_all, scores_all, counts_all, (samples, steps, time.time()-beg)
-
-    #---------------------------------------------------------------------------
-
-    def mean(self, losses, scores, counts):
-        """ Вычислить среднее по всей эпохе """
-        assert losses is not None, "Do you calculate loss at all?"
-
-        loss  = ((losses.detach().cpu() * counts).sum(dim=0) / counts.sum()).item()
-        if scores is not None:
-            scores = ((scores.detach().cpu() * counts).sum(dim=0) / counts.sum())
-        return (loss, scores)
-
-    #---------------------------------------------------------------------------
-
-    def fit_progress(self, train, batch_id, data_len, losses, scores, counts, samples, steps, tm):
-        """
-        Вывод информации о прогрессе обучения (эпоха, время, ошибка и т.п.)
-        В конкретном проекте можно перопределить.
-        """
-        loss, score = self.mean(losses, scores, counts)
-        steps, samples = max(steps, 0), max(samples, 1)             # just in case
-        st = ""
-        if score is not None and len(score):
-            st += f"score={score[0]:.4f} "                          # главная метрика
-            if len(score) > 1: st += "("                            # вспомогательные
-            for i in range(1, len(score)):
-                st += f"{score[i]:.4f}" + (", " if i+1 < len(score) else ") ")
-        st += f"loss={loss:.4f};"
-
-        st += f" best score=(val:{(self.hist.val.best.score or 0.0):.3f}[{self.hist.val.best.score_epochs or ' '}]"
-        if self.hist.val.best.score_ema:
-            st += f" ema:{(self.hist.val.best.score_ema or 0.0):.3f}"
-        st += f" trn:{(self.hist.trn.best.score or 0.0):.3f}[{self.hist.trn.best.score_epochs or ' '}]),"
-        st += f" loss=(val:{(self.hist.val.best.loss or 0.0):.3f}[{self.hist.val.best.loss_epochs or ' '}]"
-        if self.hist.val.best.loss_ema:
-            st += f" ema:{(self.hist.val.best.loss_ema or 0.0):.3f}"
-        st += f" trn:{(self.hist.trn.best.loss or 0.0):.3f}[{self.hist.trn.best.loss_epochs or ' '}])"
-
-        print(f"\r{self.epoch:3d}{'t' if train else 'v'}[{batch_id:4d}/{data_len:4d}] {st} {data_len*tm/max(batch_id,1):.0f}s", end="   ")
-
-    #---------------------------------------------------------------------------
-
-    def unit_scales(self):
-        """ Единицы измерения числа примеров и времени """
-        t_unit = self.view.units.time  if  self.view.units.time in ['ms','s','m','h']  else 's'
-        t_unit_scale = dict(ms=1e-3, s=1, m=60, h=3600)[t_unit]
-        c_unit = self.view.units.count if self.view.units.count > 0  else 1
-        c_unit_power = round(np.log10(c_unit), 0)
-        return t_unit, t_unit_scale,  c_unit, c_unit_power
-
-    #---------------------------------------------------------------------------
-
-    def validate(self, model=None, data=None):
-        """
-        Validate model without gradient computation.
-        The result is a dict with loss and score values.
-
-        Args
-        ------------
-        model
-            the model that makes the prediction (e.g. trainer.best.score_model)
-        data
-            dataset for prediction (its minibatch format should understand the model's predict_step method)
-        """
-        model = model or self.model
-        data = data or self.data.val
-        model.to(self.device)
-        losses, scores, counts, (samples_val, steps_val, tm_val) = self.fit_one_epoch(model, data, train=False)
-        loss_val, score_val = self.mean(losses, scores, counts)
-        score_val = score_val.item() if len(score_val) == 1 else score_val
-        return {'loss': loss_val, 'score': score_val }
-
-    #---------------------------------------------------------------------------
-
-    def predict(self, model, data, whole=False, batch_size=-1, n_batches=-1,  verbose:bool = True):
-        """
-        Calculate prediction for each example in data.
-        The result is a dict whose composition depends on the dict returned by the model's predict_step method.
-
-        Args
-        ------------
-        model
-            the model that makes the prediction (e.g. trainer.best.score_model)
-        data
-            dataset for prediction (its minibatch format should understand the model's predict_step method)
-        whole
-            do not process fractional dataset batches
-        batch_size
-            minibatch size in examples (it will not change for dataset), if batch_size <= 0, then as in dataset
-        n_batches
-            number of minibatches (if n_batches n_batches <= 0, then all)
-        verbose
-            display information about the calculation process
-        """
-        model = model or self.model
-
-        for callback in self.callbacks:
-            callback.on_predict_start(self, model)
-
-        model.to(self.device)
-        model.train(False)               # режим тестирование
-        torch.set_grad_enabled(False)    # вычислительный граф не строим
-        data.whole = whole               # обычно по всем примерам (и по дробному батчу)
-
-        assert hasattr(model, "predict_step"), "for prediction, the model needs to have method predict_step, witch return output tensor"
-
-        if batch_size > 0:
-            batch_size_save = data.batch_size
-            data.batch_size = batch_size
-
-        scaler = None
-        if torch.cuda.is_available() and self.dtype != torch.float32:
-            scaler = torch.cuda.amp.GradScaler()
-
-        samples, beg, lst = 0, time.time(), time.time()
-        res = dict()
-
-        for batch_id, batch in enumerate(data):
-            if n_batches > 0 and batch_id + 1 > n_batches:
-                break
-
-            for callback in self.callbacks:
-                batch = callback.on_predict_before_batch_transfer(self, model, batch, batch_id)
-
-            batch = self.to_device(batch)
-
-            for callback in self.callbacks:
-                batch = callback.on_predict_after_batch_transfer(self, model, batch, batch_id)
-
-
-            if scaler is None:
-                out = model.predict_step(batch, batch_id)
-            else:
-                with torch.autocast(device_type=self.device, dtype=self.dtype):
-                    out = model.predict_step(batch, batch_id)
-
-            if torch.is_tensor(out):
-                out = {'output': out.detach()}
-
-            for k,v in out.items():
-                assert torch.is_tensor(v), "predict_step should return only tensor or dict of tensors"
-                if k in res:
-                    if v.ndim == 1:  res[k] = torch.vstack([res[k], v.view(-1,1).detach() ])
-                    else:            res[k] = torch.vstack([res[k], v.detach() ])
-                else:
-                    if v.ndim == 1:  res[k] = v.view(-1,1).detach()
-                    else:            res[k] = v.detach()
-
-            if verbose and (time.time()-lst > 1 or batch_id+1 == len(data) ):
-                lst = time.time()
-                print(f"\r[{100*(batch_id+1)/len(data):3.0f}%]  {(time.time()-beg)/60:.2f}m", end=" ")
-
-
-        if verbose:
-            print(f" keys: {list(res.keys())}")
-        if batch_size > 0:
-            data.batch_size = batch_size_save
-        for k in res.keys():
-            res[k] = res[k].cpu()
-
-        for callback in self.callbacks:
-            callback.on_predict_end(self, model)
-
-        return res
-
-    #---------------------------------------------------------------------------
-
-    def fit(self,  epochs=None,  samples=None,
-            period_plot:  int=0,  pre_val:bool=False,
-            period_val:   int=1,  period_val_beg=1, val_beg:int = None,
-            period_point: int=1,  point_start:int=1,
-
-            monitor = [],
-            patience = None,
-            state = None,
-            period_state: int=0):
-        """
-        Args
-        ------------
-            epochs (int):
-                number of epochs for training (passes of one data_trn pack). If not defined (None) works "infinitely".
-            samples (int):
-                if defined, then will stop after this number of samples, even if epochs has not ended
-            period_plot (int=0):
-                period after which the training plot is displayed (in epochs)
-            pre_val (bool=False):
-                validate before starting training
-            period_val (int=1):
-                period after which validation run (in epochs)
-            period_val_beg (int=1):
-                validation period on the first val_beg epochs
-            val_beg (int=None):
-                the number of epochs from the start, after which the validation period will be equal to period_val.
-            period_point (int=1):
-                period after which checkpoints  are made(in epochs)
-            point_start (int=1):
-                period after fit runs will be saved checkpoints with period period_points (in epochs)
-            monitor (list=[]):
-                what to save in folders: monitor=['loss'] or monitor=['loss', 'score', 'point']
-            patience (int):
-                after how many epochs to stop if there was no better loss, but a better score during this time
-            state (ModelState=None)
-                an instance of the ModelState class that accumulates information about gradients on model parameters
-            period_state (int=0)
-                period after which the model state  plot is displayed (in epochs)
-
-        Example
-        ```
-        tariner = Trainer(model, data_trn=data_trn, data_val=data_val, score_max=True)
-        trainer.view.units(count=1e6, time='m');
-        trainer.best(copy=True)
-        trainer.set_optimizer( torch.optim.Adam(model.parameters(), lr=1e-3) )
-        trainer.fit(epochs=200, period_plot = 50, monitor=['score'], patience=100)
-        ```
-        """
-        assert self.optim    is not None, "Define the optimizer first"
-        assert self.data.trn is not None, "Define data.trn first"
-        assert len(self.data.trn) > 0,    "You don't have a single training batch!"
-
-        for callback in self.callbacks:
-            callback.on_fit_start(self, self.model)
-
-        self.set_optim_schedulers()
-        self.model.to(self.device)
-
-        if self.data.val is not None and hasattr(self.data.val, "reset"):
-            self.data.val.reset()
-        if hasattr(self.data.trn, "reset"):
-            self.data.trn.reset()
-
-        if pre_val and self.data.val is not None:
-            assert len(self.data.val) > 0, "You don't have a single validation batch!"
-            losses, scores, counts, (samples_val, steps_val, tm_val) = self.fit_one_epoch(self.model, self.data.val, train=False)
-            loss_val, score_val = self.mean(losses, scores, counts)
-            self.add_hist(self.hist.val, self.data.val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, self.scheduler.get_lr())
-            print()
-
-        epochs = epochs or 1_000_000_000
-        last_best = max(self.hist.val.best.score_epochs, self.hist.val.best.loss_epochs)
-        loss_val  = 0
-        #for epoch in tqdm(range(1, epochs+1)):
-        for epoch in range(1, epochs+1):
-            self.fit_epoch = epoch               # epoch from start fit function
-            for callback in self.callbacks:
-                callback.on_epoch_start(self, self.model)
-            for callback in self.callbacks:
-                callback.on_train_epoch_start(self, self.model)
-
-            losses, scores, counts, (samples_trn,steps_trn,tm_trn) = self.fit_one_epoch(self.model, self.data.trn, train=True, state=state)            
-            loss_trn, score_trn = self.mean(losses, scores, counts)
-            lr = self.scheduler.get_lr()
-            self.add_hist(self.hist.trn, self.data.trn.batch_size, samples_trn, steps_trn, tm_trn, loss_trn, score_trn, lr)
-
-            if self.hist.trn.best.loss is None or self.hist.trn.best.loss > loss_trn:
-                last_best = self.epoch
-                self.hist.trn.best.loss = loss_trn
-                self.hist.trn.best.loss_epochs  = self.hist.epochs
-                self.hist.trn.best.loss_samples = self.hist.samples
-                self.hist.trn.best.losses.append( (loss_trn, self.hist.epochs, self.hist.samples, self.hist.steps) )
-                for callback in self.callbacks:
-                    callback.on_best_loss(self, self.model)
-
-            if self.best_score(self.hist.trn.best.score, score_trn):
-                last_best = self.epoch
-                self.hist.trn.best.score = score_trn[0]
-                self.hist.trn.best.score_epochs  = self.hist.epochs
-                self.hist.trn.best.score_samples = self.hist.samples
-                self.hist.trn.best.scores.append((score_trn[0].item(), self.hist.epochs, self.hist.samples, self.hist.steps))
-                for callback in self.callbacks:
-                    callback.on_best_score(self, self.model)
-
-            self.update_ema_model(monitor)
-
-            for callback in self.callbacks:
-                callback.on_train_epoch_end(self, self.model)
-
-            period = period_val_beg if val_beg and  self.epoch < val_beg  else period_val
-            if  ( (period and self.epoch % period == 0) or epoch == epochs ):
-                if self.data.val is not None:
-                    for callback in self.callbacks:
-                        callback.on_validation_epoch_start(self, self.model)
-
-                    losses, scores, counts, (samples_val,steps_val,tm_val) = self.fit_one_epoch(self.model, self.data.val, train=False)
-                    loss_val, score_val = self.mean(losses, scores, counts)
-                    self.add_hist(self.hist.val, self.data.val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, lr)
-                    self.ext_hist(loss_trn, score_trn, loss_val, score_val, lr)
-                else:
-                    loss_val  = loss_trn        # no validation data
-                    score_val = score_trn
-
-                # save best validation loss:
-                if self.hist.val.best.loss is None or self.hist.val.best.loss > loss_val:
-                    last_best = self.epoch
-                    self.hist.val.best.loss =  self.best.loss = loss_val
-                    self.hist.val.best.loss_epochs  = self.hist.epochs
-                    self.hist.val.best.loss_samples = self.hist.samples
-                    self.hist.val.best.losses.append((loss_val, self.hist.epochs, self.hist.samples, self.hist.steps))
-                    if self.folders.loss and 'loss' in monitor:
-                        self.save(Path(self.folders.loss) / Path(self.folders.prefix + f"epoch_{self.epoch:04d}_loss_{loss_val:.4f}_{self.now()}.pt"), model=self.model, optim=self.optim)
-                    if self.best.copy and 'loss' in monitor:
-                        self.best.loss_models  = copy.deepcopy(self.model)
-
-                if self.best_score(self.hist.val.best.score, score_val):
-                    self.hist.val.best.score = self.best.score = score_val[0]
-                    self.hist.val.best.score_epochs  = self.hist.epochs
-                    self.hist.val.best.score_samples = self.hist.samples
-                    self.hist.val.best.scores.append( ( score_val[0].item(), self.hist.epochs, self.hist.samples, self.hist.steps) )
-                    if self.folders.score and 'score' in monitor:
-                        self.save(Path(self.folders.score) / Path(self.folders.prefix + f"epoch_{self.epoch:04d}_score_{score_val[0]:.4f}_{self.now()}.pt"), model=self.model, optim=self.optim)
-                    if self.best.copy and 'score' in monitor:
-                        self.best.score_model  = copy.deepcopy(self.model)
-
-                for callback in self.callbacks:
-                    callback.on_validation_epoch_end(self, self.model)
-
-            if period_plot > 0 and (self.epoch % period_plot == 0 or epoch == epochs):
-                if len(self.hist.trn.epochs) > 1:
-                    self.plot()
-                    for callback in self.callbacks:
-                        callback.on_after_plot(self, self.model)
-                self.stat()
-            if (state is not None) and period_state > 0 and  (self.epoch % period_state == 0 or epoch == epochs):
-                state.plot()            
-
-            if self.folders.point and 'point' in monitor and (period_point > 0 and point_start < self.epoch and self.epoch % period_point == 0 or epoch == epochs):
-                for callback in self.callbacks:
-                    callback.on_save_checkpoint(self, self.model, {})
-                score_val = score_val if score_val is not None else [0]
-                score_trn = score_trn if score_trn is not None else [0]
-                fname = f"epoch_{self.epoch:04d}({self.now()})_score(val_{score_val[0]:.4f}_trn_{score_trn[0]:.4f})_loss(val_{loss_val:.4f}_trn_{loss_trn:.4f}).pt"
-                self.save(Path(self.folders.point) / Path(self.folders.prefix + fname), model=self.model, optim=self.optim)
-
-            self.step_schedulers(1, samples_trn)
-
-            if samples is not None:
-                samples -= samples_trn
-                if samples <= 0:
-                    self.plot()
-                    self.stat()
-                    break
-
-            for callback in self.callbacks:
-                callback.on_epoch_end(self, self.model)
-
-            if patience is not None and patience > 0 and  self.epoch - last_best > patience:
-                print(f"\n!!! Stop on patience={patience}. Epoch:{self.epoch}, last best score epoch:{self.hist.val.best.score_epochs}, best loss epoch:{self.hist.val.best.loss_epochs}")
-                if period_plot > 0 and len(self.hist.trn.epochs) > 1:
-                    self.plot()
-                    for callback in self.callbacks:
-                        callback.on_after_plot(self, self.model)
-                    self.stat()
-                if period_state > 0 and state is not None:
-                    state.plot()
-                break
-
-        if period_plot <= 0:
-            self.stat()
-
-        for callback in self.callbacks:
-            callback.on_fit_end(self, self.model)
-
-
-    #---------------------------------------------------------------------------
-
-    def plot(self, view=None, hist=None, fname=None):
-        """
-        Plot training history
-        """
-        view = view or self.view
-        hist = hist or self.hist
-        plot_history(hist, view, fname)
-
-    #---------------------------------------------------------------------------
-
-    def stat(self, newline=True):
-        if newline:
-            print()
-        if self.hist.val.best.score is not None:
-            print(f"validation score={self.hist.val.best.score:.6f}, loss={self.hist.val.best.loss:.6f};  epochs={self.epoch}, samples={self.hist.samples}, steps={self.hist.steps}")
-            if self.hist.val.best.score_ema is not None:
-                print(f"ema score={self.hist.val.best.score_ema or 0.0:.6f}, loss={self.hist.val.best.loss_ema or 0.0:.6f}")
-        elif self.hist.trn.best.score is not None:
-            print(f"validation loss={self.hist.val.best.loss:.6f};  epochs={self.epoch}, samples={self.hist.samples}, steps={self.hist.steps}")
-
-        t_steps = f"{self.hist.time.trn*1_000/self.hist.steps:.2f}"   if self.hist.steps > 0 else "???"
-        t_sampl = f"{self.hist.time.trn*1_000_000/self.hist.samples:.2f}" if self.hist.samples > 0 else "???"
-        t_epoch = f"{self.hist.time.trn/self.epoch:.2f}" if self.epoch > 0 else "???"
-        print(f"times=(trn:{self.hist.time.trn/60:.2f}, val:{self.hist.time.val/60:.2f})m,  {t_epoch} s/epoch, {t_steps} s/10^3 steps,  {t_sampl} s/10^6 samples")
-
-    #---------------------------------------------------------------------------
-
-    def best_score(self, best, score):
-        return score is not None  and len(score) \
-                and (best is None \
-                or (best < score[0] and     self.score_max) \
-                or (best > score[0] and not self.score_max) )
-
-    #---------------------------------------------------------------------------
-
-    def now(self):
-        return datetime.datetime.now().strftime("%m.%d_%H-%M-%S")
-
-    #---------------------------------------------------------------------------
-
-    def add_hist(self, hist, batch_size, samples, steps, tm, loss, score, lr):
-        hist.epochs       .append(self.hist.epochs)
-        hist.samples      .append(self.hist.samples)
-        hist.steps        .append(self.hist.steps)
-        hist.samples_epoch.append(samples)
-        hist.steps_epoch  .append(steps)
-        hist.batch_size   .append(batch_size)
-        hist.times        .append(tm)
-        hist.lr           .append(lr)
-        hist.losses       .append(loss)
-        if score is not None and len(score):
-            hist.scores.append(score[0].item())
-
-    #---------------------------------------------------------------------------
-
-    def ext_hist(self, loss_trn, score_trn, loss_val, score_val, lr):
-        self.wandb and self.wandb.log({'loss_trn': loss_trn, 'score_trn': score_trn, 'loss_val': loss_val, 'score_val': score_val, 'lr': lr})
-
-    #---------------------------------------------------------------------------
-
-    def save(self, fname, model = None, optim=None, info=""):
-        try:
-            model = model or self.model
-            assert model is not None, "You don't have a model!"
-            optim = optim or self.optim
-
-            cfg = model.cfg if hasattr(model, "cfg") else Config()
-            Path(fname).parent.mkdir(parents=True, exist_ok=True)
-            state = {
-                'info':            info,
-                'date':            datetime.datetime.now(),   # дата и время
-                'model' :          model.state_dict(),        # параметры модели
-                'config':          cfg,                       # конфигурация модели
-                'class':           model.__class__,
-                'hist':            self.hist,
-                'view':            self.view,
-
-                'optim':           optim.__class__ if optim is not None else None,
-                'optim_cfg':       None,
-                'optim_state':     None,
-            }
-            if optim is not None:
-                if hasattr(optim, "defaults"):
-                    state['optim_cfg'] = optim.defaults
-                elif hasattr(optim, "cfg"):
-                    state['optim_cfg'] = optim.cfg
-
-                if hasattr(optim, "state_dict"):
-                    state['optim_state'] = optim.state_dict()
-            torch.save(state, fname)
-        except:
-            print(f"Something  wrong in the function trainer.save fname: '{fname}'")
-
-    #---------------------------------------------------------------------------
-
-    def resume(self, fname=None):
-        if fname is None:
-            list_of_points = []
-            for folder in [self.folders.loss, self.folders.score, self.folders.point]:
-                list_of_points.extend(glob.glob(f'{folder}/*') if folder else [])
-            assert len(list_of_points) != 0, 'no saves for resume'
-            fname = max(list_of_points, key=os.path.getctime)
-        
-        print('resume from weights', fname)
-        Trainer.load(fname, None, self)
-
-    #---------------------------------------------------------------------------
-
-    def load(fname, ClassModel=None, trainer=None):
-        """
-        Static method of created trainer with loaded model.
-
-        Args
-        ------------
-        fname (str):
-            file name with model parameters
-        ClassModel:
-            name of model class
-
-        Example
-        ------------
-        class Model(nn.Module):
-            ...
-
-        trainer.save("cur_model.pt")
-        ...
-
-        new_trainer = Trainer.load("cur_model.pt", Model)
-        new_trainer.plot()
-        """ 
-
-        #try:
-        state = torch.load(fname)  # , map_location='cpu'
-        print(f"info:  {state.get('info', '???')}")
-        print(f"date:  {state.get('date', '???')}")
-        print(f"model: {state.get('class','???')}")
-        print(f"optim: {state.get('optim','???')}")
-        #print(f"       {state.get('optim_cfg','???')}")
-        #except:
-        #    print(f"Cannot open file: '{fname}'")
-        #    return None
-
-        assert type(state) == dict,  f"Apparently this model was not saved by the trainer: state:{type(state)}"
-        assert 'model'  in state,    f"Apparently this model was not saved by the trainer: no 'model' in state: {list(state.keys())}"
-        assert 'config' in state,    f"Apparently this model was not saved by the trainer: no 'config' in state: {list(state.keys())}"
-
-        trainer = trainer or Trainer(None, None)
-
-        try:
-            if ClassModel is None:
-                ClassModel = state.get('class')
-            trainer.model = ClassModel(state['config'])            
-        except:
-            print(f"Can not create model class: {state.get('class')}")
-            
-
-        if trainer.model is not None:
-            try:
-                trainer.model.load_state_dict(state['model'])
-            except:
-                print("!!!! Trainer.load> can't trainer.model.load_state_dict")
-
-        if trainer.model is not None:
-            if 'optim_state' in state and 'optim' in state:
-                if state['optim'] == torch.optim.SGD:
-                    trainer.optim  = torch.optim.SGD(trainer.model.parameters(), lr=1e-5)
-                elif state['optim'] == torch.optim.Adam:
-                    trainer.optim  = torch.optim.Adam(trainer.model.parameters(), lr=1e-5)
-                elif state['optim'] == torch.optim.AdamW:
-                    trainer.optim  = torch.optim.AdamW(trainer.model.parameters(), lr=1e-5)
-
-            if trainer.optim is not None:
-                try:
-                    if 'optim_state' in state and state['optim_state'] is not None:
-                        trainer.optim.load_state_dict(state['optim_state'])
-                    elif 'state_dict' in state and state['state_dict'] is not None:  # old version  
-                        trainer.optim.load_state_dict(state['state_dict'])
-                except:
-                    print("!!!! Trainer.load> can't trainer.optim.load_state_dict")
-
-        trainer.hist(state['hist'])
-        trainer.view(state['view'])
-        trainer.epoch = trainer.hist.epochs
-        print(f"epoch: {trainer.epoch}")        
-        return trainer
-
-    #---------------------------------------------------------------------------
-
-    def load_history(fname, verbose=0):
-        """
-        Load training history from file fname
-
-        Args
-        ------------
-        fname (str):
-            file name with model parameters
-
-        Example
-        ------------
-        class Model(nn.Module):
-            ...
-
-        hist = trainer.load_history("cur_model.pt")
-        trainer.plot(hist)
-        """
-        try:
-            state = torch.load(fname, map_location='cpu')
-            if verbose:
-                print(f"info:  {state.get('info', '???')}")
-                print(f"date:  {state.get('date', '???')}")
-                print(f"model: {state.get('class','???')}")
-                print(f"optim: {state.get('optim','???')}")
-                #print(f"       {state.get('optim_cfg','???')}")
-        except:
-            print(f"Cannot open file: '{fname}'")
-            return None
-
-        return state.get('view')
-    
-    #---------------------------------------------------------------------------
-
-    def transfer(self, fname):
-        """ Load to currnet model parameters from file fname with another model """                
-        state = torch.load(fname)
-        self.model.load_state_dict(state['model'])        
-
-    #---------------------------------------------------------------------------
-
-    def wandb_init(self):
-        """
-        """
-        import wandb
-
-        assert hasattr(self.wandb_cfg, "api_key"), "Define api_key param for login to WANDB"
-        assert hasattr(self.wandb_cfg, "project_name"), "Define project_name param for attach current run to it"
-
-        run_name = self.wandb_cfg.run_name if hasattr(self.wandb_cfg, "run_name") else None
-
-        cfg = self.model.cfg if hasattr(self.model, "cfg") else Config()
-
-        self.wandb = wandb
-
-        self.wandb.login(key=self.wandb_cfg.api_key)
-        self.wandb.init(
-            # set the wandb project where this run will be logged
-            project=self.wandb_cfg.project_name,
-            name=run_name,
-            config=cfg,
-            #resume="must"
-        )
-
-    def update_ema_model(self, monitor):
-        """
-        Update weigths of EMA model with: decay * model + (1. - decay) * model_ema
-        """
-        if self.data.val is None:
-            return
-        
-        # create EMA model if not exists
-        if self.ema and (self.model_ema is None) and (self.ema_start_epoch < self.epoch):
-            self.model_ema = ModelEma(self.model, self.ema_decay, self.device)
-            return
-
-        if self.model_ema is None:
-            return
-
-        # update weights
-        self.model_ema.update(self.model)
-
-        # validate model
-        
-        losses, scores, counts, (samples_val, steps_val, tm_val) = self.fit_one_epoch(self.model_ema.module, self.data.val, train=False)
-        loss_val_ema, score_val_ema = self.mean(losses, scores, counts)
-
-        # save best EMA validation loss:
-        if self.hist.val.best.loss_ema is None or self.hist.val.best.loss_ema > loss_val_ema:
-            self.hist.val.best.loss_ema = loss_val_ema
-            if self.folders.loss_ema and 'loss_ema' in monitor:
-                self.save(Path(self.folders.loss_ema) / Path(
-                    self.folders.prefix + f"epoch_{self.epoch:04d}_loss_{loss_val_ema:.4f}_{self.now()}.pt"), model=self.model_ema.module)
-            if self.best.copy and 'loss_ema' in monitor:
-                self.best.loss_ema_model = copy.deepcopy(self.model_ema.module)
-
-        # save best EMA validation score:
-        if self.best_score(self.hist.val.best.score_ema, score_val_ema):
-            self.hist.val.best.score_ema = score_val_ema[0]
-            if self.folders.score_ema and 'score_ema' in monitor:
-                self.save(Path(self.folders.score_ema) / Path(self.folders.prefix + f"epoch_{self.epoch:04d}_score_{score_val_ema[0]:.4f}_{self.now()}.pt"), model=self.model_ema.module)
-            if self.best.copy and 'score_ema' in monitor:
-                self.best.score_ema_model = copy.deepcopy(self.model_ema.module)
+﻿import os, math, copy, time, datetime
+from   tqdm.auto import tqdm
+import numpy as np, matplotlib.pyplot as plt
+import torch, torch.nn as nn
+
+from .optim   import Scheduler
+from .plots   import plot_history
+
+class Trainer:
+    """
+    Generic model training class.
+    Any method can, of course, be overridden by inheritance or by an instance.
+    """
+    def __init__(self, model, data_trn, data_val, score_max=False) -> None:
+        """
+        Args:
+            * model     - model for traininig;
+            * data_trn  - training data (Data or DataLoader instance);
+            * data_val  - data for validation (instance of Data or DataLoader); may be missing;
+            * score_max - consider that the metric (the first column of the second tensor returned by the function `metrics` of the model ); should strive to become the maximum (for example, so for accuracy).            
+        """
+        self.model      = model
+        self.data_trn   = data_trn
+        self.data_val   = data_val
+        self.score_max = score_max       # метрика должна быть максимальной (например accuracy)
+
+        self.device     = "cuda" if torch.cuda.is_available() else "cpu"         
+        self.dtype      = torch.float32 # see training large models;
+        self.optim      = None
+        self.schedulers = []             # список шедулеров для управления обучением
+        self.scheduler  = Scheduler()    # текущий шедулер
+
+        self.copy_best_score_model = False  # to copy the best model by val score
+        self.copy_best_loss_model  = False  # to copy the best model by val loss
+
+        self.best_score_model = None     # copy of the best model by val score
+        self.best_loss_model  = None     # copy of the best model by val loss
+         
+        self.folder_loss   = None        # folder to save the best val loss models
+        self.folder_score  = None        # folder to save the best val score models
+        self.folder_checks = None        # folder to save checkpoints        
+
+        # -------------------------------- настройки для построения графиков ошибок и метрик
+        self.view = {                    
+            'w'            : 12,         # plt-plot width
+            'h'            :  5,         # plt-plot height
+            'count_units'  : 1e6,        # units for number of samples
+            'time_units'   : 's',        # time units: ms, s, m, h
+
+            'x_min'        : 0,          # minimum value in samples on the x-axis (if < 0 last x_min samples)
+            'x_max'        : None,       # maximum value in samples on the x-axis (if None - last)
+
+            'loss': {                                
+                'show'  : True,          # show loss subplot
+                'y_min' : None,          # fixing the minimum value on the y-axis
+                'y_max' : None,          # fixing the maximum value on the y-axis
+                'ticks' : None,          # how many labels on the y-axis
+                'lr'    : True,          # show learning rate
+                'labels': True,          # show labels (training events)                
+                'trn_checks': True,          # show the achievement of the minimum training loss (dots)
+                'val_checks': True,          # show the achievement of the minimum validation loss (dots)
+
+            },
+            'score': {                    
+                'show'  : True,          # show score subplot    
+                'y_min' : None,          # fixing the minimum value on the y-axis
+                'y_max' : None,          # fixing the maximum value on the y-axis
+                'ticks' : None,          # how many labels on the y-axis
+                'lr'    : True,          # show learning rate                
+                'labels': True,          # show labels (training events)
+                'trn_checks': True,      # show the achievement of the optimum training score (dots)                
+                'val_checks': True,      # show the achievement of the optimum validation score (dots)                
+            }
+        }
+
+        # -------------------------------- история и текущие метрики процесса обучения модели
+        self.hist = {                    # история обучения и валидации:
+            'samples': 0,                # число примеров в режиме обучения
+            'steps'  : 0,                # число шагов градиентного спуска
+
+            'time_trn': 0,               # общее время тренировки
+            'time_val': 0,               # общее время валидациии
+
+            'best':  {
+                'loss_val': None,        # лучшее значение валидационной ошибки
+                'loss_trn': None,        # лучшее значение тренировочная ошибки
+                'score_val': None,       # лучшее значение валидационной метрики (первой)
+                'score_trn': None,       # лучшее значение тенировочной метрики (первой)
+
+                'samples_loss_val': 0,   # когда была лучшая валидационная ошибка
+                'samples_loss_trn': 0,   # когда была лучшая тренировочная ошибка
+                'samples_score_val': 0,  # когда была лучшая валиадционная метрика
+                'samples_score_trn': 0,  # когда была лучшая тренировочная метрика
+            },
+
+            'trn'    : {'samples':[], 'steps':[], 'batch_size':[], 'lr':[], 'samples_epoch':[], 'steps_epoch':[], 'time':[], 'loss':[], 'score':[], 'best_loss':[], 'best_score':[] },
+            'val'    : {'samples':[], 'steps':[], 'batch_size':[], 'lr':[], 'samples_epoch':[], 'steps_epoch':[], 'time':[], 'loss':[], 'score':[], 'best_loss':[], 'best_score':[] },
+            'labels' : []
+        }    
+        self.hist['params'] = sum(p.numel() for p in model.parameters() if p.requires_grad)        
+
+    #---------------------------------------------------------------------------
+
+    def add_label(self, text):
+        """ Добавить пометку для графиков обучения """
+        h = self.hist
+        self.hist['labels'].append( [ text, h['samples'], h['steps'], h['time_trn'], h['time_val'] ] )
+
+    #---------------------------------------------------------------------------
+
+    def set_optimizer(self, optim):
+        """ Установить текущий оптимизатор """
+        self.optim = optim
+        self.set_optim_schedulers()
+
+    def set_optim_schedulers(self):
+        self.scheduler.optim = self.optim
+        for sch in self.schedulers:
+            sch.optim = self.optim
+
+    #---------------------------------------------------------------------------
+
+    def set_scheduler(self, scheduler):
+        self.schedulers = []
+        self.add_scheduler(scheduler)
+
+    def add_scheduler(self, scheduler):
+        scheduler.optim = self.optim
+        self.schedulers.append(scheduler)        
+
+    def del_scheduler(self, i):
+        self.schedulers.pop(i)
+
+    def clear_schedulers(self):
+        self.scheduler = Scheduler(self.optim)        
+        self.schedulers = []
+
+    def reset_schedulers(self):
+        for sch in self.schedulers:
+            sch.enable = True
+            sch.done   = 0
+
+    def stop_schedulers(self):
+        for sch in self.schedulers:
+            sch.enable = False            
+
+    def step_schedulers(self, samples_trn):
+        for sch in self.schedulers:
+            if sch.enable:
+                sch.step(samples_trn)
+                self.scheduler = sch
+                break
+
+    #---------------------------------------------------------------------------
+
+    def to_device(self, batch):
+        """ send mini-batch to device """        
+        if torch.is_tensor(batch):
+            return batch.to(self.device)
+        batch = list(batch)        
+        for i in range(len(batch)):
+            batch[i] = self.to_device(batch[i])
+        return batch
+
+    #---------------------------------------------------------------------------
+
+    def get_fun_step(self, model, train):
+        """ Получить функцию шага тренировки или dfkblfwbb """
+        fun_step = None
+        if train: 
+            if hasattr(model, "training_step"):            
+                fun_step = model.training_step
+        else:
+            if hasattr(model, "validation_step"):            
+                fun_step = model.validation_step
+            elif hasattr(model, "training_step"):            
+                fun_step = model.training_step
+
+        assert fun_step is not None, "model must has training_step function"
+        return fun_step
+
+    #---------------------------------------------------------------------------
+
+    def get_metrics(self, step):
+        """ из результатов шага обучения вделить ишибку и метрику"""
+        if torch.is_tensor(step):
+            loss   = step
+            scores = None
+        elif type(step) is dict:
+            loss  = step.get('loss')
+            scores = step.get('score')
+        if torch.is_tensor(scores) and scores.ndim == 1:
+            scores = scores.view(-1,1)
+        return loss, scores
+
+    #---------------------------------------------------------------------------
+
+    def samples_in_batch(self, batch):
+        """ сколько примров в батче """
+        if torch.is_tensor(batch):
+            return len(batch)
+        if type(batch) is list or type(batch) is tuple:
+            return self.samples_in_batch(batch[0]) 
+        assert False, "wrong type of the fist element in batch"
+    #---------------------------------------------------------------------------
+
+    def fit_epoch(self, epoch, model, data,  train=True, accumulate=1, verbose=1):
+        """
+        Args:
+            * train      - True: режим тренировки, иначе валидации
+            * accumulate - аккумулировать градиент для стольки батчей перед сдвигом оптимизатора;
+                           используем, когда большой батч или граф не помещаются в GPU
+        https://pytorch.org/blog/what-every-user-should-know-about-mixed-precision-training-in-pytorch/
+        """
+        self.model.train(train)                     # режим обучение или тестирование
+        torch.set_grad_enabled(train)               # строить или нет вычислительный граф
+
+        scaler = None
+        if torch.cuda.is_available() and self.dtype != torch.float32:
+            scaler = torch.cuda.amp.GradScaler()
+
+        if train:
+            self.optim.zero_grad()                  # обнуляем градиенты
+        
+        fun_step = self.get_fun_step(model, train)  # функция шага тренировки или валидации           
+
+        samples, steps, beg, lst = 0, 0, time.time(), time.time()
+        counts_all, losses_all,  scores_all = torch.empty(0,1), None,  None
+        for batch_id, batch in enumerate(data):    
+            num   = self.samples_in_batch(batch)
+            batch = self.to_device(batch)            
+
+            if scaler is None:
+                step = fun_step(batch, batch_id)                
+            else:
+                with torch.autocast(device_type=self.device, dtype=self.dtype):
+                    step = fun_step(batch, batch_id)
+            loss, scores = self.get_metrics(step)
+                
+            if train:
+                if scaler is None:
+                    loss.backward()   # вычисляем градиенты
+                else:
+                    scaler.scale(loss).backward()   # вычисляем градиенты
+                if (batch_id+1) % accumulate == 0:
+                    if scaler is None:
+                        self.optim.step()
+                    else:
+                        scaler.step(self.optim)     # подправляем параметры
+                        scaler.update()             # Updates the scale for next iteration
+                    self.optim.zero_grad()          # обнуляем градиенты
+                    steps      += 1                 # шагов за эпоху
+                    self.hist['steps'] += 1         # шагов за всё время
+                self.hist['samples'] += num         #  примеров за всё время
+
+            samples += num                          # просмотренных примеров за эпоху
+            losses_all = loss.detach() if losses_all is None else torch.vstack([losses_all, loss.detach()])
+            if scores is not None:
+                scores = scores.detach()
+                assert scores.ndim == 2, f"model must has tensor score in function metrics with dim==2, but got {scores.ndim}"
+                scores = scores.mean(dim=0)
+                scores_all = scores if scores_all is None else torch.vstack([scores_all, scores])
+            counts_all = torch.vstack([counts_all, torch.Tensor([num])])
+
+            if verbose and (time.time()-lst > 1 or batch_id+1 == len(data) ):
+                lst = time.time()
+                self.fit_progress(epoch, train, (batch_id+1)/len(data),
+                                  losses_all, scores_all, counts_all, samples, steps, time.time()-beg)
+
+        if train: self.hist['time_trn'] += (time.time()-beg)
+        else:     self.hist['time_val'] += (time.time()-beg)
+
+        if scores_all is not None:
+            scores_all = scores_all.cpu()
+        return losses_all.cpu(), scores_all, counts_all, (samples, steps, time.time()-beg)
+
+    #---------------------------------------------------------------------------
+
+    def mean(self, losses, scores, counts):
+        """ Вычислить среднее по всей эпохе """
+        loss  = ((losses.detach().cpu() * counts).sum(dim=0) / counts.sum()).item()
+        if scores is not None:
+            scores = ((scores.detach().cpu() * counts).sum(dim=0) / counts.sum())
+        return (loss, scores)
+
+    #---------------------------------------------------------------------------
+
+    def fit_progress(self, epoch, train, done, losses, scores, counts, samples, steps, tm):
+        """
+        Вывод информации о прогрессе обучения (эпоха, время, ошибка и т.п.)
+        В конкретном проекте можно перопределить.
+        """
+        loss, score = self.mean(losses, scores, counts)
+        steps, samples = max(steps, 0), max(samples, 1)             # just in case
+        st = ""
+        if score is not None and len(score):
+            st += f"score={score[0]:.4f} "                          # главная метрика
+            if len(score) > 1: st += "("                            # вспомогательные
+            for i in range(1, len(score)):
+                st += f"{score[i]:.4f}" + (", " if i+1 < len(score) else ") ")
+        st += f"loss={loss:.4f} "
+
+        t_unit, t_unit_scale,  c_unit, c_unit_power = self.unit_scales()
+        print(f"\r{epoch:3d}{'t' if train else 'v'}[{100*done:3.0f}%]  {st}  samples={samples} steps={steps}  time={(0.0 if steps==0 else 1e3*tm/(t_unit_scale*steps)):.3}{t_unit}/step  {c_unit*tm/(t_unit_scale*samples):.2f}{t_unit}/10^{c_unit_power:.0f}", end="                ")
+
+    #---------------------------------------------------------------------------
+
+    def unit_scales(self):
+        """ Единичы измерения числа примеров и времени """
+        view = self.view
+        t_unit = view['time_units'] if 'time_units' in view and view['time_units'] in ['ms','s','m','h']  else 's'
+        t_unit_scale = dict(ms=1e-3, s=1, m=60, h=3600)[t_unit]
+        c_unit = view['count_units'] if view.get('count_units',0) > 0  else 1
+        c_unit_power = round(np.log10(c_unit), 0)
+        return t_unit, t_unit_scale,  c_unit, c_unit_power
+
+    #---------------------------------------------------------------------------
+
+    def predict(self, model, data, verbose:bool = True, whole=False):
+        """
+        Вычислить предсказание, ошибку и метрику для каждого примера в data        
+        """
+        self.model.train(False)          # режим тестирование
+        torch.set_grad_enabled(False)    # вычислительный граф не строим
+        data.whole = whole               # обычно по всем примерам (и по дробному батчу)
+
+        assert hasattr(model, "predict_step"), "for method predict model must has method predict_step, witch return output tensor"
+
+        scaler = None
+        if torch.cuda.is_available() and self.dtype != torch.float32:
+            scaler = torch.cuda.amp.GradScaler()
+
+        samples, beg, lst = 0, time.time(), time.time()
+        output_all = None        
+        for batch_id, batch in enumerate(data):
+            num   = self.samples_in_batch(batch)
+            batch = self.to_device(batch)            
+
+            if scaler is None:
+                y_pred = model.predict_step(batch, batch_id)                                
+            else:
+                with torch.autocast(device_type=self.device, dtype=self.dtype):
+                    y_pred = model.predict_step(batch, batch_id)                    
+            
+            samples += num                      # число просмотренных примеров за эпоху            
+            output_all = y_pred.detach() if output_all is None else torch.vstack([output_all, y_pred.detach() ])            
+
+            if verbose and (time.time()-lst > 1 or batch_id+1 == len(data) ):
+                lst = time.time()
+                print(f"\r[{100*(batch_id+1)/len(data):3.0f}%]  {(time.time()-beg)/60:.2f}m", end=" ")                
+
+        return output_all.cpu()
+
+    #---------------------------------------------------------------------------
+
+    def fit(self,  epochs =None,  samples=None,            
+            pre_val:bool=False, period_val:int=1, period_plot:int=100,         
+            period_checks:int=1, period_val_beg:int = 4, samples_beg:int = None,
+            period_call:int = 0, callback = None): 
+        """
+        Args:
+            * epochs               - number of epochs for training (passes of one data_trn pack). If not defined (None) works "infinitely".
+            * samples              - if defined, then will stop after this number of samples, even if epochs has not ended
+            * pre_val              - validate before starting training
+            * period_val           - period after which validation run (in epochs)
+            * period_plot          - period after which the training plot is displayed (in epochs)
+            * period_call          - callback custom function call period
+            * callback             - custom function called with period_info
+            * period_checks        - period after which checkpoints are made and the current model is saved (in epochs)
+            * period_val_beg = 4   - validation period on the first samples_beg examples
+            * samples_beg = None   - the number of samples from the start, after which the validation period will be equal to period_val.
+        """
+        assert self.optim is not None, "Define the optimizer first"
+        self.set_optim_schedulers()        
+        self.model.to(self.device)
+        if pre_val:
+            losses, scores, counts, (samples_val, steps_val, tm_val) = self.fit_epoch(0, self.model, self.data_val, train=False)
+            loss_val, score_val = self.mean(losses, scores, counts)
+            self.add_hist(self.hist['val'], self.data_val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, self.scheduler.get_lr())
+            print()
+
+        epochs = epochs or 1_000_000
+        #for epoch in tqdm(range(1, epochs+1)):
+        for epoch in range(1, epochs+1):
+            losses, scores, counts, (samples_trn,steps_trn,tm_trn) = self.fit_epoch(epoch, self.model, self.data_trn, train=True)
+            loss_trn, score_trn = self.mean(losses, scores, counts)
+            lr = self.scheduler.get_lr()
+            self.add_hist(self.hist['trn'], self.data_trn.batch_size, samples_trn, steps_trn, tm_trn, loss_trn, score_trn, lr)
+
+            if self.hist['best']['loss_trn'] is None or self.hist['best']['loss_trn'] > loss_trn:
+                self.hist['best']['loss_trn'] = loss_trn
+                self.hist['best']['samples_loss_trn'] = self.hist['samples']
+                self.hist['trn']['best_loss'].append( (self.hist['samples'], self.hist['steps'], loss_trn) )
+
+            if self.best_score(self.hist['best']['score_trn'], score_trn):            
+                self.hist['best']['score_trn'] = score_trn[0]
+                self.hist['best']['samples_score_trn'] = self.hist['samples']
+                self.hist['trn']['best_score'].append((self.hist['samples'], self.hist['steps'], score_trn[0].item()))
+
+            period = period_val_beg if samples_beg and  self.hist['samples'] < samples_beg else period_val
+            if  (period and epoch % period == 0) or epoch == epochs:
+                losses, scores, counts, (samples_val,steps_val,tm_val) = self.fit_epoch(epoch, self.model, self.data_val, train=False)
+                loss_val, score_val = self.mean(losses, scores, counts)
+                self.add_hist(self.hist['val'], self.data_val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, lr)
+
+                # save best validation loss:
+                if self.hist['best']['loss_val'] is None or self.hist['best']['loss_val'] > loss_val:
+                    self.hist['best']['loss_val'] = loss_val
+                    self.hist['best']['samples_loss_val'] = self.hist['samples']
+                    self.hist['val']['best_loss'].append((self.hist['samples'], self.hist['steps'], loss_val))
+                    if self.folder_loss:
+                        self.save(self.model, folder=self.folder_loss, prefix=f"loss_{loss_val:.4f}_{self.now()}")
+                    if self.copy_best_loss_model:
+                        self.best_loss_model  = copy.deepcopy(self.model)
+                
+                if self.best_score(self.hist['best']['score_val'], score_val):
+                    self.hist['best']['score_val'] = score_val[0]
+                    self.hist['best']['samples_score_val'] = self.hist['samples']
+                    self.hist['val']['best_score'].append( (self.hist['samples'], self.hist['steps'], score_val[0].item()) )
+                    if self.folder_score:
+                        self.save(self.model, folder=self.folder_score, prefix=f"score_{score_val[0]:.4f}_{self.now()}")
+                    if self.copy_best_score_model:
+                        self.best_score_model  = copy.deepcopy(self.model)
+
+            if (period_plot and epoch % period_plot == 0) or epoch == epochs:
+                self.run_progress()        
+                plot_history(self.hist, self.view) 
+            
+            if callback and period_call and epoch % period_call == 0:                
+                callback()
+
+            if self.folder_checks and (epoch % period_checks == 0 or epoch == epochs):
+                self.save(self.model, folder=self.folder_checks, prefix="check_"+self.now())
+
+            self.step_schedulers(samples_trn)
+
+            if samples is not None:
+                samples -= samples_trn
+                if samples <= 0:
+                    self.run_progress()        
+                    plot_history(self.hist, self.view) 
+                    if callback:
+                        callback()
+                    break
+
+    #---------------------------------------------------------------------------
+
+    def run_progress(self):
+        print(f"\ntime = (trn:{self.hist['time_trn']/60:.2f}, val:{self.hist['time_val']/60:.2f}, tot:{(self.hist['time_trn']+self.hist['time_val'])/60:.2f})m  lr:{self.scheduler.get_lr():.1e}")
+    #---------------------------------------------------------------------------
+            
+    def best_score(self, best, score):
+        return score is not None  and len(score) \
+                and (best is None \
+                or (best < score[0] and     self.score_max) \
+                or (best > score[0] and not self.score_max) )
+
+    #---------------------------------------------------------------------------
+
+    def now(self):
+        return datetime.datetime.now().strftime("%m-%d %H:%M:%S")
+
+    #---------------------------------------------------------------------------
+
+    def add_hist(self, hist, batch_size, samples, steps, tm, loss, score, lr):
+            hist['samples']   .append(self.hist['samples'])
+            hist['steps']     .append(self.hist['steps'])
+            hist['samples_epoch']   .append(samples)
+            hist['steps_epoch']     .append(steps)
+            hist['batch_size'].append(batch_size)
+            hist['time']      .append(tm)
+            hist['lr']        .append(lr)
+            hist['loss']      .append(loss)
+            if score is not None and len(score):
+                hist['score'] .append(score[0].item())
+
+    #---------------------------------------------------------------------------
+
+    def save(self, fname, model = None, optim=None, info=""):
+        model = model or self.model
+        cfg = model.cfg
+        state = {
+            'info':            info,
+            'date':            datetime.datetime.now(),   # дата и время
+            'config':          cfg,                       # конфигурация модели
+            'model' :          model.state_dict(),        # параметры модели
+            'optimizer':       optim.state_dict() if optim is not None else None,
+            'hist':            self.hist,
+        }
+        torch.save(state, fname)
+
```

## Comparing `qunet/modules/transformer.py` & `qunet/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,511 +1,473 @@
-﻿import math, copy
+﻿"""
+Архитектуры:
+    * MLP               - полносвязная сеть с одним скрытм слоем  (B,*,n)  -> (B,*,m)
+    * CNN               - свёрточная сеть                         (B,C,H,W)-> (B,C',H',W')
+    * SelfAttention     - самовнимание (причинное или нет)        (B,T,E)  -> (B,T,E)
+    * TransformerBlock  - блок трансформера                       (B,T,E)  -> (B,T,E)
+    * PointsBlock       - блок повортора координат                (B,T,E)  -> (B,T,E)
+
+Обучение: (см. nnet_trainer)
+    * Data
+    * Trainer
+
+Полезно:
+    * nn.Bilinear       -  bilinear transformation:  x1 A x2 + b
+    * torchview         - https://github.com/mert-kurttutan/torchview
+
+См. примеры в конце файла в функции main
+                                                            (c) 2023 - QuData.com (steps)
+"""
+import os, math, copy, time, datetime
+import numpy as np, matplotlib.pyplot as plt
 import torch, torch.nn as nn
+from   tqdm.auto import tqdm
 
-from ..utils   import Config
-from .mlp      import MLP
+#========================================================================================
 
-#===============================================================================
-
-class SelfAttention(nn.Module):
+class MLP(nn.Module):
     """
-    Self Attention: (B,T,E) -> (B,T,E)
-    base on: https://github.com/karpathy/nanoGPT/blob/master/model.py
-    """
-    def __init__(self,  *args, **kvargs) -> None:
-        """
-        Self Attention: (B,T,E) -> (B,T,E)
+    Полносвязная сеть с одним или более скрытым слоем: (B,*, input) ->  (B,*, output).
+    Если слоёв более одного - cfg['hidden'] это list со списком числа нейронов в каждом слое
+    Скрытый слой может отсутствовать: hidden == 0 or == [] or stretch == 0,
+    тогда это обычный линейный слой input -> output без активационной функции
+    Пример:
+        mlp = MLP(dict(input=32, stretch=4, output=1))  # hidden = input*stretch
+        y = mlp( torch.randn(1, 32) )        
 
-        Args
-        ------------
-            E (int):
-                tokens embedding dimension
-            H (int):
-                number of heads (E % H == 0 !)
-            drop (float=0.0):
-                dropout probability
-            res (int=1):
-                kind of skip-connections (for TransformerBlock): (0) f(x) - none; (1) x+f(x), (2)  x*w+f(x) training one for all E; (3) training for each E
-            causal (bool=False):
-                kind of causal attention mask (True: GPT, False: BERT)
-            T_max (int=2048):
-                maximum number of tokens (needed for causal==True)
-
-        Example
-        ------------
-        ```
-        B, T, E, H = 1, 10, 128, 16
-        att = SelfAttention(E=E, H=H)
-        x = torch.rand(B,T,E)         # batch, tokens, embedding
-        y = att(x)                    # (B,T,E)
-        ```
-        """
+    """
+    def __init__(self, cfg) -> None:
         super().__init__()
-        self.cfg = SelfAttention.default()
-        self.cfg.set(*args, **kvargs)
-        self.create()
+        self.cfg = {
+            'input'   : 3,              # число входов  > 0
+            'output'  : 1,              # число выходов > 0
+            'hidden'  : None,           # число нейронов в скрытом слое (int или list)
+            'stretch' : 4,              # если есть, то hidden = int(stretch*input)            
+            'fun'     : 'gelu',         # активационная функция: gelu, relu, sigmoid, tanh
+            'drop'    : 0,              # dropout на выходе [0...1], если 0 - нет
+        }
+        if type(cfg) is dict:           # добавляем, меняем свойства
+            self.cfg.update(copy.deepcopy(cfg))
+        cfg = self.cfg
 
-    #---------------------------------------------------------------------------
+        assert 'hidden' in cfg or 'stretch' in cfg,   'no hidden/stretch in MLP: {cfg}'
+        assert cfg['input']>0  and cfg['output']>0, f'worng input/output in MLP: {cfg}'
 
-    def default():
-        return copy.deepcopy(Config(
-            E      = None,     # размерность эмбедига
-            H      = 1,        # число голов (E % H == 0 !)
-            res    = 1,        # kind of skip-connections (in TransformerBlock)
-            causal = False,    # причинное внимание (как в GPT) иначе как в BERT
-            T_max  = 2048,     # максимальное число токенов (нужно для causal==True)
-            drop   = 0,        # dropout на выходе внимания
-        ))
+        if type(cfg['hidden']) is list:
+            self.neurons = [cfg['input']] + cfg['hidden'] + [cfg['output']]
+        else:
+            if (cfg['hidden'] is None) and (cfg['stretch'] is not None) and cfg['stretch'] > 0:
+                cfg['hidden'] = int(cfg['stretch'] * cfg['input'])                    
+            assert cfg['hidden'] >= 0, f"worng hidden in MLP cfg: {cfg}: {type(cfg['hidden'])}"
+            if cfg['hidden'] > 0:
+                self.neurons = [cfg['input'], cfg['hidden'], cfg['output']]
+            else:
+                self.neurons = [cfg['input'], cfg['output']] 
+
+        cfg['fun']  = cfg.get('fun',  'gelu')      #  значения по умолчанию
+        cfg['drop'] = cfg.get('drop', 0)        
 
-    #---------------------------------------------------------------------------
+        self.create()
 
     def create(self):
-        cfg = self.cfg
-        assert cfg.E is not None and cfg.E > 0 and cfg.H > 0, f"must be E and H in cfg:{cfg.get_str()}"
-        assert cfg.E % cfg.H == 0,  "E must be div by H: {cfg.E} % {cfg.H} != 0"
+        cfg=self.cfg
 
-        T,E = cfg.T_max, cfg.E
+        seq = []
+        for i in range (1, len(self.neurons)):
+            seq += [ nn.Linear(self.neurons[i-1],  self.neurons[i]) ]
+            if i+1 < len(self.neurons):
+                if   cfg['fun'] == 'gelu':    seq += [ torch.nn.GELU() ]
+                elif cfg['fun'] == 'relu':    seq += [ torch.nn.ReLU() ]
+                elif cfg['fun'] == 'sigmoid': seq += [ torch.nn.Sigmoid() ]
+                elif cfg['fun'] == 'tanh':    seq += [ torch.nn.Tanh() ]
+                if cfg['drop'] > 0:
+                     seq += [ nn.Dropout(cfg['drop']) ]
 
-        self.c_attn = nn.Linear(E,3*E)  # key, query, value projections for all heads
-        self.c_proj = nn.Linear(E,  E)  # output projection
 
-        self.att_dropout  = nn.Dropout(cfg.drop)      # regularization
-        self.res_dropout  = nn.Dropout(cfg.drop)
+        self.layers = nn.Sequential(*seq)        
 
-        if cfg.causal:
-            # causal mask to ensure that attention is only applied to the left in the input sequence
-            self.register_buffer("bias", torch.tril(torch.ones(T, T)).view(1,1,T,T))
+    def forward(self, x):
+        x = self.layers(x)
+        return x
+
+#========================================================================================
+
+class CNN(nn.Module):
+    """
+    Свёрточная сеть: (B, C, H, W) ->  (B, C', H', W')
+    """
+    def __init__(self, cfg) -> None:
+        super().__init__()
+        self.cfg = {
+            'input'    : (1, 64, 64),   # input tensor shape:: (channels, height, width)
+            'output'   : None,          # output tensor shape;  sets in create()
+            'channel'  : [16,32,64],    # number of channels in each layer
+            'kernel'   : [3,3,3],       # int or list: size of the convolutional kernel
+            'stride'   : 1,             # int or list: stride of the convolutional kernel
+            'padding'  : 1,             # int or list: padding around the image
+            'pool_ker' : 2,             # int or list: max-pooling kernel
+            'pool_str' : 2,             # int or list: stride of max-pooling kernel
+            'drop'     : 0,             # int or list: dropout после каждого слоя            
+        }
+        if type(cfg) is dict:           # добавляем, меняем свойства
+            self.cfg.update(copy.deepcopy(cfg))
+        cfg = self.cfg
 
-    #---------------------------------------------------------------------------
+        n = len(cfg['channel'])
+        if type(cfg['drop'])     == int:   cfg['drop']     = [cfg['drop']]    * n
+        if type(cfg['kernel'])   == int:   cfg['kernel']   = [cfg['kernel']]  * n
+        if type(cfg['stride'])   == int:   cfg['stride']   = [cfg['stride']]  * n
+        if type(cfg['padding'])  == int:   cfg['padding']  = [cfg['padding']] * n
+        if type(cfg['pool_ker']) == int:   cfg['pool_ker'] = [cfg['pool_ker']]* n
+        if type(cfg['pool_str']) == int:   cfg['pool_str'] = [cfg['pool_str']]* n
+        if type(cfg['drop'])==float or type(cfg['drop'])==int: cfg['drop']=[cfg['drop']]*n
+        
+        self.create()
 
     def forward(self, x):
-        """ (B,T,E) -> (B,T,E) """
-        assert x.ndim == 3, f"wrong input x.ndim = {x.ndim}"
-        # batch size, sequence length, embedding dimensionality and number of heads:
-        (B,T,E), H = x.size(), self.cfg.H
-        assert E == self.cfg.E, f"wrong input {E} != {self.cfg.E}"
-
-        # calc (query, key, values) for all heads and move head forward to be the batch dim
-        q,k,v  = self.c_attn(x).split(E, dim=2)
-        k = k.view(B,T,H, E // H).transpose(1,2) # (B,H,T, hs) hs = E/nh
-        q = q.view(B,T,H, E // H).transpose(1,2) # (B,H,T, hs)
-        v = v.view(B,T,H, E // H).transpose(1,2) # (B,H,T, hs)
+        x = self.model(x)
+        return x
 
-        # causal self-attention; Self-attend: (B,H,T, hs) x (B,H, hs, T) -> (B,H,T,T)
-        att = (q @ k.transpose(-2, -1)) * (1.0 / math.sqrt(k.size(-1)))
-        if self.cfg.causal:  # заполняем верхний угол треугольной матрицы -inf
-            att = att.masked_fill(self.bias[:,:,:T,:T] == 0, float('-inf'))
-        att = torch.softmax(att, dim=-1)
-        att = self.att_dropout(att)
-        y = att @ v                          # (B,H,T,T) x (B,H,T,hs) -> (B,H,T,hs)
-        y = y.transpose(1,2).contiguous().view(B,T,E) # re-assemble all head side by side
+    def create(self):
+        c, w, h  =  self.cfg['input']
+        channels = [ c ] + self.cfg['channel']
+        layers = []
+        for i in range(len(channels)-1):
+            kernel, stride     = self.cfg['kernel']  [i], self.cfg['stride'][i]
+            padding            = self.cfg['padding'] [i]
+            pool_ker, pool_str = self.cfg['pool_ker'][i], self.cfg['pool_str'][i]
+
+            layers +=  [
+                nn.Conv2d(channels[i],channels[i+1], kernel_size=kernel, stride=stride, padding=padding),
+                nn.ReLU()]
+            h = int( (h + 2*padding - kernel) / stride + 1)
+            w = int( (w + 2*padding - kernel) / stride + 1)
+
+            if pool_ker > 1:
+                layers += [ nn.MaxPool2d(kernel_size=pool_ker, stride=pool_str) ]
+                h = int( (h - pool_ker) / pool_str + 1)
+                w = int( (w - pool_ker) / pool_str + 1)
 
-        # output projection
-        y = self.c_proj(y)
-        y = self.res_dropout(y)
-        return y                               # (B,T,E)
-
-    #---------------------------------------------------------------------------
-
-    def unit_test():
-        B, T, E, H = 1, 10, 128, 16
-        att = SelfAttention(E=E, H=H)
-        x = torch.rand(B,T,E)
-        y = att(x)
-        r1 = x.shape == y.shape
-        if not r1:
-            print(f"!! SelfAttention: x.shape={x.shape} != y.shape={y.shape}")
-
-        cfg = SelfAttention.default()(E=E)
-        att = SelfAttention(cfg)
-        y = att(x)
-        r2 = x.shape == y.shape
-        if not r2:
-            print(f"!! SelfAttention: x.shape={x.shape} != y.shape={y.shape}")
-
-        res = r1 and r2
-        if res:
-            print("ok SelfAttention")
-        return res
+            if self.cfg['drop'][i] > 0:
+                layers += [ nn.Dropout(p=self.cfg['drop'][i]) ]
+
+        self.cfg['output'] =  (channels[-1], w, h)
+        self.model =  nn.Sequential(*layers)
 
 #===============================================================================
 
-class FFT(nn.Module):
+class SelfAttention(nn.Module):
     """
-    FFT Block from FNet (see: "FNet: Mixing Tokens with Fourier Transforms")
+    Основан на: https://github.com/karpathy/nanoGPT/blob/master/model.py
     """
-    def __init__(self,  *args, **kvargs) -> None:
-        """
-        FFT Block from FNet (see: "FNet: Mixing Tokens with Fourier Transforms")
-
-        Args:
-        ------------
-            drop (float = 0.0)
-                dropout after fft
-            res (int = 1):
-                kind of skip-connections (for TransformerBlock): (0) f(x) - none; (1) x+f(x), (2)  x*w+f(x) training one for all E; (3) training for each E
-            after (int = 1)
-                after fft2: (1) take Re, (2) take Im, (3) Re**2+Im**2
-
-        Example
-        ------------
-        ```
-        B, T, E = 1, 10, 128
-        fft = FFT()
-        x = torch.rand(B,T,E)         # batch, tokens, embedding
-        y = fft(x)                    # (B,T,E)
-        ```
-        """
+    def __init__(self, cfg):
+        # cfg: emb, heads, tokens, causal, drop_attn
         super().__init__()
-        self.cfg = FFT.default()
-        self.cfg.set(*args, **kvargs)
+        self.cfg =  {
+            'emb'    : 64,              # размерность эмбедига
+            'heads'  : 8,               # число голов (emb % heads == 0 !)
+            'causal' : False,           # причинное внимание (как в GPT) иначе как в BERT
+            'tokens' : 2048,            # максимальное число тоенов (нужно для causal==True)
+            'drop'   : 0,               # dropout на выходе внимания
+        }
+        if type(cfg) is dict:           # добавляем, меняем свойства
+            self.cfg.update(copy.deepcopy(cfg))
+        cfg = self.cfg
+        
+        assert 'emb' in cfg and 'heads' in cfg, f"must be emb and heads in cfg:{cfg}"
+        assert cfg['emb'] % cfg['heads'] == 0,  "emb must be div by heads!"
+        cfg['causal'] = cfg.get('causal', False)
+        cfg['tokens'] = cfg.get('tokens', 2048)
+        cfg['drop']   = cfg.get('drop',   0)
+        
         self.create()
 
-    #---------------------------------------------------------------------------
-
-    def default():
-        return copy.deepcopy(Config(
-            res   = 1,         # kind of skip-connections (in TransformerBlock)
-            drop  = 0,         # dropout на выходе внимания
-            after = 1,         # после fft2: 1 - брать Re, 2 брать Im, 3 Re**2+Im**2
-        ))
-
-    #---------------------------------------------------------------------------
-
     def create(self):
         cfg = self.cfg
-        self.drop  = nn.Dropout(cfg.drop)
+        T,E = cfg['tokens'], cfg['emb']
 
-    #---------------------------------------------------------------------------
+        self.c_attn = nn.Linear(E,3*E)  # key, query, value projections for all heads
+        self.c_proj = nn.Linear(E,  E)  # output projection
 
-    def forward(self, x):                      # (B,T,E)
-        x = torch.fft.fft2(x)
-        if self.cfg.after   == 1:
-            x = x.real
-        elif self.cfg.after == 2:
-            x = x.imag
-        else:
-            x = x.real.pow(2) + x.imag.pow(2)
+        self.attn_dropout  = nn.Dropout(cfg['drop'])      # regularization
+        self.resid_dropout = nn.Dropout(cfg['drop'])
 
-        x = self.drop(x)
-        return x                               # (B,T,E)
+        if cfg['causal']:
+            # causal mask to ensure that attention is only applied to the left in the input sequence
+            self.register_buffer("bias", torch.tril(torch.ones(T, T)).view(1,1,T,T))
+        self.heads  = cfg['heads']
+        self.emb    = cfg['emb']
+        self.causal = cfg['causal']
+
+    def forward(self, x):  # (B,T,E)
+        B,T,E = x.size() # batch size, sequence length, embedding dimensionality (emb)
+        assert E == self.emb, "wrong input"
+
+        # calculate query, key, values for all heads in batch and move head forward to be the batch dim
+        q,k,v  = self.c_attn(x).split(self.emb, dim=2)
+        k = k.view(B,T, self.heads, E // self.heads).transpose(1,2) # (B, nh, T, hs) hs = E/nh
+        q = q.view(B,T, self.heads, E // self.heads).transpose(1,2) # (B, nh, T, hs)
+        v = v.view(B,T, self.heads, E // self.heads).transpose(1,2) # (B, nh, T, hs)
 
-    #---------------------------------------------------------------------------
+        # causal self-attention; Self-attend: (B, nh, T, hs)x(B, nh, hs, T) -> (B, nh, T,T)
+        att = (q @ k.transpose(-2, -1)) * (1.0 / math.sqrt(k.size(-1)))
+        if self.causal:  # заполняем верхний угол треугольной матрицы -inf
+            att = att.masked_fill(self.bias[:,:,:T,:T] == 0, float('-inf'))
+        att = torch.softmax(att, dim=-1)
+        att = self.attn_dropout(att)
+        y = att @ v                          # (B, nh, T, T) x (B, nh, T, hs) -> (B, nh, T, hs)
+        y = y.transpose(1, 2).contiguous().view(B,T,E) # re-assemble all head outputs side by side
 
-    def unit_test():
-        B, T, E = 1, 10, 128
-        fft = FFT()
-        x = torch.rand(B,T,E)
-        y = fft(x)
-        res = x.shape == y.shape
-        if not res:
-            print(f"!! FFT: x.shape={x.shape} != y.shape={y.shape}")
-        else:
-            print("ok FFT")
-        return res
+        # output projection
+        y = self.resid_dropout(self.c_proj(y))
+        return y            # (B,T,E)
 
 #===============================================================================
 
-
 class  TransformerBlock(nn.Module):
-    """
-    One Transformer Block (it is all you need: fft, attention, mlp)
-    """
-    def __init__(self,  *args, **kvargs) -> None:
-        """
-        One Transformer Block (it is all you need: fft, attention, mlp)
-
-        Args
-        ------------
-            E (int):
-                tokens embedding dimension
-            H (int=1):
-                number of heads (E % H == 0 !)
-            drop (float=0.0):
-                dropout probability in attention and mlp
-            res (int=1):
-                kind of skip-connections: (0) f(x) - none; (1) x+f(x), (2)  x*w+f(x) training one for all E; (3) training for each E
-            causal (bool=False):
-                kind of causal attention mask (True: GPT, False: BERT)
-            T_max (int=2048):
-                maximum number of tokens (needed for causal==True)
-
-        Example
-        ------------
-        ```
-        B, T, E, H = 1, 10, 128, 16
-        block = TransformerBlock(E=E, H=H)
-        x = torch.rand(B,T,E)
-        y = block(x)
-        ```
-        """
+    def __init__(self, cfg, created=True):
         super().__init__()
-        self.cfg = TransformerBlock.default()
-        self.cfg.set(*args)
-
-        # мы можем одним аргументом задать параметры в att и mlp
-        if 'E' in kvargs:
-            self.cfg.att.E      = kvargs['E']
-            self.cfg.mlp.input  = kvargs['E']
-            self.cfg.mlp.output = kvargs['E']
-
-        if 'H' in kvargs:
-            self.cfg.att.H = kvargs['H']
-
-        if 'res' in kvargs:
-            self.cfg.att.res = kvargs['res']
-            self.cfg.mlp.res = kvargs['res']
-            self.cfg.fft.res = kvargs['res']
-
-        if 'drop' in kvargs:
-            self.cfg.att.drop = kvargs['drop']
-            self.cfg.mlp.drop = kvargs['drop']
-            self.cfg.fft.drop = kvargs['drop']
-
-        if 'causal' in kvargs:
-            self.cfg.att.causal = kvargs['causal']
-
-        if 'T_max'  in kvargs:
-            self.cfg.att.T_max = kvargs['T_max']
-
-        if 'is_fft'  in kvargs:
-            self.cfg.is_fft = kvargs['is_fft']
-        if 'is_att'  in kvargs:
-            self.cfg.is_att = kvargs['is_att']
-        if 'is_mlp'  in kvargs:
-            self.cfg.is_mlp = kvargs['is_mlp']
-
-        self.create()
-
-    #---------------------------------------------------------------------------
-
-    def default():
-        return copy.deepcopy(Config(
-            is_fft = 0,
-            is_att = 1,
-            is_mlp = 1,
-            att = SelfAttention.default(),
-            mlp = Config(MLP.default(), stretch=4, res=1),
-            fft = FFT.default(),
-        ))
+        self.cfg = {
+            'emb'             : 64,      # размерность эмбедига
+            'res'             : 1,       # skip-connections (0-нет, 1-обычные, 2-тренеруемый, 3-покомпонентно)
+            'att': {
+                'heads'       : 1,       # число голов (emb % heads == 0 !)
+                'causal'      : False,   # причинное внимание (как в GPT) иначе как в BERT
+                'tokens'      : 1024,    # максимальное число тоенов (нужно для causal==True)
+                'drop'        : 0,       # dropout на выходе внимания
+            },
+            'mlp': {
+                'stretch'     : 4,       # увеличение от эбединга скрытого слоя (2,4,..): hidden=emb*scale
+                'drop'        : 0,       # dropout на выходе mlp
+                'fun'         : 'gelu',  # активационная MLP-функция: 'gelu','relu','sigmoid','tanh'
+            }
+        }
+        if type(cfg) is dict:            # добавляем, меняем свойства
+            self.cfg.update(copy.deepcopy(cfg))
+        cfg = self.cfg
 
-    #---------------------------------------------------------------------------
+        assert 'emb' in cfg,  "Must be emb in TransformerBlock cfg"
+        cfg['res']            = cfg.get('res', 2)
+        cfg['att']            = cfg.get('att', {})
+        cfg['att']['emb']     = cfg['emb']
+        cfg['att']['drop']    = cfg['att'].get('drop',  0)
+
+        cfg['mlp']            = cfg.get('mlp', {})
+        cfg['mlp']['input']   = cfg['emb']
+        cfg['mlp']['output']  = cfg['emb']
+        cfg['mlp']['stretch'] = cfg['mlp'].get('stretch', 4)
+        cfg['mlp']['fun']     = cfg['mlp'].get('fun',  'gelu')
+        cfg['mlp']['drop']    = cfg['mlp'].get('drop',  0)
+        
+        if created:
+            self.create()
 
     def create(self):
         cfg = self.cfg
-        assert cfg.att.E is not None and cfg.att.E > 0 and cfg.att.E == cfg.mlp.input and cfg.mlp.input == cfg.mlp.output,  f"TransformerBlock: embedding needs to be defined: E={cfg.E}, input={cfg.mlp.input}, output={cfg.mlp.output}"
-
-        if cfg.is_fft:
-            self.ln_0 = nn.LayerNorm (cfg.att.E)
-            self.fft = FFT(cfg.fft)
-
-            cfg.fft.res = max(0, min(3, cfg.fft.res))
-            if   cfg.fft.res == 3:     # training multiplier for each components
-                self.w_fft = nn.Parameter( torch.ones( cfg.att.E ) )
-            elif cfg.fft.res == 2:     # training common multiplier
-                self.w_fft   = nn.Parameter( torch.ones(1) )
-            else:                      # constant multiplayer   (0 or 1)
-                self.register_buffer("w_fft", torch.tensor(float(cfg.fft.res)))
-
-
-        if cfg.is_att:
-            self.ln_1 = nn.LayerNorm (cfg.att.E)
-            self.att  = SelfAttention(cfg.att)
-
-            cfg.att.res = max(0, min(3, cfg.att.res))
-            if   cfg.att.res == 3:     # training multiplier for each components
-                self.w_att = nn.Parameter( torch.ones( cfg.att.E ) )
-            elif cfg.att.res == 2:     # training common multiplier
-                self.w_att   = nn.Parameter( torch.ones(1) )
-            else:                      # constant multiplayer (0 or 1)
-                self.register_buffer("w_att", torch.tensor(float(cfg.att.res)))
-
-
-        if cfg.is_mlp:
-            self.ln_2 = nn.LayerNorm(cfg.att.E)
-            self.mlp  = MLP(cfg.mlp)
-
-            cfg.mlp.res = max(0, min(3, cfg.mlp.res))
-            if   cfg.mlp.res == 3:     # training multiplier for each components
-                self.w_mlp = nn.Parameter( torch.ones( cfg.att.E ) )
-            elif cfg.mlp.res == 2:     # training common multiplier
-                self.w_mlp   = nn.Parameter( torch.ones(1) )
-            else:                      # constant multiplayer   (0 or 1)
-                self.register_buffer("w_mlp", torch.tensor(float(cfg.mlp.res)))
+        self.ln_1 = nn.LayerNorm (cfg['emb'])
+        self.att  = SelfAttention(cfg['att'])
 
-    #---------------------------------------------------------------------------
+        self.mlp = None
+        if cfg['mlp']['stretch'] > 0:
+            self.ln_2 = nn.LayerNorm(cfg['emb'])
+            self.mlp  = MLP(cfg['mlp'])
+
+        if   cfg['res'] == 3:     # train multiplier for each components
+            self.w_att = nn.Parameter( torch.ones( cfg['emb'] ) )
+            self.w_mlp = nn.Parameter( torch.ones( cfg['emb'] ) )
+        elif cfg['res'] == 2:     # train common multiplier
+            self.w_att   = nn.Parameter( torch.ones(1) )
+            self.w_mlp   = nn.Parameter( torch.ones(1) )
+        else:                     # constant multiplayer
+            self.register_buffer("w_att", torch.Tensor(cfg['res']))
+            self.register_buffer("w_mlp", torch.Tensor(cfg['res']))
 
-    def forward(self, x):
+    def forward(self, x):                          # (B,T,E)
         """
-        (B,T,E) -> (B,T,E)
         Классический highway: w=sigmoid(linear(x)); x*w + (1-w)*mlp, ...
         не работал для нейтрино. Возможно это негативный эффект постоянного
         умножения x (и потом градиента) на число меньшее 1:  x*0.5*0.5*...
-        Не работал также linear(x) + mlp, с начальной единичной матрицей :(
-
-        Карпатов сделал ln на входе, хотя многие рисуют на выходе.
-        Это сказывается тоько на первом и последнем блоке.
-        Наверное как у Карпатова правильнее (нормируем перед вычислениями).
+        Не работал также linear(x) + mlp, с наяальной единичной матрицей :(
         """
-        if self.cfg.is_fft:
-            x = x * self.w_fft + self.fft(self.ln_0(x))
-        if self.cfg.is_att:
-            x = x * self.w_att + self.att(self.ln_1(x))
-        if self.cfg.is_mlp:
-            x = x * self.w_mlp + self.mlp(self.ln_2(x))
-        return x                                            # (B,T,E)
-
-    #---------------------------------------------------------------------------
-
-    def unit_test():
-        B, T, E, H = 1, 10, 128, 16
-        block = TransformerBlock(E=E, H=H)
-        x = torch.rand(B,T,E)
-        y = block(x)
-        res = x.shape == y.shape
-        if not res:
-            print(f"!! TransformerBlock: x.shape={x.shape} != y.shape={y.shape}")
-        else:
-            print("ok TransformerBlock")
-        return res
+        x = x * self.w_att + self.att(self.ln_1(x))
+        x = x * self.w_mlp + self.mlp(self.ln_2(x))
+        return x                                  # (B,T,E)
+
 
 #===============================================================================
 
 class  Transformer(nn.Module):
-    """
-    Transformer is all you need (fft, attention, mlp)
-    """
-    def __init__(self,  *args, **kvargs) -> None:
-        """
-        Transformer is all you need (fft, attention, mlp)
-
-        Args
-        ------------
-            E (int):
-                tokens embedding dim
-            H (int):
-                number of heads E % H == 0 !
-            n_blocks (int=1):
-                number of transformer blocks
-            drop: (float=0.0):
-                dropout in attention and mlp
-            res (int=1):
-                kind of skip-connections: (0) f(x) - none; (1) x+f(x), (2)  x*w+f(x) training one for all E; (3) training for each E
-            causal (bool=False):
-                kind of causal attention mask (True: GPT, False: Bert)
-            T_max  (int=2048):
-                maximum number of tokens (needed for causal==True)
-            is_mix (int=0):
-                will be
-            is_fft (int=0):
-                there is a FFT (FNet) block, can be a list (for each block)
-            is_att  (int=1):
-                there is an attention block, can be a list (for each block)
-            is_mlp  (int=1):
-                there is an MLP block, can be a list (for each block)
-
-        Example:
-        ------------
-        ```
-        m = Transformer(E=64, H=8, n_blocks=3, is_fft=[1,1,0], is_att=[0,0,1])
-
-        x = torch.rand(1,10,64)  # (B,T,E) = (batch, token, embedding)
-        y = m(x)                 # (B,T,E) -> (B,T,E)
-        ```
-        """
+    def __init__(self, cfg, created=True):
         super().__init__()
-        self.cfg = Transformer.default()
-        self.cfg.set(*args)
+        self.cfg = {                     # остальные параметры в TransformerBlock
+            'L' : 1,                     # число слоёв трансформера 
+        }
+        if type(cfg) is dict:            # добавляем, меняем свойства
+            self.cfg.update(copy.deepcopy(cfg))
+        if created:
+            self.create()
 
-        # В set не передаём kvargs, чтобы не было ворнингов по E, H и т.д.
-        if 'n_blocks' in kvargs:
-            self.cfg.n_blocks      = kvargs['n_blocks']
-        if 'is_fft' in kvargs:
-            self.cfg.is_fft      = kvargs['is_fft']
-        if 'is_att' in kvargs:
-            self.cfg.is_att      = kvargs['is_att']
-        if 'is_mlp' in kvargs:
-            self.cfg.is_mlp      = kvargs['is_mlp']
-
-        # одним аргументом задаём параметры в fft, att и mlp всех блоков
-        if 'E' in kvargs:
-            self.cfg.block.att.E      = kvargs['E']
-            self.cfg.block.mlp.input  = kvargs['E']
-            self.cfg.block.mlp.output = kvargs['E']
-
-        if 'H' in kvargs:
-            self.cfg.block.att.H = kvargs['H']
-
-        if 'res' in kvargs:
-            self.cfg.block.fft.res = kvargs['res']
-            self.cfg.block.att.res = kvargs['res']
-            self.cfg.block.mlp.res = kvargs['res']
-
-        if 'drop' in kvargs:
-            self.cfg.block.fft.drop = kvargs['drop']
-            self.cfg.block.att.drop = kvargs['drop']
-            self.cfg.block.mlp.drop = kvargs['drop']
+    def create(self):
+        self.blocks= nn.ModuleList([TransformerBlock(self.cfg) for _ in range(self.cfg['L'])])
 
-        if 'after' in kvargs:
-            self.cfg.block.fft.after = kvargs['after']
+    def forward(self, x):                          # (B,T,E)
+        for i, block in enumerate(self.blocks):  
+            #if CFG.frozen and self.training and i > CFG.L_frozen: torch.set_grad_enabled(True) 
+            x = block(x)                         # (B,T,E)            
+        return x
 
-        if 'causal' in kvargs:
-            self.cfg.block.att.causal = kvargs['causal']
+#===============================================================================
 
-        if 'T_max'  in kvargs:
-            self.cfg.block.att.T_max = kvargs['T_max']
+class  PointsBlock(nn.Module):
+    def __init__(self, cfg):
+        super().__init__()
+        self.cfg = {
+            'emb'             : 64,      # размерность эмбедига
+            'max'             : False,
+            'mean'            : True,
+            'res'             : 1,       # residual петли (0-нет, 1-обычные, 2-тренеруемые)
+            'mlp1': {
+                'stretch'     : 4,       # увеличение от эбединга скрытого слоя (2,4,..): hidden=emb*scale
+                'drop'        : 0,       # dropout на выходе mlp
+            },
+            'mlp2': {
+                'stretch'     : 4,       # увеличение от эбединга скрытого слоя (2,4,..): hidden=emb*scale
+                'drop'        : 0,       # dropout на выходе mlp
+            }
+        }
+        if type(cfg) is dict:            # добавляем, меняем свойства
+            self.cfg.update(copy.deepcopy(cfg))
+        cfg = self.cfg
+        
 
+        cfg['mean'] = cfg.get('mean', True)
+        cfg['max']  = cfg.get('max', False)
+        cfg['res']  = cfg.get('res', 2)
+        assert cfg['mean'] or cfg['max'], f"PointsBlock need mean or/and max, cfg={cfg}"
+
+        cfg['mlp1'] = cfg.get('mlp1', {})
+        cfg['mlp2'] = cfg.get('mlp2', {})
+        cfg['mlp1']['stretch'] = cfg['mlp1'].get('stretch', 4)
+        cfg['mlp2']['stretch'] = cfg['mlp2'].get('stretch', 4)
+        
         self.create()
 
-    #---------------------------------------------------------------------------
-
-    def default():
-        return copy.deepcopy(Config(
-            n_blocks  = 1,     # число слоёв трансформера
-            is_fft    = 0,     # there is a FFT (FNet) block, can be a list (for each block)
-            is_att    = 1,     # there is an attention block, can be a list (for each block)
-            is_mlp    = 1,     # there is an MLP block, can be a list (for each block)
-            block = TransformerBlock.default()
-        ))
-
-    #---------------------------------------------------------------------------
-
     def create(self):
         cfg = self.cfg
-        is_fft = [cfg.is_fft] * cfg.n_blocks  if type(cfg.is_fft) is int else cfg.is_fft
-        is_att = [cfg.is_att] * cfg.n_blocks  if type(cfg.is_att) is int else cfg.is_att
-        is_mlp = [cfg.is_mlp] * cfg.n_blocks  if type(cfg.is_mlp) is int else cfg.is_mlp
-        assert type(is_fft) is list and type(is_att) is list and type(is_mlp) is list, "Transformer: is_fft, is_att, is_mlp should be int or list of int"
-        assert len(is_fft) == len(is_att) and len(is_fft) == len(is_mlp), "Transformer: if is_fft, is_att, is_mlp are lists, their length should be the same"
-
-        blocks = []
-        for i in range(cfg.n_blocks):
-            block = TransformerBlock(self.cfg.block, is_fft=is_fft[i], is_att=is_att[i], is_mlp=is_mlp[i])
-            blocks.append(block)
-        self.blocks= nn.ModuleList(blocks)
+        E, E2 = cfg['emb'], cfg['emb']
+        self.ln_1 = nn.LayerNorm(E)
+        self.ln_2 = nn.LayerNorm(E)
+
+        n_cat = 2 if cfg['max'] and cfg['mean'] else 1
+        self.mlp_1 = MLP(dict(input=E, stretch=cfg['mlp1']['stretch'], output=E2))
+        self.fc_w  = nn.Linear(n_cat*E2, E*E)
+        self.fc_b  = nn.Linear(n_cat*E2, E)
+        self.mlp_2 = MLP(dict(input=E, stretch=cfg['mlp1']['stretch'], output=E))
+
+        if cfg['res'] == 2:
+            self.w_1   = nn.Parameter( torch.ones(1) )
+            self.w_2   = nn.Parameter( torch.ones(1) )
+        else:
+            self.w_1   = cfg['res']
+            self.w_2   = cfg['res']
 
-    #---------------------------------------------------------------------------
+        self.E       = E
+        self.is_max  = cfg['max']
+        self.is_mean = cfg['mean']
+
+
+    def forward(self, x):                                       # (B,T, E)
+        x = self.ln_1(x)                                        # (B,T, E)
+        y = self.mlp_1(x)                                       # (B,T, E')
+        agg = []
+        if self.is_mean:
+            agg.append( y.mean(dim=1) )
+        if self.is_max:
+            agg.append( y.max(dim=1)[0] )
+        y = torch.cat(agg, dim=1)                               # (B, n_cat*E')
+        w = self.fc_w(y).view(-1,self.E, self.E)                # (B, E*E) -> (B, E,E)
+        b = self.fc_b(y)[:,None,:]                              # (B, E)   -> (B, 1,E)
+
+        y = nn.Gelu()(torch.bmm(x, w) + b)                      # (B,T,E) @ (B,E,E) + (B,1,E) = (B,T,E)
+        y = y + x * self.w_1                                    # (B,T, E)
+        #y = gelu(y)
+
+        x = self.ln_2(y)                                        # (B,T, E)
+        y = self.mlp_2(x)
+        y = y  + x * self.w_2                                   # (B,T, E)
+        #y = gelu(y)
+        return y                                                # (B,T, E)
 
-    def forward(self, x):
-        """  (B,T,E) -> (B,T,E) """
-        for block in self.blocks:
-            x = block(x)                           # (B,T,E)
-        return x
+#===============================================================================
+#                                Main (Test)
+#===============================================================================
 
-    #---------------------------------------------------------------------------
+if __name__ == '__main__':
+    from torchinfo import summary
+    from torchview import draw_graph
+
+    print("*********************************************************************")
+    """
+    Пример создания блоков:
+    """
+    #tests = ['mlp','cnn', 'att', 'trf', 'pnt']
+    tests = []
+
+    if True:
+        trf = Transformer(dict(emb=3, res=1, L=5))
+        summary(trf)
+        print(trf.cfg)
+        print(trf.blocks[0].cfg)
+        B, T, E = 1, 10, trf.cfg['emb']
+        X = torch.empty( (B,T,E) )        
+        Y = trf(X)
+        print(X.shape,"->",Y.shape)
+        #model_graph = draw_graph(trf, input_size=(B,T,E), device='meta')
+        #model_graph.visual_graph
+
+
+    if 'mlp' in tests:
+        mlp = MLP(dict(input=32, hidden=[128, 64], output=1, drop=0.1))
+        summary(mlp)
+        print(mlp.cfg)
+
+    if 'cnn' in tests:
+        cnn = CNN(None)
+        summary(cnn)
+        print(cnn.cfg)
+        X = torch.empty( (1,) + cnn.cfg['input'])
+        Y = cnn(X)
+        print(X.shape,"->",Y.shape)
+
+    if 'att' in tests:
+        att = SelfAttention(dict(emb=128, heads=4))    # остальные параметры будут по умолчанию
+        print(att.cfg)
+        B, T, E = 13, 10, att.cfg['emb']
+        X = torch.empty( (B,T,E) )
+        Y = att(X)
+        print(X.shape,"->",Y.shape)
+        summary(att, input_data=X, col_width=16, depth=5, col_names=["input_size", "output_size", "num_params", "trainable"])
+
+    if 'trf' in tests:
+        trf = TransformerBlock(None, False)
+        trf.cfg['res'] = 3
+        trf.cfg['mlp']['stretch'] = 2         # меняем параметры по умолчанию
+        trf.create()                          # пересоздаём модель
+        summary(trf)
+        print(trf.cfg)
+        B, T, E = 1, 10, trf.cfg['emb']
+        X = torch.empty( (B,T,E) )
+        Y = trf(X)
+        print(X.shape,"->",Y.shape)
+        #model_graph = draw_graph(trf, input_size=(B,T,E), device='meta')
+        #model_graph.visual_graph
+
+    if 'pnt' in tests:
+        pnt = PointsBlock(dict(emb=64))
+        summary(pnt, depth=5)
+        print(pnt.cfg)
+        B, T, E = 18, 13, pnt.cfg['emb']
+        X = torch.empty( (B,T,E) )
+        Y = pnt(X)
+        print(X.shape,"->",Y.shape)
 
-    def unit_test():
-        B, T, E, H = 1, 10, 128, 16
-        m = Transformer(E=E, H=H, n_blocks=3, is_fft=[1,1,0], is_att=[0,0,1])
-        x = torch.rand(B,T,E)  # (B,T,E) = (batch, token, embedding)
-        y = m(x)               # (B,T,E) -> (B,T,E)
-
-        #for block in m.blocks: print(block.cfg)
-
-        res = x.shape == y.shape
-        if not res:
-            print(f"!! Transformer: x.shape={x.shape} != y.shape={y.shape}")
-        else:
-            print("ok Transformer")
-        return res
 
-#===============================================================================
```

## Comparing `qunet/optim/scheduler.py` & `qunet/optim.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,112 +8,74 @@
 #                                   Shedulers
 #===============================================================================
 
 class Scheduler:
     def __init__(self) -> None:
         self.optim  = None
         self.enable = False        
-        self.done_samples = 0
-        self.done_epochs  = 0
+        self.done   = 0
         self.lr     = 0
 
-    #---------------------------------------------------------------------------
-
-    def set(self, lr1=None, lr2=None, epochs=None, samples=None,  enable=True):                
-        assert samples is not None or epochs is not None, f"You should define samples:{samples} or  epochs:{epochs}"
-        assert samples is None or samples > 1,  f"Wrong samples={samples} limits in Scheduler"        
-        assert epochs  is None or epochs  > 1,  f"Wrong epochs ={epochs}  limits in Scheduler"        
-
-        self.lr1     = lr1
-        self.lr2     = lr2    
-        self.epochs  = epochs
-        self.samples = samples                
+    def set(self, lr1=None, lr2=None, samples=1e3, enable=True):        
+        self.lr1 = lr1
+        self.lr2 = lr2    
+        assert samples > 1,  "wrong samples limits in Scheduler"
+        self.samples = samples        
         self.enable  = enable
-
-        self.done_epochs  = 0
-        self.done_samples = 0                
-
+        self.done    = 0
         if enable:
             self.set_lr(self.lr1)
 
-    #---------------------------------------------------------------------------
-
     def set_lr(self, lr):
-        if self.optim is not None and lr is not None:
+        if self.optim is not None:
             for g in self.optim.param_groups:
                 g['lr'] = lr
-
-    #---------------------------------------------------------------------------
-
+        
     def get_lr(self):        
         if self.optim is None:
             return self.lr
         else:
             return self.optim.param_groups[0]['lr']    # а если не одна группа?
 
-    #---------------------------------------------------------------------------
-
-    def done(self, new_epochs, new_samples):
-        if not self.enable:
-            return True
-        
-        self.done_epochs  += new_epochs
-        self.done_samples += new_samples
-
-        if self.epochs is not None and self.done_epochs >= self.epochs:               
-            self.enable = False
-            return True
-
-        if self.samples is not None and self.done_samples >= self.samples:               
-            self.enable = False
-            return True
-
-        return False
-
-    #---------------------------------------------------------------------------
-
-    def step(self, epochs, samples):
+    def step(self, samples):
         if self.enable:
             if self.lr1 is None:
                 self.lr1 = self.get_lr()
             if self.lr2 is None:
                 self.lr2 = self.get_lr()
+            assert self.lr1 >= 0 and self.lr2 >= 0, "wrong lr limits in Scheduler"                
 
-            assert self.lr1 >= 0 and self.lr2 >= 0, f"Wrong lr1={self.lr1} or lr2={self.lr2} limits in Scheduler"                
-
-            self.lr = self.new_lr(epochs, samples)
+            self.lr = self.new_lr(samples)
             self.set_lr(self.lr)
         return self.lr
 
-    #---------------------------------------------------------------------------
-
     def plot(self, samples=1000, epochs = 100,  log=True, w=8, h=5, title=""):    
         """ 
         Draw a learning curve for `samples` passed over `epochs` epochs 
         Args:
             * samples - number of examples the optimizer must pass
-            * epochs  - number of `epochs` (optimizer steps)
+            * epochs - number of `epochs` (optimizer steps)
             * log - logarithmic y-axis scale
             * w  - chart width
             * h  - chart height
             * title - chart title
         """
-        done_epochs, done_samples = self.done_epochs, self.done_samples
-        self.done_epochs, self.done_samples = 0, 0
+        done = self.done
+        self.done = 0
         s = int(samples/epochs)
-        lr =   np.array([(self.lr1, 0)] + [ (self.step(1, s), i+1) for i in range(epochs)] )
+        lr =   np.array([(self.lr1, 0)] + [ (self.step(s), self.done) for i in range(epochs)] )
         plt.figure(figsize=(w,h), facecolor ='w')        
         plt.title(title)
         plt.plot(lr[:,1], lr[:,0], "-o", markersize=3); 
         if log: plt.yscale('log')        
         plt.xlabel("epoch"); plt.ylabel("lr"); plt.grid(ls=":");         
         plt.show()
-        self.done_epochs, self.done_samples = done_epochs, done_samples
+        self.done = done
 
-    #---------------------------------------------------------------------------
+#-------------------------------------------------------------------------------
 
     def plot_list(self, schedulers, samples=1000, epochs = 100,  log=True, w=8, h=5, title=""):
         """ 
         Draw a learning curve for `samples` passed over `epochs` epochs 
         Args:
             * schedulers - list of schedulers
             * samples - number of examples the optimizer must pass
@@ -122,182 +84,161 @@
             * w  - chart width
             * h  - chart height
             * title - chart title
         """
         assert len(schedulers) > 0
         save = [ copy.deepcopy(sch) for sch in schedulers ]
         for sch in schedulers:
-            sch.done_epochs = 0
-            sch.done_samples = 0
+            sch.done = 0
             sch.enable = True
         s = int(samples/epochs)
 
         sch = schedulers[0]
-        hist, sch_id =  [ (sch.lr1, 0) ], 0
+        hist, sch_id, tot =  [ (sch.lr1, 0) ], 0, 0
         for epoch in range(epochs):            
-            if sch is not None:
-                lr = sch.step(1, s)  
-            hist += [ (lr, epoch+1) ]
-            if sch is not None and not sch.enable:
-                sch_id += 1                
-                sch = schedulers[sch_id] if sch_id < len(schedulers) else None
+            lr = sch.step(s)            
+            tot += s
+            hist += [ (lr, tot) ]
+            if not sch.enable:
+                sch_id += 1
+                if sch_id >= len(schedulers):
+                    break
+                sch = schedulers[sch_id]
 
         hist = np.array(hist)
         plt.figure(figsize=(w,h), facecolor ='w')        
         plt.title(title)
         plt.plot(hist[:,1], hist[:,0], "-o", markersize=3); 
         if log: plt.yscale('log')        
         plt.xlabel("epoch"); plt.ylabel("lr"); plt.grid(ls=":");         
         plt.show()
         
         for i in range(len(schedulers)):             # restore
             schedulers[i] = copy.deepcopy(save[i])            
 
-#===============================================================================
+#-------------------------------------------------------------------------------
+
 
 class Scheduler_Const(Scheduler):
-    def __init__(self, lr1:float=None, epochs=None, samples=None, enable:bool=True) -> None:
+    def __init__(self, lr1:float=None, samples:int=1000, enable:bool=True) -> None:
         """ 
         The scheduler sets the learning rate to lr1 and waits for `samples` samples
 
         Args:
             * lr1 - learning rate; if None, then the current rate is taken from the optimizer                        
-            * epochs  - number of training epochs  to wait with  learning rate lr1 (if samples==None)
-            * samples - number of training samples to wait with  learning rate lr1 (if epochs==None)
+            * samples - number of training samples to wait with  learning rate lr1
         """
         super().__init__()
-        self.set(lr1=lr1, epochs=epochs,  samples=samples, enable=enable)
-
-    #---------------------------------------------------------------------------
+        self.set(lr1=lr1,  samples=samples, enable=enable)
 
-    def new_lr(self, new_epochs, new_samples):            
-        self.done(new_epochs, new_samples)
+    def new_lr(self, new_samples):            
+        self.done += new_samples
+        if self.done >= self.samples:               
+            self.enable = False
         return self.lr1
 
-#===============================================================================
+#-------------------------------------------------------------------------------
 
 class Scheduler_Line(Scheduler):
-    def __init__(self, lr1:float=None, lr2:float=None, epochs=None, samples=None, enable:bool=True) -> None:
+    def __init__(self, lr1:float=None, lr2:float=1e-5, samples:int=1000, enable:bool=True) -> None:
         """ 
         Linear interpolation between lr1 and lr2 per sample samples
         The logarithmic scale will be curved.            
         
         Args:
             * lr1 - initial learning rate; if None, then the current rate is taken from the optimizer            
             * lr2 - final learning rate after `samples` samples, starting from start
-            * epochs  - number of training epochs  to change the learning rate from lr1 to lr2 (if samples==None)         
-            * samples - number of training samples to change the learning rate from lr1 to lr2 (if epochs ==None)           
+            * samples - number of training samples to change the learning rate from lr1 to lr2            
         """
         super().__init__()
-        self.set(lr1=lr1, lr2=lr2, epochs=epochs, samples=samples, enable=enable)
+        self.set(lr1=lr1, lr2=lr2, samples=samples, enable=enable)
 
-    #---------------------------------------------------------------------------
-
-    def new_lr(self, new_epochs, new_samples):            
-        if self.done(new_epochs, new_samples):        
-            return self.lr2
+    def new_lr(self, new_samples):            
+        self.done += new_samples
+        if self.done >= self.samples:   
+            lr = self.lr2
+            self.enable = False
         else:
-            count = self.epochs      if self.epochs is not None else self.samples
-            done  = self.done_epochs if self.epochs is not None else self.done_samples
-            if count:
-                return self.lr1 + done * (self.lr2-self.lr1) / count
-        return 0
+            lr = self.lr1 + self.done * (self.lr2-self.lr1) / self.samples
+        return lr
 
-#===============================================================================
+#-------------------------------------------------------------------------------
 
 class Scheduler_Exp(Scheduler):
-    def __init__(self, lr1:float=None, lr2:float=None, epochs=None, samples=None, enable:bool=True) -> None:
+    def __init__(self, lr1:float=None, lr2:float=1e-5, samples:int=1000, enable:bool=True) -> None:
         """ 
         Exponential interpolation between lr1 and lr2 per sample samples.
         It will be a straight line on a logarithmic scale.
 
         Args:
             * lr1 - initial learning rate; if None, then the current rate is taken from the optimizer            
             * lr2 - final learning rate after `samples` samples, starting from start
-            * epochs  - number of training epochs  to change the learning rate from lr1 to lr2 (if samples==None)          
-            * samples - number of training samples to change the learning rate from lr1 to lr2 (if epochs ==None)           
+            * samples - number of training samples to change the learning rate from lr1 to lr2            
         """
         super().__init__()
-        self.set(lr1=lr1, lr2=lr2, epochs=epochs, samples=samples,  enable=enable)
-
-    #---------------------------------------------------------------------------
+        self.set(lr1=lr1, lr2=lr2, samples=samples, enable=enable)
 
-    def new_lr(self, new_epochs, new_samples):            
-        if self.done(new_epochs, new_samples):        
-            return self.lr2
+    def new_lr(self, new_samples):            
+        self.done += new_samples
+        if self.done >= self.samples:   
+            lr = self.lr2
+            self.enable = False
         else:
-            count = self.epochs if self.epochs is not None else self.samples
-            done  = self.done_epochs if self.epochs is not None else self.done_samples
             beta = self.lr2/self.lr1 if  self.lr1 > 0 and self.lr2 > 0 else 1
-            
-            if count > 0 and beta > 0:
-                return self.lr1 * math.exp(math.log(beta) * done/count)
-        return 0
+            lr = self.lr1 * math.exp(math.log(beta) * self.done/self.samples)
+        return lr
 
-#===============================================================================
+#-------------------------------------------------------------------------------
 
 class Scheduler_Cos(Scheduler):
-    def __init__(self, lr1:float=None, lr_hot:float=None,  lr2:float=None, samples=None, epochs=None, warmup=None, enable:bool=True) -> None:
+    def __init__(self, lr1:float=None, lr_hot:float=5e-3,  lr2:float=1e-5, samples:int=1000, warmup:int=100, enable:bool=True) -> None:
         """
         Cosine curve with linear heating.
 
         Args:
             * lr1 - initial learning rate; if None, then the current rate is taken from the optimizer
             * lr_hot - learning rate after warming up after `warmup` samples, starting from start
             * lr2 - final learning rate after `samples` samples, starting from start
-            * epochs  - number of training epochs to change the learning rate from lr1 to lr_hot (if samples==None)
-            * samples - number of training samples to change the learning rate from lr1 to lr2   (if epochs ==None)
-            * warmup - number of training epochs (or samples) to warm up from lr1 to lr_hot
+            * samples - number of training samples to change the learning rate from lr1 to lr2
+            * warmup - number of training samples to warm up from lr1 to lr_hot
         """
         super().__init__()
-        self.set(lr1=lr1, lr2=lr2, epochs=epochs, samples=samples,  lr_hot=lr_hot, warmup=warmup, enable=enable)
-
-    #---------------------------------------------------------------------------        
-
-    def set(self, lr1=None, lr2=None, samples=None,  epochs=None, lr_hot=None, warmup=None, enable=True):        
-        super().set(lr1=lr1, lr2=lr2, epochs=epochs, samples=samples,  enable=enable)        
-        
-        assert lr_hot is not None and lr_hot > 0,   f"wrong lr_hot={lr_hot} limit in Scheduler"
-        assert warmup is not None and warmup >= 0,  f"wrong  warm-up samples or epochs limits in Scheduler: warmup={warmup}"
-        assert samples is None or samples > warmup, f"should be fewer warm-up samples={warmup} than the total number of samples={samples}"
-        assert epochs  is None or epochs  > warmup, f"should be fewer warm-up epochs ={warmup} than the total number of epochs ={epochs}"
+        self.set(lr1=lr1, lr2=lr2, samples=samples, lr_hot=lr_hot, warmup=warmup, enable=enable)
 
-        self.lr_hot = lr_hot
-        self.warmup = warmup        
+    def set(self, lr1=1e-5, lr2=1e-5, samples=1e3, lr_hot=5e-3, warmup=1e1, enable=True):        
+        super().set(lr1=lr1, lr2=lr2, samples=samples, enable=enable)
+        self.lr_hot = lr_hot or self.get_lr()        
+        assert self.lr_hot > 0,  "wrong lr limits in Scheduler"
+        assert warmup >= 0,      "wrong samples limits in Scheduler"
+        assert samples > warmup, "should be fewer warm-up samples (warm) than the total number of samples"
+        self.warmup  = warmup
+        self.done    = 0
         if enable:
             self.set_lr(self.lr1)
 
-    #---------------------------------------------------------------------------            
-
-    def new_lr(self, new_epochs, new_samples):            
-        if self.done(new_epochs, new_samples):        
-            return self.lr2
-        else:
-            count = self.epochs if self.epochs is not None else self.samples
-            done  = self.done_epochs if self.epochs is not None else self.done_samples            
-
-            if done >= self.warmup:           # косинусное снижение
-                if count > self.warmup:
-                    s = (done - self.warmup) / (count - self.warmup)
-                    return self.lr2 + (self.lr_hot - self.lr2) * (1 + math.cos(math.pi*s)) / 2            
-            else:                                    # режим разогрева            
-                if  self.warmup > 0:
-                    return self.lr1 + (self.lr_hot - self.lr1) * done / self.warmup
-        return 0
+    def new_lr(self, new_samples):            
+        self.done += new_samples
+        if self.done >= self.samples:   
+            lr = self.lr2
+            self.enable = False
+        elif self.done >= self.warmup:           # косинусное снижение
+            s = (self.done - self.warmup) / (self.samples - self.warmup)
+            lr = self.lr2 + (self.lr_hot - self.lr2) * (1 + math.cos(math.pi*s)) / 2            
+        else:                                    # режим разогрева            
+            lr =  self.lr1 + (self.lr_hot - self.lr1) * self.done / self.warmup
+        return lr
 
 #===============================================================================
 #                                   Main
 #===============================================================================
 
 if __name__ == '__main__':
-    scheduler = Scheduler_Cos(lr1=1e-4, lr_hot=1e-2, lr2=1e-3, epochs=40, warmup=10)                
-    #scheduler = Scheduler_Exp(lr1=1e-2,  lr2=1e-6, samples=4000)                
-    #scheduler = Scheduler_Line(lr1=1e-2,  lr2=1e-3, samples=4000)                
+    #scheduler = Scheduler_Cos(lr1=1e-4, lr_hot=1e-2, lr2=1e-3, samples=4000, warmup=1000)                
+    scheduler = Scheduler_Exp(lr1=1e-2,  lr2=1e-6, samples=4000)                
     #scheduler.plot(samples=4000, epochs=50, log=True, w=5, h=4, title="ExpScheduler")
-    #scheduler.plot(samples=8000, epochs = 100)
     
     lst =[
         Scheduler_Cos  (lr1=1e-4, lr_hot=1e-2, lr2=1e-3, samples=4000, warmup=1000),
         Scheduler_Const(lr1=1e-3, samples=2000),
-        Scheduler_Exp  (lr1=1e-3, lr2=1e-5, epochs=20)
+        Scheduler_Exp  (lr1=1e-3, lr2=1e-5, samples=4000)
     ]
-    scheduler.plot_list(lst, samples=20000, epochs=100, log=True, w=5, h=4, title="Cos, Const, Exp Schedulers")
+    scheduler.plot_list(lst, samples=10000, epochs=50, log=True, w=5, h=4, title="Cos, Const, Exp Schedulers")
```

## Comparing `QuNet-0.0.87.dist-info/LICENSE` & `QuNet-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `QuNet-0.0.87.dist-info/METADATA` & `QuNet-0.0.9.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuNet
-Version: 0.0.87
+Version: 0.0.9
 Summary: Working with deep learning models
 Home-page: https://github.com/step137/qunet
 Author: synset
 Author-email: steps137ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -18,99 +18,112 @@
 [![PyPI version](https://badge.fury.io/py/torchinfo.svg)](https://badge.fury.io/py/torchinfo)
 
 
 Easy working with deep learning models.
 * Large set of custom modules for neural networks (MLP, CNN, Transformer, etc.)
 * Trainer class for training the model.
 * Various tools for visualizing the training process and the state of the model.
-* Training large models: float16, mini-batch splitting, etc.
+* Training large models: float16, mini-batch splitting if it does not fit in memory, etc.
 
 <hr>
 
 ## Install
 
 ```
 pip install qunet
 ```
 <hr>
 
 ## Usage
 
 ```python
-from qunet import Data, Trainer, Scheduler_Exp
+from qunet import Data, Trainer, ExpScheduler
 
-trainer = Trainer(model, data_trn, data_val)
+# 1. create dataset
+X = torch.rand(10000,1)               
+Y = 2*X + 1
+data_trn = Data((X,Y), batch_size=128, shuffle=True)
 
+# 2. create trainer, optimizer and scheduler (if need)                                               
+tariner = Trainer(model, data_trn)    
 trainer.set_optimizer( torch.optim.SGD(model.parameters(), lr=1e-2) )
-trainer.set_scheduler( Scheduler_Exp(lr1=1e-5, lr2=1e-4, samples=100e3) )
+trainer.set_scheduler( ExpScheduler(lr1=1e-5, lr2=1e-4, samples=100e3) )
 
-trainer.view.loss(y_min=0, y_max=0.5)
-trainer.fit(epochs=10, period_plot=5, monitor=['loss'])
+# 3. run training
+trainer.fit(epochs=100, period_plot=5)
 ```
 
 <hr>
 
 ## Model
 
 Model must be a class (successor of nn.Module) with functions:
 
 * `forward(x)` function takes input `x` and returns output `y`. 
-This function is not used directly by the coach and usually contains the complete logic of the model.
+This function is not used directly by the coach and usually contains a description of the model.
 * `training_step(batch, batch_id)` - called by the trainer during the training phase. 
 Should return a scalar loss (with computational graph).
-It can also return a dictionary like `{"loss": loss, "score": torch.hstack([accuracy, tnr, tpr])}`, where score is a quality metrics.
+It can also return a dictionary like `{"loss": scalar, "score": tensor}`, where score is a quality metric.
 * `validation_step(batch, batch_id)` - similarly called at the model validation stage.
 If it does the same calculations as `training_step`, it can be omitted.
-* `predict_step(batch, batch_id)` - required when using the `predict` method. Should return a tensor `y_pred` of the model's output (or a dictionary `{"output": y_pred, "score": metrics}`, where `metrics` are any quality metrics tensor for each example).
 
 For example, for 1D linear regression  $y=f(x)$ with mse-loss and metric as |y_pred-y_true|, model looks like:
 ```python
 class Model(nn.Module):
-    def __init__(self):              
+    def __init__(self):      
+        """ Creating Model Parameters """  
         super().__init__() 
         self.fc = nn.Linear( 1, 1 )
 
-    def forward(self, x):                                 # (B,1)
-        return self.fc(x)                                 # (B,1)
-
-    def training_step(self, batch, batch_id):        
-        x, y_true = batch                                 # the model knows the minbatch format
-        y_pred = self(x)                                  # (B,1)  forward function call
-        loss  = (y_pred - y_true).pow(2).mean()           # ()     loss for optimization (scalar)!
-        error = torch.abs(y_pred.detach()-y_true).mean()  # (B,1)  error for batch samples
-        return {'loss':loss, 'score': error}              # if no score, you can return loss
+    def forward(self, x):                            # (B,1)
+        """ Defining Model Calculations """
+        return self.fc(x)                            # (B,1)
+
+    def training_step(self, batch, batch_id):
+        """ Called by the trainer during the training step """
+        x, y_pred = batch                            # the model knows the minbatch format
+        y_true = self(x)                             # (B,1)  forward function call
+        loss   = (y_pred - y_true).pow(2).mean()     # ()     loss for optimization (scalar)!        
+        errors = torch.abs(y_pred.detach()-y_true)   # (B,1)  errors for each sample (one metric)
+        return {'loss':loss, 'score': errors}        # if there is no score, you can simply return loss
 ```
-As we can see, the model description interface is the same as the library interface <a href="https://lightning.ai/">PyTorch Lightning</a>
+As we can see, the model description interface is the same as the library interface <a href="https://lightning.ai/">Pytorch Lightning</a>
 
 <hr>
 
 ## Data
 
-QuNet has a Data class - data for model training or validation. It can be overridden or pytorch DataLoader can be used.
-The iterator `__next__`  is supposed  must return an mini-batch, has the same structure as passed `dataset` when creating the `Data`.
+The `Data` - training or validation data class. It can be overridden or pytorch DataLoader can be used.
+Iterator `__next__` of the `Data`  must return an `X,Y` tuple, where:
+* X - tensor or tuple (list) of tensors for model input,
+* Y - tensor or tuple (list) of tensors for model target values.
+
 For example, let's create training data in which two tensors X1,X2 are the input of the model and one tensor Y is the output (target):
 ```python    
-from qunet import Data
+X1, X2 = np.rand(1000,3), np.rand(1000,3,20)
+Y = X1 * torch.Sigmoid(X2).mean(-1)
 
-X1, X2 = torch.rand(1000,3), torch.rand(1000,3,20)
-Y = X1 * torch.sigmoid(X2).mean(-1)
-
-data_trn = Data( dataset=( X1, X2, Y ), batch_size=100)  
-
-for x1,x2, y in data_trn:
-    print(x1.shape, x2.shape, y.shape)  # (100,3) (100,3,20) (100,3)
+data_trn = Data( dataset=( (X1,X2), Y ) )  
 ```        
+The data minibatch tuple (X,Y) is used in the Trainer as follows:
+```python
+for b (X,Y_true) in enumerate(data):  # РїСЂРё РѕР±СѓС‡РµРЅРёРё
+    X, Y_true = to_device(X), to_device(Y_true)            
+    Y_pred = model(X)
+    loss, score = model.metrics(X, Y_pred, Y_true)
+```
+So dataset is a list or tuple of two elements (input and target).
+Each element can be a tensor or a list (tuple) of tensors.
 All tensors in the dataset are assumed to have the same length (by first index).
-The model is responsible for interpreting the composition of the mini-batch.
 
 The Data class constructor has the following parameters:
 ```python
 Data(dataset, shuffle=True, batch_size=64,  whole_batch=False, n_packs=1)
 ```
-* `dataset` - model training data: tensor X or tuple input and output tensors: (X, Y), and etc.
+* `dataset` - model input and output tuple (X, Y), as described above
 * `shuffle` - shuffle data after after passing through all examples
 * `batch_size` - minibatch size; can be changed later: data_trn.batch_size = 1024
 * `whole_batch` - return minibatches of batch_size only; if the total number of examples is not divisible by batch_size, you may end up with one small batch with an unreliable gradient. If whole_batch = True, such a batch will not be issued.
 * `n_packs` - data is split into n_packs packs; the passage of one pack is considered an training ephoch. It is used to a large dataset, when it is necessary to do validation more often.
 </ul>
 
 You can also use the standard DataLoader with Trainer:
@@ -130,216 +143,166 @@
 Using the `set_optimizer` function, the optimizer is set.
 After that, the function `fit` is called:
 ```python
 trainer = Trainer(model, data_trn, data_val)
 trainer.set_optimizer( torch.optim.SGD(model.parameters(), lr=1e-2) )
 trainer.fit(epochs=100, pre_val=True, period_plot=10)
 ```
-You can add different training schedulers, customize the output of training graphs, manage the storage of the best models and checkpoints, and much more. The Trainer class constructor has the following parameters:
+You can add different training schedulers, customize the output of training graphs, manage the storage of the best models and checkpoints, and much more.
 
 ```python
-trainer = Trainer(model, data_trn, data_val, score_max=False)
+trainer = Trainer(model, data_trn, data_val, device=None, dtype=torch.float32, score_max=False)
 ```
 
 * `model`     - model for traininig;
 * `data_trn`  - training data (Data or DataLoader instance);
 * `data_val`  - data for validation (instance of Data or DataLoader); may be missing;
-* `score_max` - consider that the metric (the first column of the tensor `score` returned by the function `training_step` of the model); should strive to become the maximum (for example, so for accuracy).
+* `score_max` - consider that the metric (the first column of the second tensor returned by the function `metrics` of the model ); should strive to become the maximum (for example, so for accuracy).
 
 Other properties of `Trainer` allow you to customize the appearance of graphs, save models, manage training, and so on.
-They will be discussed in the relevant sections. Model training starts after running the `fit` function:
+They will be discussed in the relevant sections.
 
 ```python
-trainer.fit(epochs=None,   samples=None,            
+trainer.fit(epochs =None,  samples=None,            
             pre_val=False, period_val=1, period_plot=100,         
             period_checks=1, period_val_beg = 4, samples_beg = None,
-            monitor=[], patience=None ):     
+            period_call:int = 0, callback = None):     
 ```
 
 * `epochs`         - number of epochs for training (passes of one data_trn pack). If not defined (None) works "infinitely".
 * `samples`        - if defined, then training will stop after this number of samples, even if epochs has not ended
-* `pre_val`        - validate model before starting training
-* `period_val`     - the period with which the validation model runs (in epochs)
-* `period_plot`    - the period with which the training plot is displayed  (in epochs)
-* `period_points`  - the period with which the checkpoints are made and the current model is saved (in epochs)
-* `period_val_beg` - the period with which the validation model runs on the first `samples_beg` samples. Used when validation needs to be done less frequently at the start of training.
+* `pre_val`        - validate before starting training
+* `period_val`     - period after which validation run (in epochs)
+* `period_plot`    - period after which the training plot is displayed (in epochs)
+* `period_call`    - callback custom function call period
+* `callback`       - custom function called with period_info
+* `period_checks`  - period after which checkpoints are made and the current model is saved (in epochs)
+* `period_val_beg` - validation period on the first `samples_beg` samples. Used when validation needs to be done less frequently at the start of training.
 * `samples_beg`   -  the number of samples from the start, after which the validation period will be equal to `period_val`
-* `monitor=[]`- what to save in folders: monitor=['loss'] or monitor=['loss', 'score', 'checks']
-* `patience`  - after how many epochs to stop if there was no better loss, but a better score during this time 
 
 <hr>
 
 ## Visualization of the training process
 
-When `fit` has argument `period_plot > 0`, then every `period_plot` a training plot will be displayed.
-By default it contains score and loss:
-
 <img src="img/loss.png">
 
-You can customize the appearance of graphs using the following trainer options:
 
 ```python
-trainer.view = Config(
-    w  = 12,                   # plt-plot width
-    h  =  5,                   # plt-plot height
-    units = Config(
-        unit  = 'epoch',       # 'epoch' | 'sample'
-        count = 1e6,           # units for number of samples
-        time  = 's'            # time units: ms, s, m, h
-    ),
-
-    x_min = 0,                 # minimum value in samples on the x-axis (if < 0 last x_min samples)
-    x_max = None,              # maximum value in samples on the x-axis (if None - last)
-
-    loss = Config(                                
-        show  = True,          # show loss subplot
-        y_min = None,          # fixing the minimum value on the y-axis
-        y_max = None,          # fixing the maximum value on the y-axis
-        ticks = None,          # how many labels on the y-axis
-        lr    = True,          # show learning rate
-        labels= True,          # show labels (training events)                
-        trn_checks = False,    # show the achievement of the minimum training loss (dots)
-        val_checks = True      # show the achievement of the minimum validation loss (dots)
-    ),            
-    score = Config(                                
-        show  = True,          # show score subplot    
-        y_min = None,          # fixing the minimum value on the y-axis
-        y_max = None,          # fixing the maximum value on the y-axis
-        ticks = None,          # how many labels on the y-axis
-        lr    = True,          # show learning rate                
-        labels = True,         # show labels (training events)
-        trn_checks = False,    # show the achievement of the optimum training score (dots)
-        val_checks = True      # show the achievement of the optimum validation score (dots)
-    ),
-)
+trainer.view = {                    
+    'w'            : 12,         # plt-plot width
+    'h'            :  5,         # plt-plot height
+
+    'count_units'  : 1e6,        # units for number of samples
+    'time_units'   : 's',        # time units: ms, s, m, h
+
+    'x_min'        : 0,          # minimum value in samples on the x-axis (if < 0 last x_min samples)
+    'x_max'        : None,       # maximum value in samples on the x-axis (if None - last)
+
+    'loss': {                                
+        'show'  : True,          # show loss subplot
+        'y_min' : None,          # fixing the minimum value on the y-axis
+        'y_max' : None,          # fixing the maximum value on the y-axis
+        'ticks' : None,          # how many labels on the y-axis
+        'lr'    : True,          # show learning rate        
+        'labels': True,          # show labels (training events)
+        'trn_checks': True,      # show the achievement of the minimum training loss (dots)
+        'val_checks': True,      # show the achievement of the minimum validation loss (dots)
+    },
+
+    'score': {                    
+        'show'  : True,          # show score subplot    
+        'y_min' : None,          # fixing the minimum value on the y-axis
+        'y_max' : None,          # fixing the maximum value on the y-axis
+        'ticks' : None,          # how many labels on the y-axis
+        'lr'    : True,          # show learning rate
+        'labels': True,          # show labels (training events)
+        'trn_checks': True,      # show the achievement of the optimum training score (dots)                
+        'val_checks': True,      # show the achievement of the optimum validation score (dots)                
+    }
+}
 ```
 
-You can change one parameter:
-```python
-trainer.view.loss.lr = False   # do not show learning rate on loss plot
-```
-or immediately a group of parameters:
-```python
-trainer.view.units(unit='sample', count=1e3, time='m')
-```
 
 <hr>
 
 ## Using Schedules
 
 Schedulers allow you to control the learning process by changing the learning rate according to the required algorithm.
 There can be one or more schedulers. In the latter case, they are processed sequentially one after another.
-There are the following schedulers:
-* `Scheduler_Line(lr1, lr2, epochs)` - changes the learning rate from `lr1` to `lr2` over `epochs` training epochs. If `lr1` is not specified, the optimizer's current lr is used for it.
-* `Scheduler_Exp(lr1, lr2, epochs)` - similar, but changing `lr` from `lr1` to `lr2` is exponential.
-* `Scheduler_Cos(lr1, lr_hot,  lr2, epochs, warmup)` - changing `lr` by cosine with preliminary linear heating during `warmup` epochs from `lr1` to `lr_hot`.
-* `Scheduler_Const(lr1, epochs)` - wait for `epochs` epochs with unchanged `lr` (as usual, the last value is taken if `lr1` is not set). This scheduler is useful when using lists of schedulers.
-
-Instead of `epochs`, you can specify `samples` (number of training samples)
+РЎСѓС‰РµСЃС‚РІСѓСЋС‚ СЃР»РµРґСѓСЋС‰РёРµ С€РµРґСѓР»РµСЂС‹:
+* `Scheduler_Line(lr1, lr2, samples)` - changes the learning rate from `lr1` to `lr2` over `samples` training samples. If `lr1` is not specified, the optimizer's current lr is used for it.
+* `Scheduler_Exp(lr1, lr2, samples)` - similar, but changing `lr` from `lr1` to `lr2` is exponential.
+* `Scheduler_Cos(lr1, lr_hot,  lr2, samples, warmup)` - changing `lr` by cosine with preliminary linear heating during `warmup` samples from `lr1` to `lr_hot`.
+* `Scheduler_Const(lr1, samples)` - wait for `samples` samples with unchanged `lr` (as usual, the last value is taken if `lr1` is not set). This scheduler is useful when using lists of schedulers.
 
 Each scheduler has a `plot` method that can be used to display the training plot:
 ```python
-sch = Scheduler_Cos(lr1=1e-5, lr_hot=1e-2, lr2=1e-4,  samples=10e3,  warmup=1e3)
-sch.plot(log=True, samples=20e3, epochs=100)
+sch = Scheduler_Cos(lr1=1e-5, lr_hot=1e-2, lr2=1e-4,  samples=100e3, warmup=1e3)
+sch.plot(log=True)
 ```
 You can also call the `trainer.plot_schedulers()` method of the `Trainer` class.
 It will draw the schedule of the list of schedulers added to the trainer.
 
 Compiling a list of schedulers is done by the following methods of the `Trainer` class:
 * `set_scheduler`( sch ) - set a list of schedulers from one scheduler sch (after clearing the list);
 * `add_scheduler`( sch ) - add scheduler sch
 * `del_scheduler`(i)     - remove the i-th scheduler from the list (numbering from zero)
 
 This group of methods works with all schedulers:
 * `reset_schedulers`() - reset all scheduler counters and make them active (starting from the first one)
 * `stop_schedulers` () - stop all schedulers
 * `clear_schedulers`() - clear list of schedulers
+Example:
 
-Example of learning curves of various schedulers:
 
 <img src="img/schedulers.png">
-
-An example of using schedulers can be found in:
-<a href="https://colab.research.google.com/drive/179sHb3WyHNrSJKGLfKrXaAzvShmS1SSf?usp=sharing">notebook Interpolation_F(x)</a> 
-
 <hr>
 
 ## Best Model and Checkpoints
 
-Trainer can store the best models in memory or on disk.
-Small models are convenient to keep in memory. 
-When the best validation loss or score is reached, a copy of the model is made. 
-To do this, you need to enable `train.best.copy` and specify the target value for which you want to remember the model in the `monitor` list:
+If you set these flags to `True`, then `Trainer` will save the last best model by validation score and loss:
 ```python
-trainer.best(copy=True)
-trainer.fit(epochs=200, monitor=['score'])
-trainer.save("best_score.pt", trainer.best.score_model)
+trainer.copy_best_score_model = True  # to copy the best model by val score
+trainer.copy_best_loss_model  = True  # to copy the best model by val loss
 ```
-The last best model will be in `trainer.best.loss_model` and `trainer.best.score_model`.
-The values of the corresponding metrics are in `trainer.best.loss` and `trainer.best.score`.
-These models can be used to roll back if something went wrong:
+These models can be used to roll back if something went wrong (similarly for `trainer.best_loss_model`):
 ```python
-trainer.model = copy.deepcopy(trainer.best.score_model)   
+train.model = copy.deepcopy(trainer.best_score_model)   
 ```
-To save the best models by loss and/or score on disk, you need to set folders.
-Saving will occur if you specify `monitor` in `fit`:
+
+If the following folder is defined (by default `None`), then the best model by validation loss, score will be saved on disk and intermediate versions of the model will be saved with the period `period_checks` (argument of `fit` function).
 ```python
-trainer.folders(loss='log/loss', score='log/loss',  points='log/checkpoints')
-trainer.fit(epochs=200, monitor=['score', 'loss', 'points'], period_points=10)
+trainer.folder_loss   = "models/best_loss"   # folder to save the best val loss models
+trainer.folder_score  = "models/best_score"  # folder to save the best val score models
+trainer.folder_checks = "models/checkpoints" # folder to save checkpoints        
 ```
-The best model by score and loss will be saved each time a new best value is reached.
-Checkpoints (`points`) are simply saving the current state of the model.
-They can be done with the desired periodicity in epochs (period_points=1 by default).
-
-The best score is the metric of the first element in the score.
+The best score is the metric of the first column of the second return tensor in the metrics function of the model.
 If `trainer.score_max=True`, then the higher the score, the better (for example, accuracy).
 <hr>
 
 ## Batch Argumentation
 
-When working with images, in order to "enlarge" the dataset, it is necessary to do their augmentation.
-To do this, you need to define the `trainer.transformers.trn` (and/or 'val') functions:
-
-```python
-augmentation_trn = A.Compose([
-    A.HorizontalFlip(p=0.5),                                  
-    A.ShiftScaleRotate(rotate_limit=30),
-    A.Normalize(),   # img = (img/max_pixel_value - mean) / (std)                                
-    ToTensorV2(),    # numpy -> torch;  (B,H,W,C) -> (B,C,H,W)
-])
-
-def transform_trn(batch, batch_id):
-    x, y = batch
-    B,H,W,C = x.shape
-    new_x = torch.empty(B,C,H,W)
-    for i in range(len(x)):        
-        new_x[i] = augmentation_trn(image=x[i].numpy())["image"]                
-    return (new_x, y)
-
-trainer.transforms(trn = transform_trn);
-```
-The `transform_trn` function will be called during the training phase before sending the batch to the GPU.
-
-An example of such an argumentation can be found in the <a href="https://colab.research.google.com/drive/1ThxnMrAjuFTGKXLI-93oRa9doNpP32y4?usp=sharing">notebook CIFAR10</a>  
 <hr>
 
 
 ## Working with the Large Models
 
 <hr>
 
 ## Model State Visualization
 
 <hr>
 
 ## Examples
 
-* <a href="https://colab.research.google.com/drive/179sHb3WyHNrSJKGLfKrXaAzvShmS1SSf?usp=sharing">Interpolation_F(x)</a> - interpolation of a function of one variable (example of setting up a training plot; working with the list of schedulers; adding a custom plot)
-* <a href="https://colab.research.google.com/drive/1N4b6mwUvH-o-t6VIiuhq7FMuGRabdOm0?usp=sharing">MNIST</a> - recognition of handwritten digits 0-9 (example using pytorch DataLoader, model predict, show errors, confusion matrix)
-* <a href="https://colab.research.google.com/drive/1ThxnMrAjuFTGKXLI-93oRa9doNpP32y4?usp=sharing">CIFAR10</a>  (truncated EfficientNet, pre-trained parameters, bone freezing, augmentation)
+* <a href="https://colab.research.google.com/drive/179sHb3WyHNrSJKGLfKrXaAzvShmS1SSf?usp=sharing">Interpolation_F(x)</a> - interpolation of a function of one variable (example of setting up a training plot; working with the list of schedulers; adding a custom graph)
+* <a href="https://colab.research.google.com/drive/1N4b6mwUvH-o-t6VIiuhq7FMuGRabdOm0?usp=sharing">MNIST</a> - recognition of handwritten digits 0-9 (example using pytorch DataLoader, classification task)
+
+* CIFAR  (agumantation)
+
 * Vanishing gradient
 * Regression_1D - visualization of changes in model parameters
 
 <hr>
 
 ## Versions
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

