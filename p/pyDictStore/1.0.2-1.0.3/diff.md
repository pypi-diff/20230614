# Comparing `tmp/pyDictStore-1.0.2.tar.gz` & `tmp/pyDictStore-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDictStore-1.0.2.tar", last modified: Sat Jun  3 01:15:02 2023, max compression
+gzip compressed data, was "pyDictStore-1.0.3.tar", last modified: Wed Jun 14 01:26:25 2023, max compression
```

## Comparing `pyDictStore-1.0.2.tar` & `pyDictStore-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 01:15:02.145612 pyDictStore-1.0.2/
--rw-rw-rw-   0        0        0     1090 2022-05-31 23:42:26.000000 pyDictStore-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4494 2023-06-03 01:15:02.143663 pyDictStore-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3654 2022-08-06 00:15:10.000000 pyDictStore-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 01:15:02.145612 pyDictStore-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2158 2023-06-02 18:25:43.000000 pyDictStore-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:15:02.089964 pyDictStore-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 01:15:02.112420 pyDictStore-1.0.2/src/pyDictStore/
--rw-rw-rw-   0        0        0     2794 2023-06-03 01:13:50.000000 pyDictStore-1.0.2/src/pyDictStore/__decorators__.py
--rw-rw-rw-   0        0        0      974 2022-06-05 20:49:49.000000 pyDictStore-1.0.2/src/pyDictStore/__events__.py
--rw-rw-rw-   0        0        0      545 2023-06-03 01:14:15.000000 pyDictStore-1.0.2/src/pyDictStore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:15:02.141708 pyDictStore-1.0.2/src/pyDictStore.egg-info/
--rw-rw-rw-   0        0        0     4494 2023-06-03 01:15:01.000000 pyDictStore-1.0.2/src/pyDictStore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-06-03 01:15:01.000000 pyDictStore-1.0.2/src/pyDictStore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 01:15:01.000000 pyDictStore-1.0.2/src/pyDictStore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-03 01:15:01.000000 pyDictStore-1.0.2/src/pyDictStore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 01:26:25.325569 pyDictStore-1.0.3/
+-rw-rw-rw-   0        0        0     1090 2022-05-31 23:42:26.000000 pyDictStore-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4494 2023-06-14 01:26:25.323572 pyDictStore-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3654 2022-08-06 00:15:10.000000 pyDictStore-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 01:26:25.326568 pyDictStore-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2158 2023-06-02 18:25:43.000000 pyDictStore-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:26:25.285592 pyDictStore-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:26:25.297584 pyDictStore-1.0.3/src/pyDictStore/
+-rw-rw-rw-   0        0        0     4193 2023-06-14 01:24:21.000000 pyDictStore-1.0.3/src/pyDictStore/__decorators__.py
+-rw-rw-rw-   0        0        0      974 2022-06-05 20:49:49.000000 pyDictStore-1.0.3/src/pyDictStore/__events__.py
+-rw-rw-rw-   0        0        0      545 2023-06-14 01:26:10.000000 pyDictStore-1.0.3/src/pyDictStore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:26:25.322573 pyDictStore-1.0.3/src/pyDictStore.egg-info/
+-rw-rw-rw-   0        0        0     4494 2023-06-14 01:26:25.000000 pyDictStore-1.0.3/src/pyDictStore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-06-14 01:26:25.000000 pyDictStore-1.0.3/src/pyDictStore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 01:26:25.000000 pyDictStore-1.0.3/src/pyDictStore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-14 01:26:25.000000 pyDictStore-1.0.3/src/pyDictStore.egg-info/top_level.txt
```

### Comparing `pyDictStore-1.0.2/LICENSE` & `pyDictStore-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.2/PKG-INFO` & `pyDictStore-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDictStore
-Version: 1.0.2
+Version: 1.0.3
 Summary: pyDictStore adds automated dictionary storage to properties eliminating the need for code bodies, property getters and setters. It also provides a property change event.
 Home-page: https://OpenWayside.org
 Author: Peter Varney, OpenWayside
 Author-email: pyDictStore@OpenWayside.org
 License: UNKNOWN
 Project-URL: Documentation, https://openwayside.org/rtm/pyDictStore/
 Project-URL: Source, https://github.com/OpenWayside/pyDictStore
```

### Comparing `pyDictStore-1.0.2/README.md` & `pyDictStore-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.2/setup.py` & `pyDictStore-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.2/src/pyDictStore/__decorators__.py` & `pyDictStore-1.0.3/src/pyDictStore/__decorators__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,63 @@
 from .__events__ import PropertyChangedEvent
-class storage:
-    def __init__(self, cls) -> None:
-        self.cls = cls
+#from functools import wraps
+import functools
 
-    def __call__(self, *args, **kwargs):
-        # #Add storage variable to the object instance
-        def decorate(fcn):
-            def __new__(cls,*args, **kwargs):
-                oCls = super(type(cls), cls).__new__(cls)
-                oCls.__storage__ = {}
-                cls.PropertyChanged = PropertyChangedEvent()
-                from typing import cast
-                return cast(type(cls),oCls)
-            return __new__
-        self.cls.__new__ = decorate(self.cls.__new__)
-        #Add storageSet and default(none) to properties if not already present
-        for name in [p for p in dir(self.cls) if isinstance(getattr(self.cls,p),property)]:
-            prop = getattr(self.cls,name)
-            fget = (prop.fget 
-                    if prop.fget.__qualname__ == 'default.__call__.<locals>.wrapper'
-                    else default(None)(prop.fget)
-                    )
-            fset = (prop.fset 
-                    #if prop.fset.__qualname__ == 'storageSetter.<locals>.wrapper'
-                    if isinstance(prop.fset,storageSetter)
-                    else storageSetter(prop.fset)
-                    )
-            setattr(self.cls, name, property(fget, fset, prop.fdel))  
-        return self.cls(*args,**kwargs)
+
+def storage(cls):
+    @functools.wraps(cls, updated=())
+    class storage_wrap(cls):
+        def __init__(self, *args, **kwargs) -> None:
+            self.wrapper = cls
+            self.wrapper.__storage__ = {}
+            self.wrapper.PropertyChanged = PropertyChangedEvent()
+            #Add storageSet and default(none) to properties if not already present
+            for name in [p for p in dir(self.wrapper) if isinstance(getattr(self.wrapper,p),property)]:
+                prop = getattr(self.wrapper,name)
+                fget = (prop.fget 
+                        if prop.fget.__qualname__ == 'default.__call__.<locals>.wrapper'
+                        else default(None)(prop.fget)
+                        )
+                fset = (prop.fset 
+                        #if prop.fset.__qualname__ == 'storageSetter.<locals>.wrapper'
+                        if isinstance(prop.fset,storageSetter)
+                        else storageSetter(prop.fset)
+                        )
+                setattr(self.wrapper, name, property(fget, fset, prop.fdel))
+            #Call Wrapped Class' initilizer
+            super().__init__(*args,**kwargs)
+            
+            
+
+        # def __call__(self, *args, **kwargs):
+        #     # #Add storage variable to the object instance
+        #     def decorate(fcn):
+        #         def __new__(wrapper,*args, **kwargs):
+        #             oCls = super(type(wrapper), wrapper).__new__(wrapper)
+        #             oCls.__storage__ = {}
+        #             wrapper.PropertyChanged = PropertyChangedEvent()
+        #             from typing import cast
+        #             return cast(type(wrapper),oCls)
+        #         return __new__
+        #     self.wrapper.__new__ = decorate(self.wrapper.__new__)
+        #     #Add storageSet and default(none) to properties if not already present
+        #     for name in [p for p in dir(self.wrapper) if isinstance(getattr(self.wrapper,p),property)]:
+        #         prop = getattr(self.wrapper,name)
+        #         fget = (prop.fget 
+        #                 if prop.fget.__qualname__ == 'default.__call__.<locals>.wrapper'
+        #                 else default(None)(prop.fget)
+        #                 )
+        #         fset = (prop.fset 
+        #                 #if prop.fset.__qualname__ == 'storageSetter.<locals>.wrapper'
+        #                 if isinstance(prop.fset,storageSetter)
+        #                 else storageSetter(prop.fset)
+        #                 )
+        #         setattr(self.wrapper, name, property(fget, fset, prop.fdel)) 
+        #     return self.wrapper(*args,**kwargs)
+    return storage_wrap
 
 class default:
     def __init__(self, value=None) -> None:
         self.value = value
 
     def __call__(self, function):
         def wrapper(*args, **kwargs):
```

### Comparing `pyDictStore-1.0.2/src/pyDictStore/__events__.py` & `pyDictStore-1.0.3/src/pyDictStore/__events__.py`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.2/src/pyDictStore/__init__.py` & `pyDictStore-1.0.3/src/pyDictStore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 .. include:: ../../README.md
 
 # Library functions
 '''
 
 __PROJECT__ = 'pyDictStore'
-__VERSION__ = '1.0.2'
+__VERSION__ = '1.0.3'
 
 from .__decorators__ import default, storageSetter, storage
 
 def isDefault(obj:object,prop:str) -> bool:
     '''
     Checks if an objects property is equal to its default value
     '''
```

### Comparing `pyDictStore-1.0.2/src/pyDictStore.egg-info/PKG-INFO` & `pyDictStore-1.0.3/src/pyDictStore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDictStore
-Version: 1.0.2
+Version: 1.0.3
 Summary: pyDictStore adds automated dictionary storage to properties eliminating the need for code bodies, property getters and setters. It also provides a property change event.
 Home-page: https://OpenWayside.org
 Author: Peter Varney, OpenWayside
 Author-email: pyDictStore@OpenWayside.org
 License: UNKNOWN
 Project-URL: Documentation, https://openwayside.org/rtm/pyDictStore/
 Project-URL: Source, https://github.com/OpenWayside/pyDictStore
```

