# Comparing `tmp/pylambdarest-0.3.0rc3.tar.gz` & `tmp/pylambdarest-0.3.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylambdarest-0.3.0rc3.tar", max compression
+gzip compressed data, was "pylambdarest-0.3.0rc4.tar", max compression
```

## Comparing `pylambdarest-0.3.0rc3.tar` & `pylambdarest-0.3.0rc4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/LICENSE
--rw-r--r--   0        0        0     6093 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/README.md
--rw-r--r--   0        0        0      182 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pylambdarest/__init__.py
--rw-r--r--   0        0        0     8723 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pylambdarest/applications.py
--rw-r--r--   0        0        0     2043 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pylambdarest/config.py
--rw-r--r--   0        0        0      257 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pylambdarest/exceptions.py
--rw-r--r--   0        0        0     2870 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pylambdarest/request.py
--rw-r--r--   0        0        0     1364 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pyproject.toml
--rw-r--r--   0        0        0     7083 1970-01-01 00:00:00.000000 pylambdarest-0.3.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-13 23:49:30.107776 pylambdarest-0.3.0rc4/LICENSE
+-rw-r--r--   0        0        0     6093 2023-06-13 23:49:30.107776 pylambdarest-0.3.0rc4/README.md
+-rw-r--r--   0        0        0      182 2023-06-13 23:49:30.111776 pylambdarest-0.3.0rc4/pylambdarest/__init__.py
+-rw-r--r--   0        0        0     9213 2023-06-13 23:49:30.111776 pylambdarest-0.3.0rc4/pylambdarest/applications.py
+-rw-r--r--   0        0        0     2092 2023-06-13 23:49:30.111776 pylambdarest-0.3.0rc4/pylambdarest/config.py
+-rw-r--r--   0        0        0      257 2023-06-13 23:49:30.111776 pylambdarest-0.3.0rc4/pylambdarest/exceptions.py
+-rw-r--r--   0        0        0     2870 2023-06-13 23:49:30.111776 pylambdarest-0.3.0rc4/pylambdarest/request.py
+-rw-r--r--   0        0        0     1364 2023-06-13 23:49:30.111776 pylambdarest-0.3.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     7083 1970-01-01 00:00:00.000000 pylambdarest-0.3.0rc4/PKG-INFO
```

### Comparing `pylambdarest-0.3.0rc3/LICENSE` & `pylambdarest-0.3.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylambdarest-0.3.0rc3/README.md` & `pylambdarest-0.3.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `pylambdarest-0.3.0rc3/pylambdarest/applications.py` & `pylambdarest-0.3.0rc4/pylambdarest/applications.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,34 +51,45 @@
 
         except ValidationError as err:
             return str(err).split("\n", maxsplit=1)[0]
 
         return None
 
     def _format_response(
-        self, code: int, body: Any = None, headers: Optional[dict] = None
+        self,
+        request: Request,
+        code: int,
+        body: Any = None,
+        headers: Optional[dict] = None,
     ) -> Dict[str, Any]:
         """
         Format the handler's response to the expected Lambda response format.
         """
         if not isinstance(code, int):
-            print(code, body, headers)
             raise TypeError(f"Invalid status code. {type(code)} is not int.")
         if type(headers) not in [type(None), dict]:
             raise TypeError(
                 f"Invalid headers. {type(headers)} is not in [NoneType, dict]."
             )
         response: Dict[str, Any] = {"statusCode": code}
 
         if body is not None:
             response["body"] = json.dumps(body)
 
         if self.config.ALLOW_CORS:
+            if isinstance(self.config.CORS_ORIGIN, list):
+                origin = request.headers.get("Origin") or request.headers.get(
+                    "origin"
+                )
+                if origin not in self.config.CORS_ORIGIN:
+                    origin = self.config.CORS_ORIGIN[0]
+            else:
+                origin = self.config.CORS_ORIGIN
             response["headers"] = {
-                "Access-Control-Allow-Origin": self.config.CORS_ORIGIN,
+                "Access-Control-Allow-Origin": origin,
                 "Access-Control-Allow-Credentials": self.config.CORS_ALLOW_CREDENTIALS,
             }
 
         if headers is not None:
             response["headers"] = {**response.get("headers", {}), **headers}
 
         return response
@@ -206,24 +217,28 @@
                 func_args_values: dict = {}
                 request: Request = Request(event)
 
                 if restricted is True:
                     try:
                         jwt_payload = self._check_jwt_bearer(request)
                     except AuthError:
-                        return self._format_response(401, "Unauthorized")
+                        return self._format_response(
+                            request, 401, "Unauthorized"
+                        )
 
                 validation_error = App._validate_request(
                     request,
                     body_schema_validator=body_schema_validator,
                     query_params_schema_validator=query_params_schema_validator,
                 )
                 if validation_error is not None:
                     return self._format_response(
-                        400, str(validation_error).split("\n", maxsplit=1)[0]
+                        request,
+                        400,
+                        str(validation_error).split("\n", maxsplit=1)[0],
                     )
 
                 for arg in handler_args:
                     if arg in request.path_params:
                         func_args_values[arg] = request.path_params.get(arg)
                     elif arg == "event":
                         func_args_values["event"] = event
@@ -246,12 +261,12 @@
                             f"handler got an unexpected argument '{arg}'"
                         )
 
                 res = lambda_handler(**func_args_values)
                 if not isinstance(res, tuple):
                     res = (res,)
 
-                return self._format_response(*res)
+                return self._format_response(request, *res)
 
             return wrapper
 
         return decorator
```

### Comparing `pylambdarest-0.3.0rc3/pylambdarest/config.py` & `pylambdarest-0.3.0rc4/pylambdarest/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ------
 Config object passed stored in App.
 
 """
 
 
 from enum import Enum
-from typing import Optional
+from typing import List, Optional, Union
 
 from pylambdarest.exceptions import ConfigError
 
 
 class AuthSchemeEnum(Enum):
     """
     Enumeration of the availables authentication schemes.
@@ -29,23 +29,23 @@
 
     def __init__(  # pylint: disable=R0913
         self,
         AUTH_SCHEME: Optional[AuthSchemeEnum] = None,
         JWT_SECRET: Optional[str] = None,
         JWT_ALGORITHM: Optional[str] = None,
         ALLOW_CORS: bool = False,
-        CORS_ORIGIN: Optional[str] = None,
+        CORS_ORIGIN: Optional[Union[str, List[str]]] = None,
         CORS_ALLOW_CREDENTIALS: Optional[bool] = None,
         has_jwt: Optional[bool] = None,
     ) -> None:
         self.AUTH_SCHEME: Optional[AuthSchemeEnum] = AUTH_SCHEME
         self.JWT_SECRET: Optional[str] = JWT_SECRET
         self.JWT_ALGORITHM: Optional[str] = JWT_ALGORITHM
         self.ALLOW_CORS: bool = ALLOW_CORS
-        self.CORS_ORIGIN: Optional[str] = CORS_ORIGIN
+        self.CORS_ORIGIN: Optional[Union[str, List[str]]] = CORS_ORIGIN
         self.CORS_ALLOW_CREDENTIALS: Optional[bool] = CORS_ALLOW_CREDENTIALS
 
         if (self.AUTH_SCHEME == "JWT_BEARER") and (self.JWT_SECRET is None):
             raise ConfigError(
                 "JWT_SECRET cannot be none if AUTH_SCHEME = 'JWT_BEARER'"
             )
         if self.AUTH_SCHEME == "JWT_BEARER":
```

### Comparing `pylambdarest-0.3.0rc3/pylambdarest/request.py` & `pylambdarest-0.3.0rc4/pylambdarest/request.py`

 * *Files identical despite different names*

### Comparing `pylambdarest-0.3.0rc3/pyproject.toml` & `pylambdarest-0.3.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylambdarest"
-version = "0.3.0rc3"
+version = "0.3.0rc4"
 license = "MIT"
 description = "Lightweight framework for building REST API using AWS Lambda + API Gateway"
 authors = ["Marwan Debbiche (Macbook Pro) <marwan.debbiche@gmail.com>"]
 homepage = "https://github.com/MarwanDebbiche/pylambdarest"
 repository = "https://github.com/MarwanDebbiche/pylambdarest"
 documentation = "https://pylambdarest.readthedocs.io"
 readme = "README.md"
```

### Comparing `pylambdarest-0.3.0rc3/PKG-INFO` & `pylambdarest-0.3.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylambdarest
-Version: 0.3.0rc3
+Version: 0.3.0rc4
 Summary: Lightweight framework for building REST API using AWS Lambda + API Gateway
 Home-page: https://github.com/MarwanDebbiche/pylambdarest
 License: MIT
 Keywords: aws-lambda,serverless,api-gateway,rest-api
 Author: Marwan Debbiche (Macbook Pro)
 Author-email: marwan.debbiche@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
```

