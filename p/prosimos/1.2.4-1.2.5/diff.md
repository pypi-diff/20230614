# Comparing `tmp/prosimos-1.2.4.tar.gz` & `tmp/prosimos-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosimos-1.2.4.tar", max compression
+gzip compressed data, was "prosimos-1.2.5.tar", max compression
```

## Comparing `prosimos-1.2.4.tar` & `prosimos-1.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    15059 2023-05-24 09:38:28.436268 prosimos-1.2.4/README.md
--rw-r--r--   0        0        0        0 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/__init__.py
--rw-r--r--   0        0        0     3478 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/emd_metric.py
--rw-r--r--   0        0        0      489 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/exceptions.py
--rw-r--r--   0        0        0     7248 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/inter_arrival_cases_discovery.py
--rw-r--r--   0        0        0     5615 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/log_comparison_metrics.py
--rw-r--r--   0        0        0    44084 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/log_parser.py
--rw-r--r--   0        0        0        0 2023-05-24 09:38:28.456268 prosimos-1.2.4/cli/__init__.py
--rw-r--r--   0        0        0     3539 2023-05-24 09:38:28.456268 prosimos-1.2.4/cli/diff_res_bpsim.py
--rw-r--r--   0        0        0        0 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/__init__.py
--rw-r--r--   0        0        0    44577 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/batch_processing.py
--rw-r--r--   0        0        0     4383 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/batch_processing_parser.py
--rw-r--r--   0        0        0     2626 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/case_attributes.py
--rw-r--r--   0        0        0    48440 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/control_flow_manager.py
--rw-r--r--   0        0        0      487 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/exceptions.py
--rw-r--r--   0        0        0     7340 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/execution_info.py
--rw-r--r--   0        0        0     1109 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/file_manager.py
--rw-r--r--   0        0        0     3147 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/prioritisation.py
--rw-r--r--   0        0        0     1345 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/prioritisation_parser.py
--rw-r--r--   0        0        0     3009 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/prioritisation_rules.py
--rw-r--r--   0        0        0     8585 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/probability_distributions.py
--rw-r--r--   0        0        0      467 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/resource_profile.py
--rw-r--r--   0        0        0    29275 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/simulation_engine.py
--rw-r--r--   0        0        0    22072 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/simulation_properties_parser.py
--rw-r--r--   0        0        0     6298 2023-05-24 09:38:28.560268 prosimos-1.2.4/prosimos/simulation_queues_ds.py
--rw-r--r--   0        0        0     6005 2023-05-24 09:38:28.560268 prosimos-1.2.4/prosimos/simulation_setup.py
--rw-r--r--   0        0        0    15565 2023-05-24 09:38:28.560268 prosimos-1.2.4/prosimos/simulation_stats.py
--rw-r--r--   0        0        0    14171 2023-05-24 09:38:28.560268 prosimos-1.2.4/prosimos/simulation_stats_calculator.py
--rw-r--r--   0        0        0     1730 2023-05-24 09:38:28.560268 prosimos-1.2.4/prosimos/weekday_helper.py
--rw-r--r--   0        0        0      637 2023-05-24 09:38:28.560268 prosimos-1.2.4/pyproject.toml
--rw-r--r--   0        0        0    15764 1970-01-01 00:00:00.000000 prosimos-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0    15059 2023-06-14 13:10:19.975922 prosimos-1.2.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/__init__.py
+-rw-r--r--   0        0        0     3478 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/emd_metric.py
+-rw-r--r--   0        0        0      489 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/exceptions.py
+-rw-r--r--   0        0        0     7248 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/inter_arrival_cases_discovery.py
+-rw-r--r--   0        0        0     5615 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/log_comparison_metrics.py
+-rw-r--r--   0        0        0    44084 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/log_parser.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:10:19.995922 prosimos-1.2.5/cli/__init__.py
+-rw-r--r--   0        0        0     3539 2023-06-14 13:10:19.995922 prosimos-1.2.5/cli/diff_res_bpsim.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/__init__.py
+-rw-r--r--   0        0        0    44577 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/batch_processing.py
+-rw-r--r--   0        0        0     4383 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/batch_processing_parser.py
+-rw-r--r--   0        0        0     2626 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/case_attributes.py
+-rw-r--r--   0        0        0    48440 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/control_flow_manager.py
+-rw-r--r--   0        0        0      487 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/exceptions.py
+-rw-r--r--   0        0        0     7340 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/execution_info.py
+-rw-r--r--   0        0        0     1109 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/file_manager.py
+-rw-r--r--   0        0        0     3147 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/prioritisation.py
+-rw-r--r--   0        0        0     1345 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/prioritisation_parser.py
+-rw-r--r--   0        0        0     3009 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/prioritisation_rules.py
+-rw-r--r--   0        0        0     8585 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/probability_distributions.py
+-rw-r--r--   0        0        0      467 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/resource_profile.py
+-rw-r--r--   0        0        0    29275 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_engine.py
+-rw-r--r--   0        0        0    22072 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_properties_parser.py
+-rw-r--r--   0        0        0     6298 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_queues_ds.py
+-rw-r--r--   0        0        0     6005 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_setup.py
+-rw-r--r--   0        0        0    15565 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_stats.py
+-rw-r--r--   0        0        0    14171 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_stats_calculator.py
+-rw-r--r--   0        0        0     1730 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/weekday_helper.py
+-rw-r--r--   0        0        0      637 2023-06-14 13:10:20.111923 prosimos-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0    15765 1970-01-01 00:00:00.000000 prosimos-1.2.5/PKG-INFO
```

### Comparing `prosimos-1.2.4/README.md` & `prosimos-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/bpdfr_discovery/emd_metric.py` & `prosimos-1.2.5/bpdfr_discovery/emd_metric.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/bpdfr_discovery/inter_arrival_cases_discovery.py` & `prosimos-1.2.5/bpdfr_discovery/inter_arrival_cases_discovery.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/bpdfr_discovery/log_comparison_metrics.py` & `prosimos-1.2.5/bpdfr_discovery/log_comparison_metrics.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/bpdfr_discovery/log_parser.py` & `prosimos-1.2.5/bpdfr_discovery/log_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/cli/diff_res_bpsim.py` & `prosimos-1.2.5/cli/diff_res_bpsim.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/batch_processing.py` & `prosimos-1.2.5/prosimos/batch_processing.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/batch_processing_parser.py` & `prosimos-1.2.5/prosimos/batch_processing_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/case_attributes.py` & `prosimos-1.2.5/prosimos/case_attributes.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/control_flow_manager.py` & `prosimos-1.2.5/prosimos/control_flow_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/execution_info.py` & `prosimos-1.2.5/prosimos/execution_info.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/file_manager.py` & `prosimos-1.2.5/prosimos/file_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/prioritisation.py` & `prosimos-1.2.5/prosimos/prioritisation.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/prioritisation_parser.py` & `prosimos-1.2.5/prosimos/prioritisation_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/prioritisation_rules.py` & `prosimos-1.2.5/prosimos/prioritisation_rules.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/probability_distributions.py` & `prosimos-1.2.5/prosimos/probability_distributions.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/simulation_engine.py` & `prosimos-1.2.5/prosimos/simulation_engine.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/simulation_properties_parser.py` & `prosimos-1.2.5/prosimos/simulation_properties_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/simulation_queues_ds.py` & `prosimos-1.2.5/prosimos/simulation_queues_ds.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/simulation_setup.py` & `prosimos-1.2.5/prosimos/simulation_setup.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/simulation_stats.py` & `prosimos-1.2.5/prosimos/simulation_stats.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/simulation_stats_calculator.py` & `prosimos-1.2.5/prosimos/simulation_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/prosimos/weekday_helper.py` & `prosimos-1.2.5/prosimos/weekday_helper.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.4/pyproject.toml` & `prosimos-1.2.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prosimos"
-version = "1.2.4"
+version = "1.2.5"
 description = ""
 authors = ["Iryna Halenok, Orlenys López Pintado"]
 readme = "README.md"
 packages = [
     {include = "cli"},
     {include = "prosimos"},
     {include = "bpdfr_discovery"}
@@ -15,15 +15,15 @@
 click = "^8.1.3"
 numpy = "^1.24.3"
 pandas = "^2.0.1"
 python-dateutil = "^2.8.2"
 pytz = "^2023.3"
 scipy = "^1.10.1"
 pm4py = "^2.7.4"
-pix-framework = "^0.8.7"
+pix-framework = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.scripts]
 prosimos = "cli.diff_res_bpsim:cli"
```

### Comparing `prosimos-1.2.4/PKG-INFO` & `prosimos-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: prosimos
-Version: 1.2.4
+Version: 1.2.5
 Summary: 
 Author: Iryna Halenok, Orlenys López Pintado
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: pix-framework (>=0.8.7,<0.9.0)
+Requires-Dist: pix-framework (>=0.9.0,<0.10.0)
 Requires-Dist: pm4py (>=2.7.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Prosimos
```

