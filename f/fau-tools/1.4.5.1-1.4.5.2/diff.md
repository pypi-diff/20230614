# Comparing `tmp/fau_tools-1.4.5.1.tar.gz` & `tmp/fau_tools-1.4.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fau_tools-1.4.5.1.tar", max compression
+gzip compressed data, was "fau_tools-1.4.5.2.tar", max compression
```

## Comparing `fau_tools-1.4.5.1.tar` & `fau_tools-1.4.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      179 2022-09-17 06:01:57.485247 fau_tools-1.4.5.1/Fau_tools/__init__.py
--rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.4.5.1/Fau_tools/data_structure/__init__.py
--rw-r--r--   0        0        0     3420 2023-04-20 02:46:11.824418 fau_tools-1.4.5.1/Fau_tools/data_structure/data_structure.py
--rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.4.5.1/Fau_tools/data_structure/data_structure.pyi
--rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.4.5.1/Fau_tools/torch_tools/__init__.py
--rw-r--r--   0        0        0    10050 2023-04-20 02:47:54.439467 fau_tools-1.4.5.1/Fau_tools/torch_tools/torch_tools.py
--rw-r--r--   0        0        0     1440 2023-04-20 02:46:11.825456 fau_tools-1.4.5.1/Fau_tools/torch_tools/torch_tools.pyi
--rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.4.5.1/Fau_tools/utility/__init__.py
--rw-r--r--   0        0        0    10983 2023-06-05 09:17:34.068974 fau_tools-1.4.5.1/Fau_tools/utility/utility.py
--rw-r--r--   0        0        0     1008 2023-06-05 09:23:30.478542 fau_tools-1.4.5.1/Fau_tools/utility/utility.pyi
--rw-r--r--   0        0        0     2680 2023-04-20 02:37:45.625671 fau_tools-1.4.5.1/README.md
--rw-r--r--   0        0        0     1150 2023-06-05 09:21:13.564634 fau_tools-1.4.5.1/pyproject.toml
--rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 fau_tools-1.4.5.1/PKG-INFO
+-rw-r--r--   0        0        0      179 2022-09-17 06:01:57.485247 fau_tools-1.4.5.2/Fau_tools/__init__.py
+-rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.4.5.2/Fau_tools/data_structure/__init__.py
+-rw-r--r--   0        0        0     3432 2023-06-14 07:04:20.652148 fau_tools-1.4.5.2/Fau_tools/data_structure/data_structure.py
+-rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.4.5.2/Fau_tools/data_structure/data_structure.pyi
+-rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.4.5.2/Fau_tools/torch_tools/__init__.py
+-rw-r--r--   0        0        0    10116 2023-06-14 07:06:31.832738 fau_tools-1.4.5.2/Fau_tools/torch_tools/torch_tools.py
+-rw-r--r--   0        0        0     1440 2023-04-20 02:46:11.825456 fau_tools-1.4.5.2/Fau_tools/torch_tools/torch_tools.pyi
+-rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.4.5.2/Fau_tools/utility/__init__.py
+-rw-r--r--   0        0        0    10983 2023-06-14 07:11:29.039437 fau_tools-1.4.5.2/Fau_tools/utility/utility.py
+-rw-r--r--   0        0        0     1008 2023-06-05 09:23:30.478542 fau_tools-1.4.5.2/Fau_tools/utility/utility.pyi
+-rw-r--r--   0        0        0     2680 2023-04-20 02:37:45.625671 fau_tools-1.4.5.2/README.md
+-rw-r--r--   0        0        0     1150 2023-06-14 07:13:01.011155 fau_tools-1.4.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 fau_tools-1.4.5.2/PKG-INFO
```

### Comparing `fau_tools-1.4.5.1/Fau_tools/data_structure/data_structure.py` & `fau_tools-1.4.5.2/Fau_tools/data_structure/data_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     file_name : the name of the saved model
     only_param : whether only save the parameters of the model
 
     """
     file_name = f"{file_name}.pth"
     if only_param: torch.save(self.model.state_dict(), rf"{file_name}")
     else: torch.save(self.model, rf"{file_name}")
-    cprint(rf"{__class__.__name__}: save a model named {file_name} successfully!", "green")
+    cprint(rf"{__class__.__name__}: save a model named {file_name} successfully!", color="green")
 
   @staticmethod
   def load(model, file_path, DEVICE=None):
     """
     Load the trained model that saved only parameters.
 
     A new feature added in version 1.0.0
@@ -109,15 +109,15 @@
     with open(rf"{file_name}", "w") as file:
       col_list = ", ".join(("loss", "accuracy")) + "\n"
       file.write(col_list)
       for loss, accuracy in zip(self.loss_list, self.accuracy_list):
         line = f"{loss:.6f}, {accuracy:.6f}\n"
         file.write(line)
 
-    cprint(rf"{__class__.__name__}: save a record file named {file_name} successfully!", "green")
+    cprint(rf"{__class__.__name__}: save a record file named {file_name} successfully!", color="green")
 
 
 
 
 
 class TimeManager:
   """Guess the training time costing."""
```

### Comparing `fau_tools-1.4.5.1/Fau_tools/data_structure/data_structure.pyi` & `fau_tools-1.4.5.2/Fau_tools/data_structure/data_structure.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5.1/Fau_tools/torch_tools/torch_tools.py` & `fau_tools-1.4.5.2/Fau_tools/torch_tools/torch_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,18 +39,18 @@
   if time_manager:  # for showing time process:
     average_time, elapsed_time = time_manager.get_average_time(), time_manager.get_elapsed_time()
     total_time = total * average_time
 
     elapsed_time = utility.time_to_human(elapsed_time)
     total_time = utility.time_to_human(total_time)
 
-    show += cprint(f"  [{elapsed_time}<{total_time}]", "cyan", ret=True)
+    show += cprint(f"  [{elapsed_time}<{total_time}]", color="cyan", show=False)
 
-  if loss: show += cprint(f"  loss: {loss:.6f}", "red", ret=True)
-  if accuracy: show += cprint(f"  accuracy: {accuracy:.2%}", "green", ret=True)
+  if loss: show += cprint(f"  loss: {loss:.6f}", color="red", show=False)
+  if accuracy: show += cprint(f"  accuracy: {accuracy:.2%}", color="green", show=False)
 
   print(show)
 
 
 
 def __stop_training(epoch, model_manager, threshold):
   """
@@ -135,24 +135,24 @@
   # Acquire device information
   if DEVICE is None:
     DEVICE_NAME = None
     try:
       DEVICE = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
       DEVICE_NAME = "CPU" if DEVICE == "cpu" else torch.cuda.get_device_name(0)
     except AssertionError:
-      cprint("No cuda detected.", "yellow")
+      cprint("No cuda detected.", color="yellow")
       DEVICE, DEVICE_NAME = "cpu", "CPU"
     except Exception:
-      cprint("Unknown error in torch_tools.", "red")
+      cprint("Unknown error in torch_tools.", color="red")
       DEVICE, DEVICE_NAME = "cpu", "CPU"
     finally:
-      cprint(f"{'='*10} Training in {DEVICE_NAME} {'='*10}", "green")
+      cprint(f"{'='*10} Training in {DEVICE_NAME} {'='*10}", color="green")
 
   if train_loader.batch_size == 1:
-    cprint("Warning: you shouldn't set the batch_size to 1. since if the NN uses BN, it will arise an error.", "red")
+    cprint("Warning: you shouldn't set the batch_size to 1. since if the NN uses BN, it will arise an error.", color="red")
 
   # for saving training data
   model_manager = ModelManager()
   train_recorder = TrainRecorder()
 
   # begin training
   model = model.to(DEVICE); model.train()  # initialization
@@ -179,15 +179,15 @@
 
     # update and record
     model_manager.update(model, loss_value, accuracy, epoch)
     train_recorder.update(loss_value, accuracy)
 
     # Judge early stop
     if early_stop is not None and __stop_training(epoch, model_manager, early_stop):
-      cprint(f"Early stop: The model has gone through {early_stop} epochs without being optimized.", "yellow")
+      cprint(f"Early stop: The model has gone through {early_stop} epochs without being optimized.", color="yellow")
       break
 
 
   if name is None: return  # no save
 
   # save model and process
   SAVE_NAME = f"{name}_{model_manager.get_postfix()}"
@@ -202,15 +202,15 @@
     file.write(f"loss function:\n{str(loss_function)}\n")
     file.write(f"{'-' * 20}\n")
     file.write(f"batch size: {train_loader.batch_size}\n")
     file.write(f"epoch: {EPOCH}\n")
     try:  # for saving the number of train and test data
       train_data_num = len(train_loader.batch_sampler.sampler.data_source.labels)
       test_data_num = len(test_loader.batch_sampler.sampler.data_source.labels)
-    except AttributeError: cprint("Saving the number of train and test data error.", "red")
+    except AttributeError: cprint("Saving the number of train and test data error.", color="red")
     else:
       file.write(f"{'-' * 20}\n")
       file.write(f"train_data_number: {train_data_num}\n")
       file.write(f"test_data_number: {test_data_num}\n")
 
     # save best info
     file.write(f"{'-' * 20}\n")
@@ -219,15 +219,15 @@
     # save time
     file.write(f"{'-' * 20}\n")
     cost_time = time_manager.get_elapsed_time()
     cost_time = utility.time_to_human(cost_time)
     file.write(f"Training cost: {cost_time}\n")
 
 
-  cprint(f"{torch_train.__name__}: save a parameter file named {parameters_filename} successfully!", "green")
+  cprint(f"{torch_train.__name__}: save a parameter file named {parameters_filename} successfully!", color="green")
 
 
 
 
 
 # ------------------------------------------------------------
 # --------------- Function --- plot
```

### Comparing `fau_tools-1.4.5.1/Fau_tools/torch_tools/torch_tools.pyi` & `fau_tools-1.4.5.2/Fau_tools/torch_tools/torch_tools.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5.1/Fau_tools/utility/utility.py` & `fau_tools-1.4.5.2/Fau_tools/utility/utility.py`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5.1/Fau_tools/utility/utility.pyi` & `fau_tools-1.4.5.2/Fau_tools/utility/utility.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5.1/README.md` & `fau_tools-1.4.5.2/README.md`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5.1/pyproject.toml` & `fau_tools-1.4.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 reportUnusedExpression  = false
 
 # useLibraryCodeForTypes = false
 
 
 [tool.poetry]
 name = "Fau-tools"
-version = "1.4.5.1"
+version = "1.4.5.2"
 description = "A python module. The main function is for pytorch training."
 authors = ["Fau <Fau818@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "Fau_tools"}]
 homepage   = "https://github.com/Fau818/Fau_tools"
 repository = "https://github.com/Fau818/Fau_tools"
```

### Comparing `fau_tools-1.4.5.1/PKG-INFO` & `fau_tools-1.4.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fau-tools
-Version: 1.4.5.1
+Version: 1.4.5.2
 Summary: A python module. The main function is for pytorch training.
 Home-page: https://github.com/Fau818/Fau_tools
 License: MIT
 Author: Fau
 Author-email: Fau818@qq.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
```

