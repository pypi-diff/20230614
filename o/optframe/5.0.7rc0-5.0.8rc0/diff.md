# Comparing `tmp/optframe-5.0.7rc0.tar.gz` & `tmp/optframe-5.0.8rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optframe-5.0.7rc0.tar", last modified: Mon Sep 26 21:35:02 2022, max compression
+gzip compressed data, was "optframe-5.0.8rc0.tar", last modified: Tue Sep 27 01:39:16 2022, max compression
```

## Comparing `optframe-5.0.7rc0.tar` & `optframe-5.0.8rc0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-26 21:35:02.404787 optframe-5.0.7rc0/
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)       80 2021-08-20 01:21:08.000000 optframe-5.0.7rc0/.clang-format
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      162 2021-08-20 01:21:03.000000 optframe-5.0.7rc0/CPPLINT.cfg
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     1926 2022-09-26 19:09:24.000000 optframe-5.0.7rc0/LICENSE
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      150 2022-09-26 20:02:27.000000 optframe-5.0.7rc0/MANIFEST.in
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     7267 2022-09-26 21:35:02.404787 optframe-5.0.7rc0/PKG-INFO
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     4583 2022-09-26 21:33:18.000000 optframe-5.0.7rc0/README.md
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      478 2022-09-26 21:33:18.000000 optframe-5.0.7rc0/bumpver.toml
-drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-26 21:35:02.404787 optframe-5.0.7rc0/demo/
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    13188 2022-09-26 18:41:40.000000 optframe-5.0.7rc0/demo/demo_kp.py
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    35796 2022-09-24 02:38:22.000000 optframe-5.0.7rc0/demo/draft_pyfcore.py
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      902 2022-09-26 17:55:27.000000 optframe-5.0.7rc0/makefile
-drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-26 21:35:02.404787 optframe-5.0.7rc0/optframe/
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      216 2022-09-26 21:33:18.000000 optframe-5.0.7rc0/optframe/__init__.py
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    22697 2022-09-26 18:35:32.000000 optframe-5.0.7rc0/optframe/engine.py
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    52581 2022-09-26 20:08:10.000000 optframe-5.0.7rc0/optframe/optframe_lib.cpp
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     4811 2022-09-26 18:47:36.000000 optframe-5.0.7rc0/optframe/optframe_lib.h
-drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-26 21:35:02.404787 optframe-5.0.7rc0/optframe.egg-info/
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     7267 2022-09-26 21:35:02.000000 optframe-5.0.7rc0/optframe.egg-info/PKG-INFO
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      388 2022-09-26 21:35:02.000000 optframe-5.0.7rc0/optframe.egg-info/SOURCES.txt
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)        1 2022-09-26 21:35:02.000000 optframe-5.0.7rc0/optframe.egg-info/dependency_links.txt
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)       44 2022-09-26 21:35:02.000000 optframe-5.0.7rc0/optframe.egg-info/requires.txt
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)        9 2022-09-26 21:35:02.000000 optframe-5.0.7rc0/optframe.egg-info/top_level.txt
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      852 2022-09-26 21:33:18.000000 optframe-5.0.7rc0/pyproject.toml
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)       38 2022-09-26 21:35:02.404787 optframe-5.0.7rc0/setup.cfg
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     4618 2022-09-26 21:33:18.000000 optframe-5.0.7rc0/setup.py
+drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)       80 2021-08-20 01:21:08.000000 optframe-5.0.8rc0/.clang-format
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      162 2021-08-20 01:21:03.000000 optframe-5.0.8rc0/CPPLINT.cfg
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     1926 2022-09-26 19:09:24.000000 optframe-5.0.8rc0/LICENSE
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      150 2022-09-26 20:02:27.000000 optframe-5.0.8rc0/MANIFEST.in
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     7406 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/PKG-INFO
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     4722 2022-09-27 01:38:40.000000 optframe-5.0.8rc0/README.md
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      530 2022-09-27 01:38:40.000000 optframe-5.0.8rc0/bumpver.toml
+drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/demo/
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    13188 2022-09-26 18:41:40.000000 optframe-5.0.8rc0/demo/demo_kp.py
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    35796 2022-09-24 02:38:22.000000 optframe-5.0.8rc0/demo/draft_pyfcore.py
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      958 2022-09-26 23:03:20.000000 optframe-5.0.8rc0/makefile
+drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/optframe/
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      216 2022-09-27 01:38:40.000000 optframe-5.0.8rc0/optframe/__init__.py
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    23000 2022-09-26 23:53:01.000000 optframe-5.0.8rc0/optframe/engine.py
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    52712 2022-09-26 23:47:58.000000 optframe-5.0.8rc0/optframe/optframe_lib.cpp
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     4882 2022-09-26 23:46:59.000000 optframe-5.0.8rc0/optframe/optframe_lib.h
+drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/optframe.egg-info/
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     7406 2022-09-27 01:39:16.000000 optframe-5.0.8rc0/optframe.egg-info/PKG-INFO
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      388 2022-09-27 01:39:16.000000 optframe-5.0.8rc0/optframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)        1 2022-09-27 01:39:16.000000 optframe-5.0.8rc0/optframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)       44 2022-09-27 01:39:16.000000 optframe-5.0.8rc0/optframe.egg-info/requires.txt
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)        9 2022-09-27 01:39:16.000000 optframe-5.0.8rc0/optframe.egg-info/top_level.txt
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      852 2022-09-27 01:38:40.000000 optframe-5.0.8rc0/pyproject.toml
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)       38 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/setup.cfg
+-rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     4618 2022-09-27 01:38:40.000000 optframe-5.0.8rc0/setup.py
```

### Comparing `optframe-5.0.7rc0/LICENSE` & `optframe-5.0.8rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `optframe-5.0.7rc0/PKG-INFO` & `optframe-5.0.8rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optframe
-Version: 5.0.7rc0
+Version: 5.0.8rc0
 Summary: Python bindings for OptFrame Functional Core
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
 License: OptFrame Python - Optimization Framework
         Copyright (C) 2009-2022 - MIT LICENSE
         https://github.com/optframe/pyoptframe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -43,15 +43,17 @@
 License-File: LICENSE
 
 # pyoptframe
 Python bindings for OptFrame Functional Core
 
 Install: `python -m pip install optframe`
 
-Version: `pyoptframe v5.0.7rc0`
+Version: `pyoptframe v5.0.8rc0`
+
+Documentation and Tutorials: see [PyOptFrame Quickstart](https://pyoptframe.readthedocs.io/en/latest/quickstart.html)
 
 [OptFrame](https://github.com/optframe/optframe) is a C++ framework for optimization problems, including techniques such as classic metaheuristics Simulated Annealing, Genetic Algorithm, 
 Variable Neighborhood Search, Iterated Local Search, Tabu Search, Particle Swarm Optimization, NSGA-II, and other single and multi-objective methods.
 This is a 10-year project with several practical applications in industry and academia, so feel free to use it.
 
 ## How to test
 
@@ -156,29 +158,29 @@
 
 `python -m build`
 
 `twine check dist/*`
 
 `twine upload -r testpypi dist/* --verbose`
 
-Error: Binary wheel 'optframe-5.0.7rc0-cp39-cp39-linux_x86_64.whl' has an unsupported platform tag 'linux_x86_64'. See [1](https://stackoverflow.com/questions/59451069/binary-wheel-cant-be-uploaded-on-pypi-using-twine) and [2](https://peps.python.org/pep-0513/#rationale).
+Error: Binary wheel 'optframe-5.0.8rc0-cp39-cp39-linux_x86_64.whl' has an unsupported platform tag 'linux_x86_64'. See [1](https://stackoverflow.com/questions/59451069/binary-wheel-cant-be-uploaded-on-pypi-using-twine) and [2](https://peps.python.org/pep-0513/#rationale).
 
 Solution: `rm -f dist/*.whl`
 
 `twine upload -r testpypi dist/* --verbose`
 
 Test if OK on test package website:
 
-`python -m pip install -i https://test.pypi.org/simple optframe`
+`python -m pip install -i https://test.pypi.org/simple optframe --upgrade`
 
 Finally:
 
 `twine upload dist/*`
 
-`python -m pip install optframe`
+`python -m pip install optframe --upgrade`
 
 Thanks again to: https://realpython.com/pypi-publish-python-package/
 
 
 ## Known Issues
 
 All known issues fixed :)
```

### Comparing `optframe-5.0.7rc0/README.md` & `optframe-5.0.8rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # pyoptframe
 Python bindings for OptFrame Functional Core
 
 Install: `python -m pip install optframe`
 
-Version: `pyoptframe v5.0.7rc0`
+Version: `pyoptframe v5.0.8rc0`
+
+Documentation and Tutorials: see [PyOptFrame Quickstart](https://pyoptframe.readthedocs.io/en/latest/quickstart.html)
 
 [OptFrame](https://github.com/optframe/optframe) is a C++ framework for optimization problems, including techniques such as classic metaheuristics Simulated Annealing, Genetic Algorithm, 
 Variable Neighborhood Search, Iterated Local Search, Tabu Search, Particle Swarm Optimization, NSGA-II, and other single and multi-objective methods.
 This is a 10-year project with several practical applications in industry and academia, so feel free to use it.
 
 ## How to test
 
@@ -112,29 +114,29 @@
 
 `python -m build`
 
 `twine check dist/*`
 
 `twine upload -r testpypi dist/* --verbose`
 
-Error: Binary wheel 'optframe-5.0.7rc0-cp39-cp39-linux_x86_64.whl' has an unsupported platform tag 'linux_x86_64'. See [1](https://stackoverflow.com/questions/59451069/binary-wheel-cant-be-uploaded-on-pypi-using-twine) and [2](https://peps.python.org/pep-0513/#rationale).
+Error: Binary wheel 'optframe-5.0.8rc0-cp39-cp39-linux_x86_64.whl' has an unsupported platform tag 'linux_x86_64'. See [1](https://stackoverflow.com/questions/59451069/binary-wheel-cant-be-uploaded-on-pypi-using-twine) and [2](https://peps.python.org/pep-0513/#rationale).
 
 Solution: `rm -f dist/*.whl`
 
 `twine upload -r testpypi dist/* --verbose`
 
 Test if OK on test package website:
 
-`python -m pip install -i https://test.pypi.org/simple optframe`
+`python -m pip install -i https://test.pypi.org/simple optframe --upgrade`
 
 Finally:
 
 `twine upload dist/*`
 
-`python -m pip install optframe`
+`python -m pip install optframe --upgrade`
 
 Thanks again to: https://realpython.com/pypi-publish-python-package/
 
 
 ## Known Issues
 
 All known issues fixed :)
```

### Comparing `optframe-5.0.7rc0/demo/demo_kp.py` & `optframe-5.0.8rc0/demo/demo_kp.py`

 * *Files identical despite different names*

### Comparing `optframe-5.0.7rc0/demo/draft_pyfcore.py` & `optframe-5.0.8rc0/demo/draft_pyfcore.py`

 * *Files identical despite different names*

### Comparing `optframe-5.0.7rc0/makefile` & `optframe-5.0.8rc0/makefile`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 	@echo "EXAMPLE: ln -s  my/full/optframe/include  src/optframe-src"
 	$(CC) $(CPPSTD) -g -Isrc/optframe-src/include -Wall -pedantic -Ofast --shared optframe/optframe_lib.cpp -o optframe/optframe_lib.so -fPIC
 	#readelf -s build/optframe_lib.so | grep fcore
 
 demo_local: optframe/optframe_lib.so
 	# valgrind --leak-check=full python3 demo/demo_kp.py 
 	python3 demo/demo_kp.py 
-	
+
+.PHONY: docs
+
+docs:
+	cd docs && make clean && make html
+
 
 test:   #install
 	# (cd demo/ && python3 demo_pyfcore.py)
 	(cd tests/ && python3 test_engine_kp.py)
 	
 
 install:
```

### Comparing `optframe-5.0.7rc0/optframe/engine.py` & `optframe-5.0.8rc0/optframe/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,24 +149,26 @@
 optframe_lib.optframe_api0d_get_evaluator.restype = ctypes.c_void_p
 #
 optframe_lib.optframe_api0d_get_constructive.argtypes = [
     ctypes.c_void_p, c_int32]
 optframe_lib.optframe_api0d_get_constructive.restype = ctypes.c_void_p
 ###
 
-
 # Engine: HeuristicFactory
 optframe_lib.optframe_api1d_create_engine.argtypes = [ctypes.c_int]
 optframe_lib.optframe_api1d_create_engine.restype = ctypes.c_void_p
 #
 optframe_lib.optframe_api1d_destroy_engine.argtypes = [ctypes.c_void_p]
 optframe_lib.optframe_api1d_destroy_engine.restype = ctypes.c_bool
 #
 optframe_lib.optframe_api0d_engine_test.argtypes = [ctypes.c_void_p]
 optframe_lib.optframe_api0d_engine_test.restype = ctypes.c_bool
+#
+optframe_lib.optframe_api0d_engine_welcome.argtypes = [ctypes.c_void_p]
+optframe_lib.optframe_api0d_engine_welcome.restype = None
 
 #
 optframe_lib.optframe_api1d_engine_list_builders.argtypes = [
     ctypes.c_void_p, ctypes.c_char_p]
 optframe_lib.optframe_api1d_engine_list_builders.restype = ctypes.c_int
 #
 optframe_lib.optframe_api1d_engine_list_components.argtypes = [
@@ -269,15 +271,16 @@
 # example:
 # if (loglevel >= LogLevel::Warning) { ... }
 
 
 # optframe.Engine
 class Engine(object):
     def __init__(self, apilevel: APILevel = APILevel.API1d, loglevel: LogLevel = LogLevel.Info):
-        ll_int = int(loglevel)
+        self.loglevel = loglevel
+        ll_int = int(self.loglevel)
         assert (apilevel == APILevel.API1d)
         if (loglevel >= LogLevel.Debug):
             print("Debug: Engine using API level API1d")
         self.hf = optframe_lib.optframe_api1d_create_engine(ll_int)
         self.callback_sol_deepcopy_ptr = FUNC_SOL_DEEPCOPY(
             callback_sol_deepcopy_utils)
         self.callback_sol_tostring_ptr = FUNC_SOL_TOSTRING(
@@ -293,17 +296,21 @@
         # must keep callbacks in memory, otherwise Python cleans them...
         # TODO: pass callbacks with IncRef, so that we can keep them on C++ counterpart objects...
         # TODO: think if unique_ptr<std::function<...>> is an interesting pattern of OptFCore C++
         # TODO: for now, just keep them here.
         self.callback_list.append(func)
 
     def cleanup(self):
-        print("Running optframe cleanup...")
+        if (self.loglevel >= LogLevel.Debug):
+            print("Running optframe cleanup...")
         optframe_lib.optframe_api1d_destroy_engine(self.hf)
 
+    def welcome(self):
+        optframe_lib.optframe_api0d_engine_welcome(self.hf)
+
     def print_component(self, component):
         optframe_lib.optframe_api0_component_print(component)
 
     def component_set_loglevel(self, scomponent, loglevel, recursive):
         if (not isinstance(scomponent, str)):
             assert (False)
         b_comp = scomponent.encode('ascii')
```

### Comparing `optframe-5.0.7rc0/optframe/optframe_lib.cpp` & `optframe-5.0.8rc0/optframe/optframe_lib.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -465,14 +465,20 @@
       return sol;
    }
    */
 };
 
 // ==================
 
+extern "C" void
+optframe_api0d_engine_welcome(FakeEnginePtr _engine)
+{
+   std::cout << optframe::FCore::welcome() << std::endl;
+}
+
 extern "C" FakeEnginePtr
 optframe_api1d_create_engine(int ll)
 {
    auto l = (optframe::LogLevel)ll;
    auto* _eng = new FCoreApi1Engine;
    if (l == optframe::LogLevel::Debug)
       std::cout << "Debug: will set OptFrame Engine loglevel to Debug" << std::endl;
```

### Comparing `optframe-5.0.7rc0/optframe/optframe_lib.h` & `optframe-5.0.8rc0/optframe/optframe_lib.h`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,17 @@
    bool has_best; // ("has_best", ctypes.c_bool),
    void* best_s;  // ("best_s", ctypes.py_object),
    double best_e; // ("best_e", ctypes.c_double)]
 };
 
 // ============================ Engine: HeuristicFactory ===========================
 
+extern "C" void
+optframe_api0d_engine_welcome(FakeEnginePtr _engine);
+
 extern "C" FakeEnginePtr
 optframe_api1d_create_engine(int LogLevel);
 
 extern "C" bool
 optframe_api1d_engine_check(FakeEnginePtr _engine, int p1, int p2, bool verbose);
 
 extern "C" LibSearchOutput
```

### Comparing `optframe-5.0.7rc0/optframe.egg-info/PKG-INFO` & `optframe-5.0.8rc0/optframe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optframe
-Version: 5.0.7rc0
+Version: 5.0.8rc0
 Summary: Python bindings for OptFrame Functional Core
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
 License: OptFrame Python - Optimization Framework
         Copyright (C) 2009-2022 - MIT LICENSE
         https://github.com/optframe/pyoptframe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -43,15 +43,17 @@
 License-File: LICENSE
 
 # pyoptframe
 Python bindings for OptFrame Functional Core
 
 Install: `python -m pip install optframe`
 
-Version: `pyoptframe v5.0.7rc0`
+Version: `pyoptframe v5.0.8rc0`
+
+Documentation and Tutorials: see [PyOptFrame Quickstart](https://pyoptframe.readthedocs.io/en/latest/quickstart.html)
 
 [OptFrame](https://github.com/optframe/optframe) is a C++ framework for optimization problems, including techniques such as classic metaheuristics Simulated Annealing, Genetic Algorithm, 
 Variable Neighborhood Search, Iterated Local Search, Tabu Search, Particle Swarm Optimization, NSGA-II, and other single and multi-objective methods.
 This is a 10-year project with several practical applications in industry and academia, so feel free to use it.
 
 ## How to test
 
@@ -156,29 +158,29 @@
 
 `python -m build`
 
 `twine check dist/*`
 
 `twine upload -r testpypi dist/* --verbose`
 
-Error: Binary wheel 'optframe-5.0.7rc0-cp39-cp39-linux_x86_64.whl' has an unsupported platform tag 'linux_x86_64'. See [1](https://stackoverflow.com/questions/59451069/binary-wheel-cant-be-uploaded-on-pypi-using-twine) and [2](https://peps.python.org/pep-0513/#rationale).
+Error: Binary wheel 'optframe-5.0.8rc0-cp39-cp39-linux_x86_64.whl' has an unsupported platform tag 'linux_x86_64'. See [1](https://stackoverflow.com/questions/59451069/binary-wheel-cant-be-uploaded-on-pypi-using-twine) and [2](https://peps.python.org/pep-0513/#rationale).
 
 Solution: `rm -f dist/*.whl`
 
 `twine upload -r testpypi dist/* --verbose`
 
 Test if OK on test package website:
 
-`python -m pip install -i https://test.pypi.org/simple optframe`
+`python -m pip install -i https://test.pypi.org/simple optframe --upgrade`
 
 Finally:
 
 `twine upload dist/*`
 
-`python -m pip install optframe`
+`python -m pip install optframe --upgrade`
 
 Thanks again to: https://realpython.com/pypi-publish-python-package/
 
 
 ## Known Issues
 
 All known issues fixed :)
```

### Comparing `optframe-5.0.7rc0/pyproject.toml` & `optframe-5.0.8rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools>=53.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "optframe"
-version = "5.0.7rc0"
+version = "5.0.8rc0"
 description = "Python bindings for OptFrame Functional Core"
 readme = "README.md"
 authors = [{ name = "Igor Machado Coelho", email = "igormcoelho@proton.me" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `optframe-5.0.7rc0/setup.py` & `optframe-5.0.8rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 # WHY?????
 # destination_path = sysconfig.get_python_lib()
 # => /usr/lib/python3/dist-packages
 # print("DEST PATH: ", destination_path)
 
 setup(
     name="optframe",
-    version="5.0.7rc0",
+    version="5.0.8rc0",
     py_modules=["optframe.engine"],
     ext_modules=[
         CTypesExtension(
             "optframe.optframe_lib",
             ["optframe/optframe_lib.cpp"],
             #
             # ========== ONLY IF LOCAL TESTING IS USED ===========
```

