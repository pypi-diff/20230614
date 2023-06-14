# Comparing `tmp/pyporscheconnectapi-0.0.9.tar.gz` & `tmp/pyporscheconnectapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyporscheconnectapi-0.0.9.tar", last modified: Sun Jun 20 20:57:47 2021, max compression
+gzip compressed data, was "pyporscheconnectapi-0.1.1.tar", last modified: Wed Jun 14 20:54:16 2023, max compression
```

## Comparing `pyporscheconnectapi-0.0.9.tar` & `pyporscheconnectapi-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 johan      (501) staff       (20)        0 2021-06-20 20:57:47.256555 pyporscheconnectapi-0.0.9/
--rw-r--r--   0 johan      (501) staff       (20)     1071 2021-01-26 22:38:51.000000 pyporscheconnectapi-0.0.9/LICENSE
--rw-r--r--   0 johan      (501) staff       (20)      472 2021-06-20 20:57:47.256679 pyporscheconnectapi-0.0.9/PKG-INFO
--rw-r--r--   0 johan      (501) staff       (20)     3678 2021-06-20 20:52:35.000000 pyporscheconnectapi-0.0.9/README.md
-drwxr-xr-x   0 johan      (501) staff       (20)        0 2021-06-20 20:57:47.254428 pyporscheconnectapi-0.0.9/pyporscheconnectapi/
--rw-r--r--   0 johan      (501) staff       (20)        0 2021-02-01 22:27:05.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi/__init__.py
--rw-r--r--   0 johan      (501) staff       (20)     5607 2021-06-20 20:52:35.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi/cli.py
--rw-r--r--   0 johan      (501) staff       (20)    12891 2021-06-20 20:52:35.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi/client.py
--rw-r--r--   0 johan      (501) staff       (20)     9263 2021-06-20 20:52:35.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi/connection.py
--rw-r--r--   0 johan      (501) staff       (20)     1409 2021-02-03 07:49:14.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi/exceptions.py
-drwxr-xr-x   0 johan      (501) staff       (20)        0 2021-06-20 20:57:47.256338 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/
--rw-r--r--   0 johan      (501) staff       (20)      472 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/PKG-INFO
--rw-r--r--   0 johan      (501) staff       (20)      453 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/SOURCES.txt
--rw-r--r--   0 johan      (501) staff       (20)        1 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/dependency_links.txt
--rw-r--r--   0 johan      (501) staff       (20)       60 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/entry_points.txt
--rw-r--r--   0 johan      (501) staff       (20)       10 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/requires.txt
--rw-r--r--   0 johan      (501) staff       (20)       20 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/top_level.txt
--rw-r--r--   0 johan      (501) staff       (20)      123 2021-06-20 20:57:47.257078 pyporscheconnectapi-0.0.9/setup.cfg
--rwxr-xr-x   0 johan      (501) staff       (20)      831 2021-06-20 20:54:02.000000 pyporscheconnectapi-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:54:16.728671 pyporscheconnectapi-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 20:54:16.728671 pyporscheconnectapi-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:54:16.724671 pyporscheconnectapi-0.1.1/pyporscheconnectapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19856 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:54:16.728671 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 20:54:16.728671 pyporscheconnectapi-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/setup.py
```

### Comparing `pyporscheconnectapi-0.0.9/LICENSE` & `pyporscheconnectapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.0.9/README.md` & `pyporscheconnectapi-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # pyporscheconnectapi
 A python library for Porsche Connect API
 
-This is a very early release, things are changing rapidly so use at your own risk!
+This library will let you access your car equipped with Porsche Connect. It does not work with the predecessor Porsche Car Connect.
+Porsche Connect is available for the following Porsche models:
+
+* Taycan
+* 911 (from 992)
+* Cayenne (from 2017, E3)
+* Panamera (from 2021, G2 PA)
+
+You can also take a look here, select your model and see if your model has support for Porsche Connect:
+https://connect-store.porsche.com/
+
+A Porsche Connect subscription alse needs to be active for it to work.
 
 *NOTE:* This work is not officially supported by Porsche and functionality can stop working at any time without warning
 
 ## Installation
 
 The easiest method is to install using pip3/pip (venv is also a good idea)
 ```
@@ -21,15 +32,15 @@
 Setup will add a cli under the name porschecli, see below for usage
 
 
 ## CLI usage
 
 A simple cli is provided with this library, it will cache tokens to a file to speed up invocations. It does not yet support the create/update/delete timer functionality which is present in the library.
 
-If no email or password is supplied as input arguments you will be prompted. Same goes for PIN (used to lock or unlock).
+If no email or password is supplied as input arguments and no config file with those details is found you will be prompted. Same goes for PIN (used to lock or unlock).
 The --nowait option will just request the action (or stored information) without waiting for confirmation.
 ```
 usage: cli.py [-h] [-e EMAIL] [-p PASSWORD] [-s SESSION_FILE] [-v VIN]
               [-n PIN] [-m MODEL] [-a] [-c COUNTRY] [-l LANGUAGE]
               [-z TIMEZONE] [--nowait]
               {list,overview,maintenance,summary,capabilities,emobility,position,triplongterm,tripshortterm,speedalerts,theftalerts,tokens,lock,unlock,climate-on,climate-off,directcharge-on,directcharge-off}
 
@@ -49,14 +60,28 @@
   -a, --all
   -c COUNTRY, --country COUNTRY
   -l LANGUAGE, --language LANGUAGE
   -z TIMEZONE, --timezone TIMEZONE
   --nowait
 ```
 
+## Config file (for CLI)
+
+A config file is searched for in ~/.porscheconnect.cfg and ./.porscheconnect.cfg
+The format is:
+
+```
+[porsche]
+email=<your email>
+password=<your password>
+country=<country iso code, default DE>
+language=<lang abbreviation, default de>
+timezone=<default Europe/Stockholm>
+```
+
 ## Library usage
 
 Install pyporscheconnectapi using pip (requires python > 3.6)
 
 
 ### Example client usage
 ```
```

### Comparing `pyporscheconnectapi-0.0.9/pyporscheconnectapi/connection.py` & `pyporscheconnectapi-0.1.1/pyporscheconnectapi/connection.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,216 +11,307 @@
 import time
 import base64
 import hashlib
 import os
 import re
 import urllib.parse
 from typing import Dict, Text
+from bs4 import BeautifulSoup
 
 import aiohttp
-from yarl import URL
+
+try:
+    from rich import print
+except ImportError:
+    pass
 
 from .exceptions import WrongCredentials, PorscheException
 
 _LOGGER = logging.getLogger(__name__)
 
 
+async def on_request_start(session, trace_config_ctx, params):
+    _LOGGER.debug("Starting request")
+    _LOGGER.debug(params)
+
+
+async def on_request_end(session, trace_config_ctx, params):
+    _LOGGER.debug("Ending request")
+    _LOGGER.debug(params)
+
+
+trace_config = aiohttp.TraceConfig()
+trace_config.on_request_start.append(on_request_start)
+trace_config.on_request_end.append(on_request_end)
+
+AUTHORIZATION_SERVER="identity.porsche.com"
+REDIRECT_URI="https://my.porsche.com/"
+AUDIENCE="https://api.porsche.com"
+TENANT="porsche-production"
+COUNTRY="de"
+LANGUAGE="de_DE"
+CLIENT_ID="UYsK00My6bCqJdbQhTQ0PbWmcSdIAMig"
+
+
+
 class Connection:
     """Connection to Porsche Connect API."""
 
     def __init__(
         self,
         email: Text = None,
         password: Text = None,
         websession: aiohttp.ClientSession = None,
-        language: Text = 'de',
-        country: Text = 'DE',
-        tokens = None
+        language: Text = "de",
+        country: Text = "DE",
+        tokens=None,
     ) -> None:
         """Initialize connection object."""
         self.porscheCookiedomain: Text = "https://login.porsche.com"
         self.porscheLogin: Text = "https://login.porsche.com/auth/de/de_DE"
-        self.porscheLoginAuth: Text = "https://login.porsche.com/auth/api/v1/de/de_DE/public/login"
+        self.porscheLoginAuth: Text = (
+            "https://login.porsche.com/auth/api/v1/de/de_DE/public/login"
+        )
         self.porscheAPIAuth: Text = "https://login.porsche.com/as/authorization.oauth2"
         self.porscheAPIToken: Text = "https://login.porsche.com/as/token.oauth2"
-        self.porscheAPI: Text = "https://connect-portal.porsche.com/core/api/v3/de/de_DE"
+        self.porscheAPI: Text = (
+            "https://connect-portal.porsche.com/core/api/v3/de/de_DE"
+        )
         self.porscheApplications = {
-                'portal': {
-                    'client_id': 'TZ4Vf5wnKeipJxvatJ60lPHYEzqZ4WNp',
-                    'redirect_uri': 'https://my-static02.porsche.com/static/cms/auth.html',
-                    'prefix': 'https://connect-portal.porsche.com/core/api/v3/'
-                    },
-                'carcontrol': {
-                    'client_id': 'gZLSI7ThXFB4d2ld9t8Cx2DBRvGr1zN2',
-                    'redirect_uri':  'https://connect-portal.porsche.com/myservices/auth/auth.html',
-                    'prefix': 'https://api.porsche.com/'
-                    }
-                }
+            "api": {
+                "client_id": CLIENT_ID,
+                "redirect_uri": REDIRECT_URI,
+                "prefix": "https://api.porsche.com/core/api/",
+            },
+            "profile": {
+                "client_id": CLIENT_ID,
+                "api_key": "QPw3VOLAMfI7r0nmRY8ELq4RzZpZeXEE",
+                "redirect_uri": REDIRECT_URI,
+                "prefix": "https://api.porsche.com/profiles",
+            },
+            "auth": {
+                "client_id": "4mPO3OE5Srjb1iaUGWsbqKBvvesya8oA",
+                "redirect_uri": "https://my.porsche.com/core/de/de_DE/",
+                "prefix": "https://login.porsche.com",
+            },
+            "carcontrol": {
+                "client_id": "Ux8WmyzsOAGGmvmWnW7GLEjIILHEztAs",
+                "redirect_uri": "https://my.porsche.com/myservices/auth/auth.html",
+                "prefix": "https://api.porsche.com/",
+            },
+        }
 
         self.isTokenRefreshed = False
         self.tokens = tokens or {}
         self.email = email
         self.password = password
         self.websession = websession
         self._isLoggedIn = False
         self.country = country
         self.language = language
+        self.auth_state = {}
 
-        if self.websession == None:
-            self.websession = aiohttp.ClientSession()
-        _LOGGER.debug("New connection created")
-
+        if self.websession is None:
+            self.websession = aiohttp.ClientSession(trace_configs=[trace_config])
+        _LOGGER.debug("New connection prepared")
 
     async def _login(self):
-        _LOGGER.debug("Start authentication, get initial state from login page....")
-        login_data = { 'sec': '', 'resume': '', 'thirdPartyId': '', 'state': '', 'username':
-                self.email, 'password': self.password, 'keeploggedin': 'false' }
+        _LOGGER.debug("Start authentication, get initial state from auth server")
+        # Do not follow redirect
+        start_login_url = f"https://{AUTHORIZATION_SERVER}/authorize?response_type=code&client_id={CLIENT_ID}&code_challenge_method=S256&redirect_uri={REDIRECT_URI}&ui_locales=de-DE&audience={AUDIENCE}&scope=openid"
+        async with self.websession.get(start_login_url, allow_redirects=False) as resp:
+            location = resp.headers["Location"]
+            params = urllib.parse.parse_qs(urllib.parse.urlparse(location).query)
+            _LOGGER.debug(params)
+            have_code = params.get('code', None)
+            if have_code is not None:
+                _LOGGER("We already have a code in session, skip login")
+                self.auth_state['code'] = have_code
+                return
+            self.auth_state["state"] = params["state"][0]
+            self.auth_state["client"] = params["client"][0]
+        _LOGGER.debug(self.auth_state)
 
+
+        # Post auth data
         _LOGGER.debug("POST authentication details....")
-        async with self.websession.post(self.porscheLoginAuth,  data=login_data, max_redirects=30) as resp:
+        auth_body = {
+                "sec": "high",
+                "username": self.email,
+                "password": self.password,
+                "code_challenge_method": "S256",
+                "redirect_uri": REDIRECT_URI,
+                "ui_locales": "de-DE",
+                "audience": AUDIENCE,
+                "client_id": CLIENT_ID,
+                "connection": "Username-Password-Authentication",
+                "state": self.auth_state["state"],
+                "tenant": TENANT,
+                "response_type": "code"
+                }
+        auth_url = f"https://{AUTHORIZATION_SERVER}/usernamepassword/login"
+        verify_body = {} 
+        async with self.websession.post(auth_url, headers={"Content-Type": "application/x-www-form-urlencoded"}, data=auth_body, max_redirects=30) as resp:
             # In case of wrong credentials there is a state param in the redirect url
-            last_location = resp.history[len(resp.history) - 1].headers['Location']
-            query = urllib.parse.urlparse(last_location).query
-            redirect_params = urllib.parse.parse_qs(query)
-            if "state" in redirect_params and redirect_params["state"][0] == "WRONG_CREDENTIALS":
-                raise WrongCredentials("Wrong email or password")
 
+            if resp.status == 401:
+                message = await resp.json()
+                raise WrongCredentials(message['message'])
+
+            html_body = await resp.text()
+
+            _LOGGER.debug(resp.status)
+            _LOGGER.debug(html_body)
+
+            soup = BeautifulSoup(html_body,features="html.parser")
+            hidden_tags = soup.find_all("input", type="hidden")
+            for tag in hidden_tags:
+                verify_body[tag.attrs['name']] = tag.attrs['value']
+            _LOGGER.debug(verify_body)
+
+        # Follow callback
+        _LOGGER.debug("POST authentication verification...")
+        auth_url = f"https://{AUTHORIZATION_SERVER}/login/callback"
+        resume_url = ""
+        async with self.websession.post(auth_url, headers={"Content-Type": "application/x-www-form-urlencoded"}, data=verify_body, allow_redirects=False) as resp:
+            resume_url = resp.headers['Location']
+            _LOGGER.debug(f"Resume at {resume_url}")
+
+        _LOGGER.debug("Sleeping 2.5s...")
+        time.sleep(2.5)
+
+        # Resume auth
+        auth_url = f"https://{{AUTHORIZATION_SERVER}}{resume_url}"
+        async with self.websession.get(start_login_url, allow_redirects=False) as resp:
+            location = resp.headers["Location"]
+            params = urllib.parse.parse_qs(urllib.parse.urlparse(location).query)
+            _LOGGER.debug(params)
+            self.auth_state["code"] = params["code"][0]
+            _LOGGER.debug(f"Got code {self.auth_state['code']}")
+
+        _LOGGER.debug("Sleeping 2.5s...")
+        time.sleep(2.5)
+        
         self._isLoggedIn = True
         return True
 
-
     async def getAllTokens(self):
         now = calendar.timegm(datetime.datetime.now().timetuple())
         for applicationKey in self.porscheApplications:
             application = self.porscheApplications[applicationKey]
-            token = self.tokens.get(application['client_id'], None)
-            if token is None or token['expiration'] < now:
+            token = self.tokens.get(application["client_id"], None)
+            if token is None or token["expiration"] < now:
                 token = await self._requestToken(application)
-                self.tokens[application['client_id']] = token
+                self.tokens[application["client_id"]] = token
         self.isTokenRefreshed = False
         return self.tokens
 
     async def _requestToken(self, application: Dict, wasExpired=False):
         if not self._isLoggedIn or wasExpired:
             await self._login()
 
-        _LOGGER.debug("Requesting access token for client id %s", application['client_id'])
-
-        code_verifier = base64.urlsafe_b64encode(os.urandom(40)).decode('utf-8')
-        code_verifier = re.sub('[^a-zA-Z0-9]+', '', code_verifier)
-
-        code_challenge = hashlib.sha256(code_verifier.encode('utf-8')).digest()
-        code_challenge = base64.urlsafe_b64encode(code_challenge).decode('utf-8')
-        code_challenge = code_challenge.replace('=', '')
-
-        auth_data = {
-                'scope': 'openid',
-                'response_type': 'code',
-                'access_type': 'offline',
-                'prompt': 'none',
-                'client_id': application['client_id'],
-                'redirect_uri': application['redirect_uri'],
-                'code_challenge': code_challenge,
-                'code_challenge_method': 'S256'
-                }
 
-        async with self.websession.get(self.porscheAPIAuth, params=auth_data) as resp:
-            last_location = resp.history[len(resp.history) - 1].headers['Location']
-            query = urllib.parse.urlparse(last_location).query
-            redirect_params = urllib.parse.parse_qs(query)
-            auth_code = redirect_params['code'][0]
-            _LOGGER.debug("Code %s", auth_code)
-
-        auth_token_data = {
-                'grant_type': 'authorization_code',
-                'client_id': application['client_id'],
-                'redirect_uri': application['redirect_uri'],
-                'code': auth_code,
-                'prompt': 'none',
-                'code_verifier': code_verifier
+        _LOGGER.debug("POST to acces token endpoint...")
+        auth_url = f"https://{AUTHORIZATION_SERVER}/oauth/token"
+        auth_body = {
+                "client_id": CLIENT_ID,
+                "grant_type": "authorization_code",
+                "code": self.auth_state['code'],
+                "redirect_uri": REDIRECT_URI
                 }
-        _LOGGER.debug("Data %s", auth_token_data)
-
+        _LOGGER.debug(auth_body)
+        _LOGGER.debug( "Requesting access token for client id %s", application["client_id"])
         now = calendar.timegm(datetime.datetime.now().timetuple())
-        async with self.websession.post(self.porscheAPIToken, data=auth_token_data) as resp:
+        async with self.websession.post(auth_url, headers={"Content-Type": "application/x-www-form-urlencoded"}, data=auth_body, max_redirects=30) as resp:
+            _LOGGER.debug(f"Response status {resp.status}")
             token_data = await resp.json()
-            jwt = self.jwt_payload_decode(token_data['id_token'])
+            _LOGGER.debug(token_data)
+            jwt = self.jwt_payload_decode(token_data["access_token"])
             token = token_data
-            token['expiration'] = now + token_data['expires_in']
-            token['decoded_token'] = jwt
-            token['apikey'] = jwt['aud']
-            _LOGGER.debug('Token: %s', token)
+            token["expiration"] = now + token_data.get("exp", 3600)
+            token["decoded_token"] = jwt
+            token["apikey"] = jwt["azp"]
+            _LOGGER.debug("Token: %s", token)
             self.isTokenRefreshed = True
             return token
 
-    async def get(self, url, params = None):
+
+    async def get(self, url, params=None):
         try:
             application = self._applicationForURL(url)
             headers = await self._createhead(application)
             async with self.websession.get(url, params=params, headers=headers) as resp:
                 return await resp.json()
         except aiohttp.ClientResponseError as exception_:
             raise PorscheException(exception_.status)
 
     async def post(self, url, data=None, json=None):
         try:
             application = self._applicationForURL(url)
             headers = await self._createhead(application)
-            async with self.websession.post(url, data=data, json=json, headers=headers) as resp:
+            async with self.websession.post(
+                url, data=data, json=json, headers=headers
+            ) as resp:
                 return await resp.json()
         except aiohttp.ClientResponseError as exception_:
             raise PorscheException(exception_.status)
 
     async def put(self, url, data=None, json=None):
         try:
             application = self._applicationForURL(url)
             headers = await self._createhead(application)
-            async with self.websession.put(url, data=data, json=json, headers=headers) as resp:
+            async with self.websession.put(
+                url, data=data, json=json, headers=headers
+            ) as resp:
                 return await resp.json()
         except aiohttp.ClientResponseError as exception_:
             raise PorscheException(exception_.status)
 
     async def delete(self, url, data=None, json=None):
         try:
             application = self._applicationForURL(url)
             headers = await self._createhead(application)
-            async with self.websession.delete(url, data=data, json=json, headers=headers) as resp:
+            async with self.websession.delete(
+                url, data=data, json=json, headers=headers
+            ) as resp:
                 return await resp.json()
         except aiohttp.ClientResponseError as exception_:
             raise PorscheException(exception_.status)
 
     def _applicationForURL(self, url):
-       for key in self.porscheApplications:
-           app = self.porscheApplications[key]
-           if url.startswith(app['prefix']):
-               return app
-       # else return None
-       return None
+        for key in self.porscheApplications:
+            app = self.porscheApplications[key]
+            if url.startswith(app["prefix"]):
+                return app
+        # else return None
+        return None
 
     async def _createhead(self, application):
         # If no application matched the request URL then no auth headers are added
         if application is None:
             return {}
         now = calendar.timegm(datetime.datetime.now().timetuple())
-        token = self.tokens.get(application['client_id'], None)
-        if token is None or token['expiration'] < now:
-            token = await self._requestToken(application, wasExpired=(token is not None))
-            self.tokens[application['client_id']] = token
+        token = self.tokens.get(application["client_id"], None)
+        if token is None or token["expiration"] < now:
+            token = await self._requestToken(
+                application, wasExpired=(token is not None)
+            )
+            self.tokens[application["client_id"]] = token
         head = {
             "Authorization": f"Bearer {token['access_token']}",
-            "apikey": token['apikey'],
+            "origin": "https://my.porsche.com",
+            "apikey": application.get("api_key", token["apikey"]),
             "x-vrs-url-country": self.country.lower(),
-            "x-vrs-url-language": f"{self.language.lower()}_{self.country.upper()}"
-            }
+            "x-vrs-url-language": f"{self.language.lower()}_{self.country.upper()}",
+        }
         return head
 
     def _b64_decode(self, data):
-        data += '=' * (4 - len(data) % 4)
-        return base64.b64decode(data).decode('utf-8')
+        data += "=" * (4 - len(data) % 4)
+        return base64.b64decode(data).decode("utf-8")
 
     def jwt_payload_decode(self, jwt):
-        _, payload, _ = jwt.split('.')
+        _, payload, _ = jwt.split(".")
         return json.loads(self._b64_decode(payload))
 
     async def close(self):
         await self.websession.close()
-
```

### Comparing `pyporscheconnectapi-0.0.9/pyporscheconnectapi/exceptions.py` & `pyporscheconnectapi-0.1.1/pyporscheconnectapi/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,42 +7,43 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class PorscheException(Exception):
     """Class of Porsche API exceptions."""
 
-    def __init__(self, code, *args, **kwargs):
+    def __init__(self, code=None, *args, **kwargs):
         """Initialize exceptions for the Porsche API."""
         self.message = ""
         super().__init__(*args, **kwargs)
-        self.code = code
-        if isinstance(code, str):
-            self.message = self.code
-            return
-        if self.code == 401:
-            self.message = "UNAUTHORIZED"
-        elif self.code == 404:
-            self.message = "NOT_FOUND"
-        elif self.code == 405:
-            self.message = "MOBILE_ACCESS_DISABLED"
-        elif self.code == 408:
-            self.message = "VEHICLE_UNAVAILABLE"
-        elif self.code == 423:
-            self.message = "ACCOUNT_LOCKED"
-        elif self.code == 429:
-            self.message = "TOO_MANY_REQUESTS"
-        elif self.code == 500:
-            self.message = "SERVER_ERROR"
-        elif self.code == 503:
-            self.message = "SERVICE_MAINTENANCE"
-        elif self.code == 504:
-            self.message = "UPSTREAM_TIMEOUT"
-        elif self.code > 299:
-            self.message = f"UNKNOWN_ERROR_{self.code}"
+        if code is not None:
+            self.code = code
+            if isinstance(code, str):
+                self.message = self.code
+                return
+            if self.code == 401:
+                self.message = "UNAUTHORIZED"
+            elif self.code == 404:
+                self.message = "NOT_FOUND"
+            elif self.code == 405:
+                self.message = "MOBILE_ACCESS_DISABLED"
+            elif self.code == 408:
+                self.message = "VEHICLE_UNAVAILABLE"
+            elif self.code == 423:
+                self.message = "ACCOUNT_LOCKED"
+            elif self.code == 429:
+                self.message = "TOO_MANY_REQUESTS"
+            elif self.code == 500:
+                self.message = "SERVER_ERROR"
+            elif self.code == 503:
+                self.message = "SERVICE_MAINTENANCE"
+            elif self.code == 504:
+                self.message = "UPSTREAM_TIMEOUT"
+            elif self.code > 299:
+                self.message = f"UNKNOWN_ERROR_{self.code}"
 
 
 class WrongCredentials(PorscheException):
     """Class of exceptions for incomplete credentials."""
 
     pass
```

### Comparing `pyporscheconnectapi-0.0.9/setup.py` & `pyporscheconnectapi-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 
 setup(
     name="pyporscheconnectapi",
-    version="0.0.9",
+    version="0.1.1",
     author="Johan Isaksson",
     author_email="johan@generatorhallen.se",
     description="Python library and CLI for communicating with Porsche Connect API.",
+    long_description=open("README.md", 'r').read(),
+    long_description_content_type='text/markdown',
     include_package_data=True,
     url="https://github.com/cjne/pyporscheconnectapi",
     license="MIT",
     packages=["pyporscheconnectapi"],
     python_requires=">=3.6",
-    install_requires=["aiohttp<4"],
+    install_requires=["aiohttp<4","beautifulsoup4"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Operating System :: OS Independent",
     ],
     setup_requires=("pytest-runner"),
     tests_require=(
```

