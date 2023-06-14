# Comparing `tmp/flask-marshmallow-openapi-0.1.6.tar.gz` & `tmp/flask-marshmallow-openapi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.1.6.tar", last modified: Fri Jun  9 20:01:22 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.1.7.tar", last modified: Wed Jun 14 14:07:56 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.1.6.tar` & `flask-marshmallow-openapi-0.1.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 20:01:22.603613 flask-marshmallow-openapi-0.1.6/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-09 20:00:57.000000 flask-marshmallow-openapi-0.1.6/.bumpversion.cfg
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.6/.gitignore
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.6/.python-version
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.6/LICENSE
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      838 2023-06-09 19:55:49.000000 flask-marshmallow-openapi-0.1.6/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 20:01:22.603613 flask-marshmallow-openapi-0.1.6/PKG-INFO
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     3648 2023-06-09 03:51:07.000000 flask-marshmallow-openapi-0.1.6/README.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-09 20:00:57.000000 flask-marshmallow-openapi-0.1.6/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-09 20:01:22.603613 flask-marshmallow-openapi-0.1.6/setup.cfg
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 20:01:22.595612 flask-marshmallow-openapi-0.1.6/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 20:01:22.599612 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      176 2023-06-09 20:00:57.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    13379 2023-06-09 19:47:03.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/decorators.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/helpers.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/middleware.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      641 2023-06-09 19:37:02.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/models.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 20:01:22.595612 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 20:01:22.603613 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3852 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static_collector.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 20:01:22.603613 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 20:01:22.599612 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 20:01:22.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1651 2023-06-09 20:01:22.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-09 20:01:22.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-09 20:01:22.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-09 20:01:22.000000 flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.853251 flask-marshmallow-openapi-0.1.7/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-14 14:07:20.000000 flask-marshmallow-openapi-0.1.7/.bumpversion.cfg
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.7/.gitignore
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.7/.python-version
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.7/LICENSE
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      838 2023-06-09 19:55:49.000000 flask-marshmallow-openapi-0.1.7/MANIFEST.in
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-14 14:07:56.853251 flask-marshmallow-openapi-0.1.7/PKG-INFO
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     3648 2023-06-09 03:51:07.000000 flask-marshmallow-openapi-0.1.7/README.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-14 14:07:20.000000 flask-marshmallow-openapi-0.1.7/pyproject.toml
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-14 14:07:56.853251 flask-marshmallow-openapi-0.1.7/setup.cfg
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.837251 flask-marshmallow-openapi-0.1.7/src/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.837251 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      176 2023-06-14 14:07:20.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    13858 2023-06-14 14:03:50.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/decorators.py
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/helpers.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/middleware.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      641 2023-06-09 19:37:02.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/models.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.837251 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.849251 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3852 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static_collector.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.853251 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.837251 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-14 14:07:56.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1651 2023-06-14 14:07:56.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-14 14:07:56.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-14 14:07:56.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-14 14:07:56.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.1.6/.gitignore` & `flask-marshmallow-openapi-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/LICENSE` & `flask-marshmallow-openapi-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/MANIFEST.in` & `flask-marshmallow-openapi-0.1.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/PKG-INFO` & `flask-marshmallow-openapi-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.6
+Version: 0.1.7
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.6/README.md` & `flask-marshmallow-openapi-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/pyproject.toml` & `flask-marshmallow-openapi-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.1.6"
+version = "0.1.7"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/decorators.py` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,14 +123,15 @@
     request_schema: Type[marshmallow.Schema],
     response_schema: Type[marshmallow.Schema] | None = None,
     operation_id: Optional[str] = None,
     summary: Optional[str] = None,
     errors: Optional[dict] = None,
     headers: Optional[List[dict]] = None,
     security: Securities = Securities.access_token,
+    additional_parameters: list[ParameterObject] | None = None,
 ):
     """
     Decorator that will inject standard sets of our OpenAPI POST docs into decorated
     method.
     """
 
     if not response_schema:
@@ -169,14 +170,26 @@
     # TODO: This convention of having "create" in schema name makes our code smelly,
     # come up with something more explicit
     if url_id_field and "create" not in schema_name(request_schema).lower():
         open_api_data["parameters"][0]["name"] = url_id_field
     else:
         del open_api_data["parameters"]
 
+    if additional_parameters:
+        open_api_data["parameters"] = open_api_data.get("parameters", []) + [
+            _.to_dict for _ in additional_parameters
+        ]
+
+    if "parameters" in open_api_data:
+        open_api_data["parameters"] = [
+            _ for _ in open_api_data["parameters"] if (_["name"])
+        ]
+        if not open_api_data["parameters"]:
+            del open_api_data["parameters"]
+
     tags = getattr(request_schema.opts, "tags", None) or getattr(
         response_schema.opts, "tags", None
     )
     if tags:
         open_api_data["tags"] = tags
 
     _update_errors(open_api_data, errors)
```

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/helpers.py` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/middleware.py` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/middleware.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/models.py` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/models.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static_collector.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.6
+Version: 0.1.7
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.6/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

