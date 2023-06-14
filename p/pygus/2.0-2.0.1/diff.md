# Comparing `tmp/pygus-2.0.tar.gz` & `tmp/pygus-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygus-2.0.tar", max compression
+gzip compressed data, was "pygus-2.0.1.tar", max compression
```

## Comparing `pygus-2.0.tar` & `pygus-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2022-10-31 16:02:43.286749 pygus-2.0/LICENSE
--rw-r--r--   0        0        0     1541 2023-02-22 17:36:23.738197 pygus-2.0/README-pypi.md
--rw-r--r--   0        0        0      134 2023-04-20 10:39:32.247844 pygus-2.0/pygus/__init__.py
--rw-r--r--   0        0        0      156 2023-04-20 10:39:32.248007 pygus-2.0/pygus/gus/__init__.py
--rw-r--r--   0        0        0    27311 2023-04-20 10:39:32.248384 pygus-2.0/pygus/gus/agents.py
--rw-r--r--   0        0        0     7484 2023-04-20 10:39:32.248656 pygus-2.0/pygus/gus/allometrics.py
--rw-r--r--   0        0        0     3069 2023-04-20 10:39:32.248771 pygus-2.0/pygus/gus/inputs/allometrics.json
--rw-r--r--   0        0        0       95 2023-04-20 10:39:32.248836 pygus-2.0/pygus/gus/inputs/scenario.json
--rw-r--r--   0        0        0      264 2023-04-20 10:39:32.248895 pygus-2.0/pygus/gus/inputs/site.json
--rw-r--r--   0        0        0     5932 2023-04-20 10:39:32.248983 pygus-2.0/pygus/gus/inputs/trees.csv
--rw-r--r--   0        0        0    15469 2023-04-20 10:39:32.249144 pygus-2.0/pygus/gus/models.py
--rw-r--r--   0        0        0  1566870 2023-04-20 10:39:32.257838 pygus-2.0/pygus/gus/outputs/trees_yearly.json
--rw-r--r--   0        0        0     2241 2023-04-20 12:41:09.601132 pygus-2.0/pygus/gus/utilities.py
--rw-r--r--   0        0        0     1701 2023-04-20 10:39:32.258149 pygus-2.0/pygus/gus/weather.py
--rw-r--r--   0        0        0       58 2023-04-20 10:39:32.258299 pygus-2.0/pygus/impacts/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-20 10:39:32.258425 pygus-2.0/pygus/impacts/carbon.py
--rw-r--r--   0        0        0    32960 2023-04-20 10:39:32.258637 pygus-2.0/pygus/impacts/water.py
--rw-r--r--   0        0        0     1499 2023-06-13 15:12:13.755133 pygus-2.0/pyproject.toml
--rw-r--r--   0        0        0     2655 1970-01-01 00:00:00.000000 pygus-2.0/setup.py
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 pygus-2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-31 16:02:43.286749 pygus-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1541 2023-02-22 17:36:23.738197 pygus-2.0.1/README-pypi.md
+-rw-r--r--   0        0        0      161 2023-06-13 15:15:35.246634 pygus-2.0.1/pygus/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-13 15:15:35.246958 pygus-2.0.1/pygus/gus/__init__.py
+-rw-r--r--   0        0        0    27311 2023-04-20 10:39:32.248384 pygus-2.0.1/pygus/gus/agents.py
+-rw-r--r--   0        0        0     7484 2023-04-20 10:39:32.248656 pygus-2.0.1/pygus/gus/allometrics.py
+-rw-r--r--   0        0        0     3069 2023-04-20 10:39:32.248771 pygus-2.0.1/pygus/gus/inputs/allometrics.json
+-rw-r--r--   0        0        0       95 2023-04-20 10:39:32.248836 pygus-2.0.1/pygus/gus/inputs/scenario.json
+-rw-r--r--   0        0        0      264 2023-04-20 10:39:32.248895 pygus-2.0.1/pygus/gus/inputs/site.json
+-rw-r--r--   0        0        0     5932 2023-04-20 10:39:32.248983 pygus-2.0.1/pygus/gus/inputs/trees.csv
+-rw-r--r--   0        0        0    16122 2023-06-13 15:15:35.247416 pygus-2.0.1/pygus/gus/models.py
+-rw-r--r--   0        0        0  1566870 2023-04-20 10:39:32.257838 pygus-2.0.1/pygus/gus/outputs/trees_yearly.json
+-rw-r--r--   0        0        0     4210 2023-06-13 15:15:35.247781 pygus-2.0.1/pygus/gus/utilities.py
+-rw-r--r--   0        0        0     1701 2023-04-20 10:39:32.258149 pygus-2.0.1/pygus/gus/weather.py
+-rw-r--r--   0        0        0       58 2023-04-20 10:39:32.258299 pygus-2.0.1/pygus/impacts/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-20 10:39:32.258425 pygus-2.0.1/pygus/impacts/carbon.py
+-rw-r--r--   0        0        0    32960 2023-04-20 10:39:32.258637 pygus-2.0.1/pygus/impacts/water.py
+-rw-r--r--   0        0        0     1501 2023-06-13 15:20:03.803904 pygus-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 pygus-2.0.1/setup.py
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 pygus-2.0.1/PKG-INFO
```

### Comparing `pygus-2.0/LICENSE` & `pygus-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygus-2.0/README-pypi.md` & `pygus-2.0.1/README-pypi.md`

 * *Files identical despite different names*

### Comparing `pygus-2.0/pygus/gus/agents.py` & `pygus-2.0.1/pygus/gus/agents.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0/pygus/gus/allometrics.py` & `pygus-2.0.1/pygus/gus/allometrics.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0/pygus/gus/inputs/allometrics.json` & `pygus-2.0.1/pygus/gus/inputs/allometrics.json`

 * *Files identical despite different names*

### Comparing `pygus-2.0/pygus/gus/inputs/trees.csv` & `pygus-2.0.1/pygus/gus/inputs/trees.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0/pygus/gus/models.py` & `pygus-2.0.1/pygus/gus/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,63 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 # Importing Python Libraries
-import site
+import time
+from typing import Dict, Union
+import pandas as pd
 import numpy as np
 from functools import reduce
-import json
 import logging
 
 # Importing necessary Mesa packages
 from mesa import Model
 from mesa.time import RandomActivation
 from mesa.space import MultiGrid
 from mesa.datacollection import DataCollector
 
 # Importing needed GUS objects
 from .agents import Tree
 from .allometrics import Species
 from .weather import WeatherSim
 
-
+       
+class WeatherConfig:
+    def __init__(self, mean_growth_rate: int = 153, growth_rate_var: int = 7):
+        self.mean_growth_rate = mean_growth_rate
+        self.growth_rate_var = growth_rate_var
+
+class SiteConfig:
+    """A class to hold site configuration parameters."""
+
+    def __init__(self, total_m2: int, impervious_m2: int, pervious_m2: int, weather: Union[Dict, WeatherConfig], tree_density_per_ha: int = None, site_type: str = "park"):
+        self.total_m2 = total_m2
+        self.impervious_m2 = impervious_m2
+        self.pervious_m2 = pervious_m2
+        self.tree_density_per_ha = tree_density_per_ha
+        # if weather is a dict, create a weatherConfig, else use the object
+        if isinstance(weather, dict):
+            self.weather = WeatherConfig(**weather)
+        else:
+            self.weather = weather
+        self.site_type = site_type
+         
 class Urban(Model):
     """A generic urban green space model. To be tailored according to specific sites."""
 
     # Used to hold the scaling of actual physical space within the digital space.
     # It shows the size of each cell (square) in meters.
-    # TODO: this needs to be brought up as a parameter and placed within the groups
+    # FIXME: this needs to be brought up as a parameter and placed within the groups
     #      of parameters that handle physical to digital twin mapping.
-    dt_resolution = 2  # in meters
+    # dt_resolution = 2  # in meters
 
     site_types = ["park", "street", "forest", "pocket"]
 
     def __init__(
-        self, population, species_composition, site_config, scenario, batch=False
+        self, population: pd.DataFrame, species_composition: str, site_config: SiteConfig, scenario: Dict, batch=False
     ):
         """The constructor method.
 
         Args:
             population: (:obj:`pd.DataFrame`): A dataframe tree properties are read from a site.
             species_composition (:obj:`str`): The name of the file that keeps allometrics of the tree species for the site.
             site_config: (:obj:`string`): name of the json file.
@@ -53,56 +74,45 @@
         """
         super().__init__()
         # Setting MESA specific parameters
         width = int(max(population.xpos)) + 1
         length = int(max(population.ypos)) + 1
         self.grid = MultiGrid(width, length, torus=False)
         # to be parameterized and set during initialization.
-        self.schedule = RandomActivation(self)
 
-        self._load_site_parameters(site_config)
+        self._handle_site_configuration(site_config, len(population))
         self._load_experiment_parameters(scenario)
 
         # Load species composition and their allometrics
         self.species = Species(species_composition)  # will be used by agents.
 
         # Test that the df is complete or raise keyerror
         for attribute in ["dbh", "species", "condition", "xpos", "ypos"]:
             population[attribute]
 
         # copy and import df
         self.df = population
         self.num_agents = len(population)
+        self.schedule = RandomActivation(self)
+        
         self.sapling_dbh = min(population.dbh)
         # Each entry index i, represents number of years since the biomass is decay period.
         self.release_bins = {
             "slow": np.zeros(10),  # for dead root and standing tree.
             "fast": np.zeros(10),  # for mulched biomass
         }
 
         # Create agents.
         for index, row in self.df.iterrows():
-            # Tree init
             a = Tree(
                 row.id, self, dbh=row.dbh, species=row.species, condition=row.condition
             )
             self.schedule.add(a)
 
-            # Place trees on the plot sequentially
-            # based on their id/index.
-            # TODO: This snippet may need to be converted into a function as part of
-            # initilisartion module and x,y points need to be part of input DB.
-            # x = int(index % self.grid.width)
-            # y = int(index / self.grid.height)
-
-            # # Add the agent to a random grid cell
-            # x = self.random.randrange(self.grid.width)
-            # y = self.random.randrange(self.grid.height)
-
-            # # Locate the trees based on actual physical positioning
+            # Place trees on the plot based on actual physical positioning
             x = row.xpos
             y = row.ypos
             self.grid.place_agent(a, (x, y))
 
         # This variable below works as an indexer while adding new trees to the population during the run time.
         self.current_id = max(population.id)
 
@@ -126,14 +136,15 @@
                 "Dying": lambda m: self.count(m, "condition", lambda x: x == "dying"),
                 "Poor": lambda m: self.count(m, "condition", lambda x: x == "poor"),
                 "Replaced": lambda m: self.count(
                     m, "condition", lambda x: x == "replaced"
                 ),
                 "Seq_std": self.agg_std_sequestration,
             },
+
             agent_reporters={
                 "species": "species",
                 "dbh": "dbh",
                 "height": "tree_height",
                 "crownH": "crown_height",
                 "crownW": "crown_width",
                 "canopy_overlap": "overlap_ratio",
@@ -151,121 +162,83 @@
             },
         )
         logging.info(
             "Initialisation of the Digital Twins of {} trees on a {} by {} digital space is complete!".format(
                 self.num_agents, width, length
             )
         )
-
+        
+    def run(self, steps = None):
+        """Customized MESA method that sets the major components of scenario analyses process."""
+        pop = str(self.df.shape[0])
+        if not steps:
+            steps = self.scenario.get("time_horizon_years")
+            print("Running for {} steps".format(steps))
+        start = time.time()
+        logging.info("Year:{}".format(self.schedule.time + 1))
+        for _ in range(steps):
+            self.step()
+        end = time.time()
+        print("{} steps completed (pop. {}): {}".format(steps, pop, end - start))
+        logging.info("Simulation is complete!")
+        
     def step(self):
-        """Customized MESA method that sets the major components of scenario analyses process.
-
-        Args:
-            None
-
-        Returns:
-            None
-
-        Note:
-            None
-
-        Todo:
-            None
-        """
+        """Customized MESA method that sets the major components of scenario analyses process."""
         logging.info("Year:{}".format(self.schedule.time + 1))
         self.get_weather_projection()
 
         logging.info("Agents are working ...")
         self.schedule.step()
 
         logging.info("Yearly data is being collected ...")
         self.datacollector.collect(self)
-        # print('Step:{}'.format(self.schedule.time))
+        
+        # print('Step:{} ({}s)'.format(self.schedule.time, end-start))
         # print(self.release_bins['slow'])
         # print(self.release_bins['fast'])
-
-    def _load_experiment_parameters(self, experiment):
+    
+    def impact_analysis(self) -> pd.DataFrame:
+        """
+        Provides impact analysis of the simulation
+        """
+        df_out_site = self.datacollector.get_model_vars_dataframe()
+        return Urban.format_impact_analysis(df_out_site)
+        
+    def _load_experiment_parameters(self, experiment: Dict):
         """Loads site configuration information.
 
         Args:
             experiment: (:obj:`dict`): Python dictionary that holds experiment parameters.
 
-        Returns:
-            None
-        Todo:
-            None
 
         """
 
         # Read denisty to set the digital twin resolution which is defined as
         # the cell size in terms of actual distance.
         if "maintenance_scope" in experiment.keys():
             # maintenance_scope: (:obj:`int`): It can be 0:None,1:base, 2:cared)
             self.maintenance_scope = experiment["maintenance_scope"]
         else:
             logging.warning(
                 "Maintenance scope is not given. A high maintenance site is assumed."
             )
             self.maintenance_scope = 2
 
-    def _load_site_parameters(self, config_file):
-        """Loads site configuration information.
-
-        Args:
-            config_file: (:obj:`string`): name of the json file.
-
-        Returns:
-            None
-        Todo:
-            None
-
-        """
-        try:
-            f = open(config_file)
-        except IOError as e:
-            print(str(e))
-        params = json.loads(f.read())
-
-        # read site type
-        stype = "park"  # default type
-        if "project_site_type" in params.keys():
-            if params["project_site_type"] in Urban.site_types:
-                stype = params["project_site_type"]
-            else:
-                logging.warning(
-                    "Undefined site type recognized. Park type will be used."
-                )
-        else:
-            logging.warning("Site type is not provided. Park type will be used.")
-        self.site_type = stype
-
-        # Read in growth season mean and variance to be used by weather forecasting module.
-        try:
-            self.season_mean = params["weather"]["growth_season_mean"]
-            self.season_var = params["weather"]["growth_season_var"]
-        except KeyError:
-            self.season_mean = 153
-            self.season_var = 7
-            logging.warning(
-                "Tree growth season mean and variance is not provided as expected. Global average is used."
-            )
-
-        # Read denisty to set the digital twin resolution which is defined as
-        # the cell size in terms of actual distance.
-        if "area_tree_density_per_hectare" in params.keys():
-            self.dt_resolution = np.sqrt(
-                10000 / params["area_tree_density_per_hectare"]
-            )
-            # The distance between the center of two tree trunks in meters. Even spatial distribution is assumed.
-        else:
-            logging.warning(
-                "area_tree_density_per_hectare is not given the default {} meters is used the distance from the clossest tree trunks.".format(
-                    self.dt_resolution
-                )
-            )
+    def _handle_site_configuration(self, site_config: SiteConfig, population_size: int):
+        """Loads site configuration information."""
+        
+        self.season_mean = site_config.season_mean
+        self.season_var = site_config.season_var
+        self.site_type = site_config.site_type
+        self.dt_resolution = round(
+            np.sqrt(
+                1 / (population_size / site_config.total_m2)
+            ),
+            2 # round to < decimal places
+        )
 
     def get_weather_projection(self):
         """The method retrieves wetaher projection for the current iteration,
         eg. year, at the moment it uses a simulated projections on the go,
         instead previously computed estimates or forecasts can be used as well.
 
         Args:
@@ -415,7 +388,33 @@
 
             check:
                 import scipy.integrate as integrate
                 integrate.quad(f, 0, 20) > 0.96 for k in (2:5).
         """
         k = 2 if state in ("mulched", "fast") else 5
         return 1 / k * np.exp(-1 * year / k)
+
+    @staticmethod
+    def format_impact_analysis(model_vars: pd.DataFrame) -> pd.DataFrame:
+        """
+        Cleans the output of the simulation
+        """
+        # Process and clean data after the simulation
+
+        # IMPACT ANALYSIS
+        model_vars["Cum_Seq"] = model_vars.Seq.cumsum()
+        model_vars["Avg_Seq"] = model_vars.Seq / model_vars.Alive
+        model_vars["Avg_Rel"] = model_vars.Released / model_vars.Alive
+
+        # Processing to avoid out of range float values
+        inf_count = np.isinf(model_vars).values.sum()
+        if inf_count > 0:
+            logging.debug("Cleaning {} INF values...".format(str(inf_count)))
+            model_vars.replace([np.inf, -np.inf], np.nan, inplace=True)
+
+        # Replace Nan values with 0. This can happen when the number of alive trees is 0 and the above divisions in 'IMPACT ANALYSIS' are performed.
+        has_na_values = model_vars.isnull().values.any()
+        if has_na_values:
+            logging.debug("Removing N/A values...")
+            model_vars.fillna(0, inplace=True)
+
+        return model_vars
```

### Comparing `pygus-2.0/pygus/gus/outputs/trees_yearly.json` & `pygus-2.0.1/pygus/gus/outputs/trees_yearly.json`

 * *Files identical despite different names*

### Comparing `pygus-2.0/pygus/gus/weather.py` & `pygus-2.0.1/pygus/gus/weather.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0/pygus/impacts/carbon.py` & `pygus-2.0.1/pygus/impacts/carbon.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0/pygus/impacts/water.py` & `pygus-2.0.1/pygus/impacts/water.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0/pyproject.toml` & `pygus-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyGUS"
-version = "2.0"
+version = "2.0.1"
 description = "Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis."
 authors = ["Bulent Ozel <bulent@lucidminds.ai>"] 
 maintainers = [
     "Oguzhan Yayla <oguzhan@lucidminds.ai>", 
     "Marko Petrovic <marko@lucidminds.ai>", 
     "Axel Nilsson <axel@darkmatterlabs.org>"
 ]
```

### Comparing `pygus-2.0/setup.py` & `pygus-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'pytest>=7.1.2,<8.0.0',
  'seaborn>=0.11.2,<0.12.0',
  'termcolor>=2.1.1,<3.0.0',
  'utm>=0.7.0,<0.8.0']
 
 setup_kwargs = {
     'name': 'pygus',
-    'version': '2.0',
+    'version': '2.0.1',
     'description': 'Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.',
     'long_description': '[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Versions](https://img.shields.io/pypi/pyversions/pygus)]()\n\n\n\n# gus\n![GUS-IMAGE](https://miro.medium.com/max/1400/1*fMM7rnq1RJCh-nFBGLUvyA.png)\n\nGreen Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.\n\n## Getting Started\nVisit the GUS [website documentation](https://lucidmindsai.github.io/gus/) for help with installing GUS, code documentation, and a [basic tutorial](https://github.com/lucidmindsai/gus/blob/main/notebooks/Tutorial.ipynb) to get you started. \n\n## Install from PyPi\nWe publish GUS as `pyGus` package in PyPi. Dependencies can be found in the .toml file on the GUS GitHub page. Even though installation with Poetry is possible, the most stable installation can be done via pip.\n\n```\n$ pip install pygus\n```\n\nFor further instructions and code documentation, visit [GUS Code Documentation](https://lucidmindsai.github.io/gus/)\n\n### Who maintains GUS?\nThe GUS is currently developed and maintained by [Lucidminds](https://lucidminds.ai/) and [Dark Matter Labs](https://darkmatterlabs.org/) members as part of their joint project [TreesAI](https://treesasinfrastructure.com/#/).\n\n### Notes\n* The GUS is open for PRs.\n* PRs will be reviewed by the current maintainers of the project.\n* Extensive development guidelines will be provided soon.\n* To report bugs, fixes, and questions, please use the [GitHub issues](https://github.com/lucidmindsai/gus/issues).',
     'author': 'Bulent Ozel',
     'author_email': 'bulent@lucidminds.ai',
     'maintainer': 'Oguzhan Yayla',
     'maintainer_email': 'oguzhan@lucidminds.ai',
     'url': 'https://github.com/lucidmindsai/gus',
```

### Comparing `pygus-2.0/PKG-INFO` & `pygus-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygus
-Version: 2.0
+Version: 2.0.1
 Summary: Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.
 Home-page: https://github.com/lucidmindsai/gus
 License: Apache-2.0
 Author: Bulent Ozel
 Author-email: bulent@lucidminds.ai
 Maintainer: Oguzhan Yayla
 Maintainer-email: oguzhan@lucidminds.ai
```

