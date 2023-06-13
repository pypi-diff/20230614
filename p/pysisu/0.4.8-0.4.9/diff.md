# Comparing `tmp/pysisu-0.4.8.tar.gz` & `tmp/pysisu-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysisu-0.4.8.tar", last modified: Thu Mar 30 21:26:13 2023, max compression
+gzip compressed data, was "pysisu-0.4.9.tar", last modified: Tue Apr  4 18:15:07 2023, max compression
```

## Comparing `pysisu-0.4.8.tar` & `pysisu-0.4.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.029200 pysisu-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-03-30 21:26:01.000000 pysisu-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-30 21:26:13.029200 pysisu-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-30 21:26:01.000000 pysisu-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/example_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/latest_analysis_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/proto/google/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/proto/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/proto/google/api/
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/proto/google/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/proto/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/proto/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/proto/grpc/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/proto/grpc/gateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/proto/grpc/gateway/protoc_gen_openapiv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/proto/grpc/gateway/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/proto/grpc/gateway/protoc_gen_openapiv2/options/
--rw-r--r--   0 runner    (1001) docker     (123)    27689 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/proto/grpc/gateway/protoc_gen_openapiv2/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/proto/sisu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/proto/sisu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/proto/sisu/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/proto/sisu/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/proto/sisu/v1/api/
--rw-r--r--   0 runner    (1001) docker     (123)    92839 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/proto/sisu/v1/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/pysisu_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/query_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/scripts/ensure_version_bumped.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.029200 pysisu-0.4.8/pysisu/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/tests/helpers_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/tests/test_analysis_results_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/tests/test_analysis_results_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/tests/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/tests/test_version_control.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 21:26:01.000000 pysisu-0.4.8/pysisu/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:26:13.025200 pysisu-0.4.8/pysisu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-30 21:26:13.000000 pysisu-0.4.8/pysisu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 21:26:13.000000 pysisu-0.4.8/pysisu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 21:26:13.000000 pysisu-0.4.8/pysisu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-30 21:26:13.000000 pysisu-0.4.8/pysisu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 21:26:13.000000 pysisu-0.4.8/pysisu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-30 21:26:13.029200 pysisu-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-30 21:26:01.000000 pysisu-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.738659 pysisu-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-04 18:14:54.000000 pysisu-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-04 18:15:07.738659 pysisu-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-04 18:14:54.000000 pysisu-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/example_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/latest_analysis_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/proto/google/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/proto/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/proto/google/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/proto/google/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/proto/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/proto/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/proto/grpc/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/proto/grpc/gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/proto/grpc/gateway/protoc_gen_openapiv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/proto/grpc/gateway/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/proto/grpc/gateway/protoc_gen_openapiv2/options/
+-rw-r--r--   0 runner    (1001) docker     (123)    27689 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/proto/grpc/gateway/protoc_gen_openapiv2/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/proto/sisu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/proto/sisu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/proto/sisu/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/proto/sisu/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu/proto/sisu/v1/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    96212 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/proto/sisu/v1/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/pysisu_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/query_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.738659 pysisu-0.4.9/pysisu/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/scripts/ensure_version_bumped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.738659 pysisu-0.4.9/pysisu/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/tests/helpers_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/tests/test_analysis_results_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/tests/test_analysis_results_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/tests/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/tests/test_version_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 18:14:54.000000 pysisu-0.4.9/pysisu/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:15:07.734658 pysisu-0.4.9/pysisu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-04 18:15:07.000000 pysisu-0.4.9/pysisu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-04 18:15:07.000000 pysisu-0.4.9/pysisu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 18:15:07.000000 pysisu-0.4.9/pysisu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-04 18:15:07.000000 pysisu-0.4.9/pysisu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-04 18:15:07.000000 pysisu-0.4.9/pysisu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-04 18:15:07.738659 pysisu-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-04 18:14:54.000000 pysisu-0.4.9/setup.py
```

### Comparing `pysisu-0.4.8/LICENSE` & `pysisu-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/PKG-INFO` & `pysisu-0.4.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysisu
-Version: 0.4.8
+Version: 0.4.9
 Home-page: https://github.com/sisudata/pysisu
 Author: Sisu Data
 License: Apache
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysisu
```

### Comparing `pysisu-0.4.8/README.md` & `pysisu-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/__init__.py` & `pysisu-0.4.9/pysisu/__init__.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/example_usage.py` & `pysisu-0.4.9/pysisu/example_usage.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/formats.py` & `pysisu-0.4.9/pysisu/formats.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/latest_analysis_result.py` & `pysisu-0.4.9/pysisu/latest_analysis_result.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/proto/google/api/__init__.py` & `pysisu-0.4.9/pysisu/proto/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/proto/grpc/gateway/protoc_gen_openapiv2/options/__init__.py` & `pysisu-0.4.9/pysisu/proto/grpc/gateway/protoc_gen_openapiv2/options/__init__.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/proto/sisu/v1/api/__init__.py` & `pysisu-0.4.9/pysisu/proto/sisu/v1/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1335,14 +1335,79 @@
 class DeleteDataSourceResponse(betterproto.Message):
     """Response payload for delete data source."""
 
     pass
 
 
 @dataclass(eq=False, repr=False)
+class ModifyDataSourceRequest(betterproto.Message):
+    """Request payload for modify data source."""
+
+    id: int = betterproto.uint64_field(1)
+    """The id of data source."""
+
+    datasource: "ModifyDataSourceRequestPayload" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class ModifyDataSourceRequestPayload(betterproto.Message):
+    """The body payload of data source."""
+
+    name: Optional[str] = betterproto.string_field(1, optional=True, group="_name")
+    """The table or query name of a data source."""
+
+    password: Optional[str] = betterproto.string_field(
+        2, optional=True, group="_password"
+    )
+    """The password of data source."""
+
+    uri: Optional[str] = betterproto.string_field(3, optional=True, group="_uri")
+    """The JDBC connection URI to the data source location."""
+
+    username: Optional[str] = betterproto.string_field(
+        4, optional=True, group="_username"
+    )
+    """The username of the data source."""
+
+    is_restricted: Optional[bool] = betterproto.bool_field(
+        5, optional=True, group="_is_restricted"
+    )
+    """The data source is private or not."""
+
+
+@dataclass(eq=False, repr=False)
+class ModifyDataSourceResponse(betterproto.Message):
+    """Response payload for modify data source."""
+
+    id: int = betterproto.uint64_field(1)
+    """The id of data source."""
+
+    name: str = betterproto.string_field(2)
+    """The table or query name of a data source."""
+
+    data_source_type: str = betterproto.string_field(3)
+    """The type of data source."""
+
+    connection_uri: str = betterproto.string_field(4)
+    """The JDBC connection URI to the data source location."""
+
+    data_source_username: str = betterproto.string_field(5)
+    """The username of the data source."""
+
+    private: bool = betterproto.bool_field(6)
+    """The data source is private or not."""
+
+    created_at: datetime = betterproto.message_field(7)
+    """The created timestamp of data source."""
+
+    created_by: str = betterproto.string_field(8)
+    """The creates of data source."""
+
+
+@dataclass(eq=False, repr=False)
 class DataSetsRequest(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
 class DataSetsResponse(betterproto.Message):
     datasets: List["Dataset"] = betterproto.message_field(1)
@@ -1436,36 +1501,36 @@
 
 
 @dataclass(eq=False, repr=False)
 class GetDataSourceResponse(betterproto.Message):
     """Response payload for get data source."""
 
     id: int = betterproto.uint64_field(1)
-    """Represents the id of data source."""
+    """The id of data source."""
 
     name: str = betterproto.string_field(2)
-    """Represents the table or query name of a data source."""
+    """The table or query name of a data source."""
 
     data_source_type: str = betterproto.string_field(3)
-    """Represents the type of data source."""
+    """The type of data source."""
 
     connection_uri: str = betterproto.string_field(4)
-    """Represents the JDBC connection URI to the data source location."""
+    """The JDBC connection URI to the data source location."""
 
     data_source_username: str = betterproto.string_field(5)
-    """Represents the username of the data source."""
+    """The username of the data source."""
 
     private: bool = betterproto.bool_field(6)
-    """Represents whether the data source is private or not."""
+    """The data source is private or not."""
 
     created_at: datetime = betterproto.message_field(7)
-    """Represents the created timestamp of data source."""
+    """The created timestamp of data source."""
 
     created_by: str = betterproto.string_field(8)
-    """Represents the creates of data source."""
+    """The creates of data source."""
 
 
 @dataclass(eq=False, repr=False)
 class GetDataSourceRequest(betterproto.Message):
     """Request payload for get data source."""
 
     id: int = betterproto.uint64_field(1)
@@ -2265,14 +2330,31 @@
             delete_data_source_request,
             DeleteDataSourceResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
+    async def modify_data_source(
+        self,
+        modify_data_source_request: "ModifyDataSourceRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "ModifyDataSourceResponse":
+        return await self._unary_unary(
+            "/sisu.v1.api.DataSourcesService/ModifyDataSource",
+            modify_data_source_request,
+            ModifyDataSourceResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
 
 class SegmentsServiceStub(betterproto.ServiceStub):
     async def get_segment_data(
         self,
         get_segment_data_request: "GetSegmentDataRequest",
         *,
         timeout: Optional[float] = None,
@@ -2658,14 +2740,19 @@
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def delete_data_source(
         self, delete_data_source_request: "DeleteDataSourceRequest"
     ) -> "DeleteDataSourceResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
+    async def modify_data_source(
+        self, modify_data_source_request: "ModifyDataSourceRequest"
+    ) -> "ModifyDataSourceResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
     async def __rpc_data_source_list(
         self,
         stream: "grpclib.server.Stream[DataSourceListRequest, DataSourceListResponse]",
     ) -> None:
         request = await stream.recv_message()
         response = await self.data_source_list(request)
         await stream.send_message(response)
@@ -2690,14 +2777,22 @@
         self,
         stream: "grpclib.server.Stream[DeleteDataSourceRequest, DeleteDataSourceResponse]",
     ) -> None:
         request = await stream.recv_message()
         response = await self.delete_data_source(request)
         await stream.send_message(response)
 
+    async def __rpc_modify_data_source(
+        self,
+        stream: "grpclib.server.Stream[ModifyDataSourceRequest, ModifyDataSourceResponse]",
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.modify_data_source(request)
+        await stream.send_message(response)
+
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
             "/sisu.v1.api.DataSourcesService/DataSourceList": grpclib.const.Handler(
                 self.__rpc_data_source_list,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 DataSourceListRequest,
                 DataSourceListResponse,
@@ -2716,14 +2811,20 @@
             ),
             "/sisu.v1.api.DataSourcesService/DeleteDataSource": grpclib.const.Handler(
                 self.__rpc_delete_data_source,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 DeleteDataSourceRequest,
                 DeleteDataSourceResponse,
             ),
+            "/sisu.v1.api.DataSourcesService/ModifyDataSource": grpclib.const.Handler(
+                self.__rpc_modify_data_source,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                ModifyDataSourceRequest,
+                ModifyDataSourceResponse,
+            ),
         }
 
 
 class SegmentsServiceBase(ServiceBase):
     async def get_segment_data(
         self, get_segment_data_request: "GetSegmentDataRequest"
     ) -> "GetSegmentDataResponse":
```

### Comparing `pysisu-0.4.8/pysisu/pysisu_class.py` & `pysisu-0.4.9/pysisu/pysisu_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     GetDataSourceResponse,
     GetProjectsAnalysesListResponse,
     GetProjectsListResponseListProjectResponse,
     GetSegmentDataResponse,
     MetricsListResponse,
     ModifyAnalysisRequestAnalysis,
     ModifyAnalysisResponse,
+    ModifyDataSourceRequest,
+    ModifyDataSourceResponse,
     SetAnalysisFiltersRequest,
     UpdateAnalysisRequestAnalysis,
     UpdateAnalysisResponse,
     WaterfallAnalysisResponse,
 )
 from .query_helpers import build_url, pathjoin, semver_parse
 from .version import __version__ as PYSISU_VERSION
@@ -85,19 +87,19 @@
         return self
 
     def set_api_key(self, api_key: str) -> "PySisu":
         self._api_key = api_key
         return self
 
     def _auto_paginate(
-        self,
-        analysis_id: int,
-        params: dict,
-        result: AnalysisRunResultsResponse,
-        **kwargs,
+            self,
+            analysis_id: int,
+            params: dict,
+            result: AnalysisRunResultsResponse,
+            **kwargs,
     ) -> AnalysisRunResultsResponse:
         """
         Fetches the rest of the results if there is more results to fetch.
 
         Respects the limit parameter and only fetches a maximum of params['limit'] that is left.
         """
         if not result.pagination_hints.has_more:
@@ -122,21 +124,21 @@
 
         kwargs["starting_after"] = next_cursor
 
         next_page = self.get_results(
             analysis_id, format=LatestAnalysisResultsFormats.PROTO, **kwargs
         )
         kda_result.segments = (
-            subgroups
-            + next_page.analysis_result.key_driver_analysis_result.segments
+                subgroups
+                + next_page.analysis_result.key_driver_analysis_result.segments
         )
         return result
 
     def _call_sisu_api(
-        self, url_path: int, request_method="get", json=None
+            self, url_path: int, request_method="get", json=None
     ) -> dict:
         headers = {
             "Authorization": self._api_key,
             "User-Agent": f"PySisu/{PYSISU_VERSION}",
         }
         r = requests.request(
             request_method, url_path, headers=headers, json=json
@@ -162,30 +164,30 @@
             )
             return
 
         local_major, local_minor, local_patch = semver_parse(PYSISU_VERSION)
         latest_major, latest_minor, latest_patch = semver_parse(latest_version)
 
         if local_major < latest_major or (
-            local_major == 0 and local_minor < latest_minor
+                local_major == 0 and local_minor < latest_minor
         ):
             raise PySisuDeprecatedVersionException(
                 "Pysisu has been updated with breaking changes from "
                 f"{PYSISU_VERSION} to {latest_version}; get latest version "
                 "with 'pip install -U pysisu'"
             )
         if (local_minor, local_patch) < (latest_minor, latest_patch):
             warnings.warn(
                 f"Pysisu has been updated from {PYSISU_VERSION} to "
                 f"{latest_version}; get latest version with 'pip install -U "
                 "pysisu'"
             )
 
     def fetch_sisu_api(
-        self, analysis_id: int, params: dict = {}, **kwargs
+            self, analysis_id: int, params: dict = {}, **kwargs
     ) -> dict:
         path = ["api/v1/analyses/", str(analysis_id), "runs/latest"]
         url_path = build_url(self._url, pathjoin(*path), {**params, **kwargs})
         return self._call_sisu_api(url_path)
 
     def run(self, analysis_id: int, **kwargs):
         path = ["api/v1/analyses/", str(analysis_id), "run"]
@@ -194,21 +196,21 @@
 
     def analyses(self, **kwargs) -> AnalysesListResponse:
         path = ["api/v1/analyses"]
         url_path = build_url(self._url, pathjoin(*path), kwargs)
         return AnalysesListResponse().from_dict(self._call_sisu_api(url_path))
 
     def get_results(
-        self,
-        analysis_id: int,
-        params: dict = {"confidence_gte": "LOW"},
-        auto_paginate: bool = True,
-        format: LatestAnalysisResultsFormats = LatestAnalysisResultsFormats.TABLE,
-        round_to_decimal_place: int = 2,
-        **kwargs,
+            self,
+            analysis_id: int,
+            params: dict = {"confidence_gte": "LOW"},
+            auto_paginate: bool = True,
+            format: LatestAnalysisResultsFormats = LatestAnalysisResultsFormats.TABLE,
+            round_to_decimal_place: int = 2,
+            **kwargs,
     ) -> Union[AnalysisRunResultsResponse, Table]:
         assert type(params) is dict
         assert type(kwargs) is dict
         kwargs = {**params, **kwargs}
 
         result = AnalysisRunResultsResponse().from_dict(
             self.fetch_sisu_api(analysis_id, **kwargs)
@@ -245,36 +247,36 @@
 
     def datasets(self, **kwargs) -> DataSetsResponse:
         path = ["api/v1/datasets"]
         url_path = build_url(self._url, pathjoin(*path), kwargs)
         return DataSetsResponse().from_dict(self._call_sisu_api(url_path))
 
     def get_filters(
-        self, analysis_id: int, **kwargs
+            self, analysis_id: int, **kwargs
     ) -> GetAnalysisFiltersResponse:
         path = [f"api/v1/analyses/{analysis_id}/filters"]
         url_path = build_url(self._url, pathjoin(*path), kwargs)
         return GetAnalysisFiltersResponse().from_dict(
             self._call_sisu_api(url_path)
         )
 
     def set_filters(
-        self, analysis_id: int, expr: SetAnalysisFiltersRequest, **kwargs
+            self, analysis_id: int, expr: SetAnalysisFiltersRequest, **kwargs
     ):
         path = [f"api/v1/analyses/{analysis_id}/filters"]
         url_path = build_url(self._url, pathjoin(*path), kwargs)
         expr = (
             expr.to_dict()
             if isinstance(expr, SetAnalysisFiltersRequest)
             else expr
         )
         return self._call_sisu_api(url_path, request_method="PUT", json=expr)
 
     def duplicate_analysis(
-        self, analysis_id: int, name: Optional[str] = None, **kwargs
+            self, analysis_id: int, name: Optional[str] = None, **kwargs
     ) -> DuplicateAnalysisResponse:
         path = [f"api/v1/analyses/{analysis_id}/duplicate"]
         url_path = build_url(self._url, pathjoin(*path), kwargs)
         json = {"name": name} if name else None
         return DuplicateAnalysisResponse().from_dict(
             self._call_sisu_api(url_path, request_method="POST", json=json)
         )
@@ -283,15 +285,15 @@
         path = [f"api/v1/segments/{segment_id}/data_query"]
         url_path = build_url(self._url, pathjoin(*path), {})
         return GetSegmentDataResponse().from_dict(
             self._call_sisu_api(url_path, request_method="GET")
         )
 
     def create_dataset(
-        self, data_source_id: int, body: CreateDataSetRequestDataset
+            self, data_source_id: int, body: CreateDataSetRequestDataset
     ) -> GetSegmentDataResponse:
         path = [f"api/v1/data_sources/{data_source_id}/datasets"]
         url_path = build_url(self._url, pathjoin(*path), {})
         return GetSegmentDataResponse().from_dict(
             self._call_sisu_api(
                 url_path, request_method="POST", json=body.to_dict()
             )
@@ -301,60 +303,61 @@
         path = ["api/v1/projects"]
         url_path = build_url(self._url, pathjoin(*path), {})
         return GetProjectsListResponseListProjectResponse().from_dict(
             self._call_sisu_api(url_path, request_method="GET")
         )
 
     def get_project_analyses_list(
-        self, project_id
+            self, project_id
     ) -> GetProjectsAnalysesListResponse:
         path = [f"api/v1/projects/{project_id}/analyses"]
         url_path = build_url(self._url, pathjoin(*path), {})
         return GetProjectsAnalysesListResponse().from_dict(
             self._call_sisu_api(url_path, request_method="GET")
         )
 
     def modify_analysis(
-        self,
-        analysis_id: int,
-        modify_analysis_req: ModifyAnalysisRequestAnalysis,
+            self,
+            analysis_id: int,
+            modify_analysis_req: ModifyAnalysisRequestAnalysis,
     ) -> ModifyAnalysisResponse:
         path = [f"api/v1/analyses/{analysis_id}"]
         url_path = build_url(self._url, pathjoin(*path), {})
         return ModifyAnalysisResponse().from_dict(
             self._call_sisu_api(
                 url_path,
                 request_method="PATCH",
                 json=modify_analysis_req.to_dict(),
             )
         )
 
     def update_analysis(
-        self,
-        analysis_id: int,
-        modify_analysis_req: UpdateAnalysisRequestAnalysis,
+            self,
+            analysis_id: int,
+            modify_analysis_req: UpdateAnalysisRequestAnalysis,
     ) -> UpdateAnalysisResponse:
         path = [f"api/v1/analyses/{analysis_id}"]
         url_path = build_url(self._url, pathjoin(*path), {})
         return UpdateAnalysisResponse().from_dict(
             self._call_sisu_api(
                 url_path,
                 request_method="PUT",
                 json=modify_analysis_req.to_dict(),
             )
         )
 
     def get_analysis_dimensions_list(
-        self, analysis_id
+            self, analysis_id
     ) -> AnalysisDimensionsListResponse:
         path = [f"api/v1/analyses/{analysis_id}/dimensions"]
         url_path = build_url(self._url, pathjoin(*path), {})
         return AnalysisDimensionsListResponse().from_dict(
             self._call_sisu_api(url_path, request_method="GET")
         )
+
     def get_analysis_waterfall(self, analysis_id) -> WaterfallAnalysisResponse:
         path = [f"api/v1/analyses/{analysis_id}/waterfall"]
         url_path = build_url(self._url, pathjoin(*path), {})
         return WaterfallAnalysisResponse().from_dict(
             self._call_sisu_api(url_path, request_method="GET")
         )
 
@@ -378,7 +381,22 @@
             self, connection_id: int,
     ) -> DeleteDataSourceResponse:
         path = [f"api/v1/data_sources/{connection_id}"]
         url_path = build_url(self._url, pathjoin(*path), {})
         return DeleteDataSourceResponse().from_dict(
             self._call_sisu_api(url_path, request_method="DELETE")
         )
+
+    def modify_data_source(
+            self,
+            connection_id: int,
+            modify_data_source_req: ModifyDataSourceRequest,
+    ) -> ModifyDataSourceResponse:
+        path = [f"api/v1/data_sources/{connection_id}"]
+        url_path = build_url(self._url, pathjoin(*path), {})
+        return ModifyDataSourceResponse().from_dict(
+            self._call_sisu_api(
+                url_path,
+                request_method="PATCH",
+                json=modify_data_source_req.to_dict(),
+            )
+        )
```

### Comparing `pysisu-0.4.8/pysisu/query_helpers.py` & `pysisu-0.4.9/pysisu/query_helpers.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/scripts/ensure_version_bumped.py` & `pysisu-0.4.9/pysisu/scripts/ensure_version_bumped.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/tests/conftest.py` & `pysisu-0.4.9/pysisu/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/tests/helpers_for_tests.py` & `pysisu-0.4.9/pysisu/tests/helpers_for_tests.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/tests/test_analysis_results_output.py` & `pysisu-0.4.9/pysisu/tests/test_analysis_results_output.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/tests/test_analysis_results_proto.py` & `pysisu-0.4.9/pysisu/tests/test_analysis_results_proto.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/tests/test_endpoints.py` & `pysisu-0.4.9/pysisu/tests/test_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest import mock
 
-from pysisu.proto.sisu.v1.api import CreateDataSetRequestDataset
+from pysisu.proto.sisu.v1.api import CreateDataSetRequestDataset, ModifyDataSourceRequest
+
 from .helpers_for_tests import SNAPSHOT_DICT
 
 
 def validate_api_call(mock_call_sisu_api, method=None, path=None):
     assert mock_call_sisu_api.call_count == 1
     if method is not None:
         assert mock_call_sisu_api.call_args.kwargs["request_method"] == method
@@ -171,7 +172,15 @@
 
 @mock.patch("pysisu.pysisu_class.PySisu._call_sisu_api")
 def test_delete_data_source(mock_call_sisu_api, pysisu_client):
     pysisu_client.delete_data_source(1)
     validate_api_call(
         mock_call_sisu_api, "DELETE", "api/v1/data_sources/1"
     )
+
+
+@mock.patch("pysisu.pysisu_class.PySisu._call_sisu_api")
+def test_modify_data_source(mock_call_sisu_api, pysisu_client):
+    pysisu_client.modify_data_source(1, modify_data_source_req=ModifyDataSourceRequest())
+    validate_api_call(
+        mock_call_sisu_api, "PATCH", "api/v1/data_sources/1"
+    )
```

### Comparing `pysisu-0.4.8/pysisu/tests/test_pagination.py` & `pysisu-0.4.9/pysisu/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu/tests/test_version_control.py` & `pysisu-0.4.9/pysisu/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/pysisu.egg-info/PKG-INFO` & `pysisu-0.4.9/pysisu.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysisu
-Version: 0.4.8
+Version: 0.4.9
 Home-page: https://github.com/sisudata/pysisu
 Author: Sisu Data
 License: Apache
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysisu
```

### Comparing `pysisu-0.4.8/pysisu.egg-info/SOURCES.txt` & `pysisu-0.4.9/pysisu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysisu-0.4.8/setup.py` & `pysisu-0.4.9/setup.py`

 * *Files identical despite different names*

