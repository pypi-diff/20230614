# Comparing `tmp/segments-ai-1.0.8.tar.gz` & `tmp/segments-ai-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segments-ai-1.0.8.tar", last modified: Mon Sep 19 09:53:25 2022, max compression
+gzip compressed data, was "segments-ai-1.0.9.tar", last modified: Fri Sep 23 09:02:18 2022, max compression
```

## Comparing `segments-ai-1.0.8.tar` & `segments-ai-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2022-09-19 09:53:25.514191 segments-ai-1.0.8/
--rw-r--r--   0 bert      (1000) bert      (1000)     1062 2020-01-04 18:38:00.000000 segments-ai-1.0.8/LICENSE.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)       83 2022-08-02 10:22:42.000000 segments-ai-1.0.8/MANIFEST.in
--rw-rw-r--   0 bert      (1000) bert      (1000)     1127 2022-09-19 09:53:25.514191 segments-ai-1.0.8/PKG-INFO
--rw-rw-r--   0 bert      (1000) bert      (1000)     2813 2022-08-02 10:46:08.000000 segments-ai-1.0.8/README.md
--rw-rw-r--   0 bert      (1000) bert      (1000)      499 2022-08-02 10:22:42.000000 segments-ai-1.0.8/pyproject.toml
--rw-rw-r--   0 bert      (1000) bert      (1000)      133 2022-08-02 10:22:42.000000 segments-ai-1.0.8/requirements.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      254 2022-09-16 07:47:31.000000 segments-ai-1.0.8/requirements_dev.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      190 2022-08-02 10:22:42.000000 segments-ai-1.0.8/requirements_docs.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      820 2022-09-19 09:53:25.514191 segments-ai-1.0.8/setup.cfg
--rw-rw-r--   0 bert      (1000) bert      (1000)     3186 2022-09-19 09:51:50.000000 segments-ai-1.0.8/setup.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2022-09-19 09:53:25.510191 segments-ai-1.0.8/src/
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2022-09-19 09:53:25.514191 segments-ai-1.0.8/src/segments/
--rw-rw-r--   0 bert      (1000) bert      (1000)      260 2022-08-02 10:22:42.000000 segments-ai-1.0.8/src/segments/__init__.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    74387 2022-09-19 09:52:01.000000 segments-ai-1.0.8/src/segments/client.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2022-09-19 09:53:25.514191 segments-ai-1.0.8/src/segments/data/
--rw-rw-r--   0 bert      (1000) bert      (1000)      501 2022-08-02 10:22:42.000000 segments-ai-1.0.8/src/segments/data/dataset_card_template.md
--rw-rw-r--   0 bert      (1000) bert      (1000)    14329 2022-09-16 07:47:31.000000 segments-ai-1.0.8/src/segments/dataset.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     1468 2022-08-03 10:04:24.000000 segments-ai-1.0.8/src/segments/exceptions.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    30691 2022-09-16 07:47:31.000000 segments-ai-1.0.8/src/segments/export.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    11973 2022-08-02 10:22:42.000000 segments-ai-1.0.8/src/segments/huggingface.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    12868 2022-09-19 09:49:44.000000 segments-ai-1.0.8/src/segments/typing.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    17319 2022-09-16 07:47:31.000000 segments-ai-1.0.8/src/segments/utils.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2022-09-19 09:53:25.514191 segments-ai-1.0.8/src/segments_ai.egg-info/
--rw-rw-r--   0 bert      (1000) bert      (1000)     1127 2022-09-19 09:53:25.000000 segments-ai-1.0.8/src/segments_ai.egg-info/PKG-INFO
--rw-rw-r--   0 bert      (1000) bert      (1000)      559 2022-09-19 09:53:25.000000 segments-ai-1.0.8/src/segments_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)        1 2022-09-19 09:53:25.000000 segments-ai-1.0.8/src/segments_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      467 2022-09-19 09:53:25.000000 segments-ai-1.0.8/src/segments_ai.egg-info/requires.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)        9 2022-09-19 09:53:25.000000 segments-ai-1.0.8/src/segments_ai.egg-info/top_level.txt
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2022-09-23 09:02:18.648323 segments-ai-1.0.9/
+-rw-r--r--   0 bert      (1000) bert      (1000)     1062 2020-01-04 18:38:00.000000 segments-ai-1.0.9/LICENSE.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)       83 2022-08-02 10:22:42.000000 segments-ai-1.0.9/MANIFEST.in
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1082 2022-09-23 09:02:18.648323 segments-ai-1.0.9/PKG-INFO
+-rw-rw-r--   0 bert      (1000) bert      (1000)     2813 2022-08-02 10:46:08.000000 segments-ai-1.0.9/README.md
+-rw-rw-r--   0 bert      (1000) bert      (1000)      499 2022-08-02 10:22:42.000000 segments-ai-1.0.9/pyproject.toml
+-rw-rw-r--   0 bert      (1000) bert      (1000)      133 2022-08-02 10:22:42.000000 segments-ai-1.0.9/requirements.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      254 2022-09-23 08:48:56.000000 segments-ai-1.0.9/requirements_dev.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      190 2022-08-02 10:22:42.000000 segments-ai-1.0.9/requirements_docs.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      820 2022-09-23 09:02:18.648323 segments-ai-1.0.9/setup.cfg
+-rw-rw-r--   0 bert      (1000) bert      (1000)     3186 2022-09-23 09:00:40.000000 segments-ai-1.0.9/setup.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2022-09-23 09:02:18.644323 segments-ai-1.0.9/src/
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2022-09-23 09:02:18.648323 segments-ai-1.0.9/src/segments/
+-rw-rw-r--   0 bert      (1000) bert      (1000)      260 2022-08-02 10:22:42.000000 segments-ai-1.0.9/src/segments/__init__.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    74387 2022-09-23 09:00:51.000000 segments-ai-1.0.9/src/segments/client.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2022-09-23 09:02:18.648323 segments-ai-1.0.9/src/segments/data/
+-rw-rw-r--   0 bert      (1000) bert      (1000)      501 2022-08-02 10:22:42.000000 segments-ai-1.0.9/src/segments/data/dataset_card_template.md
+-rw-rw-r--   0 bert      (1000) bert      (1000)    14329 2022-09-23 08:48:56.000000 segments-ai-1.0.9/src/segments/dataset.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1468 2022-08-03 10:04:24.000000 segments-ai-1.0.9/src/segments/exceptions.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    30691 2022-09-23 08:48:56.000000 segments-ai-1.0.9/src/segments/export.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    11973 2022-08-02 10:22:42.000000 segments-ai-1.0.9/src/segments/huggingface.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    12888 2022-09-23 08:50:13.000000 segments-ai-1.0.9/src/segments/typing.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    17319 2022-09-23 08:48:56.000000 segments-ai-1.0.9/src/segments/utils.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2022-09-23 09:02:18.648323 segments-ai-1.0.9/src/segments_ai.egg-info/
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1082 2022-09-23 09:02:18.000000 segments-ai-1.0.9/src/segments_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 bert      (1000) bert      (1000)      559 2022-09-23 09:02:18.000000 segments-ai-1.0.9/src/segments_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)        1 2022-09-23 09:02:18.000000 segments-ai-1.0.9/src/segments_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      467 2022-09-23 09:02:18.000000 segments-ai-1.0.9/src/segments_ai.egg-info/requires.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)        9 2022-09-23 09:02:18.000000 segments-ai-1.0.9/src/segments_ai.egg-info/top_level.txt
```

### Comparing `segments-ai-1.0.8/LICENSE.txt` & `segments-ai-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `segments-ai-1.0.8/README.md` & `segments-ai-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `segments-ai-1.0.8/setup.cfg` & `segments-ai-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `segments-ai-1.0.8/setup.py` & `segments-ai-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 from typing import List
 
 #############
 # Constants #
 #############
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 
 
 ####################
 # Helper functions #
 ####################
 # https://github.com/allenai/python-package-template
 def read_requirements(filename: str) -> List[str]:
```

### Comparing `segments-ai-1.0.8/src/segments/client.py` & `segments-ai-1.0.9/src/segments/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         self.api_session.mount("https://", adapter)
 
         self.s3_session = requests.Session()
         self.s3_session.mount("http://", adapter)
         self.s3_session.mount("https://", adapter)
 
         try:
-            r = self._get("/api_status/?lib_version=1.0.8")
+            r = self._get("/api_status/?lib_version=1.0.9")
             if r.status_code == 200:
                 logger.info("Initialized successfully.")
         except NetworkError as e:
             if (
                 cast(requests.exceptions.RequestException, e.cause).response.status_code
                 == 426
             ):
```

### Comparing `segments-ai-1.0.8/src/segments/dataset.py` & `segments-ai-1.0.9/src/segments/dataset.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.0.8/src/segments/exceptions.py` & `segments-ai-1.0.9/src/segments/exceptions.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.0.8/src/segments/export.py` & `segments-ai-1.0.9/src/segments/export.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.0.8/src/segments/huggingface.py` & `segments-ai-1.0.9/src/segments/huggingface.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.0.8/src/segments/typing.py` & `segments-ai-1.0.9/src/segments/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,17 +385,17 @@
 class Sample(BaseModel):
     uuid: str
     name: str
     attributes: SampleAttributes
     metadata: Dict[str, Any]
     created_at: str
     created_by: str
-    comments: List[str]
+    comments: Optional[List[str]]
     priority: float
-    has_embedding: bool
+    has_embedding: Optional[bool]
     label: Optional[Label]
     issues: Optional[List[Issue]]
     dataset_full_name: Optional[str]
 
 
 ########################
 # Dataset and labelset #
```

### Comparing `segments-ai-1.0.8/src/segments/utils.py` & `segments-ai-1.0.9/src/segments/utils.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.0.8/src/segments_ai.egg-info/SOURCES.txt` & `segments-ai-1.0.9/src/segments_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

