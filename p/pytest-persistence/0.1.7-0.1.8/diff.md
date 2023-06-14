# Comparing `tmp/pytest-persistence-0.1.7.tar.gz` & `tmp/pytest-persistence-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-persistence-0.1.7.tar", last modified: Tue May 16 11:16:38 2023, max compression
+gzip compressed data, was "pytest-persistence-0.1.8.tar", last modified: Wed Jun 14 08:30:22 2023, max compression
```

## Comparing `pytest-persistence-0.1.7.tar` & `pytest-persistence-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-05-16 11:16:38.813660 pytest-persistence-0.1.7/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1077 2021-12-07 17:34:12.000000 pytest-persistence-0.1.7/LICENSE
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      835 2023-05-16 11:16:38.813660 pytest-persistence-0.1.7/PKG-INFO
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      372 2021-12-07 17:34:12.000000 pytest-persistence-0.1.7/README.md
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-05-16 11:16:38.812660 pytest-persistence-0.1.7/pytest_persistence/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1428 2023-03-28 16:41:44.000000 pytest-persistence-0.1.7/pytest_persistence/XDistScheduling.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       22 2023-05-16 11:15:44.000000 pytest-persistence-0.1.7/pytest_persistence/__init__.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     6547 2023-05-16 10:48:26.000000 pytest-persistence-0.1.7/pytest_persistence/plugin.py
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-05-16 11:16:38.812660 pytest-persistence-0.1.7/pytest_persistence.egg-info/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      835 2023-05-16 11:16:38.000000 pytest-persistence-0.1.7/pytest_persistence.egg-info/PKG-INFO
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      396 2023-05-16 11:16:38.000000 pytest-persistence-0.1.7/pytest_persistence.egg-info/SOURCES.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)        1 2023-05-16 11:16:38.000000 pytest-persistence-0.1.7/pytest_persistence.egg-info/dependency_links.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       51 2023-05-16 11:16:38.000000 pytest-persistence-0.1.7/pytest_persistence.egg-info/entry_points.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       19 2023-05-16 11:16:38.000000 pytest-persistence-0.1.7/pytest_persistence.egg-info/top_level.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       38 2023-05-16 11:16:38.813660 pytest-persistence-0.1.7/setup.cfg
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      969 2021-12-07 17:34:12.000000 pytest-persistence-0.1.7/setup.py
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-05-16 11:16:38.813660 pytest-persistence-0.1.7/tests/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      111 2023-05-16 08:13:42.000000 pytest-persistence-0.1.7/tests/test_mock.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1980 2022-06-27 12:07:26.000000 pytest-persistence-0.1.7/tests/test_plugin.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1367 2022-06-27 12:28:20.000000 pytest-persistence-0.1.7/tests/test_unit.py
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-06-14 08:30:22.607442 pytest-persistence-0.1.8/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1077 2021-12-07 17:34:12.000000 pytest-persistence-0.1.8/LICENSE
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1033 2023-06-14 08:30:22.606442 pytest-persistence-0.1.8/PKG-INFO
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      570 2023-06-14 08:29:26.000000 pytest-persistence-0.1.8/README.md
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-06-14 08:30:22.605442 pytest-persistence-0.1.8/pytest_persistence/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1428 2023-03-28 16:41:44.000000 pytest-persistence-0.1.8/pytest_persistence/XDistScheduling.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       22 2023-06-14 08:29:52.000000 pytest-persistence-0.1.8/pytest_persistence/__init__.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     8275 2023-06-14 08:29:26.000000 pytest-persistence-0.1.8/pytest_persistence/plugin.py
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-06-14 08:30:22.606442 pytest-persistence-0.1.8/pytest_persistence.egg-info/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1033 2023-06-14 08:30:22.000000 pytest-persistence-0.1.8/pytest_persistence.egg-info/PKG-INFO
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      396 2023-06-14 08:30:22.000000 pytest-persistence-0.1.8/pytest_persistence.egg-info/SOURCES.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)        1 2023-06-14 08:30:22.000000 pytest-persistence-0.1.8/pytest_persistence.egg-info/dependency_links.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       51 2023-06-14 08:30:22.000000 pytest-persistence-0.1.8/pytest_persistence.egg-info/entry_points.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       19 2023-06-14 08:30:22.000000 pytest-persistence-0.1.8/pytest_persistence.egg-info/top_level.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       38 2023-06-14 08:30:22.607442 pytest-persistence-0.1.8/setup.cfg
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      969 2021-12-07 17:34:12.000000 pytest-persistence-0.1.8/setup.py
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-06-14 08:30:22.606442 pytest-persistence-0.1.8/tests/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      111 2023-05-16 08:13:42.000000 pytest-persistence-0.1.8/tests/test_mock.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1980 2022-06-27 12:07:26.000000 pytest-persistence-0.1.8/tests/test_plugin.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1367 2022-06-27 12:28:20.000000 pytest-persistence-0.1.8/tests/test_unit.py
```

### Comparing `pytest-persistence-0.1.7/LICENSE` & `pytest-persistence-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.7/pytest_persistence/XDistScheduling.py` & `pytest-persistence-0.1.8/pytest_persistence/XDistScheduling.py`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.7/pytest_persistence/plugin.py` & `pytest-persistence-0.1.8/pytest_persistence/plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -162,14 +162,61 @@
         self.output["tests"].update({node_id: worker_id})
 
     @pytest.hookimpl(trylast=True)
     def pytest_xdist_make_scheduler(self, config, log):
         if (test_order := self.input.get("tests")) is not None:
             return XDistScheduling(config, log, test_order)
 
+    @pytest.hookimpl(tryfirst=True)
+    def pytest_runtest_teardown(self, item, nextitem):
+        """Cleanup skipping
+
+        persistence functionality requires skip of cleanup during store obviously.
+        Otherwise fixtures would be invalid during load when the fixture does
+        something externally.
+
+        There doesn't seem to be an interface access finlaizers, non-public API is
+        in use. setupstate.stack is used to access finalizers.
+
+        Structure of setupstate.stack is documented in SetupState class in pytest.
+        It's dict of tuples.
+
+        stack == {
+            Node: (
+                [*finalizers],
+                exception
+            )
+        }
+
+        Besides clearing setupstate.stack also cached_result must be cleared and I
+        forgot why. Access to fixture is possible via closure.
+        """
+        needed = nextitem.listchain() if nextitem else []
+        # public api unknown
+        # pylint: disable=protected-access
+        stack = item.session._setupstate.stack
+
+        def fixtures(finalizers):
+            """Mine fixturedefs from stack of finalizers"""
+            for fin in finalizers:
+                if not fin.__closure__:
+                    continue
+                for cell in fin.__closure__:
+                    if hasattr(cell.cell_contents, "cached_result"):
+                        yield cell.cell_contents
+
+        for k in list(stack.keys()):
+            if k not in needed:
+                indexes = []
+                for i, v in enumerate(fixtures(stack[k][0])):
+                    v.cached_result = None
+                    indexes.append(i)
+                for i in sorted(indexes, reverse=True):
+                    del stack[k][0][i]
+
 
 def pytest_configure(config):
     """
     Hook ensures that plugin works only when the --load or --store option is present.
     """
     if config.getoption("--load") or config.getoption("--store"):
         config.pluginmanager.register(Plugin())
```

### Comparing `pytest-persistence-0.1.7/setup.py` & `pytest-persistence-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.7/tests/test_plugin.py` & `pytest-persistence-0.1.8/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.7/tests/test_unit.py` & `pytest-persistence-0.1.8/tests/test_unit.py`

 * *Files identical despite different names*

