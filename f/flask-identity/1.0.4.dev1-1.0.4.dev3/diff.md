# Comparing `tmp/flask_identity-1.0.4.dev1.tar.gz` & `tmp/flask_identity-1.0.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_identity-1.0.4.dev1.tar", max compression
+gzip compressed data, was "flask_identity-1.0.4.dev3.tar", max compression
```

## Comparing `flask_identity-1.0.4.dev1.tar` & `flask_identity-1.0.4.dev3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1119 2023-05-29 12:41:30.306646 flask_identity-1.0.4.dev1/LICENSE.rst
--rw-r--r--   0        0        0     2604 2023-05-29 12:45:53.285419 flask_identity-1.0.4.dev1/README.rst
--rw-r--r--   0        0        0      905 2023-05-31 01:12:45.393303 flask_identity-1.0.4.dev1/flask_identity/__init__.py
--rw-r--r--   0        0        0     2222 2023-06-02 01:05:10.615650 flask_identity-1.0.4.dev1/flask_identity/_hash_context.py
--rw-r--r--   0        0        0     3324 2023-06-02 01:05:42.439171 flask_identity-1.0.4.dev1/flask_identity/_token_context.py
--rw-r--r--   0        0        0     1243 2023-05-31 01:12:45.379734 flask_identity-1.0.4.dev1/flask_identity/babels.py
--rw-r--r--   0        0        0      840 2023-05-31 01:12:45.404196 flask_identity-1.0.4.dev1/flask_identity/compats.py
--rw-r--r--   0        0        0     9850 2023-05-31 02:44:57.794012 flask_identity-1.0.4.dev1/flask_identity/config.py
--rw-r--r--   0        0        0    18003 2023-06-02 01:10:46.510671 flask_identity-1.0.4.dev1/flask_identity/core.py
--rw-r--r--   0        0        0    14012 2023-05-31 01:12:45.398245 flask_identity-1.0.4.dev1/flask_identity/datastore.py
--rw-r--r--   0        0        0     7829 2023-05-31 03:09:52.352538 flask_identity-1.0.4.dev1/flask_identity/decorators.py
--rw-r--r--   0        0        0     3898 2023-05-31 01:48:31.110407 flask_identity-1.0.4.dev1/flask_identity/forms.py
--rw-r--r--   0        0        0     5239 2023-05-31 01:12:45.344624 flask_identity-1.0.4.dev1/flask_identity/mixins.py
--rw-r--r--   0        0        0      823 2023-05-29 12:41:30.313443 flask_identity-1.0.4.dev1/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo
--rw-r--r--   0        0        0     1269 2023-05-29 12:41:30.313585 flask_identity-1.0.4.dev1/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po
--rw-r--r--   0        0        0     1076 2023-05-29 12:41:30.313677 flask_identity-1.0.4.dev1/flask_identity/translations/flask_identity.pot
--rw-r--r--   0        0        0      814 2023-05-29 12:41:30.313893 flask_identity-1.0.4.dev1/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo
--rw-r--r--   0        0        0     1264 2023-05-29 12:41:30.314002 flask_identity-1.0.4.dev1/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po
--rw-r--r--   0        0        0    10110 2023-05-31 01:12:45.347764 flask_identity-1.0.4.dev1/flask_identity/utils.py
--rw-r--r--   0        0        0     6203 2023-05-31 01:12:45.382128 flask_identity-1.0.4.dev1/flask_identity/views.py
--rw-r--r--   0        0        0     1747 2023-06-02 01:19:17.850269 flask_identity-1.0.4.dev1/pyproject.toml
--rw-r--r--   0        0        0     4224 1970-01-01 00:00:00.000000 flask_identity-1.0.4.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-05-29 12:41:30.306646 flask_identity-1.0.4.dev3/LICENSE.rst
+-rw-r--r--   0        0        0     2604 2023-05-29 12:45:53.285419 flask_identity-1.0.4.dev3/README.rst
+-rw-r--r--   0        0        0      905 2023-05-31 01:12:45.393303 flask_identity-1.0.4.dev3/flask_identity/__init__.py
+-rw-r--r--   0        0        0     2225 2023-06-02 15:57:07.213555 flask_identity-1.0.4.dev3/flask_identity/_hash_context.py
+-rw-r--r--   0        0        0     3325 2023-06-02 15:57:20.326013 flask_identity-1.0.4.dev3/flask_identity/_token_context.py
+-rw-r--r--   0        0        0     1243 2023-05-31 01:12:45.379734 flask_identity-1.0.4.dev3/flask_identity/babels.py
+-rw-r--r--   0        0        0      840 2023-05-31 01:12:45.404196 flask_identity-1.0.4.dev3/flask_identity/compats.py
+-rw-r--r--   0        0        0    10558 2023-06-03 13:49:39.379245 flask_identity-1.0.4.dev3/flask_identity/config.py
+-rw-r--r--   0        0        0    18255 2023-06-02 15:51:11.741304 flask_identity-1.0.4.dev3/flask_identity/core.py
+-rw-r--r--   0        0        0    14348 2023-06-02 16:01:44.758996 flask_identity-1.0.4.dev3/flask_identity/datastore.py
+-rw-r--r--   0        0        0     7825 2023-06-03 13:28:19.267568 flask_identity-1.0.4.dev3/flask_identity/decorators.py
+-rw-r--r--   0        0        0     3944 2023-06-02 15:50:19.098559 flask_identity-1.0.4.dev3/flask_identity/forms.py
+-rw-r--r--   0        0        0     5413 2023-06-02 16:07:32.388007 flask_identity-1.0.4.dev3/flask_identity/mixins.py
+-rw-r--r--   0        0        0      823 2023-05-29 12:41:30.313443 flask_identity-1.0.4.dev3/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo
+-rw-r--r--   0        0        0     1269 2023-05-29 12:41:30.313585 flask_identity-1.0.4.dev3/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po
+-rw-r--r--   0        0        0     1076 2023-05-29 12:41:30.313677 flask_identity-1.0.4.dev3/flask_identity/translations/flask_identity.pot
+-rw-r--r--   0        0        0      814 2023-05-29 12:41:30.313893 flask_identity-1.0.4.dev3/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo
+-rw-r--r--   0        0        0     1264 2023-05-29 12:41:30.314002 flask_identity-1.0.4.dev3/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po
+-rw-r--r--   0        0        0    10158 2023-06-03 13:42:18.463471 flask_identity-1.0.4.dev3/flask_identity/utils.py
+-rw-r--r--   0        0        0     6204 2023-06-02 15:59:26.317960 flask_identity-1.0.4.dev3/flask_identity/views.py
+-rw-r--r--   0        0        0     1747 2023-06-03 13:51:27.350686 flask_identity-1.0.4.dev3/pyproject.toml
+-rw-r--r--   0        0        0     4224 1970-01-01 00:00:00.000000 flask_identity-1.0.4.dev3/PKG-INFO
```

### Comparing `flask_identity-1.0.4.dev1/LICENSE.rst` & `flask_identity-1.0.4.dev3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4.dev1/README.rst` & `flask_identity-1.0.4.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4.dev1/flask_identity/__init__.py` & `flask_identity-1.0.4.dev3/flask_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4.dev1/flask_identity/_hash_context.py` & `flask_identity-1.0.4.dev3/flask_identity/_hash_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,40 +13,40 @@
 
 from passlib.context import CryptContext
 
 
 class HashContext(object):
     """
     | Class to generate/verify hash securitied string.
-    | Hashed string can used to store context or any unencrypt context.
+    | Hashed string can be used to store context or any unencrypt context.
     """
 
     def __init__(self, app) -> None:
-        secret_key = app.config.get('IDENTITY_HASH_SALT', None)
+        secret_key = app.config.get("IDENTITY_HASH_SALT", None)
 
         if secret_key is None:
-            secret_key = app.config.get('SECRET_KEY', None)
+            secret_key = app.config.get("SECRET_KEY", None)
 
         if secret_key is None:
-            raise SystemError('Config setting SECRET_KEY or IDENTITY_HASH_SALT is missing.')
+            raise SystemError("Config setting SECRET_KEY or IDENTITY_HASH_SALT is missing.")
 
-        schemes = app.config.get('IDENTITY_HASH_SCHEMES', ['bcrypt'])
-        schemes_keywords = app.config.get('IDENTITY_HASH_OPTIONS', {})
+        schemes = app.config.get("IDENTITY_HASH_SCHEMES", ["bcrypt"])
+        schemes_keywords = app.config.get("IDENTITY_HASH_OPTIONS", {})
 
         # Create a passlib CryptContext
         self.crypt_context = CryptContext(schemes, **schemes_keywords)
 
     def hash_context(self, context: str) -> str:
         """
         Hash plaintext ``context`` using the ``IDENTITY_HASH_SCHEMES`` specified in the app config.
         :param context: Plaintext string that the user types in.
         :return: hashed context.
 
         Example:
-            ``user.context = hash_context('mycontext')``
+            ``user.context = hash_context("mycontext")``
         """
 
         # Use passlib's CryptContext to hash a context
         context_hash = self.crypt_context.encrypt(context)
 
         return context_hash
 
@@ -57,12 +57,12 @@
         :param context_hash: context hash generated by a previous call to ``hash_context()``.
         :return:
             | True when ``context`` matches ``context_hash``.
             | False otherwise.
 
         Example:
             ::
-                if verify_context('mycontext', user.context):
+                if verify_context("mycontext", user.context):
                     login_user(user)
         """
         # Use passlib's CryptContext to verify a context
         return self.crypt_context.verify(context, context_hash)
```

### Comparing `flask_identity-1.0.4.dev1/flask_identity/_token_context.py` & `flask_identity-1.0.4.dev3/flask_identity/_token_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 class TokenContext(object):
     """
     | Class to generate/verify timestamped, signed and encrypted tokens.
     | Tokens can be used as cookie or request content.
     """
 
     def __init__(self, app) -> None:
-        secret_key = app.config.get('IDENTITY_TOKEN_SALT', None)
+        secret_key = app.config.get("IDENTITY_TOKEN_SALT", None)
 
         if secret_key is None:
-            secret_key = app.config.get('SECRET_KEY', None)
+            secret_key = app.config.get("SECRET_KEY", None)
 
         if secret_key is None:
-            raise SystemError('Config setting SECRET_KEY or IDENTITY_TOKEN_SALT is missing.')
+            raise SystemError("Config setting SECRET_KEY or IDENTITY_TOKEN_SALT is missing.")
 
         # Print a warning if SECRET_KEY is too short
         key = secret_key.encode()
         if len(key) < 32:
-            print('WARNING: Identity token secret key is shorter than 32 bytes.')
-            key = key + b' ' * 32  # Make sure the key is at least 32 bytes long
+            print("WARNING: Identity token secret key is shorter than 32 bytes.")
+            key = key + b" " * 32  # Make sure the key is at least 32 bytes long
 
         key32 = key[:32]
         base64_key32 = base64.urlsafe_b64encode(key32)
 
         # Create a Fernet cypher to encrypt data -- basically AES128 in CBC mode,
         # Encrypt, timestamp, sign, and base64-encode
         self.fernet = Fernet(base64_key32)
@@ -63,35 +63,35 @@
         # Convert string to bytes
         source_bytes = source.encode()
 
         # Encrypt, timestamp, sign, and base64-encode
         encrypted_bytes = self.fernet.encrypt(source_bytes)
 
         # Convert bytes to string
-        encrypted_str = encrypted_bytes.decode('utf-8')
+        encrypted_str = encrypted_bytes.decode("utf-8")
 
-        # Remove '=' padding if needed
-        token = encrypted_str.strip('=')
+        # Remove "=" padding if needed
+        token = encrypted_str.strip("=")
         return token
 
     # noinspection PyBroadException
     def verify_token(self, token: str, ttl: timedelta = None) -> dict or None:
         """
         Verify signature, verify timestamp, and decrypt a token using ``cryptography.fernet.Fernet()``.
         :return Dictionary of origin token values.
-                The keys is the index of arguments when use `*arg` with ``generate_token``,
+                The keys are the index of arguments when use `*arg` with ``generate_token``,
                 or is argument name when use `**kwargs` with ``generate_token``.
         """
         try:
-            # Add '=' padding if needed
+            # Add "=" padding if needed
             if len(token) % 4:
-                token += '=' * (4 - len(token) % 4)
+                token += "=" * (4 - len(token) % 4)
 
             # Convert string to bytes
             encrypted_bytes = token.encode()
 
             # Verify signature, verify expiration, and decrypt using ``cryptography.fernet.Fernet()``
             source_bytes = self.fernet.decrypt(encrypted_bytes, ttl.total_seconds() if ttl else None)
-            source = source_bytes.decode('utf-8')
+            source = source_bytes.decode("utf-8")
             return json.loads(source)
         except Exception:
             return None
```

### Comparing `flask_identity-1.0.4.dev1/flask_identity/babels.py` & `flask_identity-1.0.4.dev3/flask_identity/babels.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4.dev1/flask_identity/compats.py` & `flask_identity-1.0.4.dev3/flask_identity/compats.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4.dev1/flask_identity/config.py` & `flask_identity-1.0.4.dev3/flask_identity/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,190 +12,205 @@
 
 import pkg_resources
 from datetime import timedelta
 
 default_config = {
     #: Specifies the view to redirect to if a user attempts to access a URL/endpoint that they do
     #: not have permission to access. If this value is ``None``, the user is presented with a default
+    #: HTTP 401 response.
+    #: Default: ``None``.
+    "UNAUTHORIZED_VIEW": None,
+
+    #: Specifies the view to redirect to if a user attempts to access a URL/endpoint that they do
+    #: not have authentication to access. If this value is ``None``, the user is presented with a default
     #: HTTP 403 response.
     #: Default: ``None``.
-    'UNAUTHORIZED_VIEW': None,
+    "UNAUTHENTICATED_VIEW": None,
 
     #: Specifies the default view to redirect to after a user logs in. This value can be set to a URL
     #: or an endpoint name.
-    #: Default: ``'/'``.
-    'POST_LOGIN_VIEW': '/',
+    #: Default: ``"/"``.
+    "POST_LOGIN_VIEW": "/",
 
     #: Specifies the default view to redirect to after a user logs out. This value can be set to a URL
     #: or an endpoint name.
-    #: Default: ``'/'``.
-    'POST_LOGOUT_VIEW': '/',
-
-    #: The identity field used to lookup user from ``DataStore``.
-    #: The field must defined in ``UserMixin`` based user class.
-    #: Default: ``'username'``.
-    'IDENTITY_FIELD': 'username',
+    #: Default: ``"/"``.
+    "POST_LOGOUT_VIEW": "/",
 
     #: The name used to store user token in request & session.
-    #: Default: ``'token'``.
-    'IDENTITY_TOKEN_NAME': 'token',
+    #: Default: ``"token"``.
+    "IDENTITY_TOKEN_NAME": "token",
 
     #: Specifies whether should remember user when logging in.
     #: Default: ``False``.
-    'REMEMBER_ME': False,
+    "REMEMBER_ME": False,
 
     #: The page the user is attempting to access is stored in the session
-    #: or a url parameter when redirecting to the login view; This can be either
-    #: ``'session'`` (the default) or ``'request'``.
-    #: Default: ``'request'``.
-    'NEXT_STORE': 'request',
+    #: or an url parameter when redirecting to the login view; This can be either
+    #: ``"session"`` (the default) or ``"request"``.
+    #: Default: ``"request"``.
+    "NEXT_STORE": "request",
 
     #: The key to store the source url when redirecting to the login view.
     #: The key will be used as url parameter in request or key in session.
-    #: Default: ``'_next'``.
-    'NEXT_KEY': '_next',
+    #: Default: ``"_next"``.
+    "NEXT_KEY": "_next",
 
     #: Specifies the HMAC salt. This is required for all schemes that
     #: are configured for double hashing. A good salt can be generated using:
     #: ``secrets.SystemRandom().getrandbits(128)``.
     #: Defaults to ``None``.
-    'HASH_SALT': None,
+    "HASH_SALT": None,
 
     #: The salt used to encrypt session, request or cookie token.
     #: If this value is ``None`` (the default), then will use ``SECRET_KEY`` as salt
     #: to encrypt token.
     #: Strongly recommend set it to a different value for more security.
     #: Default: ``None``.
-    'TOKEN_SALT': None,
+    "TOKEN_SALT": None,
 
     #: The default time before the token expires.
     #: It's also used as the duration for "remember me" cookie.
     #: Default: ``365 days``.
-    'TOKEN_DURATION': timedelta(days=365),
+    "TOKEN_DURATION": timedelta(days=365),
 
-    #: The custom identity data store to use. This can be either ``'pony' | 'sqlalchemy' | 'mongoengine'``,
+    #: The custom identity data store to use. This can be either ``"pony" | "sqlalchemy" | "mongoengine"``,
     #: or a custom class implement from ``IdentityStore`` and ``Store``.
     #: Default: ``None``
-    'DATASTORE_ADAPTER': 'None',
+    "DATASTORE_ADAPTER": "None",
+
+    #: The identity field used to lookup user from ``DataStore``.
+    #: The field must be defined in ``UserMixin`` based user class.
+    #: Default: ``"username"``.
+    "DATASTORE_IDENTITY_FIELD": "username",
+
+    #: The identity field used to store unique token in ``DataStore``.
+    #: This will immediately render outstanding auth tokens invalid.
+    #: Default: ``"uniquifier"``.
+    "DATASTORE_UNIQUE_TOKEN_FIELD": "uniquifier",
 
     #: Specifies if Flask-Identity should track basic user login statistics.
     #: If set to ``True``, ensure your models have the required fields/attributes
     #: and make sure to commit changes after calling ``login_user``.
     #: Be sure to use `ProxyFix <http://flask.pocoo.org/docs/0.10/deploying/wsgi-standalone/#proxy-setups>`_
     #: if you are using a proxy.
     #: Defaults to ``False``
-    'TRACKABLE': False,
+    "TRACKABLE": False,
 
     #: The form field used to mark whether enable "remember me".
-    #: Default: ``'remember'``
-    'FORM_REMEBER_FIELD': 'remember',
+    #: Default: ``"remember"``
+    "FORM_REMEBER_FIELD": "remember",
+
+    #: The form field used to store the identity login for lookup in `Datastore` with `IDENTITY_FIELD`.
+    #: Default: ``"username"``
+    "FORM_IDENTITY_FIELD": "username",
 
     #: The form field used to store the url parameter when redirecting to the login view.
-    #: Default: ``'next'``
-    'FORM_NEXT_FIELD': 'next',
+    #: Default: ``"next"``
+    "FORM_NEXT_FIELD": "next",
 
     #: The name of the "remember me" cookie.
-    #: Default: ``'remember_me'``.
-    'COOKIE_NAME': 'remember_me',
+    #: Default: ``"remember_me"``.
+    "COOKIE_NAME": "remember_me",
 
     #: The session key to store cookie remember duration.
     #: It will be used when user login in.
-    #: Default: ``'remember_seconds'``.
-    'COOKIE_DURATION_SESSION_KEY': 'remember_seconds',
+    #: Default: ``"remember_seconds"``.
+    "COOKIE_DURATION_SESSION_KEY": "remember_seconds",
 
     #: The key to store "remember" stats in session.
-    #: Default: ``'remember'``.
-    'COOKIE_SESSION_STATE_KEY': 'remember',
+    #: Default: ``"remember"``.
+    "COOKIE_SESSION_STATE_KEY": "remember",
 
     #: Whether the "remember me" cookie requires "Secure" attribute.
     #: Default: ``None``.
-    'COOKIE_SECURE': None,
+    "COOKIE_SECURE": None,
 
     #: The default domain name of the "remember me" cookie.
     #: Default: ``None``.
-    'COOKIE_DOMAIN': None,
+    "COOKIE_DOMAIN": None,
 
     #: The default path of the "remember me" cookie.
-    #: Default: ``'/'``.
-    'COOKIE_PATH': "/",
+    #: Default: ``"/"``.
+    "COOKIE_PATH": "/",
 
     #: Whether the "remember me" cookie uses HttpOnly or not.
     #: Default: ``False``.
-    'COOKIE_HTTPONLY': False,
+    "COOKIE_HTTPONLY": False,
 
     #: Whether the "remember me" cookie will be refreshed by each request.
     #: Default: ``False``.
-    'COOKIE_REFRESH_EACH_REQUEST': False,
+    "COOKIE_REFRESH_EACH_REQUEST": False,
 
     #: The mode to use session protection in.
-    #: This can be either ``'basic'`` (the default) or ``'strong'``, or ``None`` to disable it.
-    #: Default: ``'basic'``.
-    'SESSION_PROTECTION': 'basic',
+    #: This can be either ``"basic"`` (the default) or ``"strong"``, or ``None`` to disable it.
+    #: Default: ``"basic"``.
+    "SESSION_PROTECTION": "basic",
 
     #: The key to store "fresh" stats in session.
-    #: Default: ``'_fresh'``.
-    'SESSION_FRESH_KEY': '_fresh',
+    #: Default: ``"_fresh"``.
+    "SESSION_FRESH_KEY": "_fresh",
 
     #: The key to store session identity in session.
-    #: Default: ``'_sid'``.
-    'SESSION_ID_KEY': '_sid',
+    #: Default: ``"_sid"``.
+    "SESSION_ID_KEY": "_sid",
 
     #: The key to pass the token in HTTP request header.
-    #: Default: ``'X-Identity-Auth'``.
-    'REQUEST_TOKEN_AUTHENTICATION_HEADER': 'X-Identity-Auth',
+    #: Default: ``"X-Identity-Auth"``.
+    "REQUEST_TOKEN_AUTHENTICATION_HEADER": "X-Identity-Auth",
 
     #: The parameter key to pass the token in HTTP request url.
-    #: Default: ``'iauth'``.
-    'REQUEST_TOKEN_AUTHENTICATION_ARG': 'iauth',
+    #: Default: ``"iauth"``.
+    "REQUEST_TOKEN_AUTHENTICATION_ARG": "iauth",
 
     #: Specifies whether use build-in blueprint for user login and logout.
     #: Default: ``True``.
-    'BLUEPRINT_ENABLED': True,
+    "BLUEPRINT_ENABLED": True,
 
     #: Specifies the name for the build-in blueprint.
-    #: Default: ``'identity'``.
-    'BLUEPRINT_NAME': 'identity',
+    #: Default: ``"identity"``.
+    "BLUEPRINT_NAME": "identity",
 
     #: Specifies the url prefix for the build-in blueprint.
-    #: Default: ``'/identity'``.
-    'BLUEPRINT_URL_PREFIX': '/identity',
+    #: Default: ``"/identity"``.
+    "BLUEPRINT_URL_PREFIX": "/identity",
 
-    #: Specifies the sub domain for the build-in blueprint.
+    #: Specifies the subdomain for the build-in blueprint.
     #: Default: ``None``.
-    'BLUEPRINT_SUBDOMAIN': None,
+    "BLUEPRINT_SUBDOMAIN": None,
 
     #: Specifies the templates folder for the build-in blueprint.
-    #: Default: ``'templates'``.
-    'BLUEPRINT_TEMPLATE_FOLDER': 'templates',
+    #: Default: ``"templates"``.
+    "BLUEPRINT_TEMPLATE_FOLDER": "templates",
 
     #: Specifies the "login" url for the build-in blueprint.
-    #: Default: ``'/login'``.
-    'BLUEPRINT_LOGIN_URL': '/login',
+    #: Default: ``"/login"``.
+    "BLUEPRINT_LOGIN_URL": "/login",
 
     #: Specifies the http method for the "login" url of the build-in blueprint.
-    #: Default: ``['GET', 'POST']``.
-    'BLUEPRINT_LOGIN_METHODS': ['GET', 'POST'],
+    #: Default: ``["GET", "POST"]``.
+    "BLUEPRINT_LOGIN_METHODS": ["GET", "POST"],
 
     #: Specifies the "logout" url for the build-in blueprint.
-    #: Default: ``'/logout'``.
-    'BLUEPRINT_LOGOUT_URL': '/logout',
+    #: Default: ``"/logout"``.
+    "BLUEPRINT_LOGOUT_URL": "/logout",
 
     #: Specifies the http method for the "logout" url of the build-in blueprint.
-    #: Default: ``['GET', 'POST']``.
-    'BLUEPRINT_LOGOUT_METHODS': ['GET', 'POST'],
+    #: Default: ``["GET", "POST"]``.
+    "BLUEPRINT_LOGOUT_METHODS": ["GET", "POST"],
 
     #: Specifies the template name for the "login" of the build-in blueprint.
-    #: Default: ``'user_login.html'``.
-    'BLUEPRINT_LOGIN_USER_TEMPLATE': 'user_login.html',
+    #: Default: ``"user_login.html"``.
+    "BLUEPRINT_LOGIN_USER_TEMPLATE": "user_login.html",
 
     #: List of accepted password hashes.
-    #: See `Passlib CryptContext docs on Constructor Keyword ``'schemes'``
-    #: Example: ``['bcrypt', 'argon2']``
-    #:      Creates new hashes with 'bcrypt' and verifies existing hashes with 'bcrypt' and 'argon2'.
-    'HASH_SCHEMES': [
+    #: See `Passlib CryptContext docs on Constructor Keyword ``"schemes"``
+    #: Example: ``["bcrypt", "argon2"]``
+    #:      Creates new hashes with "bcrypt" and verifies existing hashes with "bcrypt" and "argon2".
+    "HASH_SCHEMES": [
         "bcrypt",
         "argon2",
         "des_crypt",
         "pbkdf2_sha256",
         "pbkdf2_sha512",
         "sha256_crypt",
         "sha512_crypt",
@@ -203,64 +218,64 @@
         "plaintext",
     ],
     #: Dictionary of CryptContext keywords and hash options.
     #: See `Passlib CryptContext docs on Constructor Keywords`
     #: and `Passlib CryptContext docs on Algorithm Options`
     #: Example: ``dict(bcrypt__rounds=12, argon2__time_cost=2, argon2__memory_cost=512)``.
     #: Default: ``dict()``
-    'HASH_OPTIONS': dict(),
+    "HASH_OPTIONS": dict(),
 
     #: A set of HTTP methods which are exempt from `login_required`.
-    #: Default: ``'OPTIONS'``.
-    'EXEMPT_METHODS': ['OPTIONS'],
+    #: Default: ``"OPTIONS"``.
+    "EXEMPT_METHODS": ["OPTIONS"],
 
     #: Specifies the name for domain used for translations.
-    #: Default: ``'flask_identity'``.
-    'I18N_DOMAIN': 'flask_identity',
+    #: Default: ``"flask_identity"``.
+    "I18N_DOMAIN": "flask_identity",
 
     #: Specifies the directory containing the MO files used for translations.
     #: Default: ``[PATH_LIB]/flask_identity/translations``.
-    'I18N_DIRNAME': pkg_resources.resource_filename('flask_identity', 'translations'),
+    "I18N_DIRNAME": pkg_resources.resource_filename("flask_identity", "translations"),
 
-    #: Flask-WTF: Set to False to disable all CSRF protection.
+    #: Flask-WTF: Set to `False` to disable all CSRF protection.
     #: Default is ``True``
-    'WTF_CSRF_ENABLED': True,
+    "WTF_CSRF_ENABLED": True,
 
     #: Flask-WTF: When using the CSRF protection extension, this controls whether every view is protected by default.
     #: Default: ``True``
-    'WTF_CSRF_CHECK_DEFAULT': True,
+    "WTF_CSRF_CHECK_DEFAULT": True,
 
     #: Flask-WTF: Random data for generating secure tokens. If this is not set then SECRET_KEY is used.
     #: Default: ``None``
-    'WTF_CSRF_SECRET_KEY': None,
+    "WTF_CSRF_SECRET_KEY": None,
 
     #: Flask-WTF: HTTP methods to protect from CSRF.
-    #: Default is ``{'POST', 'PUT', 'PATCH', 'DELETE'}``
-    'WTF_CSRF_METHODS': {'POST', 'PUT', 'PATCH', 'DELETE'},
+    #: Default is ``{"POST", "PUT", "PATCH", "DELETE"}``
+    "WTF_CSRF_METHODS": {"POST", "PUT", "PATCH", "DELETE"},
 
     #: Flask-WTF: Name of the form field and session key that holds the CSRF token.
-    #: Default: ``'csrf_token'``
-    'WTF_CSRF_FIELD_NAME': 'csrf_token',
+    #: Default: ``"csrf_token"``
+    "WTF_CSRF_FIELD_NAME": "csrf_token",
 
     #: Flask-WTF: HTTP headers to search for CSRF token when it is not provided in the form.
-    #: Default: ``['X-CSRFToken', 'X-CSRF-Token']``
-    'WTF_CSRF_HEADERS': ['X-CSRFToken', 'X-CSRF-Token'],
+    #: Default: ``["X-CSRFToken", "X-CSRF-Token"]``
+    "WTF_CSRF_HEADERS": ["X-CSRFToken", "X-CSRF-Token"],
 
     #: Flask-WTF: Max age in seconds for CSRF tokens.
     #: If set to None, the CSRF token is valid for the life of the session.
     #: Default: ``3600``
-    'WTF_CSRF_TIME_LIMIT': 3600,
+    "WTF_CSRF_TIME_LIMIT": 3600,
 
     #: Flask-WTF: Whether to enforce the same origin policy by checking that the referrer matches the host.
     #: Only applies to HTTPS requests.
     #: Default: ``True``
-    'WTF_CSRF_SSL_STRICT': True,
+    "WTF_CSRF_SSL_STRICT": True,
 
-    #: Flask-WTF: Set to False to disable Flask-Babel I18N support.
+    #: Flask-WTF: Set to `False` to disable Flask-Babel I18N support.
     #: Also set to False if you want to use WTForms’s built-in messages directly.
     #: Default: ``True``
-    'WTF_I18N_ENABLED': True,
+    "WTF_I18N_ENABLED": True,
 
     #: Specifies the endpoint to ignore CSRF check.
     #: Default: ``[]``
-    'WTF_CSRF_IGNORE_UNAUTH_ENDPOINTS': []
+    "WTF_CSRF_IGNORE_UNAUTH_ENDPOINTS": []
 }
```

### Comparing `flask_identity-1.0.4.dev1/flask_identity/core.py` & `flask_identity-1.0.4.dev3/flask_identity/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self._role_model = role_model
         self._i18n_domain = None
 
         if app is not None and user_model is not None and role_model is not None:
             self.init_app(app, db, user_model, role_model, register_blueprint, **kwargs)
 
     def __getattr__(self, name):
-        if name.upper().startswith('CONFIG_'):
+        if name.upper().startswith("CONFIG_"):
             return self._config.get(name.upper(), None)
 
         return None
 
     # noinspection PyIncorrectDocstring
     def init_app(self, app, db=None, user_model=None, role_model=None, register_blueprint=None, **kwargs):
         """
@@ -100,82 +100,82 @@
             self._role_model = role_model
 
         for key, value in self._kwargs.items():
             kwargs.setdefault(key, value)
 
         default_config.update({
             #: The i8n message of ``UNAUTHENTICATED``.
-            #: Default: ``'UNAUTHENTICATED'``.
-            'MSG_UNAUTHENTICATED': (_('UNAUTHENTICATED'), 'error'),
+            #: Default: ``"UNAUTHENTICATED"``.
+            "MSG_UNAUTHENTICATED": (_("UNAUTHENTICATED"), "error"),
 
             #: The i8n message of ``UNAUTHORIZED``.
-            #: Default: ``'UNAUTHORIZED'``.
-            'MSG_UNAUTHORIZED': (_('UNAUTHORIZED'), 'error'),
+            #: Default: ``"UNAUTHORIZED"``.
+            "MSG_UNAUTHORIZED": (_("UNAUTHORIZED"), "error"),
 
             #: The i8n message of ``Invalid Redirect Url``.
             #: Default: ``INVALID REDIRECT URL``.
-            'MSG_INVALID_REDIRECT': (_('INVALID REDIRECT URL'), 'error'),
+            "MSG_INVALID_REDIRECT": (_("INVALID REDIRECT URL"), "error"),
 
             #: The i8n message of ``Anonymous User Required``.
             #: Default: ``ANONYMOUS USER REQUIRED``.
-            'MSG_ANONYMOUS_USER_REQUIRED': (_('ANONYMOUS USER REQUIRED'), 'error'),
+            "MSG_ANONYMOUS_USER_REQUIRED": (_("ANONYMOUS USER REQUIRED"), "error"),
 
             #: The i8n message of ``User Does Not Exist``.
             #: Default: ``USER DOES NOT EXIST``.
-            'MSG_USER_DOES_NOT_EXIST': (_('USER DOES NOT EXIST'), 'error'),
+            "MSG_USER_DOES_NOT_EXIST": (_("USER DOES NOT EXIST"), "error"),
 
             #: The i8n message of ``Invalid password``.
             #: Default: ``INVALID PASSWORD``.
-            'MSG_INVALID_PASSWORD': (_('INVALID PASSWORD'), 'error'),
+            "MSG_INVALID_PASSWORD": (_("INVALID PASSWORD"), "error"),
 
             #: The i8n message of ``Account Is Disabled``.
             #: Default: ``ACCOUNT IS DISABLED``.
-            'MSG_DISABLED_ACCOUNT': (_('ACCOUNT IS DISABLED'), 'error'),
+            "MSG_DISABLED_ACCOUNT": (_("ACCOUNT IS DISABLED"), "error"),
         })
 
         for key, value in default_config.items():
-            app.config.setdefault('IDENTITY_' + key.upper(), value)
+            app.config.setdefault("IDENTITY_" + key.upper(), value)
 
         for key, value in get_config(app).items():
             kwargs[key.upper()] = value
 
         for key, value in kwargs.items():
             if hasattr(self, key.lower()):
                 setattr(self, key.lower(), value)
 
             self._config[key.upper()] = value
 
-        delattr(self, '_kwargs')
+        delattr(self, "_kwargs")
 
-        adapter = self._config['DATASTORE_ADAPTER']
+        adapter = self._config["DATASTORE_ADAPTER"]
 
-        if adapter == 'pony':
+        if adapter == "pony":
             from .datastore import PonyIdentityStore
             self._datastore = PonyIdentityStore(db, self._user_model, self._role_model)
-        elif adapter == 'sqlalchemy':
+        elif adapter == "sqlalchemy":
             from .datastore import SQLAlchemyIdentityStore
             self._datastore = SQLAlchemyIdentityStore(db, self._user_model, self._role_model)
-        elif adapter == 'mongoengine':
+        elif adapter == "mongoengine":
             from .datastore import MongoEngineIdentityStore
             self._datastore = MongoEngineIdentityStore(db, self._user_model, self._role_model)
         if isclass(adapter):
             self._datastore = adapter(db, self._user_model, self._role_model)
 
         self._hash_context = HashContext(app)
         self._token_context = TokenContext(app)
 
-        app.extensions['identity'] = self
+        app.extensions["identity"] = self
 
         app.after_request(self._update_remember_cookie)
         app.context_processor(self._default_context_processor)
 
         self.app = app
 
         if register_blueprint is None:
-            register_blueprint = self._config.get('BLUEPRINT_ENABLED', True)
+            register_blueprint = self._config.get("BLUEPRINT_ENABLED", True)
             self._register_blueprint = register_blueprint
 
         if register_blueprint:
             create_blueprint(self, __name__, app.json)
 
         self._i18n_domain = get_i18n_domain(app)
 
@@ -189,16 +189,16 @@
 
     def _add_ctx_processor(self, endpoint, fn):
         group = self._context_processors.setdefault(endpoint, [])
         fn not in group and group.append(fn)
 
     def _run_ctx_processor(self, endpoint):
         rv = {}
-        for g in [None, endpoint]:
-            for fn in self._context_processors.setdefault(g, []):
+        for ep in [None, endpoint]:
+            for fn in self._context_processors.setdefault(ep, []):
                 rv.update(fn())
         return rv
 
     def context_processor(self, endpoint, fn):
         self._add_ctx_processor(endpoint, fn)
 
     def unauthenticated_handler(self, fn):
@@ -243,27 +243,28 @@
         # Check SESSION_PROTECTION
         if self._session_protection_failed():
             return self.update_request_context_with_user()
 
         user = None
 
         # Load user from Flask Session
-        token = session.get(self._config['IDENTITY_TOKEN_NAME'])
+        token = session.get(self._config["IDENTITY_TOKEN_NAME"])
         if token is not None:
             data = self._token_context.verify_token(token)
             if data is not None:
                 user = self._load_user_from_datastore(
-                    data[self._config['IDENTITY_FIELD']], data.get('uniquifier', None)
+                    data.get(self._config["DATASTORE_IDENTITY_FIELD"], None),
+                    data.get(self._config["DATASTORE_UNIQUE_TOKEN_FIELD"], None)
                 )
 
         # Load user from Remember Me Cookie or Request Loader
         if user is None:
-            cookie_name = self._config['COOKIE_NAME']
+            cookie_name = self._config["COOKIE_NAME"]
             has_cookie = (
-                    cookie_name in request.cookies and session.get(self._config['COOKIE_SESSION_STATE_KEY']) != 'clear'
+                    cookie_name in request.cookies and session.get(self._config["COOKIE_SESSION_STATE_KEY"]) != "clear"
             )
             if has_cookie:
                 cookie = request.cookies[cookie_name]
                 user = self._load_user_from_cookie(cookie)
             else:
                 # noinspection PyTypeChecker
                 user = self._load_user_from_request(request)
@@ -275,31 +276,31 @@
         | If caller wants JSON - return 403
         | Otherwise - assume caller is html and redirect to ``IDENTITY_UNAUTHENTICATED_VIEW`` or 403
         """
         if self._unauthn_handler:
             return self._unauthn_handler()
 
         return self._unauth_response(
-            msg=self._config['MSG_UNAUTHENTICATED'],
-            view=self._config['UNAUTHENTICATED_VIEW'],
+            msg=self._config["MSG_UNAUTHENTICATED"],
+            view=self._config["UNAUTHENTICATED_VIEW"],
             code=403,
             header=header
         )
 
     def unauthorized(self, header=None):
         """
         | If caller wants JSON - return 401
         | Otherwise - assume caller is html and redirect to ``IDENTITY_UNAUTHORIZED_VIEW`` or 401
         """
         if self._unauthz_handler:
             return self._unauthz_handler()
 
         return self._unauth_response(
-            msg=self._config['MSG_UNAUTHORIZED'],
-            view=self._config['UNAUTHORIZED_VIEW'],
+            msg=self._config["MSG_UNAUTHORIZED"],
+            view=self._config["UNAUTHORIZED_VIEW"],
             code=401,
             header=header
         )
 
     def update_request_context_with_user(self, user=None):
         """
         :param user: User object
@@ -311,167 +312,169 @@
     def datastore(self) -> IdentityStore:
         """
         :return: The datastore of Identity Manager
         """
         return self._datastore
 
     def _load_user_from_datastore(self, identity_field, uniquifier=None):
+        unique_token_field = self._config["DATASTORE_UNIQUE_TOKEN_FIELD"]
         user = self._datastore.find_user(identity_field)
         if not user or not user.is_actived:
             return None
-        if not uniquifier and user and hasattr(user, 'uniquifier') and getattr(user, 'uniquifier') != uniquifier:
-            return None
+        if uniquifier and unique_token_field:
+            if hasattr(user, unique_token_field) and getattr(user, unique_token_field) != uniquifier:
+                return None
         return user
 
     def _load_user_from_cookie(self, cookie):
         # noinspection PyBroadException
         try:
-            data = self._token_context.verify_token(cookie, ttl=self._config['TOKEN_DURATION'])
-            identity_id = data[self._config['IDENTITY_FIELD']]
+            data = self._token_context.verify_token(cookie, ttl=self._config["TOKEN_DURATION"])
+            identity_id = data[self._config["DATASTORE_IDENTITY_FIELD"]]
             if identity_id is not None:
-                user = self._load_user_from_datastore(identity_id, data.get('uniquifier', None))
+                user = self._load_user_from_datastore(
+                    identity_id, data.get(self._config["DATASTORE_UNIQUE_TOKEN_FIELD"], None))
                 if user is not None:
-                    session[self._config['IDENTITY_TOKEN_NAME']] = user.get_auth_token()
-                    session[self._config['SESSION_FRESH_KEY']] = False
+                    session[self._config["IDENTITY_TOKEN_NAME"]] = user.get_auth_token()
+                    session[self._config["SESSION_FRESH_KEY"]] = False
                     return user
         except Exception:
             pass
 
         return self._anonymous_user()
 
     def _load_user_from_request(self, req):
-        header_key = self._config['REQUEST_TOKEN_AUTHENTICATION_HEADER']
-        args_key = self._config['REQUEST_TOKEN_AUTHENTICATION_ARG']
+        header_key = self._config["REQUEST_TOKEN_AUTHENTICATION_HEADER"]
+        args_key = self._config["REQUEST_TOKEN_AUTHENTICATION_ARG"]
         header_token = req.headers.get(header_key, None)
         token = req.args.get(args_key, header_token)
         if req.is_json:
             data = req.get_json(silent=True) or {}
             if isinstance(data, dict):
                 token = data.get(args_key, token)
 
         # noinspection PyBroadException
         try:
-            data = self._token_context.verify_token(token, ttl=self._config['TOKEN_DURATION'])
-            identity_field = data[self._config['IDENTITY_FIELD']]
-            user = self._load_user_from_datastore(identity_field, data.get('uniquifier', None))
+            data = self._token_context.verify_token(token, ttl=self._config["TOKEN_DURATION"])
+            identity_field = data[self._config["DATASTORE_IDENTITY_FIELD"]]
+            user = self._load_user_from_datastore(identity_field, data.get(identity_field, None))
             if user is not None:
                 return user
         except Exception:
             pass
 
         return self._anonymous_user()
 
     # noinspection PyMethodMayBeStatic
     def _get_remote_addr(self):
-        address = request.headers.get('X-Forwarded-For', request.remote_addr)
+        address = request.headers.get("X-Forwarded-For", request.remote_addr)
         if address is not None:
-            # An 'X-Forwarded-For' header includes a comma separated list of the
+            # An "X-Forwarded-For" header includes a comma separated list of the
             # addresses, the first address being the actual remote address.
-            address = address.encode('utf-8').split(b',')[0].strip()
+            address = address.encode("utf-8").split(b",")[0].strip()
         return address
 
     # noinspection PyMethodMayBeStatic
     def _session_identifier_generator(self):
-        user_agent = request.headers.get('User-Agent')
+        user_agent = request.headers.get("User-Agent")
         if user_agent is not None:
-            user_agent = user_agent.encode('utf-8')
-        base = '{0}|{1}'.format(self._get_remote_addr(), user_agent)
+            user_agent = user_agent.encode("utf-8")
+        base = "{0}|{1}".format(self._get_remote_addr(), user_agent)
         h = sha512()
-        h.update(base.encode('utf8'))
+        h.update(base.encode("utf8"))
         return h.hexdigest()
 
     # noinspection PyUnresolvedReferences,PyProtectedMember
     def _session_protection_failed(self):
         sess = session._get_current_object()
         ident = self._session_identifier_generator()
-        mode = self._config['SESSION_PROTECTION']
+        mode = self._config["SESSION_PROTECTION"]
 
-        if not mode or mode not in ['basic', 'strong']:
+        if not mode or mode not in ["basic", "strong"]:
             return False
 
-        # if the sess is empty, it's an anonymous user or just logged out
-        # so we can skip this
-        if ident != session.get(self._config['SESSION_ID_KEY'], None):
-            if mode == 'basic' or sess.permanent:
-                sess[self._config['SESSION_FRESH_KEY']] = False
+        # if the sess is empty, it's an anonymous user or just logged out, so we can skip this
+        if ident != session.get(self._config["SESSION_ID_KEY"], None):
+            if mode == "basic" or sess.permanent:
+                sess[self._config["SESSION_FRESH_KEY"]] = False
                 return False
-            elif mode == 'strong':
+            elif mode == "strong":
                 for k in _SESSION_KEYS:
                     sess.pop(k, None)
 
-                sess[self._config['COOKIE_SESSION_STATE_KEY']] = 'clear'
+                sess[self._config["COOKIE_SESSION_STATE_KEY"]] = "clear"
                 return True
 
         return False
 
     @staticmethod
     def _default_context_processor():
         return dict(current_user=get_user(), url_for_identity=url_for_identity)
 
     def _update_remember_cookie(self, response):
-        # Don't modify the session unless there's something to do.
-        remeber_key = self._config['COOKIE_SESSION_STATE_KEY']
+        # Don"t modify the session unless there"s something to do.
+        remeber_key = self._config["COOKIE_SESSION_STATE_KEY"]
         if remeber_key not in session and \
-                self._config['COOKIE_REFRESH_EACH_REQUEST']:
-            session[remeber_key] = 'set'
+                self._config["COOKIE_REFRESH_EACH_REQUEST"]:
+            session[remeber_key] = "set"
 
         if remeber_key in session:
             operation = session.pop(remeber_key, None)
 
-            if operation == 'set' and self._config['IDENTITY_TOKEN_NAME'] in session:
+            if operation == "set" and self._config["IDENTITY_TOKEN_NAME"] in session:
                 self._set_cookie(response)
-            elif operation == 'clear':
+            elif operation == "clear":
                 clear_cookie(response)
 
         return response
 
     def _set_cookie(self, response):
         # cookie settings
-        cookie_name = self._config['COOKIE_NAME']
-        domain = self._config['COOKIE_DOMAIN']
-        path = self._config['COOKIE_PATH']
-
-        secure = self._config['COOKIE_SECURE']
-        httponly = self._config['COOKIE_HTTPONLY']
-        cookie_duration_session_key = self._config['COOKIE_DURATION_SESSION_KEY']
+        cookie_name = self._config["COOKIE_NAME"]
+        domain = self._config["COOKIE_DOMAIN"]
+        path = self._config["COOKIE_PATH"]
+
+        secure = self._config["COOKIE_SECURE"]
+        httponly = self._config["COOKIE_HTTPONLY"]
+        cookie_duration_session_key = self._config["COOKIE_DURATION_SESSION_KEY"]
 
         if cookie_duration_session_key in session:
             duration = timedelta(seconds=session[cookie_duration_session_key])
         else:
-            duration = self._config['TOKEN_DURATION']
+            duration = self._config["TOKEN_DURATION"]
 
         # prepare data
-        data = session[self._config['IDENTITY_TOKEN_NAME']]
+        data = session[self._config["IDENTITY_TOKEN_NAME"]]
 
         if isinstance(duration, int):
             duration = timedelta(seconds=duration)
 
         try:
             expires = datetime.utcnow() + duration
         except TypeError:
-            raise Exception('Duration must be a datetime.timedelta, instead got: {0}'.format(duration))
+            raise Exception("Duration must be a datetime.timedelta, instead got: {0}".format(duration))
 
         # actually set it
         response.set_cookie(cookie_name, value=data, expires=expires, domain=domain, path=path, secure=secure,
                             httponly=httponly)
 
     # noinspection PyMethodMayBeStatic
-    def _unauth_response(self, msg, view, code, header, redirect_to='/'):
+    def _unauth_response(self, msg, view, code, header, redirect_to="/"):
         if request.is_json:
             return render_json(msg, code, header)
 
-        next_key = self._config['NEXT_KEY']
+        next_key = self._config["NEXT_KEY"]
 
         if view:
             if callable(view):
                 view = view()
             else:
                 try:
-                    if self._config['NEXT_STORE'] == 'session':
-                        session[self._config['SESSION_ID_KEY']] = self._session_identifier_generator()
+                    if self._config["NEXT_STORE"] == "session":
+                        session[self._config["SESSION_ID_KEY"]] = self._session_identifier_generator()
                         session[next_key] = base64_encode_param(request.url)
                         view = get_url(view)
                 except BuildError:
                     view = None
 
             if request.referrer and not request.referrer.split("?")[0].endswith(request.path):
                 redirect_to = request.referrer
```

### Comparing `flask_identity-1.0.4.dev1/flask_identity/datastore.py` & `flask_identity-1.0.4.dev3/flask_identity/datastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,55 +146,57 @@
     """
     Abstracted user identity store.
 
     :param user_model: A user model class definition
     :param role_model: A role model class definition
 
     Be aware that for mutating operations, the user/role will be added to the
-    store (by calling self.put(<object>). If the datastore is session based
+    store (by calling self.put(<object>)). If the datastore is session based
     (such as for SQLAlchemyDatastore) it is up to caller to actually
     commit the transaction by calling datastore.commit().
     """
 
     def __init__(self, user_model, role_model):
         self.user_model = user_model
         self.role_model = role_model
 
     def _prepare_role_modify_args(self, user, role):
         if not isinstance(user, self.user_model):
-            user = self.find_user(**{config_value('IDENTITY_FIELD'): user})
+            user = self.find_user(**{config_value("DATASTORE_IDENTITY_FIELD"): user})
         if isinstance(role, str):
-            role = self.find_role(**{'name': role})
+            role = self.find_role(**{"name": role})
         return user, role
 
     def _prepare_create_user_args(self, **kwargs):
         kwargs.setdefault("active", True)
         roles = kwargs.get("roles", [])
         for i, role in enumerate(roles):
             rn = role.name if isinstance(role, self.role_model) else role
             # see if the role exists
             roles[i] = self.find_role(rn)
         kwargs["roles"] = roles
-        if hasattr(self.user_model, "uniquifier"):
-            kwargs.setdefault("uniquifier", uuid.uuid4().hex)
+
+        unique_token_field = config_value("DATASTORE_UNIQUE_TOKEN_FIELD", default="uniquifier")
+        if hasattr(self.user_model, unique_token_field):
+            kwargs.setdefault(unique_token_field, uuid.uuid4().hex)
         return kwargs
 
     def find_user(self, *args, **kwargs):
         """Returns a user matching the provided parameters."""
         raise NotImplementedError
 
     def find_role(self, *args, **kwargs):
         """Returns a role matching the provided name."""
         raise NotImplementedError
 
     def add_role_to_user(self, user, role):
         """
         Adds a role to a user.
 
-        :param user: The user to manipulate. Can be an User object or lookup key id with ``'IDENTITY_IDENTITY_FIELD'``
+        :param user: The user to manipulate. Can be a User object or lookup key id with ``"IDENTITY_DATASTORE_IDENTITY_FIELD"``
         :param role: The role to add to the user. Can be a Role object or
             string role name
         """
         user, role = self._prepare_role_modify_args(user, role)
         if role not in user.roles:
             user.roles.append(role)
             # noinspection PyUnresolvedReferences
@@ -203,15 +205,15 @@
 
         return False
 
     def remove_role_from_user(self, user, role):
         """
         Removes a role from a user.
 
-        :param user: The user to manipulate. Can be an User object or lookup key id with ``'IDENTIT_IDENTITY_FIELD'``
+        :param user: The user to manipulate. Can be a User object or lookup key id with ``"IDENTIT_DATASTORE_IDENTITY_FIELD"``
         :param role: The role to remove from the user. Can be a Role object or
             string role name
         """
         rv = False
         user, role = self._prepare_role_modify_args(user, role)
         if role in user.roles:
             rv = True
@@ -265,21 +267,23 @@
         Set user's authentication token uniquifier.
         This will immediately render outstanding auth tokens invalid.
 
         :param user: User to modify
         :param uniquifier: Unique value - if none then uuid.uuid4().hex is used
 
         This method is a no-op if the user model doesn't contain the attribute
-        ``uniquifier``
+        ``DATASTORE_UNIQUE_TOKEN_FIELD``
         """
-        if not hasattr(user, "uniquifier"):
+        unique_token_field = config_value("DATASTORE_UNIQUE_TOKEN_FIELD", default="uniquifier")
+        if not hasattr(user, unique_token_field):
             return
         if not uniquifier:
             uniquifier = uuid.uuid4().hex
-        user.uniquifier = uniquifier
+
+        setattr(user, unique_token_field, uniquifier)
         # noinspection PyUnresolvedReferences
         self.save(user)
 
     def create_role(self, **kwargs):
         """
         Creates and returns a new role from the given parameters.
         Supported params (depending on RoleModel):
@@ -328,21 +332,21 @@
 
     def __init__(self, db, user_model, role_model):
         IdentityStore.__init__(self, user_model, role_model)
         PonyStore.__init__(self, db)
 
     def find_user(self, *args, **kwargs):
         if len(args) > 0:
-            kwargs.update({config_value('IDENTITY_FIELD'): args[0]})
+            kwargs.update({config_value("DATASTORE_IDENTITY_FIELD"): args[0]})
 
         return self.get(self.user_model, **kwargs)
 
     def find_role(self, *args, **kwargs):
         if len(args) > 0:
-            kwargs.update({config_value('IDENTITY_FIELD'): args[0]})
+            kwargs.update({config_value("DATASTORE_IDENTITY_FIELD"): args[0]})
 
         return self.get(self.role_model, **kwargs)
 
 
 class SQLAlchemyStore(Store):
     """
     Implements the DbAdapter interface to find, add, update and delete
@@ -357,15 +361,15 @@
 
     def delete(self, obj):
         self.db.session.delete(obj)
 
     def find(self, objectclass, **kwargs):
         query = objectclass.query
         for field_name, field_value in kwargs.items():
-            # Make sure that ObjectClass has a 'field_name' property
+            # Make sure that ObjectClass has a "field_name" property
             field = getattr(objectclass, field_name, None)
             if field is None:
                 raise KeyError(
                     "BaseAlchemyAdapter.find_first_object(): Class '%s' has no field '%s'." % (objectclass, field_name)
                 )
 
             # Add a filter to the query
@@ -373,21 +377,21 @@
 
         # Execute query
         return query.all()
 
     def get(self, objectclass, **kwargs):
         query = objectclass.query
         for field_name, field_value in kwargs.items():
-            # Make sure that ObjectClass has a 'field_name' property
+            # Make sure that ObjectClass has a "field_name" property
             field = getattr(objectclass, field_name, None)
             if field is None:
                 raise KeyError(
                     "BaseAlchemyAdapter.find_first_object(): Class '%s' has no field '%s'." % (objectclass, field_name))
 
-            # Add a case sensitive filter to the query
+            # Add a case-sensitive filter to the query
             query = query.filter(field == field_value)  # case sensitive!!
 
         # Execute query
         return query.first()
 
     def save(self, obj):
         self.db.session.add(obj)
@@ -401,21 +405,21 @@
     """
     def __init__(self, db, user_model, role_model):
         IdentityStore.__init__(self, user_model, role_model)
         SQLAlchemyStore.__init__(self, db)
 
     def find_user(self, *args, **kwargs):
         if len(args) > 0:
-            kwargs.update({config_value('IDENTITY_FIELD'): args[0]})
+            kwargs.update({config_value("DATASTORE_IDENTITY_FIELD"): args[0]})
 
         return self.get(self.user_model, **kwargs)
 
     def find_role(self, *args, **kwargs):
         if len(args) > 0:
-            kwargs.update({config_value('IDENTITY_FIELD'): args[0]})
+            kwargs.update({config_value("DATASTORE_IDENTITY_FIELD"): args[0]})
 
         return self.get(self.role_model, **kwargs)
 
 
 class MongoEngineStore(Store):
     """
     Implements the DbAdapter interface to find, add, update and delete
@@ -446,16 +450,16 @@
     """
     def __init__(self, db, user_model, role_model):
         IdentityStore.__init__(self, user_model, role_model)
         MongoEngineStore.__init__(self, db)
 
     def find_user(self, *args, **kwargs):
         if len(args) > 0:
-            kwargs.update({config_value('IDENTITY_FIELD'): args[0]})
+            kwargs.update({config_value("DATASTORE_IDENTITY_FIELD"): args[0]})
 
         return self.user_model.objects(**kwargs).first()
 
     def find_role(self, *args, **kwargs):
         if len(args) > 0:
-            kwargs.update({config_value('IDENTITY_FIELD'): args[0]})
+            kwargs.update({config_value("DATASTORE_IDENTITY_FIELD"): args[0]})
 
         return self.role_model.objects(**kwargs).first()
```

### Comparing `flask_identity-1.0.4.dev1/flask_identity/decorators.py` & `flask_identity-1.0.4.dev3/flask_identity/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,24 +31,24 @@
     if user and user.is_authenticated:
         current_identity.update_request_context_with_user(user)
         return True
 
     return False
 
 
-def auth_required(*auth_methods):
+def auth_required(auth_methods=()):
     """
     Decorator that protects endpoints through multiple mechanisms.
 
     Example::
 
-        @app.route('/dashboard')
-        @auth_required('token', 'session')
+        @app.route("/dashboard")
+        @auth_required("token", "session")
         def dashboard():
-            return 'Dashboard'
+            return "Dashboard"
 
     :param auth_methods: Specified mechanisms (token, session). If not specified
         then all current available mechanisms will be tried.
 
     Note that regardless of order specified - they will be tried in the following
     order: token, session.
 
@@ -89,15 +89,15 @@
 def login_required(view_function):
     """
     Ensure that the current user is logged in and authenticated before calling
     the actual view.
 
     For example::
 
-        @app.route('/post')
+        @app.route("/post")
         @login_required
         def post():
             pass
 
     .. Note ::
 
         Per `W3 guidelines for CORS preflight requests
@@ -105,15 +105,15 @@
         HTTP ``OPTIONS`` requests are exempt from login checks.
 
     :param view_function: The view function to decorate.
     :type view_function: function
     """
     @wraps(view_function)
     def decorated_view(*args, **kwargs):
-        if request.method in config_value('EXEMPT_METHODS'):
+        if request.method in config_value("EXEMPT_METHODS"):
             return view_function(*args, **kwargs)
         elif not current_user.is_authenticated:
             return current_identity.unauthorized()
         return view_function(*args, **kwargs)
 
     return decorated_view
 
@@ -121,28 +121,28 @@
 def roles_required(*role_names):
     """
     This decorator ensures that the current user is logged in,
     and has *all* of the specified roles (AND operation).
 
     Example::
 
-        @route('/escape')
-        @roles_required('Special', 'Agent')
-        def escape_capture():  # User must be 'Special' AND 'Agent'
+        @route("/escape")
+        @roles_required("Special", "Agent")
+        def escape_capture():  # User must be "Special" AND "Agent"
             ...
 
     Calls unauthenticated_view() when the user is not logged in
     or when user is not actived.
 
     Calls unauthorized_view() when the user does not have the required roles.
 
     Calls the decorated view otherwise.
     """
     def wrapper(view_function):
-        @wraps(view_function)    # Tells debuggers that is is a function wrapper
+        @wraps(view_function)    # Tells debuggers that is a function wrapper
         def decorator(*args, **kwargs):
             # User must have the required roles
             if not current_user.is_actived or not current_user.has_roles(*role_names):
                 # Redirect to the unauthorized page
                 return current_identity.unauthorized()
 
             # It's OK to call the view
@@ -156,49 +156,49 @@
 def roles_accepted(*role_names):
     """
     This decorator ensures that the current user is logged in,
     and has *at least one* of the specified roles (OR operation).
 
     Example::
 
-        @route('/edit_article')
-        @roles_accepted('Writer', 'Editor')
-        def edit_article():  # User must be 'Writer' OR 'Editor'
+        @route("/edit_article")
+        @roles_accepted("Writer", "Editor")
+        def edit_article():  # User must be "Writer" OR "Editor"
             ...
 
     Calls unauthenticated_view() when the user is not logged in
     or when user is not actived.
 
     Calls unauthorized_view() when the user does not have the required roles.
 
     Calls the decorated view otherwise.
     """
     # convert the list to a list containing that list.
     # Because roles_required(a, b) requires A AND B
     # while roles_required([a, b]) requires A OR B
     def wrapper(view_function):
-        @wraps(view_function)  # Tells debuggers that is is a function wrapper
+        @wraps(view_function)  # Tells debuggers that is a function wrapper
         def decorator(*args, **kwargs):
             # User must have the required roles
-            # NB: roles_required would call has_roles(*role_names): ('A', 'B') --> ('A', 'B')
-            # But: roles_accepted must call has_roles(role_names):  ('A', 'B') --< (('A', 'B'),)
+            # NB: roles_required would call has_roles(*role_names): ("A", "B") --> ("A", "B")
+            # But: roles_accepted must call has_roles(role_names):  ("A", "B") --< (("A", "B"),)
             if not current_user.is_actived() or not current_user.has_roles(role_names):
                 # Redirect to the unauthorized page
                 return current_identity.unauthorized()
 
             # It's OK to call the view
             return view_function(*args, **kwargs)
 
         return decorator
 
     return wrapper
 
 
 def unauth_csrf(fall_through=False):
-    """Decorator for endpoints that don't need authentication
+    """Decorator for endpoints that don"t need authentication
     but do want CSRF checks (available via Header rather than just form).
     This is required when setting *WTF_CSRF_CHECK_DEFAULT* = **False** since in that
     case, without this decorator, the form validation will attempt to do the CSRF
     check, and that will fail since the csrf-token is in the header (for pure JSON
     requests).
 
     This decorator does nothing unless Flask-WTF::CSRFProtect has been initialized.
@@ -209,17 +209,17 @@
 
     This decorator will suppress CSRF if caller isn't authenticated and has set the
     *WTF_CSRF_IGNORE_UNAUTH_ENDPOINTS* config variable.
 
     :param fall_through: if set to True, then if CSRF fails here - simply keep going.
         This is appropriate if underlying view is form based and once the form is
         instantiated, the csrf_token will be available.
-        Note that this can mask some errors such as 'The CSRF session token is missing.'
+        Note that this can mask some errors such as "The CSRF session token is missing."
         meaning that the caller didn't send a session cookie and instead the caller
-        might get a 'The CSRF token is missing.' error.
+        might get a "The CSRF token is missing." error.
     """
 
     def wrapper(fn):
         @wraps(fn)
         def decorated(*args, **kwargs):
             if not current_app.config.get("WTF_CSRF_ENABLED", False) or not current_app.extensions.get("csrf", None):
                 return fn(*args, **kwargs)
```

### Comparing `flask_identity-1.0.4.dev1/flask_identity/forms.py` & `flask_identity-1.0.4.dev3/flask_identity/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             payload.update(additional)
 
         return payload
 
 
 class NextFormMixin:
     def __init__(self, *args, **kwargs):
-        self._NEXT_FIELD = config_value('FORM_NEXT_FIELD')
+        self._NEXT_FIELD = config_value("FORM_NEXT_FIELD")
         setattr(NextFormMixin, self._NEXT_FIELD, HiddenField(self._NEXT_FIELD))
 
     # noinspection PyMethodMayBeStatic
     def validate_next(self, field):
         if field.data and not validate_redirect_url(field.data):
             field.data = ""
             flash(config_value("MSG_INVALID_REDIRECT"))
@@ -50,60 +50,60 @@
 
 
 class LoginForm(BaseForm, NextFormMixin):
     """
     The default login form
     """
 
-    password = PasswordField('password', validators=[DataRequired()], default='')
+    password = PasswordField("password", validators=[DataRequired()], default="")
 
     def __init__(self, *args, **kwargs):
         NextFormMixin.__init__(self, *args, **kwargs)
 
         self.user = None
-        self.next_url = None
 
-        self._IDENTITY_FIELD = config_value('IDENTITY_FIELD')
-        self._REMEBER_FIELD = config_value('FORM_REMEBER_FIELD')
+        self._IDENTITY_FIELD = config_value("FORM_IDENTITY_FIELD")
+        self._REMEBER_FIELD = config_value("FORM_REMEBER_FIELD")
 
         _unbound_fields = set(self._unbound_fields)
 
         setattr(LoginForm, self._IDENTITY_FIELD,
-                StringField(self._IDENTITY_FIELD, validators=[DataRequired()], default=''))
+                StringField(self._IDENTITY_FIELD, validators=[DataRequired()], default=""))
         setattr(LoginForm, self._REMEBER_FIELD, BooleanField(self._REMEBER_FIELD))
 
         _unbound_fields.add((self._IDENTITY_FIELD, getattr(self, self._IDENTITY_FIELD)))
         _unbound_fields.add((self._REMEBER_FIELD, getattr(self, self._REMEBER_FIELD)))
         _unbound_fields.add((self._NEXT_FIELD, getattr(self, self._NEXT_FIELD)))
 
         self._unbound_fields = list(_unbound_fields)
 
         BaseForm.__init__(self, *args, **kwargs)
 
-        if not self.next.data:
-            next_key = config_value('NEXT_KEY')
-            if config_value('NEXT_STORE') == 'request':
+        if not getattr(self, self._NEXT_FIELD).data:
+            next_key = config_value("NEXT_KEY")
+            if config_value("NEXT_STORE") == "request":
                 getattr(self, self._NEXT_FIELD).data = request.args.get(next_key, "")
             else:
                 getattr(self, self._NEXT_FIELD).data = session.get(next_key, "")
 
         getattr(self, self._REMEBER_FIELD).default = config_value("DEFAULT_REMEMBER_ME")
 
     def validate(self, extra_validators=None):
         if not super().validate():
             return False
 
-        self.user = current_identity.datastore.find_user(**{self._IDENTITY_FIELD: self.data[self._IDENTITY_FIELD]})
+        id_field = config_value("DATASTORE_IDENTITY_FIELD")
+        self.user = current_identity.datastore.find_user(**{id_field: self.data[self._IDENTITY_FIELD]})
 
         if self.user is None:
-            getattr(self, self._IDENTITY_FIELD).errors.append(get_message('USER_DOES_NOT_EXIST')[0])
+            getattr(self, self._IDENTITY_FIELD).errors.append(get_message("USER_DOES_NOT_EXIST")[0])
             return False
 
         if not self.user.verify_password(self.password.data):
-            self.password.errors.append(get_message('INVALID_PASSWORD')[0])
+            self.password.errors.append(get_message("INVALID_PASSWORD")[0])
             return False
 
         if not self.user.is_actived:
-            getattr(self, self._IDENTITY_FIELD).errors.append(get_message('DISABLED_ACCOUNT')[0])
+            getattr(self, self._IDENTITY_FIELD).errors.append(get_message("DISABLED_ACCOUNT")[0])
             return False
 
         return True
```

### Comparing `flask_identity-1.0.4.dev1/flask_identity/mixins.py` & `flask_identity-1.0.4.dev3/flask_identity/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,52 +34,52 @@
             ...
     """
 
     __hash__ = object.__hash__
 
     @property
     def is_actived(self):
-        return True if not hasattr(self, 'active') else self.active
+        return True if not hasattr(self, "active") else self.active
 
     @property
     def is_authenticated(self):
         return True
 
     @property
     def is_anonymous(self):
         return False
 
     def get_id(self):
         try:
             return str(self.id)
         except AttributeError:
-            raise NotImplementedError('No `id` attribute - override `get_id`')
+            raise NotImplementedError("No `id` attribute - override `get_id`")
 
     def has_roles(self, *requirements):
         """
-        Return True if the user has all of the specified roles. Return False otherwise.
+        Return True if the user has all the specified roles. Return False otherwise.
 
         has_roles() accepts a list of requirements:
             has_roles(requirement1, requirement2, requirement3).
 
         Each requirement is either a role_name, or a tuple_of_role_names.
-            role_name example:   'manager'
-            tuple_of_role_names: ('funny', 'witty', 'hilarious')
+            role_name example:   "manager"
+            tuple_of_role_names: ("funny", "witty", "hilarious")
 
         A role_name-requirement is accepted when the user has this role.
         A tuple_of_role_names-requirement is accepted when the user has ONE of these roles.
 
-        has_roles() returns true if ALL of the requirements have been accepted.
+        has_roles() returns true if `ALL` the requirements have been accepted.
 
         For example:
-            has_roles('a', ('b', 'c'), d)
+            has_roles("a", ("b", "c"), d)
         Translates to:
-            User has role 'a' AND (role 'b' OR role 'c') AND role 'd'
+            User has role "a" AND (role "b" OR role "c") AND role "d"
         """
-        roles = getattr(self, 'roles') if hasattr(self, 'roles') else ()
+        roles = getattr(self, "roles") if hasattr(self, "roles") else ()
         role_names = [(r.name if isinstance(r, RoleMixin) else r) for r in roles]
 
         for requirement in requirements:
             if isinstance(requirement, (list, tuple)):
                 tuple_of_role_names = requirement
                 authorized = False
                 for role_name in tuple_of_role_names:
@@ -103,31 +103,32 @@
         """
         Constructs the user's authentication token.
 
         This data **MUST** be securely signed using the identity token_context
         """
         from .utils import current_identity
 
-        field = current_identity.config_value('IDENTITY_FIELD')
-        uniquifier = getattr(self, 'uniquifier') if hasattr(self, 'uniquifier') else None
+        identity_field = current_identity.config_value("DATASTORE_IDENTITY_FIELD")
+        unique_token_field = current_identity.config_value("DATASTORE_UNIQUE_TOKEN_FIELD", default="uniquifier")
+        uniquifier = getattr(self, unique_token_field) if hasattr(self, unique_token_field) else None
 
         # noinspection PyProtectedMember
         return current_identity._token_context.generate_token({
-            field: getattr(self, field),
-            'uniquifier': uniquifier
+            identity_field: getattr(self, identity_field),
+            unique_token_field: uniquifier
         })
 
     def get_security_payload(self):
         """Serialize user object as response payload."""
         from .utils import current_identity
 
-        field = current_identity.config_value('IDENTITY_FIELD')
-        uniquifier = getattr(self, 'uniquifier') if hasattr(self, 'uniquifier') else None
+        field = current_identity.config_value("DATASTORE_IDENTITY_FIELD")
+        uniquifier = getattr(self, "uniquifier") if hasattr(self, "uniquifier") else None
 
-        return {"id": str(self.id), field: getattr(self, field), 'uniquifier': uniquifier}
+        return {"id": str(self.id), field: getattr(self, field), "uniquifier": uniquifier}
 
     def verify_password(self, passwd):
         """Verify password"""
         from .utils import current_identity
 
         # noinspection PyProtectedMember
         return current_identity._hash_context.verify_context(passwd, self.password)
```

### Comparing `flask_identity-1.0.4.dev1/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo` & `flask_identity-1.0.4.dev3/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4.dev1/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po` & `flask_identity-1.0.4.dev3/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4.dev1/flask_identity/translations/flask_identity.pot` & `flask_identity-1.0.4.dev3/flask_identity/translations/flask_identity.pot`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4.dev1/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo` & `flask_identity-1.0.4.dev3/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4.dev1/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po` & `flask_identity-1.0.4.dev3/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4.dev1/flask_identity/utils.py` & `flask_identity-1.0.4.dev3/flask_identity/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     :license: MIT, see LICENSE for more details.
 """
 
 from datetime import datetime
 from urllib.parse import parse_qsl, urlsplit, urlunsplit, urlencode
 
 # noinspection PyProtectedMember
-from flask import current_app, has_request_context, request, session, url_for, _request_ctx_stack
+from flask import current_app, has_request_context, request, session, url_for, g
 from itsdangerous import base64_decode, base64_encode
 from werkzeug.local import LocalProxy
 
 from .mixins import UserMixin
 
 current_user = LocalProxy(lambda: get_user())
-current_identity = LocalProxy(lambda: current_app.extensions['identity'])
+current_identity = LocalProxy(lambda: current_app.extensions["identity"])
 # noinspection PyProtectedMember
 localize_callback = LocalProxy(lambda: current_identity._i18n_domain.gettext)
 
 
 def _(translate):
     """Identity function to mark strings for translation."""
     return translate
@@ -38,15 +38,15 @@
 
 def login_user(user: UserMixin, uniquifier=None, remember=None, duration=None, fresh=True):
     """
     Logs a user in. You should pass the actual user object to this. If the
     user's `is_active` property is ``False``, they will not be logged in
     unless `force` is ``True``.
 
-    This will return ``True`` if the log in attempt succeeds, and ``False`` if
+    This will return ``True`` if the login attempt success, and ``False`` if
     it fails (i.e. because the user is inactive).
 
     :param user: The user object to log in.
     :type user: object
     :param uniquifier: The uniquifier for isolate login session. If ``None`` will
         use a ``uuid.hex()`` as default. Defatuls to ``None``.
     :type uniquifier: str
@@ -59,15 +59,15 @@
     :param fresh: setting this to ``False`` will log in the user with a session
         marked as not "fresh". Defaults to ``True``.
     :type fresh: bool
     """
     if not user.is_actived:
         return False
 
-    if config_value('TRACKABLE'):
+    if config_value("TRACKABLE"):
         remote_addr = request.remote_addr or None  # make sure it is None
 
         old_current_login, new_current_login = (
             user.current_login_at,
             datetime.now()
         )
         old_current_ip, new_current_ip = user.current_login_ip, remote_addr
@@ -76,84 +76,85 @@
         user.current_login_at = new_current_login
         user.last_login_ip = old_current_ip
         user.current_login_ip = new_current_ip
         user.login_count = user.login_count + 1 if user.login_count else 1
 
         current_identity.datastore.save(user)
 
-    if hasattr(user, 'uniquifier'):
+    unique_token_field = config_value("DATASTORE_UNIQUE_TOKEN_FIELD", default="uniquifier")
+    if unique_token_field and hasattr(user, unique_token_field):
         current_identity.datastore.set_uniquifier(user, uniquifier)
 
-    remember = config_value('REMEMBER_ME') if remember is None else remember
+    remember = config_value("REMEMBER_ME") if remember is None else remember
 
     # noinspection PyProtectedMember
-    session[config_value('IDENTITY_TOKEN_NAME')] = user.get_auth_token()
+    session[config_value("IDENTITY_TOKEN_NAME")] = user.get_auth_token()
 
     # noinspection PyProtectedMember
-    session[config_value('SESSION_ID_KEY')] = current_identity._session_identifier_generator()
-    session[config_value('SESSION_FRESH_KEY')] = fresh
+    session[config_value("SESSION_ID_KEY")] = current_identity._session_identifier_generator()
+    session[config_value("SESSION_FRESH_KEY")] = fresh
 
     if remember:
-        session[config_value('COOKIE_SESSION_STATE_KEY')] = 'set'
-        duration = config_value('TOKEN_DURATION') if duration is None else duration
+        session[config_value("COOKIE_SESSION_STATE_KEY")] = "set"
+        duration = config_value("TOKEN_DURATION") if duration is None else duration
         try:
-            session[config_value('COOKIE_DURATION_SESSION_KEY')] = duration.total_seconds()
+            session[config_value("COOKIE_DURATION_SESSION_KEY")] = duration.total_seconds()
         except AttributeError:
-            raise Exception('duration must be a datetime.timedelta, instead got: {0}'.format(duration))
+            raise Exception("duration must be a datetime.timedelta, instead got: {0}".format(duration))
 
     current_identity.update_request_context_with_user(user)
 
     return True
 
 
 def logout_user():
     """
     Logs a user out. (You do not need to pass the actual user.) This will
     also clean up the remember me cookie if it exists.
     """
-    id_key = config_value('IDENTITY_TOKEN_NAME')
+    id_key = config_value("IDENTITY_TOKEN_NAME")
     if id_key in session:
         session.pop(id_key)
 
-    fresh = config_value('SESSION_FRESH_KEY')
+    fresh = config_value("SESSION_FRESH_KEY")
     if fresh in session:
         session.pop(fresh)
-    sid = config_value('SESSION_ID_KEY')
+    sid = config_value("SESSION_ID_KEY")
     if sid in session:
         session.pop(sid)
 
-    cookie_name = config_value('COOKIE_NAME')
+    cookie_name = config_value("COOKIE_NAME")
     if cookie_name in request.cookies:
-        session[config_value('COOKIE_SESSION_STATE_KEY')] = 'clear'
-        remember_seconds = config_value('COOKIE_DURATION_SESSION_KEY')
+        session[config_value("COOKIE_SESSION_STATE_KEY")] = "clear"
+        remember_seconds = config_value("COOKIE_DURATION_SESSION_KEY")
         if remember_seconds in session:
             session.pop(remember_seconds)
 
     current_identity.update_request_context_with_user()
 
     return True
 
 
 def base64_encode_param(endpoint_or_url, qparams=None):
     param = get_url(endpoint_or_url, qparams)
-    return base64_encode(param).decode('utf-8')
+    return base64_encode(param).decode("utf-8")
 
 
 def base64_decode_param(param):
-    return param if not param else base64_decode(param).decode('utf-8')
+    return param if not param else base64_decode(param).decode("utf-8")
 
 
 # noinspection PyBroadException
 def get_url(endpoint_or_url, qparams=None):
     """
     Returns a URL if a valid endpoint is found. Otherwise, returns the
     provided value.
 
-    :param endpoint_or_url: The endpoint name or URL to default to
-    :param qparams: additional query params to add to end of url
+    :param endpoint_or_url: The endpoint name or URL to default to.
+    :param qparams: additional query params to add to end of then url.
     :return: URL
     """
     try:
         return transform_url(url_for(endpoint_or_url), qparams)
     except Exception:
         return transform_url(endpoint_or_url, qparams)
 
@@ -190,29 +191,29 @@
 
 
 def json_error_response(errors):
     """
     Helper to create an error response that adheres to the openapi spec.
     """
     if isinstance(errors, str):
-        # When the errors is a string, use the response/error/message format
+        # When the errors are string, use the response/error/message format
         response_json = dict(error=errors)
     elif isinstance(errors, dict):
-        # When the errors is a dict, use the DefaultJsonErrorResponse
+        # When the errors are dict, use the DefaultJsonErrorResponse
         # (response/errors/name/messages) format
         response_json = dict(errors=errors)
     else:
         raise TypeError("The errors argument should be either a str or dict.")
 
     return response_json
 
 
 def get_post_action_redirect(config_key, declared=None):
-    next_key = config_value('NEXT_KEY')
-    next_field = config_value('FORM_NEXT_FIELD')
+    next_key = config_value("NEXT_KEY")
+    next_field = config_value("FORM_NEXT_FIELD")
 
     urls = [
         base64_decode_param(get_url(request.args.get(next_key, None))),
         base64_decode_param(get_url(request.form.get(next_field, None))),
         base64_decode_param(get_url(session.get(next_key, None))),
         find_redirect("IDENTITY_" + config_key),
     ]
@@ -244,37 +245,37 @@
         or "/"
     )
     return rv
 
 
 def config_value(key, app=None, default=None):
     """
-    Get a Identity configuration value.
+    Get an Identity configuration value.
 
     :param key: The configuration key without the prefix `IDENTITY_`
     :param app: An optional specific application to inspect. Defaults to
                 Flask's `current_app`
     :param default: An optional default value if the value is not set
     """
     app = app or current_app
     return get_config(app).get(key.upper(), default)
 
 
 def get_config(app):
     """
     Conveniently get the security configuration for the specified
-    application without the 'IDENTITY_' prefix.
+    application without the "IDENTITY_" prefix.
 
     :param app: The `Flask` application to inspect
     """
     items = app.config.items()
-    prefix = 'IDENTITY_'
+    prefix = "IDENTITY_"
 
     def strip_prefix(tup):
-        return tup[0].replace('IDENTITY_', '', 1), tup[1]
+        return tup[0].replace("IDENTITY_", "", 1), tup[1]
 
     return dict([strip_prefix(i) for i in items if i[0].startswith(prefix)])
 
 
 def hash_password(password):
     """
     Hash the specified plaintext password.
@@ -294,19 +295,19 @@
                           (usually from your database)
     """
     # noinspection PyProtectedMember
     return current_identity._hash_context.verify_context(password, password_hash)
 
 
 def clear_cookie(response):
-    cookie_name = config_value('COOKIE_NAME')
-    domain = config_value('COOKIE_DOMAIN')
-    path = config_value('COOKIE_PATH')
+    cookie_name = config_value("COOKIE_NAME")
+    domain = config_value("COOKIE_DOMAIN")
+    path = config_value("COOKIE_PATH")
 
     response.delete_cookie(cookie_name, domain=domain, path=path)
 
 
 def get_user():
-    if has_request_context() and not hasattr(_request_ctx_stack.top, 'user'):
+    if has_request_context() and not hasattr(g, "user"):
         current_identity.get_current_user()
 
-    return getattr(_request_ctx_stack.top, 'user', None)
+    return g.user
```

### Comparing `flask_identity-1.0.4.dev1/flask_identity/views.py` & `flask_identity-1.0.4.dev3/flask_identity/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     Return a URL for the Flask-Identity blueprint.
 
     This is method is a wrapper of :meth:``Flask.url_for``.
 
     :param endpoint: the endpoint of the URL (name of the function)
     :param values: the variable arguments of the URL rule
     """
-    blueprint_name = current_identity.config_value('BLUEPRINT_NAME')
+    blueprint_name = current_identity.config_value("BLUEPRINT_NAME")
     if blueprint_name is None:
-        raise RuntimeError('Blueprint not registed!')
+        raise RuntimeError("Blueprint not registed!")
 
     return url_for(f"{blueprint_name}.{endpoint}", **values)
 
 
 def render_json(payload, code, headers):
     """
     Default JSON response handler.
@@ -109,18 +109,18 @@
     Allow already authenticated users. For GET this is useful for
     single-page-applications on refresh - session still active but need to
     access user info and csrf-token.
     For POST - redirects to POST_LOGIN_VIEW (forms) or returns 400 (json).
     """
     if current_user.is_authenticated and request.method == "POST":
         # Just redirect current_user to POST_LOGIN_VIEW (or next).
-        # While its tempting to try to logout the current user and login the
+        # While it's tempting to try to log out the current user and login the
         # new requested user - that simply doesn't work with CSRF.
         if request.is_json:
-            return render_json(config_value('MSG_ANONYMOUS_USER_REQUIRED'), 400, None)
+            return render_json(config_value("MSG_ANONYMOUS_USER_REQUIRED"), 400, None)
         else:
             return redirect(get_post_login_redirect())
 
     form_class = current_identity.login_form
     if form_class is None:
         from .forms import LoginForm
         form_class = LoginForm
@@ -130,15 +130,15 @@
             form = form_class(MultiDict(request.get_json()))
         else:
             form = form_class(MultiDict([]))
     else:
         form = form_class(request.form)
 
     if form.validate_on_submit():
-        remember_me = form.remember.data if config_value('FORM_REMEBER_FIELD') in form else None
+        remember_me = form.remember.data if config_value("FORM_REMEBER_FIELD") in form else None
         login_user(form.user, remember=remember_me)
         after_this_request(_commit)
 
         if not request.is_json:
             return redirect(get_post_login_redirect())
 
     if request.is_json:
@@ -161,35 +161,35 @@
     """
     View function which handles a logout request.
     """
 
     if current_user.is_authenticated:
         logout_user()
 
-    # No body is required - so if a POST and json - return OK
+    # Nobody is required - so if a POST and json - return OK
     if request.method == "POST" and request.is_json:
         return render_json({}, 200, headers=None)
 
     return redirect(get_post_logout_redirect())
 
 
 def create_blueprint(identity, import_name, json_encoder=None):
     """Creates the identity extension blueprint"""
 
     bp = Blueprint(
-        identity.config_value('BLUEPRINT_NAME'),
+        identity.config_value("BLUEPRINT_NAME"),
         import_name,
-        url_prefix=identity.config_value('BLUEPRINT_URL_PREFIX'),
-        subdomain=identity.config_value('BLUEPRINT_SUBDOMAIN'),
-        template_folder=identity.config_value('BLUEPRINT_TEMPLATE_FOLDER'),
+        url_prefix=identity.config_value("BLUEPRINT_URL_PREFIX"),
+        subdomain=identity.config_value("BLUEPRINT_SUBDOMAIN"),
+        template_folder=identity.config_value("BLUEPRINT_TEMPLATE_FOLDER"),
     )
 
     if json_encoder:
         bp.json_encoder = json_encoder
 
-    bp.route(identity.config_value('BLUEPRINT_LOGIN_URL'),
-             methods=identity.config_value('BLUEPRINT_LOGIN_METHODS'), endpoint="login")(login)
+    bp.route(identity.config_value("BLUEPRINT_LOGIN_URL"),
+             methods=identity.config_value("BLUEPRINT_LOGIN_METHODS"), endpoint="login")(login)
 
-    bp.route(identity.config_value('BLUEPRINT_LOGOUT_URL'),
-             methods=identity.config_value('BLUEPRINT_LOGOUT_METHODS'), endpoint="logout")(logout)
+    bp.route(identity.config_value("BLUEPRINT_LOGOUT_URL"),
+             methods=identity.config_value("BLUEPRINT_LOGOUT_METHODS"), endpoint="logout")(logout)
 
     identity.app.register_blueprint(bp)
```

### Comparing `flask_identity-1.0.4.dev1/pyproject.toml` & `flask_identity-1.0.4.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
 priority = "supplemental"
 
 [tool.poetry]
 name = "Flask-Identity"
-version = "1.0.4dev1"
+version = "1.0.4dev3"
 description = "A lightweight extension & library to security Flask applications quickly and simply."
 authors = ["SolardiaX <solardiax@hotmail.com>"]
 maintainers = ["SolardiaX <solardiax@hotmail.com>"]
 license = "MIT"
 readme="README.rst"
 repository="https://github.com/SolardiaX/flask-identity"
 homepage="https://github.com/SolardiaX/flask-identity"
```

### Comparing `flask_identity-1.0.4.dev1/PKG-INFO` & `flask_identity-1.0.4.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-identity
-Version: 1.0.4.dev1
+Version: 1.0.4.dev3
 Summary: A lightweight extension & library to security Flask applications quickly and simply.
 Home-page: https://github.com/SolardiaX/flask-identity
 License: MIT
 Author: SolardiaX
 Author-email: solardiax@hotmail.com
 Maintainer: SolardiaX
 Maintainer-email: solardiax@hotmail.com
```

