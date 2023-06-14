# Comparing `tmp/FlaskSimpleAuth-8.0.tar.gz` & `tmp/FlaskSimpleAuth-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlaskSimpleAuth-8.0.tar", last modified: Fri Mar  4 09:05:35 2022, max compression
+gzip compressed data, was "FlaskSimpleAuth-9.0.tar", last modified: Fri Mar  4 19:44:19 2022, max compression
```

## Comparing `FlaskSimpleAuth-8.0.tar` & `FlaskSimpleAuth-9.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwx------   0 fabien    (1001) fabien    (1001)        0 2022-03-04 09:05:35.238813 FlaskSimpleAuth-8.0/
-drwx------   0 fabien    (1001) fabien    (1001)        0 2022-03-04 09:05:35.234813 FlaskSimpleAuth-8.0/FlaskSimpleAuth.egg-info/
--rw-------   0 fabien    (1001) fabien    (1001)    38322 2022-03-04 09:05:35.000000 FlaskSimpleAuth-8.0/FlaskSimpleAuth.egg-info/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)      720 2022-03-04 09:05:35.000000 FlaskSimpleAuth-8.0/FlaskSimpleAuth.egg-info/SOURCES.txt
--rw-------   0 fabien    (1001) fabien    (1001)        1 2022-03-04 09:05:35.000000 FlaskSimpleAuth-8.0/FlaskSimpleAuth.egg-info/dependency_links.txt
--rw-------   0 fabien    (1001) fabien    (1001)       32 2022-03-04 09:05:35.000000 FlaskSimpleAuth-8.0/FlaskSimpleAuth.egg-info/requires.txt
--rw-------   0 fabien    (1001) fabien    (1001)       16 2022-03-04 09:05:35.000000 FlaskSimpleAuth-8.0/FlaskSimpleAuth.egg-info/top_level.txt
--rwx------   0 fabien    (1001) fabien    (1001)    61806 2022-03-02 18:23:09.000000 FlaskSimpleAuth-8.0/FlaskSimpleAuth.py
--rw-------   0 fabien    (1001) fabien    (1001)      114 2021-06-12 05:58:07.000000 FlaskSimpleAuth-8.0/MANIFEST.in
--rw-------   0 fabien    (1001) fabien    (1001)     1321 2022-02-27 12:34:47.000000 FlaskSimpleAuth-8.0/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)    38322 2022-03-04 09:05:35.238813 FlaskSimpleAuth-8.0/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)    30999 2022-03-04 09:04:58.000000 FlaskSimpleAuth-8.0/README.md
-drwx------   0 fabien    (1001) fabien    (1001)        0 2022-03-04 09:05:35.234813 FlaskSimpleAuth-8.0/demo/
--rw-------   0 fabien    (1001) fabien    (1001)     2064 2022-02-27 09:23:18.000000 FlaskSimpleAuth-8.0/demo/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)     7835 2022-02-26 15:01:44.000000 FlaskSimpleAuth-8.0/demo/README.md
--rw-------   0 fabien    (1001) fabien    (1001)      448 2022-02-26 14:53:31.000000 FlaskSimpleAuth-8.0/demo/app-db.conf
--rw-------   0 fabien    (1001) fabien    (1001)      450 2022-02-26 22:15:17.000000 FlaskSimpleAuth-8.0/demo/app-pg.conf
--rw-------   0 fabien    (1001) fabien    (1001)      441 2022-01-26 19:07:23.000000 FlaskSimpleAuth-8.0/demo/app-pg2.conf
--rw-------   0 fabien    (1001) fabien    (1001)     1373 2022-02-26 22:15:28.000000 FlaskSimpleAuth-8.0/demo/app.py
--rw-------   0 fabien    (1001) fabien    (1001)      753 2022-02-12 18:26:49.000000 FlaskSimpleAuth-8.0/demo/auth.py
--rw-------   0 fabien    (1001) fabien    (1001)      298 2022-02-27 10:40:10.000000 FlaskSimpleAuth-8.0/demo/create-db.sql
--rw-------   0 fabien    (1001) fabien    (1001)      296 2022-02-26 09:01:05.000000 FlaskSimpleAuth-8.0/demo/create-pg.sql
--rw-------   0 fabien    (1001) fabien    (1001)       68 2021-06-05 15:15:52.000000 FlaskSimpleAuth-8.0/demo/data.sql
--rw-------   0 fabien    (1001) fabien    (1001)      590 2022-03-02 07:55:52.000000 FlaskSimpleAuth-8.0/demo/database.py
--rwx------   0 fabien    (1001) fabien    (1001)      657 2022-02-27 09:30:18.000000 FlaskSimpleAuth-8.0/demo/pass.py
--rw-------   0 fabien    (1001) fabien    (1001)     1172 2022-02-27 07:54:12.000000 FlaskSimpleAuth-8.0/demo/queries.sql
--rw-------   0 fabien    (1001) fabien    (1001)     1652 2022-02-27 08:16:54.000000 FlaskSimpleAuth-8.0/demo/scare.py
--rw-------   0 fabien    (1001) fabien    (1001)     1275 2022-02-26 08:18:17.000000 FlaskSimpleAuth-8.0/demo/stuff.py
--rw-------   0 fabien    (1001) fabien    (1001)     8100 2022-02-27 08:17:49.000000 FlaskSimpleAuth-8.0/demo/test_demo.py
--rw-------   0 fabien    (1001) fabien    (1001)      375 2022-02-27 08:13:51.000000 FlaskSimpleAuth-8.0/demo/types_path.py
--rw-------   0 fabien    (1001) fabien    (1001)     1831 2022-02-27 08:18:08.000000 FlaskSimpleAuth-8.0/demo/users.py
--rw-------   0 fabien    (1001) fabien    (1001)      785 2022-03-04 09:05:35.238813 FlaskSimpleAuth-8.0/setup.cfg
--rw-------   0 fabien    (1001) fabien    (1001)       89 2021-02-24 19:39:37.000000 FlaskSimpleAuth-8.0/setup.py
-drwx------   0 fabien    (1001) fabien    (1001)        0 2022-03-04 09:05:35.238813 FlaskSimpleAuth-8.0/test/
--rw-------   0 fabien    (1001) fabien    (1001)     9360 2022-02-13 14:24:10.000000 FlaskSimpleAuth-8.0/test/App.py
--rw-------   0 fabien    (1001) fabien    (1001)     1897 2022-01-21 19:27:19.000000 FlaskSimpleAuth-8.0/test/AppBad.py
--rw-------   0 fabien    (1001) fabien    (1001)     1181 2022-02-13 14:23:43.000000 FlaskSimpleAuth-8.0/test/AppExt.py
--rw-------   0 fabien    (1001) fabien    (1001)     1573 2022-02-13 14:23:57.000000 FlaskSimpleAuth-8.0/test/AppFact.py
--rw-------   0 fabien    (1001) fabien    (1001)     1074 2021-04-16 11:35:28.000000 FlaskSimpleAuth-8.0/test/AppHttpAuth.py
--rw-------   0 fabien    (1001) fabien    (1001)      582 2022-01-24 14:24:26.000000 FlaskSimpleAuth-8.0/test/Auth.py
--rw-------   0 fabien    (1001) fabien    (1001)      752 2022-02-27 12:34:05.000000 FlaskSimpleAuth-8.0/test/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)      376 2021-03-22 18:55:18.000000 FlaskSimpleAuth-8.0/test/Shared.py
--rw-------   0 fabien    (1001) fabien    (1001)      512 2022-01-20 10:02:15.000000 FlaskSimpleAuth-8.0/test/SubApp.py
--rw-------   0 fabien    (1001) fabien    (1001)      209 2021-03-28 16:14:06.000000 FlaskSimpleAuth-8.0/test/digest_auth.py
--rw-------   0 fabien    (1001) fabien    (1001)    51620 2022-03-02 12:26:12.000000 FlaskSimpleAuth-8.0/test/test_flask.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2022-03-04 19:44:19.112854 FlaskSimpleAuth-9.0/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2022-03-04 19:44:19.108854 FlaskSimpleAuth-9.0/FlaskSimpleAuth.egg-info/
+-rw-------   0 fabien    (1001) fabien    (1001)    38322 2022-03-04 19:44:19.000000 FlaskSimpleAuth-9.0/FlaskSimpleAuth.egg-info/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)      735 2022-03-04 19:44:19.000000 FlaskSimpleAuth-9.0/FlaskSimpleAuth.egg-info/SOURCES.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        1 2022-03-04 19:44:19.000000 FlaskSimpleAuth-9.0/FlaskSimpleAuth.egg-info/dependency_links.txt
+-rw-------   0 fabien    (1001) fabien    (1001)       32 2022-03-04 19:44:19.000000 FlaskSimpleAuth-9.0/FlaskSimpleAuth.egg-info/requires.txt
+-rw-------   0 fabien    (1001) fabien    (1001)       16 2022-03-04 19:44:19.000000 FlaskSimpleAuth-9.0/FlaskSimpleAuth.egg-info/top_level.txt
+-rwx------   0 fabien    (1001) fabien    (1001)    62153 2022-03-04 19:42:17.000000 FlaskSimpleAuth-9.0/FlaskSimpleAuth.py
+-rw-------   0 fabien    (1001) fabien    (1001)      114 2021-06-12 05:58:07.000000 FlaskSimpleAuth-9.0/MANIFEST.in
+-rw-------   0 fabien    (1001) fabien    (1001)     1321 2022-02-27 12:34:47.000000 FlaskSimpleAuth-9.0/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)    38322 2022-03-04 19:44:19.112854 FlaskSimpleAuth-9.0/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)    30999 2022-03-04 19:42:17.000000 FlaskSimpleAuth-9.0/README.md
+drwx------   0 fabien    (1001) fabien    (1001)        0 2022-03-04 19:44:19.112854 FlaskSimpleAuth-9.0/demo/
+-rw-------   0 fabien    (1001) fabien    (1001)     2064 2022-02-27 09:23:18.000000 FlaskSimpleAuth-9.0/demo/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     7835 2022-02-26 15:01:44.000000 FlaskSimpleAuth-9.0/demo/README.md
+-rw-------   0 fabien    (1001) fabien    (1001)      448 2022-02-26 14:53:31.000000 FlaskSimpleAuth-9.0/demo/app-db.conf
+-rw-------   0 fabien    (1001) fabien    (1001)      450 2022-02-26 22:15:17.000000 FlaskSimpleAuth-9.0/demo/app-pg.conf
+-rw-------   0 fabien    (1001) fabien    (1001)      441 2022-01-26 19:07:23.000000 FlaskSimpleAuth-9.0/demo/app-pg2.conf
+-rw-------   0 fabien    (1001) fabien    (1001)     1373 2022-02-26 22:15:28.000000 FlaskSimpleAuth-9.0/demo/app.py
+-rw-------   0 fabien    (1001) fabien    (1001)      753 2022-02-12 18:26:49.000000 FlaskSimpleAuth-9.0/demo/auth.py
+-rw-------   0 fabien    (1001) fabien    (1001)      298 2022-02-27 10:40:10.000000 FlaskSimpleAuth-9.0/demo/create-db.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      296 2022-02-26 09:01:05.000000 FlaskSimpleAuth-9.0/demo/create-pg.sql
+-rw-------   0 fabien    (1001) fabien    (1001)       68 2021-06-05 15:15:52.000000 FlaskSimpleAuth-9.0/demo/data.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      590 2022-03-02 07:55:52.000000 FlaskSimpleAuth-9.0/demo/database.py
+-rwx------   0 fabien    (1001) fabien    (1001)      657 2022-02-27 09:30:18.000000 FlaskSimpleAuth-9.0/demo/pass.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1172 2022-02-27 07:54:12.000000 FlaskSimpleAuth-9.0/demo/queries.sql
+-rw-------   0 fabien    (1001) fabien    (1001)     1652 2022-02-27 08:16:54.000000 FlaskSimpleAuth-9.0/demo/scare.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1275 2022-02-26 08:18:17.000000 FlaskSimpleAuth-9.0/demo/stuff.py
+-rw-------   0 fabien    (1001) fabien    (1001)     8100 2022-02-27 08:17:49.000000 FlaskSimpleAuth-9.0/demo/test_demo.py
+-rw-------   0 fabien    (1001) fabien    (1001)      375 2022-02-27 08:13:51.000000 FlaskSimpleAuth-9.0/demo/types_path.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1831 2022-02-27 08:18:08.000000 FlaskSimpleAuth-9.0/demo/users.py
+-rw-------   0 fabien    (1001) fabien    (1001)      250 2022-03-04 19:43:35.000000 FlaskSimpleAuth-9.0/demo/users.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      785 2022-03-04 19:44:19.112854 FlaskSimpleAuth-9.0/setup.cfg
+-rw-------   0 fabien    (1001) fabien    (1001)       89 2021-02-24 19:39:37.000000 FlaskSimpleAuth-9.0/setup.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2022-03-04 19:44:19.112854 FlaskSimpleAuth-9.0/test/
+-rw-------   0 fabien    (1001) fabien    (1001)     9360 2022-02-13 14:24:10.000000 FlaskSimpleAuth-9.0/test/App.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1897 2022-01-21 19:27:19.000000 FlaskSimpleAuth-9.0/test/AppBad.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1181 2022-02-13 14:23:43.000000 FlaskSimpleAuth-9.0/test/AppExt.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1573 2022-02-13 14:23:57.000000 FlaskSimpleAuth-9.0/test/AppFact.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1074 2021-04-16 11:35:28.000000 FlaskSimpleAuth-9.0/test/AppHttpAuth.py
+-rw-------   0 fabien    (1001) fabien    (1001)      582 2022-01-24 14:24:26.000000 FlaskSimpleAuth-9.0/test/Auth.py
+-rw-------   0 fabien    (1001) fabien    (1001)      752 2022-02-27 12:34:05.000000 FlaskSimpleAuth-9.0/test/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)      376 2021-03-22 18:55:18.000000 FlaskSimpleAuth-9.0/test/Shared.py
+-rw-------   0 fabien    (1001) fabien    (1001)      512 2022-01-20 10:02:15.000000 FlaskSimpleAuth-9.0/test/SubApp.py
+-rw-------   0 fabien    (1001) fabien    (1001)      209 2021-03-28 16:14:06.000000 FlaskSimpleAuth-9.0/test/digest_auth.py
+-rw-------   0 fabien    (1001) fabien    (1001)    52017 2022-03-04 19:42:17.000000 FlaskSimpleAuth-9.0/test/test_flask.py
```

### Comparing `FlaskSimpleAuth-8.0/FlaskSimpleAuth.egg-info/PKG-INFO` & `FlaskSimpleAuth-9.0/FlaskSimpleAuth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlaskSimpleAuth
-Version: 8.0
+Version: 9.0
 Summary: Simple authentication, authorization and parameters for Flask, emphasizing configurability
 Home-page: https://github.com/zx80/flask-simple-auth
 Author: Fabien Coelho
 Author-email: flask.auth@coelho.net
 License: UNKNOWN
 Description: # Flask Simple Auth
         
@@ -806,15 +806,15 @@
         
         
         ## Versions
         
         Sources are available on [GitHub](https://github.com/zx80/flask-simple-auth)
         and packaged on [PyPI](https://pypi.org/project/FlaskSimpleAuth/).
         
-        Latest version is *8.0* published on 2022-03-04.
+        Latest version is *9.0* published on 2022-03-04.
         Initial version was *0.9.0* on 2021-02-21.
         
         See [all versions](VERSIONS.md).
         
         
         ## TODO
```

### Comparing `FlaskSimpleAuth-8.0/FlaskSimpleAuth.egg-info/SOURCES.txt` & `FlaskSimpleAuth-9.0/FlaskSimpleAuth.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 demo/pass.py
 demo/queries.sql
 demo/scare.py
 demo/stuff.py
 demo/test_demo.py
 demo/types_path.py
 demo/users.py
+demo/users.sql
 test/App.py
 test/AppBad.py
 test/AppExt.py
 test/AppFact.py
 test/AppHttpAuth.py
 test/Auth.py
 test/Makefile
```

### Comparing `FlaskSimpleAuth-8.0/FlaskSimpleAuth.py` & `FlaskSimpleAuth-9.0/FlaskSimpleAuth.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,40 +105,46 @@
     def __init__(self, obj: Any = None, set_name: str = "set", fun: Optional[Callable] = None):
         """Constructor parameters:
 
         - set_name: provide another prefix for the "set" functions.
         - obj: object to be wrapped, can also be provided later.
         - fun: function to generated a per-thread wrapped object.
         """
-        if obj and fun:
-            raise Exception("reference cannot have both obj and fun")
-        elif obj:
-            self._set_obj(obj)
-        elif fun:
-            self._set_fun(fun)
-        if set_name:
-            setattr(self, set_name, getattr(self, "_set_obj"))
+        self._set(obj=obj, fun=fun, mandatory=False)
+        if set_name and set_name != "_set":
+            setattr(self, set_name, getattr(self, "_set"))
             setattr(self, set_name + "_obj", getattr(self, "_set_obj"))
             setattr(self, set_name + "_fun", getattr(self, "_set_fun"))
 
     def _set_obj(self, obj):
         """Set current wrapped object."""
         log.debug(f"setting reference to {obj} ({type(obj)})")
         self._fun = None
         self._nthreads = 1
         self._local = self.Local()
         self._local.obj = obj
-        return obj
+        return self
 
     def _set_fun(self, fun: Callable[[int], Any]):
         """Set current wrapped object generation function."""
         self._fun = fun
         self._nthreads = 0
         self._local = threading.local()
-        pass
+        return self
+
+    def _set(self, obj: Any = None, fun: Optional[Callable[[int], Any]] = None, mandatory=True):
+        """Set current wrapped object or generation function."""
+        if obj and fun:
+            raise Exception("reference cannot set both obj and fun")
+        elif obj:
+            return self._set_obj(obj)
+        elif fun:
+            return self._set_fun(fun)
+        elif mandatory:
+            raise Exception("reference must set either obj or fun")
 
     def _get_obj(self):
         """Get current wrapped object."""
         if self._fun and not hasattr(self._local, "obj"):
             self._local.obj = self._fun(self._nthreads)
             self._nthreads += 1
         return self._local.obj
@@ -403,15 +409,15 @@
         """Add a cast function to a type."""
         if t in self._casts:
             log.warning(f"overriding type casting function for {t}")
         if cast:  # direct
             self._casts[t] = cast
         else:  # decorator
             def annotate(fun):
-                self._casts[t] = cast
+                self._casts[t] = fun
                 return fun
             return annotate
 
     def object_perms(self, domain, checker: Optional[Callable] = None):
         """Add an object permission helper for a domain."""
         if domain in self._object_perms:
             log.warning(f"overriding object permission checker for domain {domain}")
```

### Comparing `FlaskSimpleAuth-8.0/Makefile` & `FlaskSimpleAuth-9.0/Makefile`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/PKG-INFO` & `FlaskSimpleAuth-9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlaskSimpleAuth
-Version: 8.0
+Version: 9.0
 Summary: Simple authentication, authorization and parameters for Flask, emphasizing configurability
 Home-page: https://github.com/zx80/flask-simple-auth
 Author: Fabien Coelho
 Author-email: flask.auth@coelho.net
 License: UNKNOWN
 Description: # Flask Simple Auth
         
@@ -806,15 +806,15 @@
         
         
         ## Versions
         
         Sources are available on [GitHub](https://github.com/zx80/flask-simple-auth)
         and packaged on [PyPI](https://pypi.org/project/FlaskSimpleAuth/).
         
-        Latest version is *8.0* published on 2022-03-04.
+        Latest version is *9.0* published on 2022-03-04.
         Initial version was *0.9.0* on 2021-02-21.
         
         See [all versions](VERSIONS.md).
         
         
         ## TODO
```

### Comparing `FlaskSimpleAuth-8.0/README.md` & `FlaskSimpleAuth-9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -798,15 +798,15 @@
 
 
 ## Versions
 
 Sources are available on [GitHub](https://github.com/zx80/flask-simple-auth)
 and packaged on [PyPI](https://pypi.org/project/FlaskSimpleAuth/).
 
-Latest version is *8.0* published on 2022-03-04.
+Latest version is *9.0* published on 2022-03-04.
 Initial version was *0.9.0* on 2021-02-21.
 
 See [all versions](VERSIONS.md).
 
 
 ## TODO
```

### Comparing `FlaskSimpleAuth-8.0/demo/Makefile` & `FlaskSimpleAuth-9.0/demo/Makefile`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/demo/README.md` & `FlaskSimpleAuth-9.0/demo/README.md`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/demo/app.py` & `FlaskSimpleAuth-9.0/demo/app.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/demo/auth.py` & `FlaskSimpleAuth-9.0/demo/auth.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/demo/database.py` & `FlaskSimpleAuth-9.0/demo/database.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/demo/pass.py` & `FlaskSimpleAuth-9.0/demo/pass.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/demo/queries.sql` & `FlaskSimpleAuth-9.0/demo/queries.sql`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/demo/scare.py` & `FlaskSimpleAuth-9.0/demo/scare.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/demo/stuff.py` & `FlaskSimpleAuth-9.0/demo/stuff.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/demo/test_demo.py` & `FlaskSimpleAuth-9.0/demo/test_demo.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/demo/users.py` & `FlaskSimpleAuth-9.0/demo/users.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/setup.cfg` & `FlaskSimpleAuth-9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FlaskSimpleAuth
-version = 8.0
+version = 9.0
 author = Fabien Coelho
 author_email = flask.auth@coelho.net
 url = https://github.com/zx80/flask-simple-auth
 description = Simple authentication, authorization and parameters for Flask, emphasizing configurability
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `FlaskSimpleAuth-8.0/test/App.py` & `FlaskSimpleAuth-9.0/test/App.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/test/AppBad.py` & `FlaskSimpleAuth-9.0/test/AppBad.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/test/AppExt.py` & `FlaskSimpleAuth-9.0/test/AppExt.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/test/AppFact.py` & `FlaskSimpleAuth-9.0/test/AppFact.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/test/AppHttpAuth.py` & `FlaskSimpleAuth-9.0/test/AppHttpAuth.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/test/Auth.py` & `FlaskSimpleAuth-9.0/test/Auth.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/test/Makefile` & `FlaskSimpleAuth-9.0/test/Makefile`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/test/SubApp.py` & `FlaskSimpleAuth-9.0/test/SubApp.py`

 * *Files identical despite different names*

### Comparing `FlaskSimpleAuth-8.0/test/test_flask.py` & `FlaskSimpleAuth-9.0/test/test_flask.py`

 * *Files 0% similar despite different names*

```diff
@@ -687,15 +687,22 @@
     # local one is still ok
     assert r == "data: 0"
     # error
     try:
         r = fsa.Reference(obj="hello", fun=gen_data)
         assert False, "should have raised an exception"
     except Exception as e:
-        assert "reference cannot have both obj and fun" in str(e)
+        assert "reference cannot set both obj and fun" in str(e)
+    try:
+        r = fsa.Reference(set_name="add")
+        r.add()
+        assert False, "missing parameter in previous call"
+    except Exception as e:
+        assert "reference must set either obj or fun" in str(e)
+
 
 def test_www_authenticate(client):
     push_auth(app._fsa, "param")
     res = check(401, client.get("/admin"))
     pop_auth(app._fsa)
     push_auth(app._fsa, "basic")
     res = check(401, client.get("/admin"))
@@ -1212,15 +1219,19 @@
         assert False, "should not get through"
     except fsa.FSAException as e:
         assert e.status == 500 and "internal error with get_user_pass" in e.message
     # overwrite warning
     @app.cast("foo")
     def cast_foo(s: str):
         return s
-    app.cast("foo", cast_foo)
+    assert app._fsa._casts["foo"] == cast_foo
+    app.cast("foo", lambda x: cast_foo(x))
+    assert app._fsa._casts["foo"] != cast_foo
+    s = "Hello World!"
+    assert app._fsa._casts["foo"](s) == cast_foo(s)
     # type errors
     try:
         app = af.create_app(FSA_CAST="not a dict")
         assert False, "should not get through"
     except Exception as e:
         assert "FSA_CAST must be a dict" in str(e)
     try:
```

