# Comparing `tmp/intellect_core-0.1.2.tar.gz` & `tmp/intellect_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellect_core-0.1.2.tar", max compression
+gzip compressed data, was "intellect_core-0.1.3.tar", max compression
```

## Comparing `intellect_core-0.1.2.tar` & `intellect_core-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.1.2/LICENSE
--rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.1.2/intellect_core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.1.2/intellect_core/dto/__init__.py
--rw-r--r--   0        0        0     2306 2023-06-13 11:40:22.236096 intellect_core-0.1.2/intellect_core/dto/dto.py
--rw-r--r--   0        0        0     1023 2023-05-29 14:54:49.902384 intellect_core-0.1.2/intellect_core/handler.py
--rw-r--r--   0        0        0     5324 2023-06-08 14:07:17.962879 intellect_core-0.1.2/intellect_core/intelletct_server.py
--rw-r--r--   0        0        0      307 2023-06-13 11:49:13.289849 intellect_core-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.1.3/LICENSE
+-rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.1.3/intellect_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.1.3/intellect_core/dto/__init__.py
+-rw-r--r--   0        0        0     2335 2023-06-13 13:18:22.425868 intellect_core-0.1.3/intellect_core/dto/dto.py
+-rw-r--r--   0        0        0     1023 2023-05-29 14:54:49.902384 intellect_core-0.1.3/intellect_core/handler.py
+-rw-r--r--   0        0        0     5324 2023-06-08 14:07:17.962879 intellect_core-0.1.3/intellect_core/intelletct_server.py
+-rw-r--r--   0        0        0      307 2023-06-13 13:18:22.433868 intellect_core-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.1.3/PKG-INFO
```

### Comparing `intellect_core-0.1.2/intellect_core/dto/dto.py` & `intellect_core-0.1.3/intellect_core/dto/dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     intellect_host: str
     intellect_port: int
     host_user: str
     host_password: str
     token_expires: int  # seconds
     access_level: int
     access_department_id: int  # for temp pass
+    enable_integration: bool
 
 
 class IntellectVisitDto:
     class Create(BaseModel):
         objid: int
         name: str | None  # second_name
         surname: str | None  # first_name
```

### Comparing `intellect_core-0.1.2/intellect_core/handler.py` & `intellect_core-0.1.3/intellect_core/handler.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.1.2/intellect_core/intelletct_server.py` & `intellect_core-0.1.3/intellect_core/intelletct_server.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.1.2/PKG-INFO` & `intellect_core-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellect-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: Модуль интеграции с Интеллект
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

