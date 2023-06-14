# Comparing `tmp/leggedsnake-0.3.0.tar.gz` & `tmp/leggedsnake-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leggedsnake-0.3.0.tar", last modified: Wed Jul 21 18:44:34 2021, max compression
+gzip compressed data, was "leggedsnake-0.3.1.tar", last modified: Wed Jun 14 07:18:29 2023, max compression
```

## Comparing `leggedsnake-0.3.0.tar` & `leggedsnake-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 18:44:34.219545 leggedsnake-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     5210 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    17344 2021-07-21 18:44:34.219545 leggedsnake-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9398 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 18:44:34.215545 leggedsnake-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/docs/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (121)    28583 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/docs/changeloglink.html
--rw-r--r--   0 runner    (1001) docker     (121)    25259 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/docs/genindex.html
--rw-r--r--   0 runner    (1001) docker     (121)    30647 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (121)     7036 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/docs/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (121)    27009 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/docs/readmelink.html
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/docs/search.html
--rw-r--r--   0 runner    (1001) docker     (121)    16337 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/docs/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 18:44:34.219545 leggedsnake-0.3.0/leggedsnake/
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/leggedsnake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22707 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/leggedsnake/dynamiclinkage.py
--rw-r--r--   0 runner    (1001) docker     (121)    14785 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/leggedsnake/geneticoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    17270 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/leggedsnake/physicsengine.py
--rw-r--r--   0 runner    (1001) docker     (121)   559093 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/leggedsnake/show_evolution.py
--rw-r--r--   0 runner    (1001) docker     (121)     4810 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/leggedsnake/utility.py
--rw-r--r--   0 runner    (1001) docker     (121)     3780 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/leggedsnake/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 18:44:34.219545 leggedsnake-0.3.0/leggedsnake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17344 2021-07-21 18:44:34.000000 leggedsnake-0.3.0/leggedsnake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      637 2021-07-21 18:44:34.000000 leggedsnake-0.3.0/leggedsnake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-21 18:44:34.000000 leggedsnake-0.3.0/leggedsnake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-07-21 18:44:34.000000 leggedsnake-0.3.0/leggedsnake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-07-21 18:44:34.000000 leggedsnake-0.3.0/leggedsnake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-07-21 18:44:34.219545 leggedsnake-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      199 2021-07-21 18:44:25.000000 leggedsnake-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:29.307823 leggedsnake-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)    28583 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/changeloglink.html
+-rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    30647 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/readmelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16337 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/leggedsnake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/dynamiclinkage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/geneticoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/physicsengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/show_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/leggedsnake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-06-14 07:18:29.000000 leggedsnake-0.3.1/leggedsnake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-14 07:18:29.000000 leggedsnake-0.3.1/leggedsnake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:18:29.000000 leggedsnake-0.3.1/leggedsnake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 07:18:29.000000 leggedsnake-0.3.1/leggedsnake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 07:18:29.000000 leggedsnake-0.3.1/leggedsnake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/tests/test_utility.py
```

### Comparing `leggedsnake-0.3.0/CODE_OF_CONDUCT.md` & `leggedsnake-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.0/LICENSE.rst` & `leggedsnake-0.3.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.0/PKG-INFO` & `leggedsnake-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: leggedsnake
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simulate and optimize planar leg mechanisms using PSO and GA
 Home-page: https://hugofara.github.io/leggedsnake/
 Author: Hugo Farajallah
 License: MIT License
 Project-URL: Changelog, https://hugofara.github.io/leggedsnake/changeloglink.html
 Project-URL: Source, https://github.com/HugoFara/leggedsnake
 Keywords: linkage,leg mechanism,optimization,leggedsnake,walking linkage
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Life
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,325 +19,475 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# leggedsnake
+
 [![PyPI version fury.io](https://badge.fury.io/py/leggedsnake.svg)](https://pypi.python.org/pypi/leggedsnake/)
-[![Downloads](https://static.pepy.tech/personalized-badge/leggedsnake?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads/week)](https://pepy.tech/project/leggedsnake)
+[![Downloads](https://static.pepy.tech/personalized-badge/leggedsnake?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/leggedsnake)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg )](https://raw.githubusercontent.com/HugoFara/leggedsnake/master/LICENSE.rst)
-# leggedsnake
-LeggedSnake is a project intended to make the simulation of walking linkages fast and easy. We believe that building walking linkages is fun and could be useful. Our philosophy is to provide a quick way of building, optimizing and testing walking linkages.
+
+LeggedSnake is a project intended to make the simulation of walking linkages fast and easy. 
+We believe that building walking linkages is fun and could be useful.
+Our philosophy is to provide a quick way of building, optimizing and testing walking linkages.
 
 We handle planar [leg mechanisms](https://en.wikipedia.org/wiki/Leg_mechanism) in three main parts:
+
 * Linkage conception in simple Python relying on [pylinkage](https://github.com/HugoFara/pylinkage).
 * Kinematic optimization with ``Walker`` class, inheriting from pylinkage's ``Linkage`` class.
 * Dynamic simulation and its optimization using genetic algorithms.
 
 ## Quick links
+
 * For the documentation, check the docs at [hugofara.github.io/leggedsnake](https://hugofara.github.io/leggedsnake/)!
 * Source code is hosted on GitHub as [HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake)
 * We also provide a Python package on PyPi, test [leggedsnake](https://pypi.org/project/leggedsnake/).
 * If you just want to chill out looking at walking linkages striving to survive, join the [discussions](https://github.com/HugoFara/leggedsnake/discussions).
 
 Contributors are welcome!
 
 ## Installation
+
 ### Using pip
+
 The package is hosted on PyPi as [leggedsnake](https://pypi.org/project/leggedsnake/), use:
-``pip install leggedsnake``
+
+```bash
+pip install leggedsnake
+```
 
 ### Setting up Virtual Environment
-We provide an [environment.yml](https://github.com/HugoFara/leggedsnake/blob/master/environment.yml) file for conda. Use ``conda env update --file environment.yml --name leggedsnake-env`` to install the requirements in a separate environment. 
 
-If you are looking for a development version, check the GitHub repo under [HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake). 
+We provide an [environment.yml](https://github.com/HugoFara/leggedsnake/blob/master/environment.yml) file for conda. 
+Use ``conda env update --file environment.yml --name leggedsnake-env`` to install the requirements in a separate environment.
+
+If you are looking for a development version, check the GitHub repo under 
+[HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake).
 
-## Requirements
 
-Python 3, numpy for calculation, matplotlib for drawing, and standard libraries. 
+## Contribute
 
-For kinematic optimization you can either use the built-in algorithm, or [PySwarms](https://pyswarms.readthedocs.io/en/latest/), under MIT license. PySwarms is a much more complexe package which provides quick calculations, however with modern laptops the built-in swarm optimization should be quick enough to fit your needs.
+Download the latest GitHub version, then install the dev requirements in ``requirements-dev.txt``.
 
-Dynamic optimization relies on multiple packages. First of all it uses [Pymunk](http://www.pymunk.org/en/latest/index.html), made by Victor Blomqvist, as a physics engine. Then you can either use the built-in algorithm, or the GA module from [PyGAD](https://pygad.readthedocs.io/en/latest/). PyGAD is a complete library providing much more than genetic algorithms, so it might be heavy. PyGAD is more complete than the built-in however, so I haven't decided to continue on PyGAD or switch for another solution in the future.
+In a nutshell
+
+```bash
+git clone https://github.com/HugoFara/leggedsnake.git
+cd leggedsnake
+pip install -r requirements-dev.txt
+```
+
+### Testing
+
+We use unittest. Just run ``python3 -m unittest discover .`` from the main folder.
+
+### Release
+
+This section is mainly intended for maintainers. 
+Fell free to use the tools described here, but they are not necessary in any way.
+
+* To publish a new version, use ``bump2version``. For instance ``bump2version minor``.
+* Regenerate the documentation with ``make html`` (uses Sphinx).
 
 ## Usage
 
-The demo script is [strider.py](https://github.com/HugoFara/leggedsnake/blob/master/docs/examples/strider.py), which demonstrates all the techniques about the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html).
+The demo script is [strider.py](https://github.com/HugoFara/leggedsnake/blob/master/docs/examples/strider.py), which
+demonstrates all the techniques about the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html).
 
 ### Defining a ``Walker``
-First, you need to define joints for your ``Walker`` as described in [pylinkage](https://github.com/HugoFara/pylinkage) documentation. Once your joints (let's say they are in a joint object), you should have something like that:
-```python
+
+First, you need to define joints for your ``Walker`` as described in [pylinkage](https://github.com/HugoFara/pylinkage)
+documentation. Once your joints (let's say they are in a joint object), you should have something like that:
+
+```python3
 import leggedsnake as ls
 
 # Center of the Walker
-A = ls.Static(x=0, y=0, name="A")
-B = ls.Crank(1, 0, distance=1, angle=0.31, name="Crank")
-# etc... let's say with have joints up to E
+linkage = {
+    "A": ls.Static(x=0, y=0, name="A"),
+    "B": ls.Crank(1, 0, distance=1, angle=0.31, name="Crank")
+    # etc...
+}
 my_walker = ls.Walker(
-  joints=(A, B, C, D, E),
-  name="My Walker"
+    joints=linkage.values(),
+    name="My Walker"
 )
 ```
 
-``Walker`` is just a herited class of ``Linkage``, with some useful methods, and behaves quite the same way.
+``Walker`` is just an inherited class of ``Linkage``, with some useful methods, and behaves quite the same way.
 
 ### Kinematic optimization using Particle Swarm Optimization (PSO)
-No change compared to a classic linkage optimization. You should use the ``step`` and ``stride`` method from the [utility module](https://github.com/HugoFara/leggedsnake/blob/master/leggedsnake/utility.py) as fitness functions. 
+
+No change compared to a classic linkage optimization. You should use the ``step`` and ``stride`` method from the 
+[utility module](https://github.com/HugoFara/leggedsnake/blob/master/leggedsnake/utility.py) as fitness functions.
 This set of rules should work well for a stride **maximisation** problem:
+
 1. Rebuild the Walker with the provided set of dimensions, and do a complete turn.
-1. If the Walker raise an UnbuildableError, its score is 0 (or ``- float('inf')`` if you use other evaluation functions.
-1. Verify if it can pass a certain obstacke using ``step`` function. If not, its score is 0.
-1. Eventually mesure the length of its stide with the ``stride`` function. Return this length as its score.
+2. If the Walker raises an UnbuildableError, its score is 0 (or ``-float('inf')`` if you use other evaluation functions).
+3. Verify if it can pass a certain obstacle using ``step`` function. If not, its score is 0.
+4. Eventually measure the length of its stride with the ``stride`` function. Return this length as its score.
 
 ### Dynamic Optimization using Genetic Algorithm (GA)
-Kinematic optimization is fast, however it can return weird results, and it has no sense of gravity while walking heavily relies on gravity. This is why you may need to use dynamic optimization thanks to [Pymunk](http://www.pymunk.org/en/latest/index.html). However the calculation is much more slower, and you can no longer tests millions of linkages as in PSO (or you will need time). This is why we use [genetic algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm), because it can provide good results with less parents.
 
-We handle everything almost evything world definition to linkage conversion. Appart from the GA parameters, you just have to define a fitness function. Here are the main steps for a **maximisation problem**:
-1. Create a function of two arguments, the first one should be the paramaters of the linkage, the second the initial positions for the joints.
-1. Try to do a revolution in **kinematic simulation**. If the Walker raises an ``UnbuildableError`` set its score to ``-float('inf')``.
-1. Otherwise use this procedure 
+Kinematic optimization is fast, but it can return weird results, and it has no sense of gravity while walking heavily
+relies on gravity. This is why you may need to use dynamic optimization thanks to
+[Pymunk](http://www.pymunk.org/en/latest/index.html). However, the calculation is much slower, and you can no
+longer test millions of linkages as in PSO (or you will need time). This is why we
+use [genetic algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm), because it can provide good results with
+fewer parents.
+
+We handle everything almost everything world definition to linkage conversion. Apart from the GA parameters, you just
+have to define a fitness function. Here are the main steps for a **maximisation problem**:
+
+1. Create a function of two arguments, the first one should be the parameters of the linkage, the second the initial positions for the joints.
+2. Try to do a revolution in **kinematic simulation**. If the Walker raises an ``UnbuildableError`` set its score to ``-float('inf')``.
+3. Otherwise, use the following procedure:
+
+```python3
+import leggedsnake as ls
 
-```python
 def dynamic_linkage_fitness(walker):
-  """
-  Make the dynamic evalutaion of a Walker.
-  
-  Return yield and initial position of joints.
-  """
-  world = pe.World()
-  # We handle all the conversions
-  world.add_linkage(walker)
-  # Simulation duration (in seconds)
-  duration = 40
-  # Somme of yields
-  tot = 0
-  # Motor turned on duration
-  dur = 0
-  n = duration * pe.params["camera"]["fps"]
-  n /= pe.params["simul"]["time_coef"]
-  for j in range(int(n)):
-      efficiency, energy = world.update(j)
-      tot += efficiency
-      dur += energy
-  if dur == 0:
-      return - float('inf'), list()
-  print("Score:", tot / dur)
-  # Return 100 times average yield, and initial positions as the final score
-  return tot / dur, pos
+    """
+    Make the dynamic evaluation of a Walker.
+    
+    Return yield and initial position of joints.
+    """
+    world = ls.World()
+    # We handle all the conversions
+    world.add_linkage(walker)
+    # Simulation duration (in seconds)
+    duration = 40
+    # Somme of yields
+    tot = 0
+    # Motor turned on duration
+    dur = 0
+    n = duration * ls.params["camera"]["fps"]
+    n /= ls.params["simul"]["time_coef"]
+    pos = tuple(walker.step())[-1]
+    for j in range(int(n)):
+        efficiency, energy = world.update(j)
+        tot += efficiency
+        dur += energy
+    if dur == 0:
+        return - float('inf'), list()
+    print("Score:", tot / dur)
+    # Return 100 times average yield, and initial positions as the final score
+    return tot / dur, pos
 ```
 
-And now, relax while your computer recreates a civilisation of walking machines!
+And now, relax while your computer creates a civilization of walking machines!
 
 ### Visualization
-For this part we will focus on the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html), an exemple file is provided at ``docs/examples/strider.py``. The linkage looks like this:
+
+For this part we will focus on the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html), 
+an example file is provided at ``docs/examples/strider.py``.
+
+The linkage looks like this:
 ![A Kinematic representation of Strider linkage](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Kinematic%20unoptimized%20Strider.gif)
 
 Looks cool? Let's simulate it dynamically!
 
 ![Dynamic one-leg-pair Strider being tested](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Dynamic%20unoptimized%20one-legged%20Strider.gif)
 
-Oops! Here is what you get when you forget to add more legs! There is **real danger here**, because your walker crawls well, you will be able to optimize efficiently the "crawler", *which may be not your goal*. 
+Oops! Here is what you get when you forget to add more legs! There is **real danger here**, because your walker crawls
+well, you will be able to optimize efficiently the "crawler", *which may be not your goal*.
 
-Let's add three more leg pairs. Why three? Many legs means more mass and constraints, so less yield and more intensive computations. On the other hand, we always want the center of mass over the [support line](https://en.wikipedia.org/wiki/Support_polygon), which means that if the walker begins to lift a foot (let's say a front foot), and another doesn't come on the ground ahead of it, the linkage will to fall nose to the ground. With more foots we make the "snooping" time shorter, and a total of four leg pairs is a minimum for this *unoptimized* version. 
+Let's add three more leg pairs. Why three? Many legs mean more mass and constraints, so less yield and more intensive
+computations. On the other hand, we always want the center of mass over the
+[support line](https://en.wikipedia.org/wiki/Support_polygon), which means that if the walker begins to lift a foot
+(let's say a front foot), and another doesn't come on the ground ahead of it, the linkage will fall nose to the
+ground. With more feet, we make the "snooping" time shorter, and a total of four leg pairs is a minimum for this
+*unoptimized* version.
 
 A simple way to do it is:
+
 ```python
 my_linkage.add_legs(3) # Replace "my_linkage" with your Walker object
 ```
+
 Let's have a look at the artist:
 
 ![Dynamic four-leg-pair unoptimized Strider](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Dynamic%20unoptimized%20strider.gif)
 
 ## Advice
-Use the vizualisation tools provided! The optimization tools should always give you a score with a better fitness, but it might not be what you expected. Tailor your optimization and *then* go for a long run will make you save a lot of time.
 
-**Do not** use optimized linkages from the start! The risk is to fall to quickly into a suboptimal solution. They are several mechanisms to prevent that (starting from random position), however it can always have an impact on the rest of the optimization.
+Use the visualisation tools provided! The optimization tools should always give you a score with a better fitness,
+but it might not be what you expected. Tailor your optimization and *then* go for a long run will make you save a lot
+of time.
+
+**Do not** use optimized linkages from the start! The risk is to fall to quickly into a suboptimal solution. They are
+several mechanisms to prevent that (starting from random position), but it can always have an impact on the rest of
+the optimization.
+
+Try to minimize the number of elements in the optimizations! You can often use some linkage properties to reduce the
+number of simulation parameters. For instance, the Strider linkage has axial symmetry. While it is irrelevant to use
+this property in dynamic simulation, you can use "half" your Strider in a kinematic optimization, which is much faster.
 
-Try to minimize the number of elements in the optimizations! You can often use some linkage's properties to reduce the number of simulation parameters. For instance, the Strider linkage has an axial symmetry. While it is irrelevant to use this property in dynamic simulation, you can use "half" your Strider in a kinematic optimization, which is much faster:
 ![A Kinematic half Strider](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Kinematic%20half-Strider.gif)
 
+## Requirements
+
+Python 3, numpy for calculation, matplotlib for drawing, and standard libraries.
+
+For kinematic optimization, you can either use the built-in algorithm, or
+[PySwarms](https://pyswarms.readthedocs.io/en/latest/), under MIT license. 
+PySwarms is a much more complex package which provides quick calculations, 
+however, with modern laptops the built-in swarm optimization should be quick enough
+to fit your needs.
+
+Dynamic optimization relies on multiple packages.
+First of all, it uses [Pymunk](http://www.pymunk.org/en/latest/index.html),
+made by Victor Blomqvist, as its physics engine. 
+The genetic algorithm optimizer is home-made, 
+but feel free to use any external tool suiting your needs!
 # Changelog
+
 All notable changes to the LeggedSnake will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased]
+## [0.3.1] - 2023-06-14
+
+Starting from 0.3.1, we won't include "-alpha" or "-beta" in the naming scheme,
+as it is considered irrelevant.
+
+### Added in 0.3.1
+
+- ``requirements-dev.txt`` that contain dev requirements. It makes contribution easier.
+- PyCharm configuration files.
+
+### Changed in 0.3.1
+
+- Animations are now all stored in local variables, and no longer in an "ani"
+global list of animations.
+
+### Fixed in 0.3.1
+
+- The main example file ``strider.py`` was launching animations for each subprocess.
+This file is now considered an executable.
+- ``evolutionary_optimization_builtin`` was during the last evaluation of linkages.
+- ``data_descriptors`` were not save for the first line of data only in
+  ``geneticoptimizer``.
+- Multiple grammar corrections.
+- The ``video`` function of ``physicsengine.py`` now effectively launches the video (no call to plt.show required).
+- The ``video`` function of ``physicsengine.py`` using ``debug=True`` was crashing.
 
 ## [0.3.0-beta] - 2021-07-21
-### Added
- - Multiprocessing is here! The genetic optimization can now be run in parallel!
-   Performances got improved by 65 % using 4 processes only.
-
-### Changed
- - We now save data using JSON! Slow computer users, you can relax and stop 
-   computing when you want.
- - The sidebar in the documentation a bit more useful.
- - Not having tqdm will cause an exception.
 
-### Fixed
- - Corrected the example, the genetic optimization is now properly fixed but
+### Added in 0.3.0
+
+- Multiprocessing is here! The genetic optimization can now be run in parallel!
+  Performances got improved by 65 % using 4 processes only.
+
+### Changed in 0.3.0
+
+- We now save data using JSON! Slow computer users, you can relax and stop
+  computing when you want.
+- The sidebar in the documentation is a bit more useful.
+- Not having tqdm will cause an exception.
+
+### Fixed in 0.3.0
+
+- Corrected the example, the genetic optimization is now properly fixed but
 slower.
 
-### Removed
- - native support for PyGAD is no longer present.
- - ``evolutionnary_optimization`` (replaced by ``evolutionary_optimization``).
- - Data saved in the old txt format are no longer readable (were they?)
+### Removed in 0.3.0
+
+- Native support for PyGAD is no longer present.
+- ``evolutionnary_optimization`` (replaced by ``evolutionary_optimization``).
+- Data saved in the old txt format are no longer readable (were they readable?)
 
 ## [0.2.0-alpha] - 2021-07-14
-### Added
- - Dependency to [tqdm](https://tqdm.github.io/) and matplotlib.
- - The ``evolutionary_optimization`` replaces ``evolutionnary_optimization``.
-   - The ``ite`` parameter renamed ``iters`` for consistency with pylinkage.
-   - The new parameter ``verbose`` let you display a nice progress bar, more 
-     information on optimization state, or nothing.
- - The best solution can be displayed with PyGAD as well.
-
-### Changed
- - Typos and cleans-up in ``docs/examples/strider.py``.
- - ``evolutionnary_optimization_legacy`` renamed to 
-   ``evolutionary_optimization_builtin``.
-   
-### Deprecated
- - ``evolutionnary_optimization`` is now deprecated. Please use 
-   ``evolutionary_optimization``.
-
-### Removed
- - Explicit dependency to PyGAD. There is no longer an annoying message when 
-   PyGAD is not installed.
+
+### Added in 0.2.0
+
+- Dependency to [tqdm](https://tqdm.github.io/) and matplotlib.
+- The ``evolutionary_optimization`` replaces ``evolutionnary_optimization``.
+  - The ``ite`` parameter renamed ``iters`` for consistency with pylinkage.
+  - The new parameter ``verbose`` let you display a nice progress bar, more
+    information on optimization state, or nothing.
+- The best solution can be displayed with PyGAD as well.
+
+### Changed in 0.2.0
+
+- Typos and cleans-up in ``docs/examples/strider.py``.
+- ``evolutionnary_optimization_legacy`` renamed to
+  ``evolutionary_optimization_builtin``.
+
+### Deprecated in 0.2.0
+
+- ``evolutionnary_optimization`` is now deprecated. Please use
+  ``evolutionary_optimization``.
+
+### Removed in 0.2.0
+
+- Explicit dependency to PyGAD. There is no longer an annoying message when
+  PyGAD is not installed.
 
 ## [0.1.4-alpha] - 2021-07-12
-### Added
- - It is now possible and advised to import class and functions using quick 
-   paths, for instance ``from leggedsnake import Walker`` instead of 
-   ``from leggedsnake.walker import Walker``.
- - You do no longer have to manually import 
-   [pylinkage](https://hugofara.github.io/pylinkage/), we silently import the 
-   useful stuff for you.
- - We now use [bump2version](https://pypi.org/project/bump2version/) for version
-   maintenance.
- - This is fixed by the ``road_y`` parameter in ``World`` let you define a 
-   custom height for the base ground.
-
-### Changed
- - ``docs/examples/strider.py`` has been updated to the latest version of 
-   leggedsnake 0.1.4.
-   
-### Fixed
- - The full swarm representation in polar graph has been repaired in 
-   ``docs/examples/strider.py``.
- - During a dynamic simulation, linkages with long legs could appear through the
-   road.
- - The documentation was not properly rendered because Napoleon (NumPy coding 
-   style) was not integrated.
+
+### Added in 0.1.4
+
+- It is now possible and advised to import class and functions using quick
+  paths, for instance ``from leggedsnake import Walker`` instead of
+  ``from leggedsnake.walker import Walker``.
+- You do no longer have to manually import
+  [pylinkage](https://hugofara.github.io/pylinkage/), we silently import the
+  useful stuff for you.
+- We now use [bump2version](https://pypi.org/project/bump2version/) for version
+  maintenance.
+- This is fixed by the ``road_y`` parameter in ``World`` let you define a
+  custom height for the base ground.
+
+### Changed in 0.1.4
+
+- ``docs/examples/strider.py`` has been updated to the latest version of
+  leggedsnake 0.1.4.
+
+### Fixed in 0.1.4
+
+- The full swarm representation in polar graph has been repaired in
+  ``docs/examples/strider.py``.
+- During a dynamic simulation, linkages with long legs could appear through the
+  road.
+- The documentation was not properly rendered because Napoleon (NumPy coding
+  style) was not integrated.
 
 ## [0.1.3-alpha] - 2021-07-10
+
 This package was lacking real documentation, it is fixed in this version.
-### Added
- - Sphinx documentation!
- - Website hosted on GitHub pages, check 
-   [hugofara.github.io/leggedsnake](https://hugofara.github.io/leggedsnake/)!
- - Expanded README with the quick links section.
-
-### Changed
- - Tests moved from ``leggedsnake/tests`` to ``tests/``.
- - Examples moved from ``leggedsnake/examples/`` to ``docs/examples/``.
- - I was testing my code on ``leggedsnake/examples/strider.py``  (old path) and
-   that's why it was a big mess. I cleaned up that all. Sorry for the 
-   inconvenience!
-
-### Fixed
- - A lot of outdated code in the ``leggedsnake/examples/strider.py``
- - Changelog URL was broken in ``setup.cfg``.
+
+### Added in 0.1.3
+
+- Sphinx documentation!
+- Website hosted on GitHub pages, check
+  [hugofara.github.io/leggedsnake](https://hugofara.github.io/leggedsnake/)!
+- Expanded README with the quick links section.
+
+### Changed in 0.1.3
+
+- Tests moved from ``leggedsnake/tests`` to ``tests/``.
+- Examples moved from ``leggedsnake/examples/`` to ``docs/examples/``.
+- I was testing my code on ``leggedsnake/examples/strider.py``  (the old path) and
+  that's why it was a big mess. I cleaned up that all. Sorry for the
+  inconvenience!
+
+### Fixed in 0.1.3
+
+- A lot of outdated code in the ``leggedsnake/examples/strider.py``
+- Changelog URL was broken in ``setup.cfg``.
 
 ## [0.1.2-alpha] - 2021-07-07
-### Changed
- - The ``step`` function execution speed has been increased by 25% when 
-   ``return_res`` is ``True``! Small performance improvement when ``return_res``
-   is ``False``.
- - The ``size`` argument of ``step`` function is now known as ``witdh``.
- - We now require pylinkage>=0.4.0.
-
-### Fixed
- - Files in ``leggedsnake/examples/`` were not included in the PyPi package.
- - The example was incompatible with pylinkage 0.4.0.
- - Test suite was unusable by tox.
- - Tests fixed.
- - Incompatible argument between PyGAD init_pop and built-in GA.
 
-### Security
- - Tests with ``tox.ini`` now include Python 3.9 and Flake 8.
+### Added in 0.1.2
+
+- Security: tests with ``tox.ini`` now include Python 3.9 and Flake 8.
+
+### Changed in 0.1.2
+
+- The ``step`` function execution speed has been increased by 25% when
+  ``return_res`` is ``True``! Small performance improvement when ``return_res``
+  is ``False``.
+- The ``size`` argument of ``step`` function is now known as ``witdh``.
+- We now require pylinkage>=0.4.0.
+
+### Fixed in 0.1.2
+
+- Files in ``leggedsnake/examples/`` were not included in the PyPi package.
+- The example was incompatible with pylinkage 0.4.0.
+- Test suite was unusable by tox.
+- Tests fixed.
+- Incompatible argument between PyGAD init_pop and built-in GA.
 
 ## [0.1.1-alpha] - 2021-06-26
-### Added
- - The example file ``examples/strider.py`` is now shipped with the Python 
-   package.
- - ``leggedsnake/geneticoptimizer.py`` can now automatically switch to the 
-   built-in GA algorithm if PyGAD is not installed.
 
-### Changed
- - ``setup.cfg`` metadata
+### Added in 0.1.1
+
+- The example file ``examples/strider.py`` is now shipped with the Python
+  package.
+- ``leggedsnake/geneticoptimizer.py`` can now automatically switch to the
+  built-in GA algorithm if PyGAD is not installed.
+
+### Changed in 0.1.1
+
+- ``setup.cfg`` metadata
 
 ## [0.1.0-alpha] - 2021-06-25
-### Added
- - Code vulnerabilities automatic checks
- - Example videos in ``examples/images/``
-
-### Changed
- - Manny reforms in code style, to make the dynamic part naming conventions 
-   consistent with Pymunk. 
- - Images in the ``README.md``!
-
-### Fixed
- - You can now define linkages with an enormous number of legs. Systems with
-   many should no longer break physics but your CPU instead :)
+
+### Added in 0.1.0
+
+- Code vulnerabilities automatic checks
+- Example videos in ``examples/images/``
+
+### Changed in 0.1.0
+
+- Many reforms in code style in order to make the dynamic part of naming conventions
+  consistent with Pymunk.
+- Images in the ``README.md``!
+
+### Fixed in 0.1.0
+
+- You can now define linkages with an enormous number of legs. Systems with
+  many should no longer break physics but your CPU instead :)
 
 ## [0.0.3-alpha] - 2021-06-23
-### Added
- - Started walktrough demo in ``README.md``
- - Automatic release to PyPi
-
-### Fixed
- - Pymunk version should be at least 6.0.0 in requirement files.
- - Some URLs typos in ``README.md``
- - Versioning tests not executing (GitHub action)
+
+### Added in 0.0.3
+
+- Started walkthrough demo in ``README.md``
+- Automatic release to PyPi
+
+### Fixed in 0.0.3
+
+- Pymunk version should be at least 6.0.0 in requirement files.
+- Some URLs typos in ``README.md``
+- Versioning tests not executing (GitHub action)
 
 ## [0.0.2-alpha] - 2021-06-22
-### Added
+
+### Added in 0.0.2
+
 - ``requirement.txt`` was absent due to ``.gitignore`` misconfiguration.
 
-### Changed
- - ``.gitignore`` now ignores .txt files only in the leggedsnake folder.
- - ``environment.yml`` more flexible (versions can be superior to the selected). 
-   pymunk>5.0.0 and pylinkage added.
- - ``leggedsnake/utility.py`` not having zipfile or xml modules error 
-   encapsulation.
-
-### Fixed
- - ``setup.cfg`` was not PyPi compatible. Removed mail (use GitHub!), we now 
-   explicitly say that ``README.md`` is markdown (PyPi is conservative)
-   
+### Changed in 0.0.2
+
+- ``.gitignore`` now ignores .txt files only in the leggedsnake folder.
+- ``environment.yml`` more flexible (versions can be superior to the selected).
+  pymunk>5.0.0 and pylinkage added.
+- ``leggedsnake/utility.py`` not having zipfile or xml modules error
+  encapsulation.
+
+### Fixed in 0.0.2
+
+- ``setup.cfg`` was not PyPi compatible. Removed mail (use GitHub!), we now
+  explicitly say that ``README.md`` is markdown (PyPi is conservative)
+
 ## [0.0.1-alpha] - 2021-06-22
-Basic version, supporting Genetic Algorithm optimization, but with various 
+
+Basic version, supporting Genetic Algorithm optimization, but with various
 problems.
-### Added
- - ``CODE_OF_CONDUCT.md`` to help community.
- - ``LICENSE`` MIT License.
- - ``MANIFEST.in`` to include more files.
- - ``README.md`` as a very minimal version.
- - ``environment.yml`` with matplotlib, numpy, and pygad requirement.
- - ``examples/strider.py`` a complete demo with Strider linkage.
- - ``leggedsnake/__init__.py``.
- - ``leggedsnake/dynamiclinkage.py``.
- - ``leggedsnake/geneticoptimizer.py``.
- - ``leggedsnake/physicsengine.py``.
- - ``leggedsnake/show_evolution.py`` just a legacy package, no utility.
- - ``leggedsnake/tests/test_utility.py`` untested test case
- - ``leggedsnake/utility.py`` contain some useful evaluation function (``step``
-   and ``stride``) and a broken GeoGebra interface.
- - ``walker.py`` defines the ``Walker`` object.
- - ``pyproject.toml``. 
- - ``setup.cfg``.
- - ``setup.py`` empty, for compatibility purposes only.
- - ``tox.ini`` tox with Python 3.7 and 3.8
 
+### Added in 0.0.1
+
+- ``CODE_OF_CONDUCT.md`` to help community.
+- ``LICENSE`` MIT License.
+- ``MANIFEST.in`` to include more files.
+- ``README.md`` as a very minimal version.
+- ``environment.yml`` with matplotlib, numpy, and pygad requirement.
+- ``examples/strider.py`` a complete demo with Strider linkage.
+- ``leggedsnake/__init__.py``.
+- ``leggedsnake/dynamiclinkage.py``.
+- ``leggedsnake/geneticoptimizer.py``.
+- ``leggedsnake/physicsengine.py``.
+- ``leggedsnake/show_evolution.py`` just a legacy package, no utility.
+- ``leggedsnake/tests/test_utility.py`` untested test case
+- ``leggedsnake/utility.py`` contain some useful evaluation function (``step``
+  and ``stride``) and a broken GeoGebra interface.
+- ``walker.py`` defines the ``Walker`` object.
+- ``pyproject.toml``.
+- ``setup.cfg``.
+- ``setup.py`` empty, for compatibility purposes only.
+- ``tox.ini`` tox with Python 3.7 and 3.8.
```

### Comparing `leggedsnake-0.3.0/README.md` & `leggedsnake-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,132 +1,219 @@
+# leggedsnake
+
 [![PyPI version fury.io](https://badge.fury.io/py/leggedsnake.svg)](https://pypi.python.org/pypi/leggedsnake/)
-[![Downloads](https://static.pepy.tech/personalized-badge/leggedsnake?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads/week)](https://pepy.tech/project/leggedsnake)
+[![Downloads](https://static.pepy.tech/personalized-badge/leggedsnake?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/leggedsnake)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg )](https://raw.githubusercontent.com/HugoFara/leggedsnake/master/LICENSE.rst)
-# leggedsnake
-LeggedSnake is a project intended to make the simulation of walking linkages fast and easy. We believe that building walking linkages is fun and could be useful. Our philosophy is to provide a quick way of building, optimizing and testing walking linkages.
+
+LeggedSnake is a project intended to make the simulation of walking linkages fast and easy. 
+We believe that building walking linkages is fun and could be useful.
+Our philosophy is to provide a quick way of building, optimizing and testing walking linkages.
 
 We handle planar [leg mechanisms](https://en.wikipedia.org/wiki/Leg_mechanism) in three main parts:
+
 * Linkage conception in simple Python relying on [pylinkage](https://github.com/HugoFara/pylinkage).
 * Kinematic optimization with ``Walker`` class, inheriting from pylinkage's ``Linkage`` class.
 * Dynamic simulation and its optimization using genetic algorithms.
 
 ## Quick links
+
 * For the documentation, check the docs at [hugofara.github.io/leggedsnake](https://hugofara.github.io/leggedsnake/)!
 * Source code is hosted on GitHub as [HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake)
 * We also provide a Python package on PyPi, test [leggedsnake](https://pypi.org/project/leggedsnake/).
 * If you just want to chill out looking at walking linkages striving to survive, join the [discussions](https://github.com/HugoFara/leggedsnake/discussions).
 
 Contributors are welcome!
 
 ## Installation
+
 ### Using pip
+
 The package is hosted on PyPi as [leggedsnake](https://pypi.org/project/leggedsnake/), use:
-``pip install leggedsnake``
+
+```bash
+pip install leggedsnake
+```
 
 ### Setting up Virtual Environment
-We provide an [environment.yml](https://github.com/HugoFara/leggedsnake/blob/master/environment.yml) file for conda. Use ``conda env update --file environment.yml --name leggedsnake-env`` to install the requirements in a separate environment. 
 
-If you are looking for a development version, check the GitHub repo under [HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake). 
+We provide an [environment.yml](https://github.com/HugoFara/leggedsnake/blob/master/environment.yml) file for conda. 
+Use ``conda env update --file environment.yml --name leggedsnake-env`` to install the requirements in a separate environment.
 
-## Requirements
+If you are looking for a development version, check the GitHub repo under 
+[HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake).
+
+
+## Contribute
+
+Download the latest GitHub version, then install the dev requirements in ``requirements-dev.txt``.
+
+In a nutshell
+
+```bash
+git clone https://github.com/HugoFara/leggedsnake.git
+cd leggedsnake
+pip install -r requirements-dev.txt
+```
+
+### Testing
 
-Python 3, numpy for calculation, matplotlib for drawing, and standard libraries. 
+We use unittest. Just run ``python3 -m unittest discover .`` from the main folder.
 
-For kinematic optimization you can either use the built-in algorithm, or [PySwarms](https://pyswarms.readthedocs.io/en/latest/), under MIT license. PySwarms is a much more complexe package which provides quick calculations, however with modern laptops the built-in swarm optimization should be quick enough to fit your needs.
+### Release
 
-Dynamic optimization relies on multiple packages. First of all it uses [Pymunk](http://www.pymunk.org/en/latest/index.html), made by Victor Blomqvist, as a physics engine. Then you can either use the built-in algorithm, or the GA module from [PyGAD](https://pygad.readthedocs.io/en/latest/). PyGAD is a complete library providing much more than genetic algorithms, so it might be heavy. PyGAD is more complete than the built-in however, so I haven't decided to continue on PyGAD or switch for another solution in the future.
+This section is mainly intended for maintainers. 
+Fell free to use the tools described here, but they are not necessary in any way.
+
+* To publish a new version, use ``bump2version``. For instance ``bump2version minor``.
+* Regenerate the documentation with ``make html`` (uses Sphinx).
 
 ## Usage
 
-The demo script is [strider.py](https://github.com/HugoFara/leggedsnake/blob/master/docs/examples/strider.py), which demonstrates all the techniques about the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html).
+The demo script is [strider.py](https://github.com/HugoFara/leggedsnake/blob/master/docs/examples/strider.py), which
+demonstrates all the techniques about the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html).
 
 ### Defining a ``Walker``
-First, you need to define joints for your ``Walker`` as described in [pylinkage](https://github.com/HugoFara/pylinkage) documentation. Once your joints (let's say they are in a joint object), you should have something like that:
-```python
+
+First, you need to define joints for your ``Walker`` as described in [pylinkage](https://github.com/HugoFara/pylinkage)
+documentation. Once your joints (let's say they are in a joint object), you should have something like that:
+
+```python3
 import leggedsnake as ls
 
 # Center of the Walker
-A = ls.Static(x=0, y=0, name="A")
-B = ls.Crank(1, 0, distance=1, angle=0.31, name="Crank")
-# etc... let's say with have joints up to E
+linkage = {
+    "A": ls.Static(x=0, y=0, name="A"),
+    "B": ls.Crank(1, 0, distance=1, angle=0.31, name="Crank")
+    # etc...
+}
 my_walker = ls.Walker(
-  joints=(A, B, C, D, E),
-  name="My Walker"
+    joints=linkage.values(),
+    name="My Walker"
 )
 ```
 
-``Walker`` is just a herited class of ``Linkage``, with some useful methods, and behaves quite the same way.
+``Walker`` is just an inherited class of ``Linkage``, with some useful methods, and behaves quite the same way.
 
 ### Kinematic optimization using Particle Swarm Optimization (PSO)
-No change compared to a classic linkage optimization. You should use the ``step`` and ``stride`` method from the [utility module](https://github.com/HugoFara/leggedsnake/blob/master/leggedsnake/utility.py) as fitness functions. 
+
+No change compared to a classic linkage optimization. You should use the ``step`` and ``stride`` method from the 
+[utility module](https://github.com/HugoFara/leggedsnake/blob/master/leggedsnake/utility.py) as fitness functions.
 This set of rules should work well for a stride **maximisation** problem:
+
 1. Rebuild the Walker with the provided set of dimensions, and do a complete turn.
-1. If the Walker raise an UnbuildableError, its score is 0 (or ``- float('inf')`` if you use other evaluation functions.
-1. Verify if it can pass a certain obstacke using ``step`` function. If not, its score is 0.
-1. Eventually mesure the length of its stide with the ``stride`` function. Return this length as its score.
+2. If the Walker raises an UnbuildableError, its score is 0 (or ``-float('inf')`` if you use other evaluation functions).
+3. Verify if it can pass a certain obstacle using ``step`` function. If not, its score is 0.
+4. Eventually measure the length of its stride with the ``stride`` function. Return this length as its score.
 
 ### Dynamic Optimization using Genetic Algorithm (GA)
-Kinematic optimization is fast, however it can return weird results, and it has no sense of gravity while walking heavily relies on gravity. This is why you may need to use dynamic optimization thanks to [Pymunk](http://www.pymunk.org/en/latest/index.html). However the calculation is much more slower, and you can no longer tests millions of linkages as in PSO (or you will need time). This is why we use [genetic algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm), because it can provide good results with less parents.
 
-We handle everything almost evything world definition to linkage conversion. Appart from the GA parameters, you just have to define a fitness function. Here are the main steps for a **maximisation problem**:
-1. Create a function of two arguments, the first one should be the paramaters of the linkage, the second the initial positions for the joints.
-1. Try to do a revolution in **kinematic simulation**. If the Walker raises an ``UnbuildableError`` set its score to ``-float('inf')``.
-1. Otherwise use this procedure 
+Kinematic optimization is fast, but it can return weird results, and it has no sense of gravity while walking heavily
+relies on gravity. This is why you may need to use dynamic optimization thanks to
+[Pymunk](http://www.pymunk.org/en/latest/index.html). However, the calculation is much slower, and you can no
+longer test millions of linkages as in PSO (or you will need time). This is why we
+use [genetic algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm), because it can provide good results with
+fewer parents.
+
+We handle everything almost everything world definition to linkage conversion. Apart from the GA parameters, you just
+have to define a fitness function. Here are the main steps for a **maximisation problem**:
+
+1. Create a function of two arguments, the first one should be the parameters of the linkage, the second the initial positions for the joints.
+2. Try to do a revolution in **kinematic simulation**. If the Walker raises an ``UnbuildableError`` set its score to ``-float('inf')``.
+3. Otherwise, use the following procedure:
+
+```python3
+import leggedsnake as ls
 
-```python
 def dynamic_linkage_fitness(walker):
-  """
-  Make the dynamic evalutaion of a Walker.
-  
-  Return yield and initial position of joints.
-  """
-  world = pe.World()
-  # We handle all the conversions
-  world.add_linkage(walker)
-  # Simulation duration (in seconds)
-  duration = 40
-  # Somme of yields
-  tot = 0
-  # Motor turned on duration
-  dur = 0
-  n = duration * pe.params["camera"]["fps"]
-  n /= pe.params["simul"]["time_coef"]
-  for j in range(int(n)):
-      efficiency, energy = world.update(j)
-      tot += efficiency
-      dur += energy
-  if dur == 0:
-      return - float('inf'), list()
-  print("Score:", tot / dur)
-  # Return 100 times average yield, and initial positions as the final score
-  return tot / dur, pos
+    """
+    Make the dynamic evaluation of a Walker.
+    
+    Return yield and initial position of joints.
+    """
+    world = ls.World()
+    # We handle all the conversions
+    world.add_linkage(walker)
+    # Simulation duration (in seconds)
+    duration = 40
+    # Somme of yields
+    tot = 0
+    # Motor turned on duration
+    dur = 0
+    n = duration * ls.params["camera"]["fps"]
+    n /= ls.params["simul"]["time_coef"]
+    pos = tuple(walker.step())[-1]
+    for j in range(int(n)):
+        efficiency, energy = world.update(j)
+        tot += efficiency
+        dur += energy
+    if dur == 0:
+        return - float('inf'), list()
+    print("Score:", tot / dur)
+    # Return 100 times average yield, and initial positions as the final score
+    return tot / dur, pos
 ```
 
-And now, relax while your computer recreates a civilisation of walking machines!
+And now, relax while your computer creates a civilization of walking machines!
 
 ### Visualization
-For this part we will focus on the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html), an exemple file is provided at ``docs/examples/strider.py``. The linkage looks like this:
+
+For this part we will focus on the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html), 
+an example file is provided at ``docs/examples/strider.py``.
+
+The linkage looks like this:
 ![A Kinematic representation of Strider linkage](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Kinematic%20unoptimized%20Strider.gif)
 
 Looks cool? Let's simulate it dynamically!
 
 ![Dynamic one-leg-pair Strider being tested](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Dynamic%20unoptimized%20one-legged%20Strider.gif)
 
-Oops! Here is what you get when you forget to add more legs! There is **real danger here**, because your walker crawls well, you will be able to optimize efficiently the "crawler", *which may be not your goal*. 
+Oops! Here is what you get when you forget to add more legs! There is **real danger here**, because your walker crawls
+well, you will be able to optimize efficiently the "crawler", *which may be not your goal*.
 
-Let's add three more leg pairs. Why three? Many legs means more mass and constraints, so less yield and more intensive computations. On the other hand, we always want the center of mass over the [support line](https://en.wikipedia.org/wiki/Support_polygon), which means that if the walker begins to lift a foot (let's say a front foot), and another doesn't come on the ground ahead of it, the linkage will to fall nose to the ground. With more foots we make the "snooping" time shorter, and a total of four leg pairs is a minimum for this *unoptimized* version. 
+Let's add three more leg pairs. Why three? Many legs mean more mass and constraints, so less yield and more intensive
+computations. On the other hand, we always want the center of mass over the
+[support line](https://en.wikipedia.org/wiki/Support_polygon), which means that if the walker begins to lift a foot
+(let's say a front foot), and another doesn't come on the ground ahead of it, the linkage will fall nose to the
+ground. With more feet, we make the "snooping" time shorter, and a total of four leg pairs is a minimum for this
+*unoptimized* version.
 
 A simple way to do it is:
+
 ```python
 my_linkage.add_legs(3) # Replace "my_linkage" with your Walker object
 ```
+
 Let's have a look at the artist:
 
 ![Dynamic four-leg-pair unoptimized Strider](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Dynamic%20unoptimized%20strider.gif)
 
 ## Advice
-Use the vizualisation tools provided! The optimization tools should always give you a score with a better fitness, but it might not be what you expected. Tailor your optimization and *then* go for a long run will make you save a lot of time.
 
-**Do not** use optimized linkages from the start! The risk is to fall to quickly into a suboptimal solution. They are several mechanisms to prevent that (starting from random position), however it can always have an impact on the rest of the optimization.
+Use the visualisation tools provided! The optimization tools should always give you a score with a better fitness,
+but it might not be what you expected. Tailor your optimization and *then* go for a long run will make you save a lot
+of time.
+
+**Do not** use optimized linkages from the start! The risk is to fall to quickly into a suboptimal solution. They are
+several mechanisms to prevent that (starting from random position), but it can always have an impact on the rest of
+the optimization.
+
+Try to minimize the number of elements in the optimizations! You can often use some linkage properties to reduce the
+number of simulation parameters. For instance, the Strider linkage has axial symmetry. While it is irrelevant to use
+this property in dynamic simulation, you can use "half" your Strider in a kinematic optimization, which is much faster.
 
-Try to minimize the number of elements in the optimizations! You can often use some linkage's properties to reduce the number of simulation parameters. For instance, the Strider linkage has an axial symmetry. While it is irrelevant to use this property in dynamic simulation, you can use "half" your Strider in a kinematic optimization, which is much faster:
 ![A Kinematic half Strider](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Kinematic%20half-Strider.gif)
+
+## Requirements
+
+Python 3, numpy for calculation, matplotlib for drawing, and standard libraries.
+
+For kinematic optimization, you can either use the built-in algorithm, or
+[PySwarms](https://pyswarms.readthedocs.io/en/latest/), under MIT license. 
+PySwarms is a much more complex package which provides quick calculations, 
+however, with modern laptops the built-in swarm optimization should be quick enough
+to fit your needs.
+
+Dynamic optimization relies on multiple packages.
+First of all, it uses [Pymunk](http://www.pymunk.org/en/latest/index.html),
+made by Victor Blomqvist, as its physics engine. 
+The genetic algorithm optimizer is home-made, 
+but feel free to use any external tool suiting your needs!
```

### Comparing `leggedsnake-0.3.0/docs/changeloglink.html` & `leggedsnake-0.3.1/docs/changeloglink.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.0/docs/genindex.html` & `leggedsnake-0.3.1/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.0/docs/index.html` & `leggedsnake-0.3.1/docs/index.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.0/docs/objects.inv` & `leggedsnake-0.3.1/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.0/docs/py-modindex.html` & `leggedsnake-0.3.1/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.0/docs/readmelink.html` & `leggedsnake-0.3.1/docs/readmelink.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.0/docs/search.html` & `leggedsnake-0.3.1/docs/search.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.0/docs/searchindex.js` & `leggedsnake-0.3.1/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.0/leggedsnake/__init__.py` & `leggedsnake-0.3.1/leggedsnake/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Main module of leggedsnake library, to build walking machines easily.
+Main module of the leggedsnake library, to build walking machines easily.
 
-Please see https://hugofara.github.io/leggedsnake/ for a complete documentation.
-A local copy should have been shipped with this package under the docs folder.
+Please see https://hugofara.github.io/leggedsnake/ for complete documentation.
+A local copy should have been shipped with this package under the docs/ folder.
 
 Created on Thu Jun 10 20:35:00 2021
 
 @author: HugoFara
 """
 
 # Pylinkage is a sister project and some kind of backend for leggedsnake
@@ -32,8 +32,8 @@
 )
 from .physicsengine import (
     video, video_debug,
     params,
     World, VisualWorld
 )
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `leggedsnake-0.3.0/leggedsnake/dynamiclinkage.py` & `leggedsnake-0.3.1/leggedsnake/dynamiclinkage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 The dynamiclinkage module is an interface between Pymunk and a kinematic linkage.
 
-It provide various classes to overwrite the pylinkage.Joint objects.
-It also includes a DynamicLinkage that inheritates from
+It provides various classes to overwrite the pylinkage.Joint objects.
+It also includes a DynamicLinkage that inherits from
 pylinkage.linkage.Linkage.
-Enventually a handy convert_to_dynamic_linkage methoc can generate a
+Eventually a handy convert_to_dynamic_linkage method can generate a
 DynamicLinkage from a pylinkage.linkage.Linkage.
 """
 import abc
 from math import atan2
 import pymunk as pm
 from pylinkage import linkage
 from pylinkage.geometry import dist, cyl_to_cart
@@ -29,23 +29,23 @@
         Parameters
         ----------
         body0 : pymunk.body.Body, optional
             First Body to link to. The default is None.
         body1 : pymunk.body.Body, optional
             Second Body to link to. The default is None
         space : pymunk.space.Space, optional
-            Simulation space in which the DynamicJoint exist.
+            Simulation space in which the DynamicJoint exists.
             The default is None.
         radius : float, optional
-            DynamicJoint will generate hulles of this radius. The default is .3.
+            DynamicJoint will generate hulls of this radius. The default is .3.
         density : float, optional
             Density of the hull, mass will be computed accordingly.
             The default is 1.
         shape_filter : pymunk.shapes.ShapeFilter, optional
-            Prevent hulles from colliding with each another. Useful is the same
+            Prevent hulls from colliding with each other. Useful is the same
             linkage for instance. The default is None.
         """
         if isinstance(body0, pm.Body):
             self._a = body0
             self._anchor_a = body0.world_to_local(self.coord())
         if isinstance(body1, pm.Body):
             self._b = body1
@@ -57,23 +57,23 @@
         # All the Joint/constraint that are on the same bar
         self.superposed = set()
 
     def __generate_link__(self, body, parent_pos):
         """
         Create a pymunk.Segment between two joints on a body and return it.
 
-        First extremity of the segment is self Joint position, the other is
+        The first extremity of the segment is self Joint position, the other is
         parent_pos (a position).
 
         Parameters
         ----------
         body : pymunk.Body
             The Body you want the link to be added to.
         parent_pos : sequence
-            Any sequence of two float. It give th
+            Any sequence of two floats. It give th
 
         Returns
         -------
         seg : pymunk.Segment
             The segment joining the two joints of the body.
 
         """
@@ -89,17 +89,17 @@
         """
         Create a pymunk.Body and assign it to the specified interface.
 
         Parameters
         ----------
         index : int, optional
             The interface index to assign the body to.
-            0 : assign to self.a
-            1 : assign to selb.b
-            2 : assign to self.a and self.b
+            0: assign to self.a
+            1: assign to self.b
+            2: assign to self.a and self.b
             The default is 0.
 
         Returns
         -------
         None.
 
         """
@@ -146,15 +146,15 @@
                        ' {} and {}, parents of {}: {}.')
             raise Exception(message.format(joints[0], joints[1], self, inter))
 
     def reload(self):
         """
         Reload DynamicJoint coordinates.
 
-        Coordinates only depend of Body position and DO NOT use any linkage
+        Coordinates only depend on Body position and DO NOT use any linkage
         constraint.
 
         Returns
         -------
         None.
 
         """
@@ -235,38 +235,38 @@
         if self.joint0 is not None:
             self.set_anchor_a(self.joint0, self.r, self.angle)
         if self.joint1 is not None:
             self.set_anchor_b(self.joint1)
 
     def set_anchor_a(self, joint, distance=None, angle=None):
         """
-        Set first anchor charactertics.
+        Set first anchor characteristics.
 
         Parameters
         ----------
         joint : DynamicJoint
-            DynamicJoint to use as achor_a.
+            DynamicJoint to use as anchor_a.
         distance : float, optional
             Distance to keep constant. The default is None.
         angle : float, optional
             Angle (in radians)  (joint1, joint0, self). The default is None.
 
         Returns
         -------
         None.
 
         """
         linkage.Fixed.set_anchor0(self, joint, distance, angle)
 
     def set_anchor_b(self, joint):
         """
-        Set second anchor caracteristics.
+        Set second anchor characteristics.
 
         It will create errors if called before anchor_a is properly defined.
-        SIDE EFFECT : it create two Segment and add them to self.space.
+        SIDE EFFECT: creates two Segment objects and adds them to self.space.
 
         Parameters
         ----------
         joint : DynamicJoint
             Joint to use as anchor_b.
 
         Returns
@@ -283,15 +283,15 @@
         self._anchor_b = self._b.world_to_local(self.coord())
         self.space.add(self.__generate_link__(self._a, joint.coord()))
 
     def reload(self):
         """
         Reload DynamicJoint coordinates.
 
-        Coordinates only depend of Body position and DO NOT use any linkage
+        Coordinates only depend on Body position and DO NOT use any linkage
         constraint.
 
         Returns
         -------
         None.
 
         """
@@ -317,15 +317,15 @@
         if self.joint0 is not None:
             self.set_anchor_a(self.joint0, self.r0)
         if self.joint1 is not None:
             self.set_anchor_b(self.joint1, self.r1)
 
     def set_anchor_a(self, joint, distance=None):
         """
-        Set anchor_a caracteristics.
+        Set anchor_a characteristics.
 
         Parameters
         ----------
         joint : DynamicJoint
             DynamicJoint to use as anchor_a.
         distance : float, optional
             Distance to keep constant between anchor_a and self.
@@ -348,15 +348,15 @@
                 joint.coord())
             pivot.collide_bodies = False
             joint.superposed.add(pivot)
             self.space.add(pivot)
 
     def set_anchor_b(self, joint, distance=None):
         """
-        Set anchor_b caracteristics.
+        Set anchor_b characteristics.
 
         Parameters
         ----------
         joint : DynamicJoint
             DynamicJoint to use as anchor_b.
         distance : float, optional
             Distance to keep constant between anchor_b and self.
@@ -380,30 +380,30 @@
             joint.superposed.add(pivot_b)
             self.space.add(self.pivot, pivot_b)
 
     def reload(self):
         """
         Reload DynamicJoint coordinates.
 
-        Coordinates only depend of Body position and DO NOT use any linkage
+        Coordinates only depend on Body position and DO NOT use any linkage
         constraint.
 
         Returns
         -------
         None.
 
         """
         DynamicJoint.reload(self)
 
 
 class Motor(linkage.Crank, DynamicJoint):
     """
     A Motor is a crank.
 
-    It makes a link between a body and a sencond link it creates. It attaches
+    It makes a link between a body and a second link it creates. It attaches
     them with a PivotJoint, and adds a SimpleMotor over it. The bodies are now
     constrained to rotate around one each other.
 
     The Motor is placed at the extremity of the body it creates.
     """
 
     def __init__(self, x=None, y=None, joint0=None, space=None,
@@ -415,15 +415,15 @@
         DynamicJoint.__init__(self, space=space, density=density,
                               shape_filter=shape_filter, radius=radius)
         if joint0 is not None:
             self.set_anchor_a(joint0, distance=distance)
 
     def __get_reference_body__(self, body=None):
         """
-        Find a body that can be used as reference body.
+        Find a body that can be used as a reference body.
 
         Parameters
         ----------
         body : pymunk.Body, optional
             Body to use as reference Body.
             If set to None, use self.joint0_a.
             The default is None.
@@ -433,15 +433,15 @@
         ValueError
             Raised when body argument is not None and not in self.joint0
             bodies.
 
         Returns
         -------
         pymunk.Body
-            A valid Body to be used as reference.
+            A valid Body to be used as a reference.
 
         """
         if body is None:
             return self.joint0._a
         if body in (self.joint0._a, self.joint0._b):
             return body
         message = 'Argument body should in {} bodies'
@@ -455,15 +455,15 @@
             seg = self.__generate_link__(body, self.joint0.coord())
             self._a = self._b = body
             self._anchor_b = body.world_to_local(self.coord())
             self.space.add(body, seg)
 
     def set_anchor_a(self, joint, distance=None):
         """
-        Set anchor_a caracteristics.
+        Set anchor_a characteristics.
 
         Parameters
         ----------
         joint : DynamicJoint
             DynamicJoint to use as anchor_a.
         distance : float, optional
             Distance to keep constant between anchor_a and self.
@@ -485,33 +485,33 @@
             self.joint0.superposed.add(self.actuator)
             self.space.add(self.pivot, self.actuator)
 
     def reload(self):
         """
         Reload DynamicJoint coordinates.
 
-        Coordinates only depend of Body position and DO NOT use any linkage
+        Coordinates only depend on Body position and DO NOT use any linkage
         constraint.
 
         Returns
         -------
         None.
 
         """
         DynamicJoint.reload(self)
 
 
 class DynamicLinkage(linkage.Linkage):
     """
-    Dynamic couterpart of a kinematic linkage.Linkage.
+    Dynamic counterpart of a kinematic linkage.Linkage.
 
     It has several attributes linked to its dynamic nature and is close to an
     empty shell in the ways you will use it.
 
-    Please not that it carries a load, which is relevant with real-world
+    Please note that it carries a load, which is relevant with real-world
     simulation where the weight of legs is small compared to the weight of the
     frame.
     """
 
     __slots__ = ['joint_to_rigidbodies', 'rigidbodies', 'body', 'height',
                  'mechanical_energy', 'mass', 'space', 'density',
                  '_thickness', 'filter']
@@ -521,15 +521,15 @@
         """
         Instanciate a new DynamicLinkage.
 
         Parameters
         ----------
         joints : linkage.Joint
             Joints to be part of the linkage. Kinematic joints will be
-            converted in there dynamic equivalents.
+            converted to their dynamic equivalents.
         space : pymunk.Space
             Space in which linkage should be instantiated.
         density : float, optional
             Density of the Bodies in the linkage. The default is 1.
         load : float, optional
             Mass of the load to carry. The default is 0.
         name : TYPE, optional
@@ -631,15 +631,15 @@
         vertices = (-.5, -.5), (-.5, .5), (.5, .5), (.5, -.5)
         segs = []
         for i, vertex in enumerate(vertices):
             segs.append(pm.Segment(load, vertex,
                                    vertices[(i + 1) % len(vertices)],
                                    self._thickness))
             segs[-1].density = self.density
-            # Rigodbodies in this group won't collide
+            # Rigidbodies in this group won't collide
             segs[-1].filter = self.filter
         self.space.add(load, *segs)
         return load
 
 
 def convert_to_dynamic_linkage(kinematic_linkage, space, density=1,
                                load=1):
```

### Comparing `leggedsnake-0.3.0/leggedsnake/geneticoptimizer.py` & `leggedsnake-0.3.1/leggedsnake/geneticoptimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 The geneticoptimizer module provides optimizers and wrappers for GA.
 
-As for now I didn't tried a convincing Genetic Algorithm library. This is why
-you it is built-in here. Feel free to propose a copyleft library on GitHub!
+As for now, I didn't try a convincing Genetic Algorithm library. This is why
+it is built-in here. Feel free to propose a copyleft library on GitHub!
 
 Created on Thu Jun 10 21:20:47 2021.
 
 @author: HugoFara
 """
 import os.path
 import json
 import multiprocessing as mp
 import numpy as np
-from numpy.random import rand, normal, randint
+import numpy.random as nprand
 # Progress bar
 import tqdm
 from pylinkage.geometry import dist
 
 
 def tqdm_verbosity(iterable, verbose=True, *args, **kwargs):
     """Wrapper for tqdm, that let you specify if you want verbosity."""
@@ -49,35 +49,37 @@
 def save_population(file_path, population, verbose=False, data_descriptors=None):
     """
     Save the population to a json file.
 
     Parameters
     ----------
     file_path : str
-    population : list of dna
+        Path of the file to write to.
+    population : list
+        Sequence of dna
     verbose : bool
+        Enable or not verbosity (outputs success).
     data_descriptors : dict
         Any additional value you want to save for the current generation.
     """
     if not os.path.exists(file_path):
-        data = [{'turn': 0, 'population': population}]
-        with open(file_path, 'x') as file:
-            json.dump(data, file)
+        data = []
+        turn = 0
     else:
         with open(file_path, 'r') as file:
             data = json.load(file)
         turn = data[-1]['turn'] + 1
-        data.append({
-            'turn': turn,
-            'population': population
-        })
-        if data_descriptors is not None:
-            data[-1].update(data_descriptors)
-        with open(file_path, 'w') as file:
-            json.dump(data, file)
+    data.append({
+        'turn': turn,
+        'population': population
+    })
+    if data_descriptors is not None:
+        data[-1].update(data_descriptors)
+    with open(file_path, 'w') as file:
+        json.dump(data, file)
     if verbose:
         print('Data saved.')
 
 
 def birth(par1, par2, prob):
     """
     Return a new individual with par1 and par2 as parents (two sequences).
@@ -100,17 +102,17 @@
     -------
     child : list[float, tuple of float, tuple of tuple of float]
         Dna of the child.
 
     """
     child = [0, [], []]
     for gene1, gene2 in zip(par1[1], par2[1]):
-        child[1].append(normal((gene1 if rand() < .5 else gene2), prob))
+        child[1].append(nprand.normal((gene1 if nprand.rand() < .5 else gene2), prob))
     for pos1, pos2 in zip(par1[2], par2[2]):
-        child[2].append(pos1 if rand() < .5 else pos2)
+        child[2].append(pos1 if nprand.rand() < .5 else pos2)
     return child
 
 
 def evaluate_individual(dna, fitness, fitness_args):
     """Simple evaluation for a single individual.
 
     Parameters
@@ -152,31 +154,31 @@
         List of the individuals' DNAs
     fitness : callable
         Fitness function of signature fitness(dna, fitness_args) → float.
     fitness_args : tuple
         Additional arguments to pass to the fitness function. Usually the
         initial positions of the joints.
     verbose : bool, default=True
-        To display informations about population evaluation.
+        To display information about population evaluation.
     processes : int, default=1
-        Number of processes involved for a multiprocessors evaluation.
+        Number of processes involved for a multiprocessor evaluation.
 
     See Also
     --------
     evaluate_individual : same function but on a single DNA.
     """
-    # For multiprocessing we load the processes
+    # For multiprocessing, we load the processes
     if processes > 1:
-        res = [None] * len(pop)
         with mp.Pool(processes=processes) as pool:
             # Load the processes
-            for i, dna in enumerate(pop):
-                res[i] = pool.apply_async(
+            res = [
+                pool.apply_async(
                     evaluate_individual, (dna, fitness, fitness_args)
-                )
+                ) for dna in pop
+            ]
             # Then get data
             for result, dna in zip(res, pop):
                 dna[0], dna[2] = result.get()
     else:
         for dna in pop:
             dna[0], dna[2] = evaluate_individual(dna, fitness, fitness_args)
 
@@ -187,28 +189,28 @@
         print("Scores:", [dna[1] for dna in pop])
         print("Genetic diversity: ", diversity)
 
 
 def select_parents(pop, verbose=True):
     """Selection 1/4 of the population as parents."""
     median = np.median([dna[0] for dna in pop])
-    # Index of best individual
+    # Index of the best individual
     best_index, best_dna = max(enumerate(pop), key=lambda x: x[1][0])
     # Parents selection, 1/4 of population
     parents = []
     indexes = []
     for j, individual in enumerate(pop):
         # Parents whose score is above median.
-        # Individuals with best fitness are more likely to be selected
+        # Individuals with the best fitness are more likely to be selected
         if (
                 .5 * (individual[0] - best_dna[0]) / (best_dna[0] - median)
-        ) + 1 > max(rand(), .5):
+        ) + 1 > max(nprand.rand(), .5):
             parents.append(individual)
             indexes.append(j)
-    # Add best individual if needed
+    # Add the best individual if needed
     if best_index not in indexes:
         parents.insert(0, best_dna)
         indexes.append(best_index)
     # Add a random parent if odd number
     if len(parents) % 2:
         for j, individual in enumerate(pop):
             if j not in indexes:
@@ -220,17 +222,17 @@
     return parents
 
 
 def make_children(parents, prob, max_genetic_dist=float('inf')):
     children = []
     j = 0
     while len(parents) > 1 and j < 100:
-        par1 = parents.pop(randint(len(parents) - 1))
+        par1 = parents.pop(nprand.randint(len(parents) - 1))
         if len(parents) > 1:
-            par2 = parents.pop(randint(len(parents) - 1))
+            par2 = parents.pop(nprand.randint(len(parents) - 1))
         else:
             par2 = parents.pop()
         if dist(par1[1], par2[1]) < max_genetic_dist:
             children.append(birth(par1, par2, prob))
         elif parents:
             parents.append(par1)
             parents.append(par2)
@@ -262,15 +264,15 @@
     iters : int
         Number of iterations.
     **kwargs : dict
         Other useful parameters for the optimization.
 
         max_pop : int, default=11
             Maximum number of individuals. The default is 11.
-        init_pop : sequence of object, default=None
+        init_pop : sequence of objects, default=None
             Initial population, for wider INITIAL genetic diversity.
             The default is None.
         max_genetic_dist : float, default=.7
             Maximum genetic distance, before individuals
             cannot reproduce (separated species). The default is .7.
         startnstop : bool, default=False
             Ability to close program without loosing population.
@@ -305,22 +307,22 @@
 
     max_pop = kwargs_switcher('max_pop', kwargs, 11)
     max_genetic_dist = kwargs_switcher('max_genetic_dist', kwargs, .7)
     verbose = kwargs_switcher('verbose', kwargs, 1)
     fitness_args = kwargs_switcher('fitness_args', kwargs, None)
     # Number of evaluations to run in parallel
     processes = kwargs_switcher('processes', kwargs, default=1)
-    # "Garden of Eden" phase, add enough children to get as much individuals as
+    # "Garden of Eden" phase, add enough children to get as many individuals as
     # required
     init_pop = kwargs_switcher('init_pop', kwargs, default=max_pop)
-    for i in range(len(pop), init_pop):
+    for _ in range(len(pop), init_pop):
         pop.append(
             birth(
-                pop[randint(len(pop) - 1)],
-                pop[randint(len(pop) - 1)],
+                pop[nprand.randint(len(pop) - 1)],
+                pop[nprand.randint(len(pop) - 1)],
                 prob
             )
         )
     postfix = [
         "best_score", max(x[0] for x in pop),
         "best_dimensions", max(pop, key=lambda x: x[0])[1]
     ]
@@ -363,15 +365,15 @@
         # Children generation
         children = make_children(parents, prob, max_genetic_dist)
         # Add to population
         pop.extend(children)
 
     out = []
     for dna in pop:
-        fit = fitness(dna)
+        fit = evaluate_individual(dna, fitness, fitness_args)
         if isinstance(fit, tuple):
             out.append((fit[0], fit[1], dna[2]))
         else:
             out.append((fit, dna[1], dna[2]))
     out.sort(key=lambda x: x[0], reverse=True)
     return out
 
@@ -395,24 +397,24 @@
     Parameters
     ----------
     dna : list[float, tuple of float, tuple of tuple of float]
         DNA of a linkage in format (score, dimensions, initial coordinates).
     prob : float or list of float, default=.07
         Mutation probability for each gene.
     fitness : callable
-        Evaluation function for an MAXIMISATION problem.
+        Evaluation function for a MAXIMISATION problem.
         Must return a float.
     iters : int
         Number of iterations.
     **kwargs : dict
         Other useful parameters for the optimization.
 
         max_pop : int, optional
             Maximum number of individuals. The default is 11.
-        init_pop : sequence of object, optional
+        init_pop : sequence of objects, optional
             Initial population, for wider INITIAL genetic diversity.
             The default is None.
         max_genetic_dist : float, optional
             Maximum genetic distance, before individuals
             cannot reproduce (separated species). The default is .7.
         startnstop : bool, optional
             Ability to close program without loosing population.
```

### Comparing `leggedsnake-0.3.0/leggedsnake/physicsengine.py` & `leggedsnake-0.3.1/leggedsnake/physicsengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 The physicsengine module gives a dynamic behavior to legged mechanism.
 
-Is uses the 2D physics engine chipmunk, this is why it can only be used on
+It uses the 2D physics engine chipmunk, this is why it can only be used on
 planar mechanisms.
-In theory you can use any type of mechanism, and not only planar mechanisms.
-In practice we do generate the road and some other parameters as the gravity,
+In theory, you can use any type of mechanism, and not only planar mechanisms.
+In practice, we do generate the road and some other parameters as the gravity,
 so it can be difficult to test something other than a walker.
 
-Created on Sat May 25 14:56:01 2019.
+Created on Sat May 25 2019 14:56:01.
 
 @author: HugoFara
 """
 import numpy as np
 import pymunk as pm
 import pymunk.matplotlib_util
 import matplotlib.pyplot as plt
@@ -28,15 +28,15 @@
     "ground": {
         # Nominal slope (radian)
         "slope": 10 * np.pi / 180,
         # Maximal step height
         "max_step": .5,
         # Steps frequency
         "step_freq": .1,
-        # Terrain variations, should not be above 1
+        # Terrain variations should not be above 1
         "noise": .9,
         # Road trunks length
         "section_len": 1,
         # Ground friction coefficient root
         "friction": .5 ** .5
     },
     # Studied system parameters
@@ -63,15 +63,15 @@
         # Number of calculations for each frame
         "calc_rate": 300,
         # Maximal number of subcalculations
         "max_sub": 50,
     },
     # Display parameters
     "camera": {
-        # Do you want to follow system of view whole scene?
+        # Do you want to follow a system of view whole scene?
         "dynamic_camera": True,
         # Required frames per second
         "fps": 20,
     },
 }
 
 
@@ -86,15 +86,15 @@
             constraint.max_force = params["physics"]["max_force"] * (np.exp(
                 - len_c / 25) / 2 + .5)
         constraint.error_bias = (1 - .1 * np.exp(-len_c / 60)) ** 60
 
 
 class World:
     """
-    A world contain a space of simulation, at least one linkage, and a road.
+    A world contains a space of simulation, at least one linkage, and a road.
 
     It is not intended to be rendered visually per se, see VisualWorld for
     this purpose.
     """
 
     def __init__(self, space=None, road_y=-5):
         """
@@ -103,15 +103,15 @@
         Add rigidbodies in linkage.
 
         Parameters
         ----------
         space : pymunk.space.Space, optional
             Space of simulation. The default is None.
         road_y : float, optional
-            The ordinate of the ground. Useful when likages have long legs.
+            The ordinate of the ground. Useful when linkages have long legs.
             The default is -5.
         """
         if isinstance(space, pm.Space):
             self.space = space
         else:
             self.space = pm.Space()
             self.space.gravity = params["physics"]["gravity"]
@@ -139,19 +139,19 @@
         self.linkages.append(dynamiclinkage)
         for s in self.space.shapes:
             s.friction = params["ground"]["friction"]
         set_space_constraints(self.space)
 
     def __update_linkage__(self, linkage, power):
         """Update a specific linkage."""
-        crank = next(j for j in linkage.joints if isinstance(j, Crank))
+        linkage_crank = next(j for j in linkage.joints if isinstance(j, Crank))
         if (
-                crank.actuator.max_force == 0
+                linkage_crank.actuator.max_force == 0
                 and norm(linkage.body.velocity) < .1):
-            crank.actuator.max_force = params["linkage"]["torque"]
+            linkage_crank.actuator.max_force = params["linkage"]["torque"]
             linkage.height = linkage.body.position.y
             linkage.mechanical_energy = (.5 * linkage.mass
                                          * norm(linkage.body.velocity) ** 2)
 
         # Energy from the motor in this step
         energy = power * params["simul"]["time_coef"] / params["camera"]["fps"]
         if hasattr(linkage, 'height') and energy != 0.:
@@ -354,15 +354,15 @@
         # Return modified objects for animation optimisation
         return (
             [self.draw_linkage(linkage.joints) for linkage in self.linkages]
             + self.road_im)
 
 
 def recalc_linkage(linkage):
-    """Assign the good position to all joints."""
+    """Assign a good position to all joints."""
     for j in linkage.joints:
         j.reload()
 
 
 def linkage_bb(linkage):
     """
     Return the bounding box for this linkage.
@@ -385,17 +385,17 @@
     bbox = linkage_bb(linkage)
     world.ax.clear()
     world.ax.set_xlim(int(bbox[3]) - 5, int(bbox[1]) + 5)
     world.ax.set_ylim(int(bbox[2]) - 5, int(bbox[0]) + 5)
     world.ax.scatter([i.x for i in linkage.joints],
                      [i.y for i in linkage.joints], c='r')
     for j in linkage.joints:
-        for shape in j.a.shapes:
-            begin = j.a.local_to_world(shape.a)
-            end = j.a.local_to_world(shape.b)
+        for shape in j._a.shapes:
+            begin = j._a.local_to_world(shape.a)
+            end = j._a.local_to_world(shape.b)
             world.ax.plot([begin[0], end[0]], [begin[1], end[1]])
     options = pymunk.matplotlib_util.DrawOptions(world.ax)
     options.constraint_color = (.1, .1, .1, .0)
     world.space.debug_draw(options)
 
 
 def video_debug(linkage):
@@ -413,17 +413,14 @@
         for i in range(params["simul"]["calc_rate"]):
             world.space.step(dt)
         recalc_linkage(dynamiclinkage)
         im_debug(world, dynamiclinkage)
         plt.pause(.2)
 
 
-ani = []
-
-
 def video(linkage, duration=30, save=False):
     """
     Give the rigidbody a dynamic model and launch simulation with video.
 
     Parameters
     ----------
     linkage : Union[pylinkage.linkage.Linkage,
@@ -440,26 +437,26 @@
     else:
         world = VisualWorld(road_y=road_y)
     world.add_linkage(linkage)
     # Number of frames for the selected duration
     n = int(params["camera"]["fps"] * duration
             / params["simul"]["time_coef"])
 
-    ani.append(
-        anim.FuncAnimation(
-            world.fig, world.update, frames=range(1, n),
-            interval=int(1000 / params["camera"]["fps"]),
-            repeat=False, blit=False
-        )
+    animation = anim.FuncAnimation(
+        world.fig, world.update, frames=range(1, n),
+        interval=int(1000 / params["camera"]["fps"]),
+        repeat=False, blit=False
     )
     if save:
         writer = anim.FFMpegWriter(fps=params["camera"]["fps"], bitrate=2500)
-        ani[-1].save(f"Dynamic {linkage.name}.mp4", writer=writer)
+        animation.save(f"Dynamic {linkage.name}.mp4", writer=writer)
     else:
-        world.fig.show()
+        plt.show()
+        if animation:
+            pass
 
 
 if __name__ == "__main__":
     base = Static(0, 0, name="Main trick")
     crank = Crank(1, 0, name="The crank", angle=1, joint0=base)
     follower = Pivot(0, 2, joint0=base, joint1=crank, distance0=2,
                      distance1=1)
```

### Comparing `leggedsnake-0.3.0/leggedsnake/utility.py` & `leggedsnake-0.3.1/leggedsnake/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 Also known as WalkerUtility.
 
-This module aims to standardize and simplify study of walking mechanisms.
+This module aims to standardize and simplify the study of walking mechanisms.
 
-It contain useful functions that make study of planar mechanisms easy.
+It contains useful functions that make study of planar mechanisms easy.
 
-Created on Sat Nov 17 20:35:39 2018.
+Created on Sat Nov 17 2018 20:35:39.
 
 @author: HugoFara
 """
 from pylinkage.geometry import bounding_box
 
 try:
     # Used to read GeoGebra file
@@ -113,15 +113,15 @@
     bb = bounding_box(points)
     # Quick sort for unfit systems
     if bb[2] - bb[0] < height or bb[1] - bb[3] < width:
         return False
     # Origin of ordinates, for computing obstacle's height
     if y_min is None:
         y_min = bb[0]
-    # Index of first point passing obstacle
+    # Index of a first point passing obstacle
     for i, point in enumerate(points):
         if point[1] - y_min >= height:
             break
     x = point[0]
     ok = False
     # Index of the first point passing the obstacle, or the last one that have
     # the good height
```

### Comparing `leggedsnake-0.3.0/leggedsnake/walker.py` & `leggedsnake-0.3.1/leggedsnake/walker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-The walker module give a simple interface between a generic linkage and a Walker.
+The walker module gives a simple interface between a generic linkage and a Walker.
 
 A generic linkage should be understood as a pylinkage.linkage.Linkage. Thus a
 Walker is a kinematic mechanism (not dynamic).
 
-Created on Thu Jun 10 21:13:12 2021.
+Created on Thu Jun 10 2021 21:13:12.
 
 @author: HugoFara
 """
 from math import tau
 import pylinkage.linkage as lk
 
 
 class Walker(lk.Linkage):
-    """A Walker, or a leg mechanism, is a Linkage with some useful methods."""
+    """A Walker, or a leg mechanism is a Linkage with some useful methods."""
 
     def add_legs(self, number=2):
         """
         Add legs to a linkage, mostly for a dynamic simulation.
 
-        The leg is a subset a joints whose position inheritates from a crank.
+        The leg is a subset a joints whose position inherits from a crank.
 
         Parameters
         ----------
         number : int, optional
             Number of legs to add. The default is 2.
 
         Returns
@@ -38,16 +38,16 @@
         # We use at least 12 steps to avoid bad initial positions
         new_positions = tuple(
             self.step(
                 (number + 1) * iterations_factor,
                 self.get_rotation_period() / (number + 1) / iterations_factor
             )
         )[iterations_factor - 1:-1:iterations_factor]
-        # Because we have per-leg iterations
-        # we have to save crank informations
+        # Because we have per-leg iterations,
+        # we have to save crank information
         crank_memory = dict(zip(self._cranks, self._cranks))
         # For each leg
         for i, positions in enumerate(new_positions):
             equiv = {None: None}
             # For each new joint
             for pos, j in zip(positions, self._solve_order):
                 if isinstance(j.joint0, lk.Static) and j.joint0 not in equiv:
@@ -86,21 +86,21 @@
         self.joints += tuple(new_joints)
         self._solve_order += tuple(new_joints)
 
     def get_foots(self):
         """
         Return the list of foot joints, joints that should be used as foots.
 
-        Formally, they are joints without children, there position does not
+        Formally, they are joints without children; their positions do not
         influence other joints.
 
         Returns
         -------
         candidates : list
-            List of terminal joints, foots.
+            List of terminal joints, feet.
 
         """
         candidates = list(self.joints)
         for j in self.joints:
             if j.joint0 in candidates:
                 candidates.remove(j.joint0)
             if hasattr(j, 'joint1') and j.joint1 in candidates:
```

### Comparing `leggedsnake-0.3.0/leggedsnake.egg-info/PKG-INFO` & `leggedsnake-0.3.1/leggedsnake.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: leggedsnake
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simulate and optimize planar leg mechanisms using PSO and GA
 Home-page: https://hugofara.github.io/leggedsnake/
 Author: Hugo Farajallah
 License: MIT License
 Project-URL: Changelog, https://hugofara.github.io/leggedsnake/changeloglink.html
 Project-URL: Source, https://github.com/HugoFara/leggedsnake
 Keywords: linkage,leg mechanism,optimization,leggedsnake,walking linkage
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Life
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,325 +19,475 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# leggedsnake
+
 [![PyPI version fury.io](https://badge.fury.io/py/leggedsnake.svg)](https://pypi.python.org/pypi/leggedsnake/)
-[![Downloads](https://static.pepy.tech/personalized-badge/leggedsnake?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads/week)](https://pepy.tech/project/leggedsnake)
+[![Downloads](https://static.pepy.tech/personalized-badge/leggedsnake?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/leggedsnake)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg )](https://raw.githubusercontent.com/HugoFara/leggedsnake/master/LICENSE.rst)
-# leggedsnake
-LeggedSnake is a project intended to make the simulation of walking linkages fast and easy. We believe that building walking linkages is fun and could be useful. Our philosophy is to provide a quick way of building, optimizing and testing walking linkages.
+
+LeggedSnake is a project intended to make the simulation of walking linkages fast and easy. 
+We believe that building walking linkages is fun and could be useful.
+Our philosophy is to provide a quick way of building, optimizing and testing walking linkages.
 
 We handle planar [leg mechanisms](https://en.wikipedia.org/wiki/Leg_mechanism) in three main parts:
+
 * Linkage conception in simple Python relying on [pylinkage](https://github.com/HugoFara/pylinkage).
 * Kinematic optimization with ``Walker`` class, inheriting from pylinkage's ``Linkage`` class.
 * Dynamic simulation and its optimization using genetic algorithms.
 
 ## Quick links
+
 * For the documentation, check the docs at [hugofara.github.io/leggedsnake](https://hugofara.github.io/leggedsnake/)!
 * Source code is hosted on GitHub as [HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake)
 * We also provide a Python package on PyPi, test [leggedsnake](https://pypi.org/project/leggedsnake/).
 * If you just want to chill out looking at walking linkages striving to survive, join the [discussions](https://github.com/HugoFara/leggedsnake/discussions).
 
 Contributors are welcome!
 
 ## Installation
+
 ### Using pip
+
 The package is hosted on PyPi as [leggedsnake](https://pypi.org/project/leggedsnake/), use:
-``pip install leggedsnake``
+
+```bash
+pip install leggedsnake
+```
 
 ### Setting up Virtual Environment
-We provide an [environment.yml](https://github.com/HugoFara/leggedsnake/blob/master/environment.yml) file for conda. Use ``conda env update --file environment.yml --name leggedsnake-env`` to install the requirements in a separate environment. 
 
-If you are looking for a development version, check the GitHub repo under [HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake). 
+We provide an [environment.yml](https://github.com/HugoFara/leggedsnake/blob/master/environment.yml) file for conda. 
+Use ``conda env update --file environment.yml --name leggedsnake-env`` to install the requirements in a separate environment.
+
+If you are looking for a development version, check the GitHub repo under 
+[HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake).
 
-## Requirements
 
-Python 3, numpy for calculation, matplotlib for drawing, and standard libraries. 
+## Contribute
 
-For kinematic optimization you can either use the built-in algorithm, or [PySwarms](https://pyswarms.readthedocs.io/en/latest/), under MIT license. PySwarms is a much more complexe package which provides quick calculations, however with modern laptops the built-in swarm optimization should be quick enough to fit your needs.
+Download the latest GitHub version, then install the dev requirements in ``requirements-dev.txt``.
 
-Dynamic optimization relies on multiple packages. First of all it uses [Pymunk](http://www.pymunk.org/en/latest/index.html), made by Victor Blomqvist, as a physics engine. Then you can either use the built-in algorithm, or the GA module from [PyGAD](https://pygad.readthedocs.io/en/latest/). PyGAD is a complete library providing much more than genetic algorithms, so it might be heavy. PyGAD is more complete than the built-in however, so I haven't decided to continue on PyGAD or switch for another solution in the future.
+In a nutshell
+
+```bash
+git clone https://github.com/HugoFara/leggedsnake.git
+cd leggedsnake
+pip install -r requirements-dev.txt
+```
+
+### Testing
+
+We use unittest. Just run ``python3 -m unittest discover .`` from the main folder.
+
+### Release
+
+This section is mainly intended for maintainers. 
+Fell free to use the tools described here, but they are not necessary in any way.
+
+* To publish a new version, use ``bump2version``. For instance ``bump2version minor``.
+* Regenerate the documentation with ``make html`` (uses Sphinx).
 
 ## Usage
 
-The demo script is [strider.py](https://github.com/HugoFara/leggedsnake/blob/master/docs/examples/strider.py), which demonstrates all the techniques about the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html).
+The demo script is [strider.py](https://github.com/HugoFara/leggedsnake/blob/master/docs/examples/strider.py), which
+demonstrates all the techniques about the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html).
 
 ### Defining a ``Walker``
-First, you need to define joints for your ``Walker`` as described in [pylinkage](https://github.com/HugoFara/pylinkage) documentation. Once your joints (let's say they are in a joint object), you should have something like that:
-```python
+
+First, you need to define joints for your ``Walker`` as described in [pylinkage](https://github.com/HugoFara/pylinkage)
+documentation. Once your joints (let's say they are in a joint object), you should have something like that:
+
+```python3
 import leggedsnake as ls
 
 # Center of the Walker
-A = ls.Static(x=0, y=0, name="A")
-B = ls.Crank(1, 0, distance=1, angle=0.31, name="Crank")
-# etc... let's say with have joints up to E
+linkage = {
+    "A": ls.Static(x=0, y=0, name="A"),
+    "B": ls.Crank(1, 0, distance=1, angle=0.31, name="Crank")
+    # etc...
+}
 my_walker = ls.Walker(
-  joints=(A, B, C, D, E),
-  name="My Walker"
+    joints=linkage.values(),
+    name="My Walker"
 )
 ```
 
-``Walker`` is just a herited class of ``Linkage``, with some useful methods, and behaves quite the same way.
+``Walker`` is just an inherited class of ``Linkage``, with some useful methods, and behaves quite the same way.
 
 ### Kinematic optimization using Particle Swarm Optimization (PSO)
-No change compared to a classic linkage optimization. You should use the ``step`` and ``stride`` method from the [utility module](https://github.com/HugoFara/leggedsnake/blob/master/leggedsnake/utility.py) as fitness functions. 
+
+No change compared to a classic linkage optimization. You should use the ``step`` and ``stride`` method from the 
+[utility module](https://github.com/HugoFara/leggedsnake/blob/master/leggedsnake/utility.py) as fitness functions.
 This set of rules should work well for a stride **maximisation** problem:
+
 1. Rebuild the Walker with the provided set of dimensions, and do a complete turn.
-1. If the Walker raise an UnbuildableError, its score is 0 (or ``- float('inf')`` if you use other evaluation functions.
-1. Verify if it can pass a certain obstacke using ``step`` function. If not, its score is 0.
-1. Eventually mesure the length of its stide with the ``stride`` function. Return this length as its score.
+2. If the Walker raises an UnbuildableError, its score is 0 (or ``-float('inf')`` if you use other evaluation functions).
+3. Verify if it can pass a certain obstacle using ``step`` function. If not, its score is 0.
+4. Eventually measure the length of its stride with the ``stride`` function. Return this length as its score.
 
 ### Dynamic Optimization using Genetic Algorithm (GA)
-Kinematic optimization is fast, however it can return weird results, and it has no sense of gravity while walking heavily relies on gravity. This is why you may need to use dynamic optimization thanks to [Pymunk](http://www.pymunk.org/en/latest/index.html). However the calculation is much more slower, and you can no longer tests millions of linkages as in PSO (or you will need time). This is why we use [genetic algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm), because it can provide good results with less parents.
 
-We handle everything almost evything world definition to linkage conversion. Appart from the GA parameters, you just have to define a fitness function. Here are the main steps for a **maximisation problem**:
-1. Create a function of two arguments, the first one should be the paramaters of the linkage, the second the initial positions for the joints.
-1. Try to do a revolution in **kinematic simulation**. If the Walker raises an ``UnbuildableError`` set its score to ``-float('inf')``.
-1. Otherwise use this procedure 
+Kinematic optimization is fast, but it can return weird results, and it has no sense of gravity while walking heavily
+relies on gravity. This is why you may need to use dynamic optimization thanks to
+[Pymunk](http://www.pymunk.org/en/latest/index.html). However, the calculation is much slower, and you can no
+longer test millions of linkages as in PSO (or you will need time). This is why we
+use [genetic algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm), because it can provide good results with
+fewer parents.
+
+We handle everything almost everything world definition to linkage conversion. Apart from the GA parameters, you just
+have to define a fitness function. Here are the main steps for a **maximisation problem**:
+
+1. Create a function of two arguments, the first one should be the parameters of the linkage, the second the initial positions for the joints.
+2. Try to do a revolution in **kinematic simulation**. If the Walker raises an ``UnbuildableError`` set its score to ``-float('inf')``.
+3. Otherwise, use the following procedure:
+
+```python3
+import leggedsnake as ls
 
-```python
 def dynamic_linkage_fitness(walker):
-  """
-  Make the dynamic evalutaion of a Walker.
-  
-  Return yield and initial position of joints.
-  """
-  world = pe.World()
-  # We handle all the conversions
-  world.add_linkage(walker)
-  # Simulation duration (in seconds)
-  duration = 40
-  # Somme of yields
-  tot = 0
-  # Motor turned on duration
-  dur = 0
-  n = duration * pe.params["camera"]["fps"]
-  n /= pe.params["simul"]["time_coef"]
-  for j in range(int(n)):
-      efficiency, energy = world.update(j)
-      tot += efficiency
-      dur += energy
-  if dur == 0:
-      return - float('inf'), list()
-  print("Score:", tot / dur)
-  # Return 100 times average yield, and initial positions as the final score
-  return tot / dur, pos
+    """
+    Make the dynamic evaluation of a Walker.
+    
+    Return yield and initial position of joints.
+    """
+    world = ls.World()
+    # We handle all the conversions
+    world.add_linkage(walker)
+    # Simulation duration (in seconds)
+    duration = 40
+    # Somme of yields
+    tot = 0
+    # Motor turned on duration
+    dur = 0
+    n = duration * ls.params["camera"]["fps"]
+    n /= ls.params["simul"]["time_coef"]
+    pos = tuple(walker.step())[-1]
+    for j in range(int(n)):
+        efficiency, energy = world.update(j)
+        tot += efficiency
+        dur += energy
+    if dur == 0:
+        return - float('inf'), list()
+    print("Score:", tot / dur)
+    # Return 100 times average yield, and initial positions as the final score
+    return tot / dur, pos
 ```
 
-And now, relax while your computer recreates a civilisation of walking machines!
+And now, relax while your computer creates a civilization of walking machines!
 
 ### Visualization
-For this part we will focus on the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html), an exemple file is provided at ``docs/examples/strider.py``. The linkage looks like this:
+
+For this part we will focus on the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html), 
+an example file is provided at ``docs/examples/strider.py``.
+
+The linkage looks like this:
 ![A Kinematic representation of Strider linkage](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Kinematic%20unoptimized%20Strider.gif)
 
 Looks cool? Let's simulate it dynamically!
 
 ![Dynamic one-leg-pair Strider being tested](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Dynamic%20unoptimized%20one-legged%20Strider.gif)
 
-Oops! Here is what you get when you forget to add more legs! There is **real danger here**, because your walker crawls well, you will be able to optimize efficiently the "crawler", *which may be not your goal*. 
+Oops! Here is what you get when you forget to add more legs! There is **real danger here**, because your walker crawls
+well, you will be able to optimize efficiently the "crawler", *which may be not your goal*.
 
-Let's add three more leg pairs. Why three? Many legs means more mass and constraints, so less yield and more intensive computations. On the other hand, we always want the center of mass over the [support line](https://en.wikipedia.org/wiki/Support_polygon), which means that if the walker begins to lift a foot (let's say a front foot), and another doesn't come on the ground ahead of it, the linkage will to fall nose to the ground. With more foots we make the "snooping" time shorter, and a total of four leg pairs is a minimum for this *unoptimized* version. 
+Let's add three more leg pairs. Why three? Many legs mean more mass and constraints, so less yield and more intensive
+computations. On the other hand, we always want the center of mass over the
+[support line](https://en.wikipedia.org/wiki/Support_polygon), which means that if the walker begins to lift a foot
+(let's say a front foot), and another doesn't come on the ground ahead of it, the linkage will fall nose to the
+ground. With more feet, we make the "snooping" time shorter, and a total of four leg pairs is a minimum for this
+*unoptimized* version.
 
 A simple way to do it is:
+
 ```python
 my_linkage.add_legs(3) # Replace "my_linkage" with your Walker object
 ```
+
 Let's have a look at the artist:
 
 ![Dynamic four-leg-pair unoptimized Strider](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Dynamic%20unoptimized%20strider.gif)
 
 ## Advice
-Use the vizualisation tools provided! The optimization tools should always give you a score with a better fitness, but it might not be what you expected. Tailor your optimization and *then* go for a long run will make you save a lot of time.
 
-**Do not** use optimized linkages from the start! The risk is to fall to quickly into a suboptimal solution. They are several mechanisms to prevent that (starting from random position), however it can always have an impact on the rest of the optimization.
+Use the visualisation tools provided! The optimization tools should always give you a score with a better fitness,
+but it might not be what you expected. Tailor your optimization and *then* go for a long run will make you save a lot
+of time.
+
+**Do not** use optimized linkages from the start! The risk is to fall to quickly into a suboptimal solution. They are
+several mechanisms to prevent that (starting from random position), but it can always have an impact on the rest of
+the optimization.
+
+Try to minimize the number of elements in the optimizations! You can often use some linkage properties to reduce the
+number of simulation parameters. For instance, the Strider linkage has axial symmetry. While it is irrelevant to use
+this property in dynamic simulation, you can use "half" your Strider in a kinematic optimization, which is much faster.
 
-Try to minimize the number of elements in the optimizations! You can often use some linkage's properties to reduce the number of simulation parameters. For instance, the Strider linkage has an axial symmetry. While it is irrelevant to use this property in dynamic simulation, you can use "half" your Strider in a kinematic optimization, which is much faster:
 ![A Kinematic half Strider](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Kinematic%20half-Strider.gif)
 
+## Requirements
+
+Python 3, numpy for calculation, matplotlib for drawing, and standard libraries.
+
+For kinematic optimization, you can either use the built-in algorithm, or
+[PySwarms](https://pyswarms.readthedocs.io/en/latest/), under MIT license. 
+PySwarms is a much more complex package which provides quick calculations, 
+however, with modern laptops the built-in swarm optimization should be quick enough
+to fit your needs.
+
+Dynamic optimization relies on multiple packages.
+First of all, it uses [Pymunk](http://www.pymunk.org/en/latest/index.html),
+made by Victor Blomqvist, as its physics engine. 
+The genetic algorithm optimizer is home-made, 
+but feel free to use any external tool suiting your needs!
 # Changelog
+
 All notable changes to the LeggedSnake will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased]
+## [0.3.1] - 2023-06-14
+
+Starting from 0.3.1, we won't include "-alpha" or "-beta" in the naming scheme,
+as it is considered irrelevant.
+
+### Added in 0.3.1
+
+- ``requirements-dev.txt`` that contain dev requirements. It makes contribution easier.
+- PyCharm configuration files.
+
+### Changed in 0.3.1
+
+- Animations are now all stored in local variables, and no longer in an "ani"
+global list of animations.
+
+### Fixed in 0.3.1
+
+- The main example file ``strider.py`` was launching animations for each subprocess.
+This file is now considered an executable.
+- ``evolutionary_optimization_builtin`` was during the last evaluation of linkages.
+- ``data_descriptors`` were not save for the first line of data only in
+  ``geneticoptimizer``.
+- Multiple grammar corrections.
+- The ``video`` function of ``physicsengine.py`` now effectively launches the video (no call to plt.show required).
+- The ``video`` function of ``physicsengine.py`` using ``debug=True`` was crashing.
 
 ## [0.3.0-beta] - 2021-07-21
-### Added
- - Multiprocessing is here! The genetic optimization can now be run in parallel!
-   Performances got improved by 65 % using 4 processes only.
-
-### Changed
- - We now save data using JSON! Slow computer users, you can relax and stop 
-   computing when you want.
- - The sidebar in the documentation a bit more useful.
- - Not having tqdm will cause an exception.
 
-### Fixed
- - Corrected the example, the genetic optimization is now properly fixed but
+### Added in 0.3.0
+
+- Multiprocessing is here! The genetic optimization can now be run in parallel!
+  Performances got improved by 65 % using 4 processes only.
+
+### Changed in 0.3.0
+
+- We now save data using JSON! Slow computer users, you can relax and stop
+  computing when you want.
+- The sidebar in the documentation is a bit more useful.
+- Not having tqdm will cause an exception.
+
+### Fixed in 0.3.0
+
+- Corrected the example, the genetic optimization is now properly fixed but
 slower.
 
-### Removed
- - native support for PyGAD is no longer present.
- - ``evolutionnary_optimization`` (replaced by ``evolutionary_optimization``).
- - Data saved in the old txt format are no longer readable (were they?)
+### Removed in 0.3.0
+
+- Native support for PyGAD is no longer present.
+- ``evolutionnary_optimization`` (replaced by ``evolutionary_optimization``).
+- Data saved in the old txt format are no longer readable (were they readable?)
 
 ## [0.2.0-alpha] - 2021-07-14
-### Added
- - Dependency to [tqdm](https://tqdm.github.io/) and matplotlib.
- - The ``evolutionary_optimization`` replaces ``evolutionnary_optimization``.
-   - The ``ite`` parameter renamed ``iters`` for consistency with pylinkage.
-   - The new parameter ``verbose`` let you display a nice progress bar, more 
-     information on optimization state, or nothing.
- - The best solution can be displayed with PyGAD as well.
-
-### Changed
- - Typos and cleans-up in ``docs/examples/strider.py``.
- - ``evolutionnary_optimization_legacy`` renamed to 
-   ``evolutionary_optimization_builtin``.
-   
-### Deprecated
- - ``evolutionnary_optimization`` is now deprecated. Please use 
-   ``evolutionary_optimization``.
-
-### Removed
- - Explicit dependency to PyGAD. There is no longer an annoying message when 
-   PyGAD is not installed.
+
+### Added in 0.2.0
+
+- Dependency to [tqdm](https://tqdm.github.io/) and matplotlib.
+- The ``evolutionary_optimization`` replaces ``evolutionnary_optimization``.
+  - The ``ite`` parameter renamed ``iters`` for consistency with pylinkage.
+  - The new parameter ``verbose`` let you display a nice progress bar, more
+    information on optimization state, or nothing.
+- The best solution can be displayed with PyGAD as well.
+
+### Changed in 0.2.0
+
+- Typos and cleans-up in ``docs/examples/strider.py``.
+- ``evolutionnary_optimization_legacy`` renamed to
+  ``evolutionary_optimization_builtin``.
+
+### Deprecated in 0.2.0
+
+- ``evolutionnary_optimization`` is now deprecated. Please use
+  ``evolutionary_optimization``.
+
+### Removed in 0.2.0
+
+- Explicit dependency to PyGAD. There is no longer an annoying message when
+  PyGAD is not installed.
 
 ## [0.1.4-alpha] - 2021-07-12
-### Added
- - It is now possible and advised to import class and functions using quick 
-   paths, for instance ``from leggedsnake import Walker`` instead of 
-   ``from leggedsnake.walker import Walker``.
- - You do no longer have to manually import 
-   [pylinkage](https://hugofara.github.io/pylinkage/), we silently import the 
-   useful stuff for you.
- - We now use [bump2version](https://pypi.org/project/bump2version/) for version
-   maintenance.
- - This is fixed by the ``road_y`` parameter in ``World`` let you define a 
-   custom height for the base ground.
-
-### Changed
- - ``docs/examples/strider.py`` has been updated to the latest version of 
-   leggedsnake 0.1.4.
-   
-### Fixed
- - The full swarm representation in polar graph has been repaired in 
-   ``docs/examples/strider.py``.
- - During a dynamic simulation, linkages with long legs could appear through the
-   road.
- - The documentation was not properly rendered because Napoleon (NumPy coding 
-   style) was not integrated.
+
+### Added in 0.1.4
+
+- It is now possible and advised to import class and functions using quick
+  paths, for instance ``from leggedsnake import Walker`` instead of
+  ``from leggedsnake.walker import Walker``.
+- You do no longer have to manually import
+  [pylinkage](https://hugofara.github.io/pylinkage/), we silently import the
+  useful stuff for you.
+- We now use [bump2version](https://pypi.org/project/bump2version/) for version
+  maintenance.
+- This is fixed by the ``road_y`` parameter in ``World`` let you define a
+  custom height for the base ground.
+
+### Changed in 0.1.4
+
+- ``docs/examples/strider.py`` has been updated to the latest version of
+  leggedsnake 0.1.4.
+
+### Fixed in 0.1.4
+
+- The full swarm representation in polar graph has been repaired in
+  ``docs/examples/strider.py``.
+- During a dynamic simulation, linkages with long legs could appear through the
+  road.
+- The documentation was not properly rendered because Napoleon (NumPy coding
+  style) was not integrated.
 
 ## [0.1.3-alpha] - 2021-07-10
+
 This package was lacking real documentation, it is fixed in this version.
-### Added
- - Sphinx documentation!
- - Website hosted on GitHub pages, check 
-   [hugofara.github.io/leggedsnake](https://hugofara.github.io/leggedsnake/)!
- - Expanded README with the quick links section.
-
-### Changed
- - Tests moved from ``leggedsnake/tests`` to ``tests/``.
- - Examples moved from ``leggedsnake/examples/`` to ``docs/examples/``.
- - I was testing my code on ``leggedsnake/examples/strider.py``  (old path) and
-   that's why it was a big mess. I cleaned up that all. Sorry for the 
-   inconvenience!
-
-### Fixed
- - A lot of outdated code in the ``leggedsnake/examples/strider.py``
- - Changelog URL was broken in ``setup.cfg``.
+
+### Added in 0.1.3
+
+- Sphinx documentation!
+- Website hosted on GitHub pages, check
+  [hugofara.github.io/leggedsnake](https://hugofara.github.io/leggedsnake/)!
+- Expanded README with the quick links section.
+
+### Changed in 0.1.3
+
+- Tests moved from ``leggedsnake/tests`` to ``tests/``.
+- Examples moved from ``leggedsnake/examples/`` to ``docs/examples/``.
+- I was testing my code on ``leggedsnake/examples/strider.py``  (the old path) and
+  that's why it was a big mess. I cleaned up that all. Sorry for the
+  inconvenience!
+
+### Fixed in 0.1.3
+
+- A lot of outdated code in the ``leggedsnake/examples/strider.py``
+- Changelog URL was broken in ``setup.cfg``.
 
 ## [0.1.2-alpha] - 2021-07-07
-### Changed
- - The ``step`` function execution speed has been increased by 25% when 
-   ``return_res`` is ``True``! Small performance improvement when ``return_res``
-   is ``False``.
- - The ``size`` argument of ``step`` function is now known as ``witdh``.
- - We now require pylinkage>=0.4.0.
-
-### Fixed
- - Files in ``leggedsnake/examples/`` were not included in the PyPi package.
- - The example was incompatible with pylinkage 0.4.0.
- - Test suite was unusable by tox.
- - Tests fixed.
- - Incompatible argument between PyGAD init_pop and built-in GA.
 
-### Security
- - Tests with ``tox.ini`` now include Python 3.9 and Flake 8.
+### Added in 0.1.2
+
+- Security: tests with ``tox.ini`` now include Python 3.9 and Flake 8.
+
+### Changed in 0.1.2
+
+- The ``step`` function execution speed has been increased by 25% when
+  ``return_res`` is ``True``! Small performance improvement when ``return_res``
+  is ``False``.
+- The ``size`` argument of ``step`` function is now known as ``witdh``.
+- We now require pylinkage>=0.4.0.
+
+### Fixed in 0.1.2
+
+- Files in ``leggedsnake/examples/`` were not included in the PyPi package.
+- The example was incompatible with pylinkage 0.4.0.
+- Test suite was unusable by tox.
+- Tests fixed.
+- Incompatible argument between PyGAD init_pop and built-in GA.
 
 ## [0.1.1-alpha] - 2021-06-26
-### Added
- - The example file ``examples/strider.py`` is now shipped with the Python 
-   package.
- - ``leggedsnake/geneticoptimizer.py`` can now automatically switch to the 
-   built-in GA algorithm if PyGAD is not installed.
 
-### Changed
- - ``setup.cfg`` metadata
+### Added in 0.1.1
+
+- The example file ``examples/strider.py`` is now shipped with the Python
+  package.
+- ``leggedsnake/geneticoptimizer.py`` can now automatically switch to the
+  built-in GA algorithm if PyGAD is not installed.
+
+### Changed in 0.1.1
+
+- ``setup.cfg`` metadata
 
 ## [0.1.0-alpha] - 2021-06-25
-### Added
- - Code vulnerabilities automatic checks
- - Example videos in ``examples/images/``
-
-### Changed
- - Manny reforms in code style, to make the dynamic part naming conventions 
-   consistent with Pymunk. 
- - Images in the ``README.md``!
-
-### Fixed
- - You can now define linkages with an enormous number of legs. Systems with
-   many should no longer break physics but your CPU instead :)
+
+### Added in 0.1.0
+
+- Code vulnerabilities automatic checks
+- Example videos in ``examples/images/``
+
+### Changed in 0.1.0
+
+- Many reforms in code style in order to make the dynamic part of naming conventions
+  consistent with Pymunk.
+- Images in the ``README.md``!
+
+### Fixed in 0.1.0
+
+- You can now define linkages with an enormous number of legs. Systems with
+  many should no longer break physics but your CPU instead :)
 
 ## [0.0.3-alpha] - 2021-06-23
-### Added
- - Started walktrough demo in ``README.md``
- - Automatic release to PyPi
-
-### Fixed
- - Pymunk version should be at least 6.0.0 in requirement files.
- - Some URLs typos in ``README.md``
- - Versioning tests not executing (GitHub action)
+
+### Added in 0.0.3
+
+- Started walkthrough demo in ``README.md``
+- Automatic release to PyPi
+
+### Fixed in 0.0.3
+
+- Pymunk version should be at least 6.0.0 in requirement files.
+- Some URLs typos in ``README.md``
+- Versioning tests not executing (GitHub action)
 
 ## [0.0.2-alpha] - 2021-06-22
-### Added
+
+### Added in 0.0.2
+
 - ``requirement.txt`` was absent due to ``.gitignore`` misconfiguration.
 
-### Changed
- - ``.gitignore`` now ignores .txt files only in the leggedsnake folder.
- - ``environment.yml`` more flexible (versions can be superior to the selected). 
-   pymunk>5.0.0 and pylinkage added.
- - ``leggedsnake/utility.py`` not having zipfile or xml modules error 
-   encapsulation.
-
-### Fixed
- - ``setup.cfg`` was not PyPi compatible. Removed mail (use GitHub!), we now 
-   explicitly say that ``README.md`` is markdown (PyPi is conservative)
-   
+### Changed in 0.0.2
+
+- ``.gitignore`` now ignores .txt files only in the leggedsnake folder.
+- ``environment.yml`` more flexible (versions can be superior to the selected).
+  pymunk>5.0.0 and pylinkage added.
+- ``leggedsnake/utility.py`` not having zipfile or xml modules error
+  encapsulation.
+
+### Fixed in 0.0.2
+
+- ``setup.cfg`` was not PyPi compatible. Removed mail (use GitHub!), we now
+  explicitly say that ``README.md`` is markdown (PyPi is conservative)
+
 ## [0.0.1-alpha] - 2021-06-22
-Basic version, supporting Genetic Algorithm optimization, but with various 
+
+Basic version, supporting Genetic Algorithm optimization, but with various
 problems.
-### Added
- - ``CODE_OF_CONDUCT.md`` to help community.
- - ``LICENSE`` MIT License.
- - ``MANIFEST.in`` to include more files.
- - ``README.md`` as a very minimal version.
- - ``environment.yml`` with matplotlib, numpy, and pygad requirement.
- - ``examples/strider.py`` a complete demo with Strider linkage.
- - ``leggedsnake/__init__.py``.
- - ``leggedsnake/dynamiclinkage.py``.
- - ``leggedsnake/geneticoptimizer.py``.
- - ``leggedsnake/physicsengine.py``.
- - ``leggedsnake/show_evolution.py`` just a legacy package, no utility.
- - ``leggedsnake/tests/test_utility.py`` untested test case
- - ``leggedsnake/utility.py`` contain some useful evaluation function (``step``
-   and ``stride``) and a broken GeoGebra interface.
- - ``walker.py`` defines the ``Walker`` object.
- - ``pyproject.toml``. 
- - ``setup.cfg``.
- - ``setup.py`` empty, for compatibility purposes only.
- - ``tox.ini`` tox with Python 3.7 and 3.8
 
+### Added in 0.0.1
+
+- ``CODE_OF_CONDUCT.md`` to help community.
+- ``LICENSE`` MIT License.
+- ``MANIFEST.in`` to include more files.
+- ``README.md`` as a very minimal version.
+- ``environment.yml`` with matplotlib, numpy, and pygad requirement.
+- ``examples/strider.py`` a complete demo with Strider linkage.
+- ``leggedsnake/__init__.py``.
+- ``leggedsnake/dynamiclinkage.py``.
+- ``leggedsnake/geneticoptimizer.py``.
+- ``leggedsnake/physicsengine.py``.
+- ``leggedsnake/show_evolution.py`` just a legacy package, no utility.
+- ``leggedsnake/tests/test_utility.py`` untested test case
+- ``leggedsnake/utility.py`` contain some useful evaluation function (``step``
+  and ``stride``) and a broken GeoGebra interface.
+- ``walker.py`` defines the ``Walker`` object.
+- ``pyproject.toml``.
+- ``setup.cfg``.
+- ``setup.py`` empty, for compatibility purposes only.
+- ``tox.ini`` tox with Python 3.7 and 3.8.
```

### Comparing `leggedsnake-0.3.0/leggedsnake.egg-info/SOURCES.txt` & `leggedsnake-0.3.1/leggedsnake.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.md
 CODE_OF_CONDUCT.md
 LICENSE.rst
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
@@ -22,8 +23,9 @@
 leggedsnake/show_evolution.py
 leggedsnake/utility.py
 leggedsnake/walker.py
 leggedsnake.egg-info/PKG-INFO
 leggedsnake.egg-info/SOURCES.txt
 leggedsnake.egg-info/dependency_links.txt
 leggedsnake.egg-info/requires.txt
-leggedsnake.egg-info/top_level.txt
+leggedsnake.egg-info/top_level.txt
+tests/test_utility.py
```

### Comparing `leggedsnake-0.3.0/setup.cfg` & `leggedsnake-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.0
+current_version = 0.3.1
 commit = False
 tag = False
 
 [metadata]
 name = leggedsnake
 version = attr: leggedsnake.__version__
 author = Hugo Farajallah
```

