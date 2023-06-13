# Comparing `tmp/Navix-0.1.2.tar.gz` & `tmp/Navix-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Navix-0.1.2.tar", last modified: Tue Jun 13 21:32:18 2023, max compression
+gzip compressed data, was "Navix-0.1.3.tar", last modified: Tue Jun 13 21:59:21 2023, max compression
```

## Comparing `Navix-0.1.2.tar` & `Navix-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.872310 Navix-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.864310 Navix-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.868310 Navix-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 21:32:08.000000 Navix-0.1.2/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-13 21:32:08.000000 Navix-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 21:32:08.000000 Navix-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 21:32:08.000000 Navix-0.1.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 21:32:08.000000 Navix-0.1.2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-13 21:32:08.000000 Navix-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 21:32:08.000000 Navix-0.1.2/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.868310 Navix-0.1.2/Navix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-06-13 21:32:18.000000 Navix-0.1.2/Navix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 21:32:18.000000 Navix-0.1.2/Navix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:32:18.000000 Navix-0.1.2/Navix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 21:32:18.000000 Navix-0.1.2/Navix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 21:32:18.000000 Navix-0.1.2/Navix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-06-13 21:32:18.872310 Navix-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-13 21:32:08.000000 Navix-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.868310 Navix-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-13 21:32:08.000000 Navix-0.1.2/docs/profiling.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.872310 Navix-0.1.2/navix/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.872310 Navix-0.1.2/navix/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/environments/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/environments/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/termination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-13 21:32:08.000000 Navix-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 21:32:08.000000 Navix-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:32:18.872310 Navix-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.872310 Navix-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-13 21:32:08.000000 Navix-0.1.2/tests/test_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.068319 Navix-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.060319 Navix-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.064319 Navix-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 21:59:06.000000 Navix-0.1.3/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-13 21:59:06.000000 Navix-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 21:59:06.000000 Navix-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 21:59:06.000000 Navix-0.1.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 21:59:06.000000 Navix-0.1.3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-13 21:59:06.000000 Navix-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 21:59:06.000000 Navix-0.1.3/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.064319 Navix-0.1.3/Navix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-06-13 21:59:21.000000 Navix-0.1.3/Navix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 21:59:21.000000 Navix-0.1.3/Navix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:59:21.000000 Navix-0.1.3/Navix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 21:59:21.000000 Navix-0.1.3/Navix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 21:59:21.000000 Navix-0.1.3/Navix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-06-13 21:59:21.068319 Navix-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-13 21:59:06.000000 Navix-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.064319 Navix-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-13 21:59:06.000000 Navix-0.1.3/docs/profiling.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.068319 Navix-0.1.3/navix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.068319 Navix-0.1.3/navix/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/environments/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/environments/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-13 21:59:06.000000 Navix-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 21:59:06.000000 Navix-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:59:21.068319 Navix-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.068319 Navix-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-13 21:59:06.000000 Navix-0.1.3/tests/test_environment.py
```

### Comparing `Navix-0.1.2/.github/workflows/CD.yml` & `Navix-0.1.3/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/.github/workflows/CI.yml` & `Navix-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/.gitignore` & `Navix-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/COPYRIGHT` & `Navix-0.1.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/LICENSE` & `Navix-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/Navix.egg-info/PKG-INFO` & `Navix-0.1.3/Navix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.1.2
+Version: 0.1.3
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -250,15 +250,15 @@
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
-NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **~2000x** faster with Autograd and XLA support.
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
 We currently support the OSs supported by JAX.
 You can find a description [here](https://github.com/google/jax#installation).
```

### Comparing `Navix-0.1.2/Navix.egg-info/SOURCES.txt` & `Navix-0.1.3/Navix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/PKG-INFO` & `Navix-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.1.2
+Version: 0.1.3
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -250,15 +250,15 @@
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
-NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **~2000x** faster with Autograd and XLA support.
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
 We currently support the OSs supported by JAX.
 You can find a description [here](https://github.com/google/jax#installation).
```

### Comparing `Navix-0.1.2/README.md` & `Navix-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
-NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **~2000x** faster with Autograd and XLA support.
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
 We currently support the OSs supported by JAX.
 You can find a description [here](https://github.com/google/jax#installation).
```

### Comparing `Navix-0.1.2/navix/__init__.py` & `Navix-0.1.3/navix/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
 
 
 from . import (
     actions,
     components,
     grid,
```

### Comparing `Navix-0.1.2/navix/actions.py` & `Navix-0.1.3/navix/actions.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/navix/components.py` & `Navix-0.1.3/navix/components.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/navix/environments/__init__.py` & `Navix-0.1.3/navix/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/navix/environments/environment.py` & `Navix-0.1.3/navix/environments/environment.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/navix/environments/room.py` & `Navix-0.1.3/navix/environments/room.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/navix/grid.py` & `Navix-0.1.3/navix/grid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/navix/observations.py` & `Navix-0.1.3/navix/observations.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/navix/tasks.py` & `Navix-0.1.3/navix/tasks.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/navix/termination.py` & `Navix-0.1.3/navix/termination.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/navix/transitions.py` & `Navix-0.1.3/navix/transitions.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/pyproject.toml` & `Navix-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Navix-0.1.2/tests/test_environment.py` & `Navix-0.1.3/tests/test_environment.py`

 * *Files identical despite different names*

