# Comparing `tmp/objtyping-0.5.3.tar.gz` & `tmp/objtyping-0.5.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objtyping-0.5.3.tar", last modified: Wed Feb  8 11:58:20 2023, max compression
+gzip compressed data, was "objtyping-0.5.3.post2.tar", last modified: Wed Jun 14 03:10:46 2023, max compression
```

## Comparing `objtyping-0.5.3.tar` & `objtyping-0.5.3.post2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 11:58:20.767006 objtyping-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-08 11:58:06.000000 objtyping-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-02-08 11:58:20.767006 objtyping-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-02-08 11:58:06.000000 objtyping-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 11:58:20.763006 objtyping-0.5.3/objtyping/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-08 11:58:06.000000 objtyping-0.5.3/objtyping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-02-08 11:58:06.000000 objtyping-0.5.3/objtyping/objtyping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 11:58:20.763006 objtyping-0.5.3/objtyping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-02-08 11:58:20.000000 objtyping-0.5.3/objtyping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-08 11:58:20.000000 objtyping-0.5.3/objtyping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 11:58:20.000000 objtyping-0.5.3/objtyping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-08 11:58:20.000000 objtyping-0.5.3/objtyping.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-08 11:58:06.000000 objtyping-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 11:58:20.767006 objtyping-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-02-08 11:58:06.000000 objtyping-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 11:58:20.767006 objtyping-0.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-08 11:58:06.000000 objtyping-0.5.3/test/test_objtyping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/objtyping/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/objtyping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/objtyping/objtyping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/objtyping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-14 03:10:46.000000 objtyping-0.5.3.post2/objtyping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-14 03:10:46.000000 objtyping-0.5.3.post2/objtyping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:10:46.000000 objtyping-0.5.3.post2/objtyping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 03:10:46.000000 objtyping-0.5.3.post2/objtyping.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/test/test_objtyping.py
```

### Comparing `objtyping-0.5.3/LICENSE` & `objtyping-0.5.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `objtyping-0.5.3/PKG-INFO` & `objtyping-0.5.3.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objtyping
-Version: 0.5.3
+Version: 0.5.3.post2
 Summary: convert a primitive dict-list data structure to/from an instance of user-defined class.
 Author: Song Hui
 Author-email: songofhawk@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `objtyping-0.5.3/README.md` & `objtyping-0.5.3.post2/README.md`

 * *Files identical despite different names*

### Comparing `objtyping-0.5.3/objtyping/objtyping.py` & `objtyping-0.5.3.post2/objtyping/objtyping.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,50 +148,58 @@
         return False
 
 
 class Primitiver:
     DEFAULT_DATE_TIME_FORMAT = '%Y-%m-%d %H:%M:%S'
     DEFAULT_DATE_FORMAT = '%Y-%m-%d'
 
-    max_depth = 6
+    max_depth = 100  # 最大深度，超过最大深度的数据，会返回null，实际调用的时候，这个值会被 to_primitive 函数给定的 max_depth 参数覆盖
     ignore_protected = True
     format_datetime = True
     ignores = None
 
     def __init__(self, root):
         """
         :param root: 要转换的对象，通常是一个类实例
         """
         self.root = root
         self.all_objs = set()
         self.ignores = []
 
     def convert(self):
-        objtype = type(self.root)
+        if self._is_sqlalchemy_query(self.root):
+            return None
+        return self._convert(self.root, 0, set())
+
+    @staticmethod
+    def _is_sqlalchemy_query(obj):
+        objtype = type(obj)
         if objtype.__name__ == 'BaseQuery' and objtype.__module__ and objtype.__module__.find('sqlalchemy') >= 0:
             # SqlAlchemy 的 BaseQuery 对象，承载了太多属性，特别是在一个复杂项目中，还可能关联到 celery 对象，读取时会加锁，性能很差；
             # 而且调用端大概率不是真的想转换这个对象，而是想转换查询结果
-            print('It seems you give a SqlAlchemy Query object to convert, which is not supported now.'
+            print(f'It seems you give a SqlAlchemy Query object to convert, which is not supported now.'
                   'Do you want a query result object instead?')
-            return None
-
-        return self._convert(self.root, 0, set())
+            return True
+        else:
+            return False
 
     def _convert(self, obj:Any, depth:int, objs_chain:Set):
         """
         把指定的对象，转换成dict-list结构
         :param obj: 要转换的对象，通常是一个类实例
         :param depth:
         :return: 一个dict-list嵌套的结构，可用于序列化
         """
         try:
             if obj is None or depth > self.max_depth:
                 return None
             if inspect.isfunction(obj) or inspect.ismethod(obj):
                 return None
+            if self._is_sqlalchemy_query(obj):
+                return None
 
             if not is_basic_type(obj) and id(obj) in objs_chain:
                 return f'$$recursive reference:{str(obj)}$$'
             else:
                 objs_chain.add(id(obj))
 
             if isinstance(obj, list) or isinstance(obj, tuple) or isinstance(obj, set):
@@ -233,14 +241,14 @@
                     # 其他类型直接转为字符串
                     return str(obj)
         except Exception as e:
             print(f'convert "{type(obj)}" to primitive error:{e}')
             return None
 
 
-def to_primitive(obj, max_depth=10, ignore_protected=True, format_date_time=True, ignores=None):
+def to_primitive(obj, max_depth=20, ignore_protected=True, format_date_time=True, ignores=None):
     pri = Primitiver(obj)
     pri.max_depth = max_depth
     pri.ignore_protected = ignore_protected
     pri.format_datetime = format_date_time
     pri.ignores = [] if ignores is None else ignores
     return pri.convert()
```

### Comparing `objtyping-0.5.3/objtyping.egg-info/PKG-INFO` & `objtyping-0.5.3.post2/objtyping.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objtyping
-Version: 0.5.3
+Version: 0.5.3.post2
 Summary: convert a primitive dict-list data structure to/from an instance of user-defined class.
 Author: Song Hui
 Author-email: songofhawk@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `objtyping-0.5.3/setup.py` & `objtyping-0.5.3.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="objtyping",
 
     # version of the module
-    version="0.5.3",
+    version="0.5.3.r2",
 
     # Name of Author
     author="Song Hui",
 
     # your Email address
     author_email="songofhawk@gmail.com",
```

### Comparing `objtyping-0.5.3/test/test_objtyping.py` & `objtyping-0.5.3.post2/test/test_objtyping.py`

 * *Files identical despite different names*

