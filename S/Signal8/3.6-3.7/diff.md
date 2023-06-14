# Comparing `tmp/Signal8-3.6.tar.gz` & `tmp/Signal8-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-3.6.tar", last modified: Tue Jun 13 18:29:09 2023, max compression
+gzip compressed data, was "Signal8-3.7.tar", last modified: Wed Jun 14 03:18:22 2023, max compression
```

## Comparing `Signal8-3.6.tar` & `Signal8-3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:29:09.632022 Signal8-3.6/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.6/LICENSE
--rw-rw-rw-   0        0        0     5356 2023-06-13 18:29:09.627024 Signal8-3.6/PKG-INFO
--rw-rw-rw-   0        0        0     4858 2023-06-12 22:34:01.000000 Signal8-3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 18:29:09.542024 Signal8-3.6/Signal8/
--rw-rw-rw-   0        0        0    11138 2023-06-13 18:22:14.000000 Signal8-3.6/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-12 18:52:22.000000 Signal8-3.6/Signal8/__init__.py
--rw-rw-rw-   0        0        0      214 2023-06-13 18:14:07.000000 Signal8-3.6/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:29:09.620032 Signal8-3.6/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.6/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5469 2023-06-13 18:21:58.000000 Signal8-3.6/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     1116 2023-06-12 21:36:47.000000 Signal8-3.6/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.6/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12597 2023-06-13 18:21:42.000000 Signal8-3.6/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.6/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:29:09.588023 Signal8-3.6/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5356 2023-06-13 18:29:09.000000 Signal8-3.6/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-06-13 18:29:09.000000 Signal8-3.6/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:29:09.000000 Signal8-3.6/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-13 18:29:09.000000 Signal8-3.6/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 18:29:09.632022 Signal8-3.6/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-13 18:28:09.000000 Signal8-3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:18:22.205922 Signal8-3.7/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.7/LICENSE
+-rw-rw-rw-   0        0        0     5356 2023-06-14 03:18:22.203923 Signal8-3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4858 2023-06-12 22:34:01.000000 Signal8-3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 03:18:22.039921 Signal8-3.7/Signal8/
+-rw-rw-rw-   0        0        0    11138 2023-06-14 03:16:13.000000 Signal8-3.7/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-12 18:52:22.000000 Signal8-3.7/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-06-13 18:14:07.000000 Signal8-3.7/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:18:22.195928 Signal8-3.7/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.7/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5469 2023-06-13 18:21:58.000000 Signal8-3.7/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     1116 2023-06-12 21:36:47.000000 Signal8-3.7/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.7/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12804 2023-06-14 03:13:43.000000 Signal8-3.7/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.7/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:18:22.133922 Signal8-3.7/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5356 2023-06-14 03:18:21.000000 Signal8-3.7/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-06-14 03:18:21.000000 Signal8-3.7/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:18:21.000000 Signal8-3.7/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 03:18:21.000000 Signal8-3.7/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 03:18:22.206920 Signal8-3.7/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-14 03:17:11.000000 Signal8-3.7/setup.py
```

### Comparing `Signal8-3.6/LICENSE` & `Signal8-3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-3.6/PKG-INFO` & `Signal8-3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.6
+Version: 3.7
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-3.6/README.md` & `Signal8-3.7/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-3.6/Signal8/Signal8.py` & `Signal8-3.7/Signal8/Signal8.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.6/Signal8/utils/core.py` & `Signal8-3.7/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.6/Signal8/utils/problems.py` & `Signal8-3.7/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.6/Signal8/utils/simple_env.py` & `Signal8-3.7/Signal8/utils/simple_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,16 +70,16 @@
             self.observation_spaces[agent.name] = spaces.Box(
                 low=-np.float32(1),
                 high=+np.float32(1),
                 shape=(obs_dim,),
                 dtype=np.float32,
             )
         
-        # state space is used by aerial agent, encodes agents and large obstacles
-        state_dim = len(world.agents) * 2 + len(world.large_obstacles) * 2
+        # state space is used by aerial agent; it encodes the positions of all agents, obstacles, and goals
+        state_dim = len(world.agents) * 2 + len(world.large_obstacles) * 2 + len(world.agents) * 2
         self.state_space = spaces.Box(
             low=-np.float32(1),
             high=+np.float32(1),
             shape=(state_dim,),
             dtype=np.float32,
         )
         self.steps = 0
@@ -104,18 +104,21 @@
             raise Exception('The state of the system can only be retrieved at the start of an episode before any steps have been taken.')
         
         state = np.zeros(self.state_space.shape)
         
         for i, agent in enumerate(self.world.agents):
             state[2*i : 2*i+2] = agent.state.p_pos
 
-        # Calculate the starting index for the obstacles in the state array
         start_idx = 2 * len(self.world.agents)
         for i, obstacle in enumerate(self.world.large_obstacles):
             state[start_idx + 2*i : start_idx + 2*i+2] = obstacle.state.p_pos
+        
+        start_idx = 2 * len(self.world.agents) + 2 * len(self.world.large_obstacles)
+        for i, agent in enumerate(self.world.agents):
+            state[start_idx + 2*i : start_idx + 2*i+2] = agent.goal_a.state.p_pos
              
         return np.concatenate(state, axis=None)
 
     def reset(self, seed=None, return_info=False, options=None):        
         if seed is not None:
             self.seed(seed=seed)
```

### Comparing `Signal8-3.6/Signal8/utils/test_dynamic_obs.py` & `Signal8-3.7/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.6/Signal8.egg-info/PKG-INFO` & `Signal8-3.7/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.6
+Version: 3.7
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-3.6/setup.py` & `Signal8-3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="3.6",
+    version="3.7",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

