# Comparing `tmp/orange-system-dynamics-1.0.1.tar.gz` & `tmp/orange-system-dynamics-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orange-system-dynamics-1.0.1.tar", last modified: Mon Mar 20 13:39:27 2023, max compression
+gzip compressed data, was "orange-system-dynamics-1.0.2.tar", last modified: Mon Jun  5 18:50:48 2023, max compression
```

## Comparing `orange-system-dynamics-1.0.1.tar` & `orange-system-dynamics-1.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:39:27.516884 orange-system-dynamics-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4392 2023-03-20 13:39:27.516884 orange-system-dynamics-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3894 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:39:27.488884 orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4392 2023-03-20 13:39:27.000000 orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1486 2023-03-20 13:39:27.000000 orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 13:39:27.000000 orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      138 2023-03-20 13:39:27.000000 orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-20 13:39:27.000000 orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 13:39:27.000000 orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      154 2023-03-20 13:39:27.000000 orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-20 13:39:27.000000 orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:39:27.448883 orange-system-dynamics-1.0.1/orangecontrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:39:27.520884 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-20 13:39:27.520884 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:39:27.500884 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-03-07 15:35:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7762 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     6425 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     2707 2023-03-07 15:35:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/eurostat.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-03-07 15:35:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/geolocalization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:39:27.516884 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/
--rw-rw-rw-   0 root         (0) root         (0)     1279 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/agent.svg
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/environment.svg
--rw-rw-rw-   0 root         (0) root         (0)     6390 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/eurostat.svg
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/geolocation.svg
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/load_simulation.svg
--rw-rw-rw-   0 root         (0) root         (0)     1626 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/name.svg
--rw-rw-rw-   0 root         (0) root         (0)     4932 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/statemachine.svg
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-03-20 13:04:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/load_simulation.py
--rw-rw-rw-   0 root         (0) root         (0)     3096 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/name_table.py
--rw-rw-rw-   0 root         (0) root         (0)     7175 2023-03-07 15:35:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)     2315 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/statemachine.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1189 2023-03-20 13:39:27.516884 orange-system-dynamics-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-03-07 15:35:55.000000 orange-system-dynamics-1.0.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 18:50:48.546629 orange-system-dynamics-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5196 2023-06-05 18:50:48.546629 orange-system-dynamics-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4698 2023-06-05 18:45:58.000000 orange-system-dynamics-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 18:50:48.478628 orange-system-dynamics-1.0.2/orange_system_dynamics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5196 2023-06-05 18:50:48.000000 orange-system-dynamics-1.0.2/orange_system_dynamics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-06-05 18:50:48.000000 orange-system-dynamics-1.0.2/orange_system_dynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 18:50:48.000000 orange-system-dynamics-1.0.2/orange_system_dynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-05 18:50:48.000000 orange-system-dynamics-1.0.2/orange_system_dynamics.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-05 18:50:48.000000 orange-system-dynamics-1.0.2/orange_system_dynamics.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 18:50:48.000000 orange-system-dynamics-1.0.2/orange_system_dynamics.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-05 18:50:48.000000 orange-system-dynamics-1.0.2/orange_system_dynamics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-05 18:50:48.000000 orange-system-dynamics-1.0.2/orange_system_dynamics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 18:50:48.446627 orange-system-dynamics-1.0.2/orangecontrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 18:50:48.546629 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-05 18:50:48.546629 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 18:50:48.482628 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-03-07 15:35:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     6425 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2023-03-07 15:35:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/geolocalization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 18:50:48.534629 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/agent.svg
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/environment.svg
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/geolocation.svg
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/load_simulation.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/name.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6390 2023-04-03 15:20:02.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/service.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4932 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/statemachine.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-03-20 13:04:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/load_simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3096 2023-06-05 18:45:58.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/name_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    14523 2023-04-03 15:27:08.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/service_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     7175 2023-03-07 15:35:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2315 2023-03-20 12:56:55.000000 orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/statemachine.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-04-03 15:20:02.000000 orange-system-dynamics-1.0.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1189 2023-06-05 18:50:48.546629 orange-system-dynamics-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-03-07 15:35:55.000000 orange-system-dynamics-1.0.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-03-06 17:08:41.000000 orange-system-dynamics-1.0.2/versioneer.py
```

### Comparing `orange-system-dynamics-1.0.1/PKG-INFO` & `orange-system-dynamics-1.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: orange-system-dynamics
-Version: 1.0.1
-Summary: Add-on containing widgets for system dynamics operations
-Home-page: https://gitlab.com/drb-python/samples/odm/sd_addon
-Author: GAEL Systems
-Author-email: drb-python@gael.fr
-License: LGPLv3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Environment :: Plugins
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # Orange3 System Dynamics Add-on
 
 This is an add-on for [Orange3](https://orangedatamining.com/) allowing to
 perform simulation using _System Dynamic Modeling_ (SDM) mechanism.
 
 ## Orange Data Mining
 **ODM** (_Orange Data Mining_) is an open source machine learning and data
@@ -57,91 +43,91 @@
 
 ### System Dynamics
 
 System dynamics (SD) is an approach to understanding the nonlinear behaviour
 of complex systems over time using stocks, flows,
 internal feedback loops, table functions and time delays.
 
-![](screenshots/Workflow_Example.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Workflow_Example.png)
 
 ### Load Simulation Widget
 `Load Simulation` widget is used to load simulation models in .mdl or .xmile format,
 it outputs the model for Simulation.
 
-![](screenshots/Load.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Load.png)
 
 ### Simulation Widget
 Once the model is loaded, the `Simulation` Widget is updated to show model's
 variables grouped by:
 - Time Controls: contains the initial time, the final time and defined time
 step
 - Stocks: contains all model’s stocks, can be used to change any stock’s
 initial value
 - Auxiliary Values: contains  all the auxiliary values, can also be changed
 
-![](screenshots/Simulation.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Simulation.png)
 
 Once the Run Simulation button’s hit, the model is run, the widget outputs an
 Orange Data Table, we use the `Line Chart` Widget to visualize results of
 simulation: 
 
-![](screenshots/Line_Chart.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Line_Chart.png)
 
 Other widgets have been used to perform step by step execution of simulation, by simply running the 
 results through `As Timeseries` while indicating Time as the index variable:
 
-![](screenshots/As_Timeseries.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/As_Timeseries.png)
 
 Next, using `Time Slice` which was adapted to commit a cumulative step by step simulation 
 to the Line Chart:
 
-![](screenshots/Time_Slice.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Time_Slice.png)
 
 In another example; we run the simulation in two different regions: 
 
 - Paris (France)
 
 - Algiers(Algeria) and Casablanca (Morocco)
 
 with different simulation parameters each time, we variate the total population, 
 contact infectivity and the stocks (infectious, recovered, susceptible).
 We simply add the results together using Concatenate:
 
-![](screenshots/Workflow_Example1.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Workflow_Example1.png)
 
 We can also show the results in Geo Map, after adding Latitude and Longitude information: 
 
-![](screenshots/Geo_Map.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Geo_Map.png)
 
 ### Agent Based Model 
 
 An agent-based model (ABM) is a computational model for simulating the actions 
 and interactions of autonomous agents (both individual or collective entities such as 
 organizations or groups) in order to 
 understand the behavior of a system and what governs its outcomes.
 
-![](screenshots/Workflow_Example2.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Workflow_Example2.png)
 
 ### State Machine Widget
 `State Machine` widget is used to read a .yaml file containing a statemachine.
 
-![](screenshots/State_Machine.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/State_Machine.png)
 
 ### Agent Widget
-̀`Agent` widget creates an agent from a statemachine, it outputs the model used for 
+̀Agent` widget creates an agent from a statemachine, it outputs the model used for 
 creating multi-agent system environment.
 
-![](screenshots/Agent.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Agent.png)
 
 `Multi Agent Environment` is used to define interactions between agents 
 in a multi-agent system configuration.
 
-![](screenshots/Multi_Agent.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Multi_Agent.png)
 
 Once the Run Simulation button’s hit, the model is run, the widget outputs an
 Orange Data Table, we use the `Line Chart` Widget to visualize results of
 simulation: 
 
-![](screenshots/Line_Chart2.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Line_Chart.png)
```

### Comparing `orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/PKG-INFO` & `orange-system-dynamics-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-system-dynamics
-Version: 1.0.1
+Version: 1.0.2
 Summary: Add-on containing widgets for system dynamics operations
 Home-page: https://gitlab.com/drb-python/samples/odm/sd_addon
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
@@ -57,91 +57,91 @@
 
 ### System Dynamics
 
 System dynamics (SD) is an approach to understanding the nonlinear behaviour
 of complex systems over time using stocks, flows,
 internal feedback loops, table functions and time delays.
 
-![](screenshots/Workflow_Example.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Workflow_Example.png)
 
 ### Load Simulation Widget
 `Load Simulation` widget is used to load simulation models in .mdl or .xmile format,
 it outputs the model for Simulation.
 
-![](screenshots/Load.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Load.png)
 
 ### Simulation Widget
 Once the model is loaded, the `Simulation` Widget is updated to show model's
 variables grouped by:
 - Time Controls: contains the initial time, the final time and defined time
 step
 - Stocks: contains all model’s stocks, can be used to change any stock’s
 initial value
 - Auxiliary Values: contains  all the auxiliary values, can also be changed
 
-![](screenshots/Simulation.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Simulation.png)
 
 Once the Run Simulation button’s hit, the model is run, the widget outputs an
 Orange Data Table, we use the `Line Chart` Widget to visualize results of
 simulation: 
 
-![](screenshots/Line_Chart.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Line_Chart.png)
 
 Other widgets have been used to perform step by step execution of simulation, by simply running the 
 results through `As Timeseries` while indicating Time as the index variable:
 
-![](screenshots/As_Timeseries.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/As_Timeseries.png)
 
 Next, using `Time Slice` which was adapted to commit a cumulative step by step simulation 
 to the Line Chart:
 
-![](screenshots/Time_Slice.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Time_Slice.png)
 
 In another example; we run the simulation in two different regions: 
 
 - Paris (France)
 
 - Algiers(Algeria) and Casablanca (Morocco)
 
 with different simulation parameters each time, we variate the total population, 
 contact infectivity and the stocks (infectious, recovered, susceptible).
 We simply add the results together using Concatenate:
 
-![](screenshots/Workflow_Example1.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Workflow_Example1.png)
 
 We can also show the results in Geo Map, after adding Latitude and Longitude information: 
 
-![](screenshots/Geo_Map.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Geo_Map.png)
 
 ### Agent Based Model 
 
 An agent-based model (ABM) is a computational model for simulating the actions 
 and interactions of autonomous agents (both individual or collective entities such as 
 organizations or groups) in order to 
 understand the behavior of a system and what governs its outcomes.
 
-![](screenshots/Workflow_Example2.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Workflow_Example2.png)
 
 ### State Machine Widget
 `State Machine` widget is used to read a .yaml file containing a statemachine.
 
-![](screenshots/State_Machine.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/State_Machine.png)
 
 ### Agent Widget
-̀`Agent` widget creates an agent from a statemachine, it outputs the model used for 
+̀Agent` widget creates an agent from a statemachine, it outputs the model used for 
 creating multi-agent system environment.
 
-![](screenshots/Agent.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Agent.png)
 
 `Multi Agent Environment` is used to define interactions between agents 
 in a multi-agent system configuration.
 
-![](screenshots/Multi_Agent.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Multi_Agent.png)
 
 Once the Run Simulation button’s hit, the model is run, the widget outputs an
 Orange Data Table, we use the `Line Chart` Widget to visualize results of
 simulation: 
 
-![](screenshots/Line_Chart2.png)
+![](https://gitlab.com/drb-python/samples/odm/sd_addon/-/raw/main/screenshots/Line_Chart.png)
```

### Comparing `orange-system-dynamics-1.0.1/orange_system_dynamics.egg-info/SOURCES.txt` & `orange-system-dynamics-1.0.2/orange_system_dynamics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 orange_system_dynamics.egg-info/requires.txt
 orange_system_dynamics.egg-info/top_level.txt
 orangecontrib/system_dynamics/__init__.py
 orangecontrib/system_dynamics/_version.py
 orangecontrib/system_dynamics/widgets/__init__.py
 orangecontrib/system_dynamics/widgets/agent.py
 orangecontrib/system_dynamics/widgets/environment.py
-orangecontrib/system_dynamics/widgets/eurostat.py
 orangecontrib/system_dynamics/widgets/geolocalization.py
 orangecontrib/system_dynamics/widgets/load_simulation.py
 orangecontrib/system_dynamics/widgets/name_table.py
+orangecontrib/system_dynamics/widgets/service_table.py
 orangecontrib/system_dynamics/widgets/simulation.py
 orangecontrib/system_dynamics/widgets/statemachine.py
 orangecontrib/system_dynamics/widgets/icons/agent.svg
 orangecontrib/system_dynamics/widgets/icons/category.svg
 orangecontrib/system_dynamics/widgets/icons/environment.svg
-orangecontrib/system_dynamics/widgets/icons/eurostat.svg
 orangecontrib/system_dynamics/widgets/icons/geolocation.svg
 orangecontrib/system_dynamics/widgets/icons/load_simulation.svg
 orangecontrib/system_dynamics/widgets/icons/name.svg
+orangecontrib/system_dynamics/widgets/icons/service.svg
 orangecontrib/system_dynamics/widgets/icons/statemachine.svg
```

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/agent.py` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/agent.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/environment.py` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/environment.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/geolocalization.py` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/geolocalization.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/agent.svg` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/agent.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/environment.svg` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/environment.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/eurostat.svg` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/service.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/name.svg` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/name.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/icons/statemachine.svg` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/icons/statemachine.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/load_simulation.py` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/load_simulation.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/name_table.py` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/name_table.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/simulation.py` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/simulation.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/orangecontrib/system_dynamics/widgets/statemachine.py` & `orange-system-dynamics-1.0.2/orangecontrib/system_dynamics/widgets/statemachine.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/setup.cfg` & `orange-system-dynamics-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.0.1/versioneer.py` & `orange-system-dynamics-1.0.2/versioneer.py`

 * *Files identical despite different names*

