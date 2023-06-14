# Comparing `tmp/dbis-functional-dependencies-0.0.5.tar.gz` & `tmp/dbis-functional-dependencies-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-functional-dependencies-0.0.5.tar", last modified: Sat Jun 11 08:35:16 2022, max compression
+gzip compressed data, was "dbis-functional-dependencies-0.0.7.tar", last modified: Sun Jun 12 13:47:41 2022, max compression
```

## Comparing `dbis-functional-dependencies-0.0.5.tar` & `dbis-functional-dependencies-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 wf        (1000) wf        (1000)        0 2022-06-11 08:35:16.375349 dbis-functional-dependencies-0.0.5/
--rw-rw-r--   0 wf        (1000) wf        (1000)     1194 2022-06-11 08:35:16.375349 dbis-functional-dependencies-0.0.5/PKG-INFO
--rw-rw-r--   0 wf        (1000) wf        (1000)      493 2022-06-09 05:01:40.000000 dbis-functional-dependencies-0.0.5/README.md
-drwxrwxr-x   0 wf        (1000) wf        (1000)        0 2022-06-11 08:35:16.367349 dbis-functional-dependencies-0.0.5/dbis_functional_dependencies.egg-info/
--rw-rw-r--   0 wf        (1000) wf        (1000)     1194 2022-06-11 08:35:15.000000 dbis-functional-dependencies-0.0.5/dbis_functional_dependencies.egg-info/PKG-INFO
--rw-rw-r--   0 wf        (1000) wf        (1000)      395 2022-06-11 08:35:16.000000 dbis-functional-dependencies-0.0.5/dbis_functional_dependencies.egg-info/SOURCES.txt
--rw-rw-r--   0 wf        (1000) wf        (1000)        1 2022-06-11 08:35:15.000000 dbis-functional-dependencies-0.0.5/dbis_functional_dependencies.egg-info/dependency_links.txt
--rw-rw-r--   0 wf        (1000) wf        (1000)       24 2022-06-11 08:35:15.000000 dbis-functional-dependencies-0.0.5/dbis_functional_dependencies.egg-info/top_level.txt
-drwxrwxr-x   0 wf        (1000) wf        (1000)        0 2022-06-11 08:35:16.371349 dbis-functional-dependencies-0.0.5/functional_dependencies/
--rw-rw-r--   0 wf        (1000) wf        (1000)    20723 2022-06-11 08:29:08.000000 dbis-functional-dependencies-0.0.5/functional_dependencies/BCNF.py
--rw-rw-r--   0 wf        (1000) wf        (1000)        0 2022-06-04 09:14:59.000000 dbis-functional-dependencies-0.0.5/functional_dependencies/__init__.py
--rw-rw-r--   0 wf        (1000) wf        (1000)     3854 2022-06-11 08:02:47.000000 dbis-functional-dependencies-0.0.5/functional_dependencies/fdcheck.py
--rw-rw-r--   0 wf        (1000) wf        (1000)    23990 2022-06-09 04:33:23.000000 dbis-functional-dependencies-0.0.5/functional_dependencies/fds.py
--rw-rw-r--   0 wf        (1000) wf        (1000)     4693 2022-06-10 06:56:33.000000 dbis-functional-dependencies-0.0.5/functional_dependencies/fdsbase.py
--rw-rw-r--   0 wf        (1000) wf        (1000)       38 2022-06-11 08:35:16.375349 dbis-functional-dependencies-0.0.5/setup.cfg
--rw-rw-r--   0 wf        (1000) wf        (1000)     1157 2022-06-11 08:29:53.000000 dbis-functional-dependencies-0.0.5/setup.py
+drwxr-xr-x   0 wf         (501) staff       (20)        0 2022-06-12 13:47:41.323490 dbis-functional-dependencies-0.0.7/
+-rw-r--r--   0 wf         (501) staff       (20)    11357 2022-06-12 05:40:27.000000 dbis-functional-dependencies-0.0.7/LICENSE
+-rw-r--r--   0 wf         (501) staff       (20)     1129 2022-06-12 13:47:41.323242 dbis-functional-dependencies-0.0.7/PKG-INFO
+-rw-r--r--   0 wf         (501) staff       (20)      493 2022-06-12 05:40:27.000000 dbis-functional-dependencies-0.0.7/README.md
+drwxr-xr-x   0 wf         (501) staff       (20)        0 2022-06-12 13:47:41.320240 dbis-functional-dependencies-0.0.7/dbis_functional_dependencies.egg-info/
+-rw-r--r--   0 wf         (501) staff       (20)     1129 2022-06-12 13:47:40.000000 dbis-functional-dependencies-0.0.7/dbis_functional_dependencies.egg-info/PKG-INFO
+-rw-r--r--   0 wf         (501) staff       (20)      403 2022-06-12 13:47:41.000000 dbis-functional-dependencies-0.0.7/dbis_functional_dependencies.egg-info/SOURCES.txt
+-rw-r--r--   0 wf         (501) staff       (20)        1 2022-06-12 13:47:40.000000 dbis-functional-dependencies-0.0.7/dbis_functional_dependencies.egg-info/dependency_links.txt
+-rw-r--r--   0 wf         (501) staff       (20)       24 2022-06-12 13:47:40.000000 dbis-functional-dependencies-0.0.7/dbis_functional_dependencies.egg-info/top_level.txt
+drwxr-xr-x   0 wf         (501) staff       (20)        0 2022-06-12 13:47:41.322639 dbis-functional-dependencies-0.0.7/functional_dependencies/
+-rw-r--r--   0 wf         (501) staff       (20)    22485 2022-06-12 05:40:27.000000 dbis-functional-dependencies-0.0.7/functional_dependencies/BCNF.py
+-rw-r--r--   0 wf         (501) staff       (20)        0 2022-05-03 09:47:19.000000 dbis-functional-dependencies-0.0.7/functional_dependencies/__init__.py
+-rw-r--r--   0 wf         (501) staff       (20)     3854 2022-06-12 05:40:27.000000 dbis-functional-dependencies-0.0.7/functional_dependencies/fdcheck.py
+-rw-r--r--   0 wf         (501) staff       (20)    23990 2022-06-12 05:40:27.000000 dbis-functional-dependencies-0.0.7/functional_dependencies/fds.py
+-rw-r--r--   0 wf         (501) staff       (20)     5683 2022-06-12 13:44:49.000000 dbis-functional-dependencies-0.0.7/functional_dependencies/fdsbase.py
+-rw-r--r--   0 wf         (501) staff       (20)       38 2022-06-12 13:47:41.323570 dbis-functional-dependencies-0.0.7/setup.cfg
+-rw-r--r--   0 wf         (501) staff       (20)     1157 2022-06-12 13:46:40.000000 dbis-functional-dependencies-0.0.7/setup.py
```

### Comparing `dbis-functional-dependencies-0.0.5/PKG-INFO` & `dbis-functional-dependencies-0.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dbis-functional-dependencies
-Version: 0.0.5
+Version: 0.0.7
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Home-page: https://git.rwth-aachen.de/i5/teaching/dbis-functional-dependencies
 Author: Wolfgang Fahl
 Author-email: fahl@dbis.rwth-aachen.de
 License: Apache
-Description: # dbis-functional-dependencies
-        
-        Functional Dependencies and Normal Forms for Relational Databases
-        
-        [![PyPI Status](https://img.shields.io/pypi/v/dbis-functional-dependencies.svg)](https://pypi.python.org/pypi/dbis-functional-dependencies/)
-        [![pypi](https://img.shields.io/pypi/pyversions/dbis-functional-dependencies)](https://pypi.org/project/dbis-functional-dependencies/)
-        [![License](https://img.shields.io/pypi/l/dbis-functional-dependencies)](https://www.apache.org/licenses/LICENSE-2.0)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dbis-functional-dependencies
+
+Functional Dependencies and Normal Forms for Relational Databases
+
+[![PyPI Status](https://img.shields.io/pypi/v/dbis-functional-dependencies.svg)](https://pypi.python.org/pypi/dbis-functional-dependencies/)
+[![pypi](https://img.shields.io/pypi/pyversions/dbis-functional-dependencies)](https://pypi.org/project/dbis-functional-dependencies/)
+[![License](https://img.shields.io/pypi/l/dbis-functional-dependencies)](https://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `dbis-functional-dependencies-0.0.5/dbis_functional_dependencies.egg-info/PKG-INFO` & `dbis-functional-dependencies-0.0.7/dbis_functional_dependencies.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dbis-functional-dependencies
-Version: 0.0.5
+Version: 0.0.7
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Home-page: https://git.rwth-aachen.de/i5/teaching/dbis-functional-dependencies
 Author: Wolfgang Fahl
 Author-email: fahl@dbis.rwth-aachen.de
 License: Apache
-Description: # dbis-functional-dependencies
-        
-        Functional Dependencies and Normal Forms for Relational Databases
-        
-        [![PyPI Status](https://img.shields.io/pypi/v/dbis-functional-dependencies.svg)](https://pypi.python.org/pypi/dbis-functional-dependencies/)
-        [![pypi](https://img.shields.io/pypi/pyversions/dbis-functional-dependencies)](https://pypi.org/project/dbis-functional-dependencies/)
-        [![License](https://img.shields.io/pypi/l/dbis-functional-dependencies)](https://www.apache.org/licenses/LICENSE-2.0)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dbis-functional-dependencies
+
+Functional Dependencies and Normal Forms for Relational Databases
+
+[![PyPI Status](https://img.shields.io/pypi/v/dbis-functional-dependencies.svg)](https://pypi.python.org/pypi/dbis-functional-dependencies/)
+[![pypi](https://img.shields.io/pypi/pyversions/dbis-functional-dependencies)](https://pypi.org/project/dbis-functional-dependencies/)
+[![License](https://img.shields.io/pypi/l/dbis-functional-dependencies)](https://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `dbis-functional-dependencies-0.0.5/functional_dependencies/BCNF.py` & `dbis-functional-dependencies-0.0.7/functional_dependencies/BCNF.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,24 @@
         '''
         text_list=[]
         for a_set in set_list: 
             text_list.append(Set.stringify_set(a_set,notation=notation))
         text_list=sorted(text_list)
         return text_list
     
+    def copy(self):
+        fds = FunctionalDependencySet()
+        fds.title = self.title
+        fds.description = self.description
+        fds.notation = self.notation
+        fds.debug = self.debug
+        fds.attributes = self.attributes.copy()
+        fds.attribute_map = self.attribute_map.copy()
+        fds.dependencies = self.dependencies.copy()
+        fds.isdecomposed = self.isdecomposed
     
     def stringify_dependencies(self):
         '''
         stringifies the set of dependencies
         '''
         text='{'
         delim=''
@@ -191,22 +201,45 @@
             closure_left = self.get_attr_closure(left)
             if closure_left != self.attributes:
                 return False
         return True
 
     def decompose2(self):
         '''
-        decomposition algorithm done right
+        decomposition algorithm according to DBIS-VL
+        Source: https://dbis.rwth-aachen.de/dbis-vl/RelDesign#page=82
         '''
-        tables = {self.copy()}
-        for fdset in tables:
-            if not fdset.isBCNF():
-                for left,right in fdset.dependencies:
-                    if fdset.get_attr_closure(left) != fdset.attributes:
-                        tables.remove(fdset)
+        self.isdecomposed = True
+        fds = FunctionalDependencySet()
+        fds.attributes = self.attributes.copy()
+        fds.dependencies = self.dependencies.copy()
+        not_bcnf = [fds]
+        bcnf = []
+        while not_bcnf:
+            fds = not_bcnf.pop(0)
+            if fds.isBCNF():
+                bcnf.append(fds.attributes)
+            else:
+                new_fds1 = FunctionalDependencySet()
+                new_fds2 = FunctionalDependencySet()
+                for dep in fds.dependencies:
+                    left, right = dep
+                    if fds.get_attr_closure(left) != fds.attributes:
+                        # create new fdsets along the dependecy we decompose with
+                        new_fds1.attributes = left | right
+                        new_fds2.attributes = fds.attributes - right
+                        # find dependencies that belong to the new fdsets
+                        new_fds1.dependencies = [fd for fd in fds.dependencies if (fd[0] | fd[1]) <= new_fds1.attributes]
+                        new_fds2.dependencies = [fd for fd in fds.dependencies if (fd[0] | fd[1]) <= new_fds2.attributes]
+                        new_fds2.dependencies = new_fds2.dependencies + [(fd[0], fd[1].intersection(new_fds2.attributes)) for fd in fds.dependencies if fd[0] <= new_fds2.attributes and len(fd[1].intersection(new_fds2.attributes)) != 0]
+                        break
+                not_bcnf.append(new_fds1)
+                not_bcnf.append(new_fds2)
+        self.tables = bcnf
+        return bcnf
 
     
     def decompose(self):
         '''
         decomposition algorithm
         '''
         self.isdecomposed = True
```

### Comparing `dbis-functional-dependencies-0.0.5/functional_dependencies/fdcheck.py` & `dbis-functional-dependencies-0.0.7/functional_dependencies/fdcheck.py`

 * *Files identical despite different names*

### Comparing `dbis-functional-dependencies-0.0.5/functional_dependencies/fds.py` & `dbis-functional-dependencies-0.0.7/functional_dependencies/fds.py`

 * *Files identical despite different names*

### Comparing `dbis-functional-dependencies-0.0.5/functional_dependencies/fdsbase.py` & `dbis-functional-dependencies-0.0.7/functional_dependencies/fdsbase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 '''
 Created on 2022-06-08
 
 @author: wf
 '''
 from enum import Enum
+import copy
 
 class Notation(str,Enum):
     '''
     a notation to be used for stringifcation
     '''
     math="LaTex math symbols"   
     utf8="UTF-8 Symbols"  
@@ -24,46 +25,53 @@
         '''
         constructor
         '''
         super().__init__(*args,**kwargs)
         
     def __str__(self):
         text=Set.stringify_set(self,notation=Set.notation)
-        return text
+        return text        
     
     @classmethod    
     def stringify_set(cls,pSet,notation:Notation):
         '''
         return a string representation of the given set using the given delimiter
         
         Args:
             pSet(set): the set to stringify
             delim(str): the delimiter to use
         '''
         sortedElements=sorted([str(elem) for elem in pSet])
-        elementDelim=","
-        if notation==Notation.short:
-            elementDelim='' # Thin space would be better
-        if notation==Notation.short:
-            text=''    
-        elif notation==Notation.math:
-            text="\{"
-        else:
-            text="{"
-
-        delim=""
-        for element in sortedElements:
-            text+=f"{delim}{element}"
-            delim=elementDelim
-        if notation==Notation.short:
-            pass 
-        elif notation==Notation.math:
-            text+="\}"
-        else:
-            text+="}"      
+        if len(sortedElements)==0:
+            # empty set
+            if notation==Notation.math:
+                text="\emptyset"
+            else:
+                text="∅"
+        else:    
+            elementDelim=","
+            if notation==Notation.short:
+                elementDelim='' # Thin space would be better
+            if notation==Notation.short:
+                text=''    
+            elif notation==Notation.math:
+                text="\{"
+            else:
+                text="{"
+    
+            delim=""    
+            for element in sortedElements:
+                text+=f"{delim}{element}"
+                delim=elementDelim
+            if notation==Notation.short:
+                pass 
+            elif notation==Notation.math:
+                text+="\}"
+            else:
+                text+="}"      
         return text
     
 class FD(object):
     """A functional dependency with left- and right-hand side."""
     notation=Notation.plain
 
     def __init__(self, left, right):
@@ -132,36 +140,55 @@
     """A relation schema consists of a set of attributes and a set of FDs.
 
     Various normal forms exist to describe "good" schemata.  Normalization
     is the process of creating schemata that satisfy certain normal forms.
     The class of synthesis algorithms targets 3NF.
     """
 
-    def __init__(self, attributes:Set, fds,notation:Notation=None):
+    def __init__(self, attributes:Set, fds,name:str="R",notation:Notation=None):
         """
         Construct relation schema with attributes and FDs.
         
         Args:
             attributes(list): a list of Attributes
             fds(FunctionalDependencySet): a set of FDs
+            name(string): the name of the RelatonSchema
+            notation(Notation): the notation to use
         """
         if notation is None:
             notation=Notation.utf8
         self.notation=notation
         self.attributes = attributes
         self.fds = fds
+        self.name=name
         
     def __str__(self):
         text=RelSchema.stringify(self, self.notation)
         return text
         
     @classmethod
     def stringify(cls,rs,notation):
         '''
         return a textual representation of the given relational schema in the given notation
         '''
-        text="R={"
-        text+=Set.stringify_set(rs.attributes, notation)
-        text+=f",{rs.fds}"
-        text+="}"
-        return text
-           
+        attrText=Set.stringify_set(rs.attributes, notation)
+        fds=copy.deepcopy(rs.fds)
+        fds.notation=notation
+        fdsText=str(fds)
+        rsSet=Set([attrText,fdsText])
+        rsSetText=Set.stringify_set(rsSet,notation=notation)
+        rsText=f"{rs.name}={rsSetText}"
+        return rsText
+    
+    def findCandidateKeys(self):
+        '''
+        find candidate keys
+        '''
+        cklist=[]
+        for foundKeySet in self.fds.find_candidate_keys():
+            keySet=Set()
+            for foundKey in foundKeySet:
+                attr=self.fds.attribute_map[foundKey]
+                keySet.update([attr])
+            cklist.append(keySet)
+        return cklist    
+
```

### Comparing `dbis-functional-dependencies-0.0.5/setup.py` & `dbis-functional-dependencies-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 from setuptools import setup
 
 class Version(object):
     name="relational_model"
     description="RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
-    version='0.0.5'
+    version='0.0.7'
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent.resolve()
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
```

