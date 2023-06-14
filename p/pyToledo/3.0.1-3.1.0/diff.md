# Comparing `tmp/pyToledo-3.0.1.tar.gz` & `tmp/pyToledo-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyToledo-3.0.1.tar", last modified: Sun Mar 12 18:37:21 2023, max compression
+gzip compressed data, was "pyToledo-3.1.0.tar", last modified: Wed Jun 14 18:57:44 2023, max compression
```

## Comparing `pyToledo-3.0.1.tar` & `pyToledo-3.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-03-12 18:37:21.182515 pyToledo-3.0.1/
--rw-r--r--   0 arch      (1000) arch      (1000)    35149 2023-03-11 22:35:39.000000 pyToledo-3.0.1/LICENSE
--rw-r--r--   0 arch      (1000) arch      (1000)       26 2023-03-11 22:35:39.000000 pyToledo-3.0.1/MANIFEST.in
--rw-r--r--   0 arch      (1000) arch      (1000)     5013 2023-03-12 18:37:21.179181 pyToledo-3.0.1/PKG-INFO
--rw-r--r--   0 arch      (1000) arch      (1000)     4449 2023-03-12 10:09:55.000000 pyToledo-3.0.1/README.md
-drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-03-12 18:37:21.169181 pyToledo-3.0.1/pyToledo.egg-info/
--rw-r--r--   0 arch      (1000) arch      (1000)     5013 2023-03-12 18:37:21.000000 pyToledo-3.0.1/pyToledo.egg-info/PKG-INFO
--rw-r--r--   0 arch      (1000) arch      (1000)      354 2023-03-12 18:37:21.000000 pyToledo-3.0.1/pyToledo.egg-info/SOURCES.txt
--rw-r--r--   0 arch      (1000) arch      (1000)        1 2023-03-12 18:37:21.000000 pyToledo-3.0.1/pyToledo.egg-info/dependency_links.txt
--rw-r--r--   0 arch      (1000) arch      (1000)       57 2023-03-12 18:37:21.000000 pyToledo-3.0.1/pyToledo.egg-info/requires.txt
--rw-r--r--   0 arch      (1000) arch      (1000)        7 2023-03-12 18:37:21.000000 pyToledo-3.0.1/pyToledo.egg-info/top_level.txt
--rw-r--r--   0 arch      (1000) arch      (1000)       86 2023-03-11 22:35:39.000000 pyToledo-3.0.1/pyproject.toml
--rw-r--r--   0 arch      (1000) arch      (1000)       38 2023-03-12 18:37:21.182515 pyToledo-3.0.1/setup.cfg
--rw-r--r--   0 arch      (1000) arch      (1000)     1056 2023-03-12 18:34:31.000000 pyToledo-3.0.1/setup.py
-drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-03-12 18:37:21.179181 pyToledo-3.0.1/toledo/
--rw-r--r--   0 arch      (1000) arch      (1000)       69 2023-03-11 22:35:39.000000 pyToledo-3.0.1/toledo/__init__.py
--rw-r--r--   0 arch      (1000) arch      (1000)     2241 2023-03-11 22:35:39.000000 pyToledo-3.0.1/toledo/__main__.py
--rw-r--r--   0 arch      (1000) arch      (1000)     7333 2023-03-11 22:35:39.000000 pyToledo-3.0.1/toledo/api.py
--rw-r--r--   0 arch      (1000) arch      (1000)     1134 2023-03-11 22:35:39.000000 pyToledo-3.0.1/toledo/config.yaml
--rw-r--r--   0 arch      (1000) arch      (1000)     3663 2023-03-12 09:58:19.000000 pyToledo-3.0.1/toledo/dashboard.py
--rw-r--r--   0 arch      (1000) arch      (1000)     4323 2023-03-12 09:58:31.000000 pyToledo-3.0.1/toledo/kuloket.py
--rw-r--r--   0 arch      (1000) arch      (1000)     5546 2023-03-12 09:57:27.000000 pyToledo-3.0.1/toledo/portal.py
--rw-r--r--   0 arch      (1000) arch      (1000)    10785 2023-03-12 10:08:44.000000 pyToledo-3.0.1/toledo/utils.py
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-06-14 18:57:44.499800 pyToledo-3.1.0/
+-rw-r--r--   0 arch      (1000) arch      (1000)    35149 2023-03-11 22:35:39.000000 pyToledo-3.1.0/LICENSE
+-rw-r--r--   0 arch      (1000) arch      (1000)       26 2023-03-11 22:35:39.000000 pyToledo-3.1.0/MANIFEST.in
+-rw-r--r--   0 arch      (1000) arch      (1000)     8787 2023-06-14 18:57:44.499800 pyToledo-3.1.0/PKG-INFO
+-rw-r--r--   0 arch      (1000) arch      (1000)     8223 2023-06-14 18:49:49.000000 pyToledo-3.1.0/README.md
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-06-14 18:57:44.493134 pyToledo-3.1.0/pyToledo.egg-info/
+-rw-r--r--   0 arch      (1000) arch      (1000)     8787 2023-06-14 18:57:44.000000 pyToledo-3.1.0/pyToledo.egg-info/PKG-INFO
+-rw-r--r--   0 arch      (1000) arch      (1000)      374 2023-06-14 18:57:44.000000 pyToledo-3.1.0/pyToledo.egg-info/SOURCES.txt
+-rw-r--r--   0 arch      (1000) arch      (1000)        1 2023-06-14 18:57:44.000000 pyToledo-3.1.0/pyToledo.egg-info/dependency_links.txt
+-rw-r--r--   0 arch      (1000) arch      (1000)       57 2023-06-14 18:57:44.000000 pyToledo-3.1.0/pyToledo.egg-info/requires.txt
+-rw-r--r--   0 arch      (1000) arch      (1000)        7 2023-06-14 18:57:44.000000 pyToledo-3.1.0/pyToledo.egg-info/top_level.txt
+-rw-r--r--   0 arch      (1000) arch      (1000)       86 2023-03-11 22:35:39.000000 pyToledo-3.1.0/pyproject.toml
+-rw-r--r--   0 arch      (1000) arch      (1000)       38 2023-06-14 18:57:44.499800 pyToledo-3.1.0/setup.cfg
+-rw-r--r--   0 arch      (1000) arch      (1000)     1056 2023-06-11 11:10:40.000000 pyToledo-3.1.0/setup.py
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-06-14 18:57:44.499800 pyToledo-3.1.0/toledo/
+-rw-r--r--   0 arch      (1000) arch      (1000)       69 2023-06-11 11:10:29.000000 pyToledo-3.1.0/toledo/__init__.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     6030 2023-06-14 18:46:21.000000 pyToledo-3.1.0/toledo/__main__.py
+-rw-r--r--   0 arch      (1000) arch      (1000)    10019 2023-06-14 18:39:09.000000 pyToledo-3.1.0/toledo/api.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     1666 2023-06-10 14:31:03.000000 pyToledo-3.1.0/toledo/config.yaml
+-rw-r--r--   0 arch      (1000) arch      (1000)     3663 2023-06-10 15:23:04.000000 pyToledo-3.1.0/toledo/dashboard.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     4323 2023-03-12 09:58:31.000000 pyToledo-3.1.0/toledo/kuloket.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     5670 2023-06-08 19:52:44.000000 pyToledo-3.1.0/toledo/portal.py
+-rw-r--r--   0 arch      (1000) arch      (1000)    11499 2023-06-11 13:29:09.000000 pyToledo-3.1.0/toledo/utils.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     6419 2023-06-14 18:27:37.000000 pyToledo-3.1.0/toledo/vivesplus.py
```

### Comparing `pyToledo-3.0.1/LICENSE` & `pyToledo-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyToledo-3.0.1/setup.py` & `pyToledo-3.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setuptools.setup(
     name="pyToledo",
-    version="3.0.1",
+    version="3.1.0",
     description="pyToledo is a Python library to interact with the common virtual learning environment for the Association KU Leuven a.k.a Toledo.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/DaanVervacke/pyToledo",
     author="Vervacke Daan",
     author_email="daan.vervacke@student.vives.be",
     license="GPLv3",
```

### Comparing `pyToledo-3.0.1/toledo/api.py` & `pyToledo-3.1.0/toledo/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 
             self._UPCOMING_URL = parser['API']['UpcomingEndpoint']
             self._ENROLLMENTS_URL = parser['API']['EnrollmentsEndpoint']
             self._EVENTS_URL = parser['API']['EventsEndpoint']
             self._TODO_URL = parser['API']['TodoEndpoint']
             self._LINK_URL = parser['API']['LinkEndpoint']
             self._SCHEDULE_URL = parser['API']['ScheduleEndpoint']
-
+            self._VIVESPLUS_SCHEDULE_URL = parser['API']['VivesPlusScheduleEndpoint']
+            
             self._TASK = parser['API_TO_DO']['Task']
             self._TEST = parser['API_TO_DO']['Test']
             self._VARIOUS = parser['API_TO_DO']['Various']
 
             self._SESSION = session
 
         except FileNotFoundError:
@@ -261,12 +262,126 @@
                 f'SCHEDULE: You need an api object with an extended portal session (kuloket) to use this method')
 
         except Exception as ex:
 
             sys.exit(f'SCHEDULE: {ex}')
 
 
-def create_api_object(session: requests.Session) -> ToledoApi:
+class VivesPlusApi:
+
+    def __init__(self, session: requests.Session) -> None:
+
+        try:
+
+            with open(os.path.join(os.path.dirname(__file__), 'config.yaml'), 'r') as f:
+                parser = yaml.safe_load(f)
+                f.close()
+
+            self._VIVESPLUS_SCHEDULE_URL = parser['API']['VivesPlusScheduleEndpoint']
+            self._VIVESPLUS_STUDENT_URL = parser['API']['VivesPlusStudentEndpoint']
+            self._VIVESPLUS_DASHBOARD_URL = parser['API']['VivesPlusDashboardEndpoint']
+            self._VIVESPLUS_NOTICES_URL = parser['API']['VivesPlusNoticesEndpoint']
+
+            self._SESSION = session
+
+        except FileNotFoundError:
+            sys.exit('API: Unable to find find config.yaml!')
+
+        except Exception:
+            sys.exit('API: Failed to create API object!')
+
+    
+    ''' VIVES PLUS METHODS '''
+
+    def get_schedule(self, start_date, end_date) -> str:
+
+        try:
+
+            r = self._SESSION.get(
+                url=self._VIVESPLUS_SCHEDULE_URL,
+                params={
+                    'from': start_date,
+                    'to': end_date
+                }
+            )
+
+            r.raise_for_status()
+
+            return r.json()
+
+        except Exception as ex:
+
+            sys.exit(f'SCHEDULE URL: {ex}')
+    
+    def get_student_info(self) -> str:
+
+        try:
+
+            r = self._SESSION.get(
+                url=self._VIVESPLUS_STUDENT_URL
+            )
+
+            r.raise_for_status()
+
+            return r.json()
+
+        except Exception as ex:
+
+            sys.exit(f'STUDENT URL: {ex}')
+
+    def get_dashboard(self) -> str:
+
+        try:
+
+            r = self._SESSION.get(
+                url=self._VIVESPLUS_DASHBOARD_URL
+            )
+
+            r.raise_for_status()
+
+            return r.json()
+
+        except Exception as ex:
+
+            sys.exit(f'DASHBOARD URL: {ex}')
+
+    def get_notices(self) -> str:
+
+        try:
+
+            r = self._SESSION.get(
+                url=self._VIVESPLUS_NOTICES_URL
+            )
+
+            r.raise_for_status()
+
+            return r.json()
+
+        except Exception as ex:
+
+            sys.exit(f'NOTICES URL: {ex}')
+    
+    def get_authorization_token(self) -> str:
+
+        try:
+
+            return {
+                    'token': self._SESSION.headers.get('Authorization')
+                }
+            
+        
+        except Exception as ex:
+
+            sys.exit(f'AUTHORIZATION TOKEN: {ex}')
+    
+
+def create_toledo_api_object(session: requests.Session) -> ToledoApi:
 
     return ToledoApi(
         session=session
     )
+
+def create_vivesplus_api_object(session: requests.Session) -> VivesPlusApi:
+
+    return VivesPlusApi(
+        session=session
+    )
```

### Comparing `pyToledo-3.0.1/toledo/config.yaml` & `pyToledo-3.1.0/toledo/config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 USER:
   UserAgent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.246
+  UserAgentMobile: Mozilla/5.0 (Linux; Android 8.1.0; Moto G (5S) Plus Build/OPS28.65-36-14; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/114.0.5735.61 Mobile Safari/537.36
 
 LOGIN:
   PortalURL: https://toledo.kuleuven.be/portal/
+  PortalURLMobile: https://vivesplus.azurewebsites.net/mobile/login/jwt
   DashboardURL: https://toledo.kuleuven.be/dashboard/
   AuthorizationEndpoint: https://idp.kuleuven.be/auth/realms/kuleuven/protocol/openid-connect/auth/
   TokenEndpoint: https://idp.kuleuven.be/auth/realms/kuleuven/protocol/openid-connect/token/
   BrokerEndpoint: https://idp.kuleuven.be/auth/realms/kuleuven/broker/saml-p-idp/endpoint
   
 API:
   UpcomingEndpoint: https://toledo.kuleuven.be/portal/api/upcoming/
   EnrollmentsEndpoint: https://toledo.kuleuven.be/portal/api/enrollments/
   EventsEndpoint: https://toledo.kuleuven.be/portal/api/events/
   TodoEndpoint: https://learning-analytics-cygnus.icts.kuleuven.be/api/users/availableUserContentState/
   LinkEndpoint: https://toledo.kuleuven.be/portal/api/links/
   ScheduleEndpoint: https://webwsp.aps.kuleuven.be/sap/opu/odata/sap/ZC_EP_SCHEDULE_SRV/$batch
+  VivesPlusScheduleEndpoint: https://plus.vives.be/api/events
+  VivesPlusStudentEndpoint: https://plus.vives.be/api/students/me
+  VivesPlusDashboardEndpoint: https://vivesplus.azurewebsites.net/api/dashboard
+  VivesPlusNoticesEndpoint: https://plus.vives.be/api/notices
 
 API_TO_DO:
   Task: x-bb-assignment
   Test: x-bb-asmt-test-link
   Various: x-bb-asmt-survey-link
```

### Comparing `pyToledo-3.0.1/toledo/dashboard.py` & `pyToledo-3.1.0/toledo/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyToledo-3.0.1/toledo/kuloket.py` & `pyToledo-3.1.0/toledo/kuloket.py`

 * *Files identical despite different names*

### Comparing `pyToledo-3.0.1/toledo/portal.py` & `pyToledo-3.1.0/toledo/portal.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,32 +139,36 @@
 
             # Get fifth csrf token
             fifth_csrf = get_saml2_csrf(
                 html=fifth_csrf_html
             )
 
             # Get shib_idp_session_ss
-            shib_idp_session_ss = get_shib_idp_session_ss(html=fifth_csrf_html)
+            #shib_idp_session_ss = get_shib_idp_session_ss(html=fifth_csrf_html)
 
             # Post fifth csrf token
             relaystate_samlresponse_html = post_saml2_csrf(
-                post_info=fifth_csrf
+                post_info=fifth_csrf,
+                event_id='proceed'
             )
 
             # Get RelayState & SAMLResponse
             relaystate_samlresponse = get_saml2_relay_and_response(
                 html=relaystate_samlresponse_html
             )
 
+            if relaystate_samlresponse is None:
+
+                raise Exception('Please create a recovery code before using this package!')
+            
             # Post RelayState & SAMLResponse
             post_saml2_relay_and_response(
                 post_info=relaystate_samlresponse
             )
             
-            # At this point we have obtained the shibsession token
             return SESSION
 
         except requests.exceptions.HTTPError as errh:
             sys.exit("Http Error:", errh)
         except requests.exceptions.ConnectionError as errc:
             sys.exit("Error Connecting:", errc)
         except requests.exceptions.Timeout as errt:
```

### Comparing `pyToledo-3.0.1/toledo/utils.py` & `pyToledo-3.1.0/toledo/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     soup = BeautifulSoup(html, 'html.parser')
 
     form = soup.body.form
 
     return {
 
         'url': form['action'],
-        'relaystate': form.find('input', {'name': 'RelayState'})['value'],
+        'relaystate': form.find('input', {'name': 'RelayState'})['value'] if form.find('input', {'name': 'RelayState'}) is not None else None ,
         'samlrequest': form.find('input', {'name': 'SAMLRequest'})['value'],
     }
 
 
 def get_saml2_relay_and_response(html: str) -> dict:
     ''' Searches and returns url, relaysate and samlresponse values from provided html
         Returns None when the relaystate can't be found
@@ -68,14 +68,22 @@
 
         return {
 
             'url': form['action'],
             'relaystate': form.find('input', {'name': 'RelayState'})['value'],
             'samlresponse': form.find('input', {'name': 'SAMLResponse'})['value'],
         }
+    
+    elif form.find('input', {'name': 'SAMLResponse'}) is not None:
+
+        return {
+
+            'url': form['action'],
+            'samlresponse': form.find('input', {'name': 'SAMLResponse'})['value'],
+        }
 
     else:
 
         return None
 
 
 def get_saml2_csrf(html: str) -> dict:
@@ -149,15 +157,15 @@
         return query['code'][0]
 
     else:
 
         return r.text
 
 
-def post_saml2_csrf(post_info: dict, session_ss: str = '') -> str:
+def post_saml2_csrf(post_info: dict, session_ss: str = '', event_id: str = '') -> str:
     ''' HTTP POST csrf token and return html'''
     
     url = f'https://idp.kuleuven.be{post_info["url"]}' if 'https://idp.kuleuven.be' not in post_info["url"] else post_info["url"] 
 
     r = SESSION.post(
         url=url,
         data={
@@ -165,15 +173,15 @@
             'shib_idp_ls_exception.shib_idp_session_ss': '',
             'shib_idp_ls_success.shib_idp_session_ss': 'true',
             'shib_idp_ls_value.shib_idp_session_ss': session_ss,
             'shib_idp_ls_exception.shib_idp_persistent_ss': '',
             'shib_idp_ls_success.shib_idp_persistent_ss': 'true',
             'shib_idp_ls_value.shib_idp_persistent_ss': '',
             'shib_idp_ls_supported': 'true',
-            '_eventId_proceed': ''
+            '_eventId_proceed': event_id
 
         }
     )
     
     r.raise_for_status()
 
     if r.history:
@@ -235,15 +243,33 @@
         
         while True:
             
             if 'LOGIN' in await websocket.recv():
                 break
             
         return fourth_csrf
-        
+    
+
+''' VIVES PLUS METHODS '''
+
+def get_vivesplus_auth_token(post_info: dict) -> str:
+    ''' HTTP POST samlresponse and return Vives Plus auth'''
+
+    r = SESSION.post(
+        url=post_info['url'],
+        data={
+            'SAMLResponse': post_info['samlresponse']
+        },
+    )
+
+    r.raise_for_status()
+
+    SESSION.headers.update({
+        'Authorization': f"Bearer {r.json()['id_token']}"
+    })
 
 
 ''' OTHER METHODS '''
 
 
 def openid_connect_auth(state: str, code_challenge: str, url: str) -> str:
     ''' HTTP GET with sate and code_challenge as parameters
```

