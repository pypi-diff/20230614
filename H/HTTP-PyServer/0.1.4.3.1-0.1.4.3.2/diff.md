# Comparing `tmp/HTTP-PyServer-0.1.4.3.1.tar.gz` & `tmp/HTTP-PyServer-0.1.4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.1.4.3.1.tar", last modified: Tue Jun 13 18:45:01 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.1.4.3.2.tar", last modified: Wed Jun 14 04:15:45 2023, max compression
```

## Comparing `HTTP-PyServer-0.1.4.3.1.tar` & `HTTP-PyServer-0.1.4.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:45:01.073362 HTTP-PyServer-0.1.4.3.1/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4.3.1/LICENSE
--rw-rw-rw-   0        0        0     2108 2023-06-13 18:45:01.072364 HTTP-PyServer-0.1.4.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2023-06-11 01:47:44.000000 HTTP-PyServer-0.1.4.3.1/README.md
--rw-rw-rw-   0        0        0      645 2023-06-13 18:44:48.000000 HTTP-PyServer-0.1.4.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 18:45:01.073362 HTTP-PyServer-0.1.4.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 18:45:00.987591 HTTP-PyServer-0.1.4.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 18:45:01.017510 HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2108 2023-06-13 18:45:00.000000 HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-13 18:45:00.000000 HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:45:00.000000 HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 18:45:00.000000 HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 18:45:01.069373 HTTP-PyServer-0.1.4.3.1/src/server/
--rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4.3.1/src/server/__init__.py
--rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4.3.1/src/server/cache.py
--rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4.3.1/src/server/render.py
--rw-rw-rw-   0        0        0     4667 2023-06-12 00:04:01.000000 HTTP-PyServer-0.1.4.3.1/src/server/request.py
--rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4.3.1/src/server/response.py
--rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4.3.1/src/server/response_codes.py
--rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4.3.1/src/server/response_messages.py
--rw-rw-rw-   0        0        0     8866 2023-06-11 23:42:15.000000 HTTP-PyServer-0.1.4.3.1/src/server/routes.py
--rw-rw-rw-   0        0        0     7390 2023-06-13 18:43:49.000000 HTTP-PyServer-0.1.4.3.1/src/server/server.py
--rw-rw-rw-   0        0        0     3588 2023-06-11 23:50:14.000000 HTTP-PyServer-0.1.4.3.1/src/server/sessions.py
--rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4.3.1/src/server/template.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:15:45.273543 HTTP-PyServer-0.1.4.3.2/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2108 2023-06-14 04:15:45.272546 HTTP-PyServer-0.1.4.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-06-11 01:47:44.000000 HTTP-PyServer-0.1.4.3.2/README.md
+-rw-rw-rw-   0        0        0      645 2023-06-14 04:15:18.000000 HTTP-PyServer-0.1.4.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 04:15:45.274541 HTTP-PyServer-0.1.4.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 04:15:44.891525 HTTP-PyServer-0.1.4.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 04:15:45.048636 HTTP-PyServer-0.1.4.3.2/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2108 2023-06-14 04:15:44.000000 HTTP-PyServer-0.1.4.3.2/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-14 04:15:44.000000 HTTP-PyServer-0.1.4.3.2/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 04:15:44.000000 HTTP-PyServer-0.1.4.3.2/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 04:15:44.000000 HTTP-PyServer-0.1.4.3.2/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 04:15:45.270553 HTTP-PyServer-0.1.4.3.2/src/server/
+-rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4.3.2/src/server/__init__.py
+-rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4.3.2/src/server/cache.py
+-rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4.3.2/src/server/render.py
+-rw-rw-rw-   0        0        0     4894 2023-06-14 04:14:32.000000 HTTP-PyServer-0.1.4.3.2/src/server/request.py
+-rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4.3.2/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4.3.2/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4.3.2/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     8941 2023-06-14 04:13:31.000000 HTTP-PyServer-0.1.4.3.2/src/server/routes.py
+-rw-rw-rw-   0        0        0     7552 2023-06-14 04:14:29.000000 HTTP-PyServer-0.1.4.3.2/src/server/server.py
+-rw-rw-rw-   0        0        0     3588 2023-06-11 23:50:14.000000 HTTP-PyServer-0.1.4.3.2/src/server/sessions.py
+-rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4.3.2/src/server/template.py
```

### Comparing `HTTP-PyServer-0.1.4.3.1/LICENSE` & `HTTP-PyServer-0.1.4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3.1/PKG-INFO` & `HTTP-PyServer-0.1.4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.4.3.1
+Version: 0.1.4.3.2
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.4.3.1/README.md` & `HTTP-PyServer-0.1.4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3.1/pyproject.toml` & `HTTP-PyServer-0.1.4.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.1.4.3.1"
+version = "0.1.4.3.2"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.1.4.3.2/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.4.3.1
+Version: 0.1.4.3.2
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.4.3.1/src/server/cache.py` & `HTTP-PyServer-0.1.4.3.2/src/server/cache.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3.1/src/server/render.py` & `HTTP-PyServer-0.1.4.3.2/src/server/render.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3.1/src/server/request.py` & `HTTP-PyServer-0.1.4.3.2/src/server/request.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,15 +93,17 @@
     def cookies(self) -> dict[str, list[str]]:
         '''Returns the request cookies as a dictionary.'''
 
         try:
 
             cookies = {}
 
-            for cookie in self.headers.get('Cookie').split(';'):
+            raw_cookies = self.headers.get('Cookie') or self.headers.get('cookie')
+
+            for cookie in raw_cookies.split(';'):
 
                 key, value = list(urllib.parse.parse_qs(cookie.strip()).items())[0]
 
                 cookies[key] = value[0]
 
             return cookies
         
@@ -120,16 +122,19 @@
 
         return urllib.parse.parse_qs(self.body.decode(encoding = 'utf-8',
                                                       errors = 'ignore'))
     
     def files(self) -> dict[str, bytes]:
 
         try:
+
+            content_type = self.headers.get('Content-Type') or\
+            self.headers.get('content-type')
         
-            boundry = self.headers.get('Content-Type').split('; ')[1].split('=')[1]
+            boundry = content_type.split('; ')[1].split('=')[1]
 
             parts = self.body.split(b'--' + boundry.encode(encoding = 'utf-8',
                                     errors = 'ignore') + b'\r\n')[1:]
             
             parts[-1] = parts[-1].split(b'--' + boundry.encode(encoding = 'utf-8',
                                     errors = 'ignore') + b'--\r\n')[0]
 
@@ -148,15 +153,16 @@
                 full_header = full_header.decode(encoding = 'utf-8',
                                                  errors = 'ignore').split('\r\n')
 
                 headers = {name: value for name, value in 
                            [header.split(': ') for header in full_header]}
                 
                 if filename:=(
-                   headers.get('Content-Disposition').split('=')[-1].strip('"')):
+                   (headers.get('Content-Disposition') or \
+                    headers.get('content-disposition')).split('=')[-1].strip('"')):
 
                     files[filename] = body
 
             except Exception:
 
                 continue
```

### Comparing `HTTP-PyServer-0.1.4.3.1/src/server/response.py` & `HTTP-PyServer-0.1.4.3.2/src/server/response.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3.1/src/server/response_codes.py` & `HTTP-PyServer-0.1.4.3.2/src/server/response_codes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3.1/src/server/response_messages.py` & `HTTP-PyServer-0.1.4.3.2/src/server/response_messages.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3.1/src/server/routes.py` & `HTTP-PyServer-0.1.4.3.2/src/server/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,16 @@
                                                  session,
                                                  *wildcard_values)
                     
                     if isinstance(message, str):
 
                         message = render.text(text = message)
 
-                    if cookies:=message.headers.get('Set-Cookie'):
+                    if cookies:=(message.headers.get('Set-Cookie') or \
+                                 message.headers.get('set-cookie')):
 
                         cookies += f', SESSION_ID={session.id}; \
 Expires={session.expires}'
 
                         message.headers['Set-Cookie'] = cookies
 
                     else:
```

### Comparing `HTTP-PyServer-0.1.4.3.1/src/server/server.py` & `HTTP-PyServer-0.1.4.3.2/src/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,16 @@
                         self._logger.error(f'Invalid request from \
 {address[0]}:{address[1]}, closing connection.')
 
                     connection.close()
 
                     return None
 
-                if content_length:=parsed_request.headers.get('Content-Length'):
+                if content_length:=(parsed_request.headers.get('Content-Length') or \
+                                    parsed_request.headers.get('content-length')):
 
                     content_length = int(content_length)
                         
                     while (body_length:=len(raw_request.split(b'\r\n\r\n', 1)[1]))\
                     < (content_length):
 
                         raw_request += connection.recv(content_length - body_length)
@@ -197,15 +198,16 @@
                                                 request = parsed_request))
                 
                 if self._logger:
 
                     self._logger.debug(f'Sent {parsed_request.method} response to \
 {address[0]}:{address[1]} for {parsed_request.path if parsed_request.path else "/"}')
 
-                if not parsed_request.headers.get('Connection') == 'keep-alive':
+                if not (parsed_request.headers.get('Connection') or \
+                        parsed_request.headers.get('connection')) == 'keep-alive':
 
                     try:
                 
                         connection.close()
 
                     except Exception:
```

### Comparing `HTTP-PyServer-0.1.4.3.1/src/server/sessions.py` & `HTTP-PyServer-0.1.4.3.2/src/server/sessions.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3.1/src/server/template.py` & `HTTP-PyServer-0.1.4.3.2/src/server/template.py`

 * *Files identical despite different names*

