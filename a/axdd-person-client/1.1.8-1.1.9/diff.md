# Comparing `tmp/axdd-person-client-1.1.8.tar.gz` & `tmp/axdd-person-client-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axdd-person-client-1.1.8.tar", last modified: Mon May 15 16:09:45 2023, max compression
+gzip compressed data, was "axdd-person-client-1.1.9.tar", last modified: Wed May 24 23:20:45 2023, max compression
```

## Comparing `axdd-person-client-1.1.8.tar` & `axdd-person-client-1.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.266085 axdd-person-client-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-15 16:09:45.266085 axdd-person-client-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.262085 axdd-person-client-1.1.8/axdd_person_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-15 16:09:44.000000 axdd-person-client-1.1.8/axdd_person_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-15 16:09:45.000000 axdd-person-client-1.1.8/axdd_person_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 16:09:44.000000 axdd-person-client-1.1.8/axdd_person_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-15 16:09:44.000000 axdd-person-client-1.1.8/axdd_person_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-15 16:09:44.000000 axdd-person-client-1.1.8/axdd_person_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.262085 axdd-person-client-1.1.8/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 16:09:45.266085 axdd-person-client-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.262085 axdd-person-client-1.1.8/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.262085 axdd-person-client-1.1.8/uw_person_client/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27839 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/clients/core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/clients/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.266085 axdd-person-client-1.1.8/uw_person_client/databases/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/databases/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/databases/uwpds.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.266085 axdd-person-client-1.1.8/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (122)    35780 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/tests/test_core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/tests/test_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 23:20:45.353480 axdd-person-client-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-24 23:20:45.353480 axdd-person-client-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 23:20:45.353480 axdd-person-client-1.1.9/axdd_person_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-24 23:20:45.000000 axdd-person-client-1.1.9/axdd_person_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-24 23:20:45.000000 axdd-person-client-1.1.9/axdd_person_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 23:20:45.000000 axdd-person-client-1.1.9/axdd_person_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-24 23:20:45.000000 axdd-person-client-1.1.9/axdd_person_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-24 23:20:45.000000 axdd-person-client-1.1.9/axdd_person_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 23:20:45.353480 axdd-person-client-1.1.9/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 23:20:45.353480 axdd-person-client-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 23:20:45.353480 axdd-person-client-1.1.9/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 23:20:45.353480 axdd-person-client-1.1.9/uw_person_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27839 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/clients/core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/clients/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 23:20:45.353480 axdd-person-client-1.1.9/uw_person_client/databases/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/databases/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6512 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/databases/uwpds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 23:20:45.353480 axdd-person-client-1.1.9/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35780 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/tests/test_core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-24 23:20:36.000000 axdd-person-client-1.1.9/uw_person_client/tests/test_mock_client.py
```

### Comparing `axdd-person-client-1.1.8/LICENSE` & `axdd-person-client-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/PKG-INFO` & `axdd-person-client-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.8
+Version: 1.1.9
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.8/README.md` & `axdd-person-client-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/axdd_person_client.egg-info/PKG-INFO` & `axdd-person-client-1.1.9/axdd_person_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.8
+Version: 1.1.9
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.8/axdd_person_client.egg-info/SOURCES.txt` & `axdd-person-client-1.1.9/axdd_person_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/conf/settings.py` & `axdd-person-client-1.1.9/conf/settings.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/setup.py` & `axdd-person-client-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/uw_person_client/clients/__init__.py` & `axdd-person-client-1.1.9/uw_person_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/uw_person_client/clients/core_client.py` & `axdd-person-client-1.1.9/uw_person_client/clients/core_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/uw_person_client/clients/mock_client.py` & `axdd-person-client-1.1.9/uw_person_client/clients/mock_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/uw_person_client/components.py` & `axdd-person-client-1.1.9/uw_person_client/components.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/uw_person_client/databases/__init__.py` & `axdd-person-client-1.1.9/uw_person_client/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/uw_person_client/databases/postgres.py` & `axdd-person-client-1.1.9/uw_person_client/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/uw_person_client/databases/uwpds.py` & `axdd-person-client-1.1.9/uw_person_client/databases/uwpds.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             transcript = relationship(
                 "Transcript", back_populates="student", uselist=True,
                 viewonly=True)
             transfer = relationship(
                 "transfer", back_populates="student", uselist=True,
                 viewonly=True)
             degree = relationship(
-                "degree", back_populates="student", uselist=True,
+                "Degree", back_populates="student", uselist=True,
                 viewonly=True)
             student_hold = relationship(
                 "student_hold", back_populates="student", uselist=True,
                 order_by="student_hold.seq", viewonly=True)
             academic_term_id = Column(
                 'academic_term_id', ForeignKey('term.id', ondelete="CASCADE"))
             academic_term = \
@@ -126,13 +126,23 @@
             leave_ends_term_id = Column('leave_ends_term_id',
                                         ForeignKey('term.id',
                                                    ondelete="CASCADE"))
             leave_ends_term = relationship("term",
                                            foreign_keys=[leave_ends_term_id],
                                            viewonly=True)
 
+        class Degree(UWPDS.Base):
+            __tablename__ = "degree"
+            __table_args__ = {'extend_existing': True}
+            degree_term_id = Column('degree_term_id',
+                                    ForeignKey('term.id', ondelete="CASCADE"))
+            degree_term = relationship("term",
+                                       foreign_keys=[degree_term_id],
+                                       viewonly=True)
+
         UWPDS.Base.prepare(self.engine, reflect=True)
         UWPDS.Base.classes.student = Student
         UWPDS.Base.classes.employee = Employee
         UWPDS.Base.classes.transcript = Transcript
+        UWPDS.Base.classes.degree = Degree
         UWPDS.Base.classes.student_to_sport = student_to_sport
         UWPDS.Base.classes.student_to_adviser = student_to_adviser
```

### Comparing `axdd-person-client-1.1.8/uw_person_client/tests/test_core_client.py` & `axdd-person-client-1.1.9/uw_person_client/tests/test_core_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.8/uw_person_client/tests/test_mock_client.py` & `axdd-person-client-1.1.9/uw_person_client/tests/test_mock_client.py`

 * *Files identical despite different names*

