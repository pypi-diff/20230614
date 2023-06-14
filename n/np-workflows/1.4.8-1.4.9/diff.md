# Comparing `tmp/np_workflows-1.4.8.tar.gz` & `tmp/np_workflows-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_workflows-1.4.8.tar", max compression
+gzip compressed data, was "np_workflows-1.4.9.tar", max compression
```

## Comparing `np_workflows-1.4.8.tar` & `np_workflows-1.4.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1331 2023-03-31 21:40:33.929251 np_workflows-1.4.8/pyproject.toml
--rw-r--r--   0        0        0      701 2023-03-17 23:19:28.815209 np_workflows-1.4.8/README.md
--rw-r--r--   0        0        0      238 2023-03-07 00:58:26.213008 np_workflows-1.4.8/src/np_workflows/__init__.py
--rw-r--r--   0        0        0    10071 2023-02-02 02:47:52.020772 np_workflows-1.4.8/src/np_workflows/assets/images/logo_np_hab.png
--rw-r--r--   0        0        0    19349 2023-02-02 02:47:52.021771 np_workflows-1.4.8/src/np_workflows/assets/images/logo_np_vis.png
--rw-r--r--   0        0        0       39 2023-02-20 22:40:54.036068 np_workflows-1.4.8/src/np_workflows/experiments/__init__.py
--rw-r--r--   0        0        0      114 2023-03-09 03:08:15.270031 np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/__init__.py
--rw-r--r--   0        0        0     2094 2023-03-17 23:19:28.822209 np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py
--rw-r--r--   0        0        0     4004 2023-03-17 23:19:28.824209 np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py
--rw-r--r--   0        0        0     4400 2023-02-23 00:51:23.316978 np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py
--rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py
--rw-r--r--   0        0        0     8383 2023-03-17 23:19:28.825209 np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py
--rw-r--r--   0        0        0     2335 2023-03-17 23:19:28.826207 np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py
--rw-r--r--   0        0        0     8693 2023-03-17 23:19:28.828209 np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py
--rw-r--r--   0        0        0      131 2023-03-07 00:47:58.271771 np_workflows-1.4.8/src/np_workflows/shared/__init__.py
--rw-r--r--   0        0        0    15025 2023-03-22 01:12:13.212055 np_workflows-1.4.8/src/np_workflows/shared/base_experiments.py
--rw-r--r--   0        0        0     6074 2023-03-17 23:19:28.830208 np_workflows-1.4.8/src/np_workflows/shared/npxc.py
--rw-r--r--   0        0        0    22759 2023-03-22 21:20:12.875230 np_workflows-1.4.8/src/np_workflows/shared/widgets.py
--rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 np_workflows-1.4.8/setup.py
--rw-r--r--   0        0        0     1430 1970-01-01 00:00:00.000000 np_workflows-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1330 2023-04-12 00:42:18.794128 np_workflows-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0      701 2023-03-17 23:19:28.815209 np_workflows-1.4.9/README.md
+-rw-r--r--   0        0        0      238 2023-03-07 00:58:26.213008 np_workflows-1.4.9/src/np_workflows/__init__.py
+-rw-r--r--   0        0        0    10071 2023-02-02 02:47:52.020772 np_workflows-1.4.9/src/np_workflows/assets/images/logo_np_hab.png
+-rw-r--r--   0        0        0    19349 2023-02-02 02:47:52.021771 np_workflows-1.4.9/src/np_workflows/assets/images/logo_np_vis.png
+-rw-r--r--   0        0        0       39 2023-02-20 22:40:54.036068 np_workflows-1.4.9/src/np_workflows/experiments/__init__.py
+-rw-r--r--   0        0        0      114 2023-03-09 03:08:15.270031 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/__init__.py
+-rw-r--r--   0        0        0     2094 2023-03-17 23:19:28.822209 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py
+-rw-r--r--   0        0        0     4004 2023-03-17 23:19:28.824209 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py
+-rw-r--r--   0        0        0     4400 2023-02-23 00:51:23.316978 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py
+-rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py
+-rw-r--r--   0        0        0     8512 2023-04-03 20:46:08.140120 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py
+-rw-r--r--   0        0        0     2335 2023-03-17 23:19:28.826207 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py
+-rw-r--r--   0        0        0     8693 2023-03-17 23:19:28.828209 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py
+-rw-r--r--   0        0        0      131 2023-03-07 00:47:58.271771 np_workflows-1.4.9/src/np_workflows/shared/__init__.py
+-rw-r--r--   0        0        0    14760 2023-04-03 22:57:54.450052 np_workflows-1.4.9/src/np_workflows/shared/base_experiments.py
+-rw-r--r--   0        0        0     6074 2023-03-17 23:19:28.830208 np_workflows-1.4.9/src/np_workflows/shared/npxc.py
+-rw-r--r--   0        0        0    25569 2023-04-12 00:38:16.173714 np_workflows-1.4.9/src/np_workflows/shared/widgets.py
+-rw-r--r--   0        0        0     1868 1970-01-01 00:00:00.000000 np_workflows-1.4.9/setup.py
+-rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 np_workflows-1.4.9/PKG-INFO
```

### Comparing `np_workflows-1.4.8/pyproject.toml` & `np_workflows-1.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "np-workflows"
-version = "1.4.8"
+version = "1.4.9"
 description = "Ecephys and behavior workflows for the Mindscope Neuropixels team."
 authors = ["Ben Hardcastle <ben.hardcastle@alleninstitute.org>"]
 readme = "README.md"
 packages = [{include = "np_workflows", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 np-services = ">= 0.1.46"
-np-session = ">=0.4.27"
+np-session = ">=0.5.1"
 np-probe-targets = "*"
 np-datajoint = "*"
 ipywidgets = "^7"
 pydantic = "^1"
 jupyterlab = "^3.6"
 jupyterlab-git = "^0.41.0"
 jupyter-scheduler = "^1.2.0"
```

### Comparing `np_workflows-1.4.8/README.md` & `np_workflows-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.8/src/np_workflows/assets/images/logo_np_hab.png` & `np_workflows-1.4.9/src/np_workflows/assets/images/logo_np_hab.png`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.8/src/np_workflows/assets/images/logo_np_vis.png` & `np_workflows-1.4.9/src/np_workflows/assets/images/logo_np_vis.png`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py` & `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py` & `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py` & `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py` & `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py` & `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,15 +106,16 @@
         match self.ttn_session:
             case TTNSession.PRETEST:
                 return
             case TTNSession.HAB_60 | TTNSession.HAB_90 | TTNSession.HAB_120:
                 self.session.project.state['latest_hab'] = self.session.id
             case TTNSession.EPHYS:
                 self.session.project.state['latest_ephys'] = self.session.id
-            
+                self.session.project.state['sessions'] = self.session.project.state.get('sessions', []) + [self.session.id]
+                
     def run_stim_scripts(self) -> None:
 
         self.update_state()
         
         for stim in ('mapping', 'main', 'opto'):
             
             if not (params := self.params[stim]):
```

### Comparing `np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py` & `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.8/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py` & `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.8/src/np_workflows/shared/base_experiments.py` & `np_workflows-1.4.9/src/np_workflows/shared/base_experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,16 +243,16 @@
                 logger.debug(f'Renaming: {name} already has probe letter suffix - aborted')
                 continue
             if length := len(split_folders := [_ for _ in folders if _.name == name]) != 2:
                 logger.info(f'Renaming: {length} folders found for {name}, expected 2 - aborted')
                 continue
             logger.debug('Renaming split ephys folders %r', split_folders)
             for folder, probe_letters in zip(sorted(split_folders, key=lambda x: x.as_posix()), ('ABC', 'DEF')):
-                folder.replace(folder.with_name(f'{name}_probe{probe_letters}'))
-                renamed_folders.append(folder)
+                renamed = folder.replace(folder.with_name(f'{name}_probe{probe_letters}'))
+                renamed_folders.append(renamed)
             logger.info('Renamed split ephys folders %r', split_folders)
         np_services.OpenEphys.data_files = renamed_folders
         
     def copy_data_files(self) -> None:
         """Copy data files from raw data storage to session folder for all services."""
         for service in self.services:
             match service.__name__:
@@ -321,26 +321,18 @@
         
     def copy_ephys(self) -> None:
         # copy ephys       
         self.rename_split_ephys_folders()
         password = np_config.fetch('/logins')['svc_neuropix']['password']
         ssh = fabric.Connection(host=np_services.OpenEphys.host, user='svc_neuropix', connect_kwargs=dict(password=password))
         for ephys_folder in np_services.OpenEphys.data_files:
-
-            if ephys_folder.drive.endswith("A"):
-                probes = '_probeABC'
-            elif ephys_folder.drive.endswith("B"):
-                probes = '_probeDEF'
-            else:
-                probes = '_probes'
-                
             with contextlib.suppress(Exception):
                 with ssh:
                     ssh.run(
-                    f'robocopy "{ephys_folder}" "{self.session.npexp_path / (self.session.npexp_path.name + probes)}" /j /s /xo' 
+                    f'robocopy "{ephys_folder}" "{self.session.npexp_path / ephys_folder.name} /j /s /xo' 
                     # /j unbuffered, /s incl non-empty subdirs, /xo exclude src files older than dest
                     ) 
                            
                            
 class Ephys(WithLims):
     default_session_type = 'ephys'
```

### Comparing `np_workflows-1.4.8/src/np_workflows/shared/npxc.py` & `np_workflows-1.4.9/src/np_workflows/shared/npxc.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.8/src/np_workflows/shared/widgets.py` & `np_workflows-1.4.9/src/np_workflows/shared/widgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -288,18 +288,18 @@
         session.platform_json.wheel_height = height_counter.value
         session.mouse.state['wheel_height'] = height_counter.value
         save_button.button_style = 'success'
         save_button.description = 'Saved'
     save_button.on_click(on_click)
     return IPython.display.display(ipw.VBox([height_counter,save_button]))
     
-    
+
 def di_widget(session: np_session.Session) -> IPython.display.DisplayHandle | None:
     "Supply a path or a platform json instance. Saves a JSON file with the dye used in the session and a timestamp."
-
+    
     di_info: dict[str, int | str] = dict(
         EndTime=0, StartTime=npxc.now(), dii_description="", times_dipped=0, previous_uses="",
     )
     di_info.update(session.platform_json.DiINotes)
     
     layout = ipw.Layout(max_width='180px')
     dipped_counter = ipw.IntText(value=0, min=0, max=99, description="Dipped count", layout=layout)
@@ -321,14 +321,72 @@
         
     save_button.on_click(on_click)
     return IPython.display.display(ipw.VBox([
         dipped_counter, dye_dropdown, 
         usage_counter, save_button]))
 
     
+def dye_info_widget(session: np_session.Session) -> IPython.display.DisplayHandle | None:
+    """
+    - scan barcode or enter ID number for the dye used
+    - change dye description if incorrect (DiI, DiO)
+    - increment number of times probes were dipped this session
+    - hit `Save` to store info in platform.json
+    """
+    
+    di_info: dict[str, int | str] = dict(
+        EndTime=0, StartTime=npxc.now(), dii_description="", times_dipped=0, previous_uses="",
+    )
+    di_info.update(session.platform_json.DiINotes)
+    
+    width = lambda w: ipw.Layout(max_width=f'{w}px')
+    
+    dye_id_entry = ipw.Text(value=None, description='Dye ID', layout=width(250), placeholder='Enter ID or scan barcode')
+    dye_usage_button = ipw.Button(description='Record single use', button_style='warning', layout=width(180))
+    first_usage = ipw.Text(value='', description="First use", layout=width(250), disabled=True)
+    dye_dropdown = ipw.Dropdown(description="Description:", options=np_session.Dye.descriptions, layout=width(180))
+    dipped_counter = ipw.IntText(value=di_info['times_dipped'], min=0, max=99, description="Dipped count", layout=width(150))
+    usage_counter = ipw.IntText(value=int(di_info['previous_uses']), min=0, max=99, description="Previous uses", layout=width(180), disabled=True)
+    save_button = ipw.Button(description='Save', button_style='warning', layout=width(180))
+    if (desc := di_info['dii_description']) in np_session.Dye.descriptions:
+        dye_dropdown.value = desc
+        
+    def update_display(_):
+        with contextlib.suppress(Exception):
+            dye = np_session.Dye(int(str(dye_id_entry.value)))
+            dye_dropdown.value = dye.description
+            usage_counter.value = dye.previous_uses
+            first_usage.value = f'{dye.first_use}'
+    dye_id_entry.observe(update_display, 'value')
+    
+    def record_dye_usage():
+        with contextlib.suppress(Exception):
+            dye = np_session.Dye(int(str(dye_id_entry.value)))
+            dye.description = dye_dropdown.value
+            dye.increment_uses()
+        
+    def update_di_info():
+        di_info['EndTime'] = npxc.now()
+        di_info['times_dipped'] = str(dipped_counter.value)
+        di_info['dii_description'] = str(dye_dropdown.value)
+        di_info['previous_uses'] = str(usage_counter.value)
+        
+    def on_click(b):
+        update_di_info()
+        record_dye_usage()
+        session.platform_json.DiINotes = di_info
+        save_button.description = 'Saved'
+        save_button.button_style = 'success'
+        
+    save_button.on_click(on_click)
+    return IPython.display.display(ipw.VBox([
+        dye_id_entry,
+        dipped_counter, dye_dropdown, 
+        usage_counter, first_usage, save_button]))
+
 def dye_widget(session_folder: pathlib.Path) -> IPython.display.DisplayHandle | None:
     "Supply a path - saves a JSON file with the dye used in the session and a timestamp."
 
     di_info: dict[str, int | str] = dict(
         EndTime=0, StartTime=0, dii_description="DiI", times_dipped=0,
     )
```

### Comparing `np_workflows-1.4.8/setup.py` & `np_workflows-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,20 @@
  'ipywidgets>=7,<8',
  'jupyter-scheduler>=1.2.0,<2.0.0',
  'jupyterlab-git>=0.41.0,<0.42.0',
  'jupyterlab>=3.6,<4.0',
  'np-datajoint',
  'np-probe-targets',
  'np-services>=0.1.46',
- 'np-session>=0.4.27',
+ 'np-session>=0.5.1',
  'pydantic>=1,<2']
 
 setup_kwargs = {
     'name': 'np-workflows',
-    'version': '1.4.8',
+    'version': '1.4.9',
     'description': 'Ecephys and behavior workflows for the Mindscope Neuropixels team.',
     'long_description': '# np_workflows\n\nThis package contains all the Python code required to run Mindscope Neuropixels experiments.\n\nExperiment workflows and related tasks are coordinated by Jupyter notebooks maintained here:\nhttps://github.com/AllenInstitute/np_notebooks\n\nRunning the notebooks requires a Python environment with:\n- Python >= 3.11\n- np_workflows\n- Jupyter / JupyterLab\n\n```\ngit clone https://github.com/AllenInstitute/np_notebooks\nconda create -n workflows python=3.11\npip install np_workflows\npip install jupyterlab\n```\n\n\nKeep the `np_workflows` package up-to-date by running `pip install\nnp_workflows -U` before each use\n\nTo develop this package `git clone` then `poetry install`\n',
     'author': 'Ben Hardcastle',
     'author_email': 'ben.hardcastle@alleninstitute.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `np_workflows-1.4.8/PKG-INFO` & `np_workflows-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: np-workflows
-Version: 1.4.8
+Version: 1.4.9
 Summary: Ecephys and behavior workflows for the Mindscope Neuropixels team.
 Author: Ben Hardcastle
 Author-email: ben.hardcastle@alleninstitute.org
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipylab (>=0.6.0,<0.7.0)
 Requires-Dist: ipywidgets (>=7,<8)
 Requires-Dist: jupyter-scheduler (>=1.2.0,<2.0.0)
 Requires-Dist: jupyterlab (>=3.6,<4.0)
 Requires-Dist: jupyterlab-git (>=0.41.0,<0.42.0)
 Requires-Dist: np-datajoint
 Requires-Dist: np-probe-targets
 Requires-Dist: np-services (>=0.1.46)
-Requires-Dist: np-session (>=0.4.27)
+Requires-Dist: np-session (>=0.5.1)
 Requires-Dist: pydantic (>=1,<2)
 Description-Content-Type: text/markdown
 
 # np_workflows
 
 This package contains all the Python code required to run Mindscope Neuropixels experiments.
```

