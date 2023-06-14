# Comparing `tmp/shareconnect-1.0.0.10.tar.gz` & `tmp/shareconnect-1.0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareconnect-1.0.0.10.tar", last modified: Tue May  9 11:39:58 2023, max compression
+gzip compressed data, was "shareconnect-1.0.0.11.tar", last modified: Wed Jun 14 06:17:18 2023, max compression
```

## Comparing `shareconnect-1.0.0.10.tar` & `shareconnect-1.0.0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 rimagiri  (1000) rimagiri  (1000)        0 2023-05-09 11:39:58.954440 shareconnect-1.0.0.10/
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)    10677 2023-05-09 11:39:58.954440 shareconnect-1.0.0.10/PKG-INFO
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)     8046 2023-05-09 11:05:48.000000 shareconnect-1.0.0.10/README.md
-drwxrwxr-x   0 rimagiri  (1000) rimagiri  (1000)        0 2023-05-09 11:39:58.954440 shareconnect-1.0.0.10/SharekhanApi/
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)      221 2023-04-12 07:02:59.000000 shareconnect-1.0.0.10/SharekhanApi/__init__.py
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)    17062 2023-05-09 11:13:11.000000 shareconnect-1.0.0.10/SharekhanApi/sharekhanConnect.py
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)     1922 2023-05-08 08:18:55.000000 shareconnect-1.0.0.10/SharekhanApi/sharekhanExceptions.py
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)     4936 2023-05-09 10:46:58.000000 shareconnect-1.0.0.10/SharekhanApi/sharekhanWebsocket.py
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)       38 2023-05-09 11:39:58.954440 shareconnect-1.0.0.10/setup.cfg
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)     1110 2023-05-08 11:25:15.000000 shareconnect-1.0.0.10/setup.py
-drwxrwxr-x   0 rimagiri  (1000) rimagiri  (1000)        0 2023-05-09 11:39:58.954440 shareconnect-1.0.0.10/shareconnect.egg-info/
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)    10677 2023-05-09 11:39:58.000000 shareconnect-1.0.0.10/shareconnect.egg-info/PKG-INFO
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)      356 2023-05-09 11:39:58.000000 shareconnect-1.0.0.10/shareconnect.egg-info/SOURCES.txt
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)        1 2023-05-09 11:39:58.000000 shareconnect-1.0.0.10/shareconnect.egg-info/dependency_links.txt
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)       49 2023-05-09 11:39:58.000000 shareconnect-1.0.0.10/shareconnect.egg-info/requires.txt
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)       18 2023-05-09 11:39:58.000000 shareconnect-1.0.0.10/shareconnect.egg-info/top_level.txt
-drwxrwxr-x   0 rimagiri  (1000) rimagiri  (1000)        0 2023-05-09 11:39:58.954440 shareconnect-1.0.0.10/test/
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)        0 2023-03-31 10:07:30.000000 shareconnect-1.0.0.10/test/__init__.py
--rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)     4754 2023-05-09 11:05:48.000000 shareconnect-1.0.0.10/test/test.py
+drwxrwxr-x   0 rimagiri  (1000) rimagiri  (1000)        0 2023-06-14 06:17:18.078778 shareconnect-1.0.0.11/
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)    10787 2023-06-14 06:17:18.078778 shareconnect-1.0.0.11/PKG-INFO
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)     8148 2023-06-14 06:11:18.000000 shareconnect-1.0.0.11/README.md
+drwxrwxr-x   0 rimagiri  (1000) rimagiri  (1000)        0 2023-06-14 06:17:18.074778 shareconnect-1.0.0.11/SharekhanApi/
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)      221 2023-04-12 07:02:59.000000 shareconnect-1.0.0.11/SharekhanApi/__init__.py
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)    15942 2023-06-14 06:11:18.000000 shareconnect-1.0.0.11/SharekhanApi/sharekhanConnect.py
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)     1922 2023-05-08 08:18:55.000000 shareconnect-1.0.0.11/SharekhanApi/sharekhanExceptions.py
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)     4936 2023-05-09 10:46:58.000000 shareconnect-1.0.0.11/SharekhanApi/sharekhanWebsocket.py
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)       38 2023-06-14 06:17:18.078778 shareconnect-1.0.0.11/setup.cfg
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)     1110 2023-06-13 11:27:12.000000 shareconnect-1.0.0.11/setup.py
+drwxrwxr-x   0 rimagiri  (1000) rimagiri  (1000)        0 2023-06-14 06:17:18.078778 shareconnect-1.0.0.11/shareconnect.egg-info/
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)    10787 2023-06-14 06:17:18.000000 shareconnect-1.0.0.11/shareconnect.egg-info/PKG-INFO
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)      356 2023-06-14 06:17:18.000000 shareconnect-1.0.0.11/shareconnect.egg-info/SOURCES.txt
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)        1 2023-06-14 06:17:18.000000 shareconnect-1.0.0.11/shareconnect.egg-info/dependency_links.txt
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)       49 2023-06-14 06:17:18.000000 shareconnect-1.0.0.11/shareconnect.egg-info/requires.txt
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)       18 2023-06-14 06:17:18.000000 shareconnect-1.0.0.11/shareconnect.egg-info/top_level.txt
+drwxrwxr-x   0 rimagiri  (1000) rimagiri  (1000)        0 2023-06-14 06:17:18.078778 shareconnect-1.0.0.11/test/
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)        0 2023-03-31 10:07:30.000000 shareconnect-1.0.0.11/test/__init__.py
+-rw-rw-r--   0 rimagiri  (1000) rimagiri  (1000)     4916 2023-06-14 06:11:18.000000 shareconnect-1.0.0.11/test/test.py
```

### Comparing `shareconnect-1.0.0.10/PKG-INFO` & `shareconnect-1.0.0.11/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareconnect
-Version: 1.0.0.10
+Version: 1.0.0.11
 Summary: Sharekhan Data Feed Trading Api Server
 Home-page: UNKNOWN
 Author: rg-sharekhanapi
 Author-email: shareconnect@sharekhan.com
 License: UNKNOWN
 Description: # SHARECONNECT-PYTHON
         
@@ -27,41 +27,42 @@
             
             api_key = "Your API-KEY"
             login = SharekhanConnect(api_key)
             vendor_key = "Vendor key" 
                 """Pass the vendor key for vendor login otherwise keep it blank"""
             version_id = "Version Id"
                 """Only null/1005/1006 version id is allowed to be passed"""
+            state=12345
             url = login.login_url(vendor_key=vendor_key, version_id=version_id)
             """This will provide you the redirect login url which can be used to login in the sharekhan account"""
             print(url)
         
             
             """After Successfully Login You will receive the request token value then you have to decrypt the token value by using secret key and then swap the request token which is a combination of RequestId and CustomerId.Then after that decrypt the request token value."""
             
             request_token = "Valid Request Token Value"
             secret_key = "Your Secret Key value"
         
-            """Use generate session method when you are passing version id """
+           """Use generate session method when you are passing version id """
             session=login.generate_session(request_token,secret_key)
+            # Generating access token for version id and pass parameters as it is passed below 
+            access_token=login.get_access_token(api_key,session,state,versionId=version_id)
             
             """Use generate session without version id method when you are not passing version id """
             sessionwithoutvesionId=login.generate_session_without_versionId(request_token,secret_key)
+            # Generating access token for without version id 
+            access_token=login.get_access_token(api_key,sessionwithoutvesionId,state)
             
-            # Generate access token
-            
-            """ You have to pass the encrypted request token after manipulation """
-            
-            requestToken="Your Encrypted request token value getting from generate session method"
-            access_token=login.get_access_token(apiKey=api_key,requestToken,userId=12345,versionId=1005)
             print(access_token)
             
             # Make a object for SharekhanConnect class
             """Here we are passing the api-key, access-token and vendor-key(when needed) as a request header parameters"""
-            sharekhan = SharekhanConnect(api_key,access_token=access_token,vendor_key=vendor_key)
+            access_token = "Your access token value"
+            sharekhan = SharekhanConnect(api_key,access_token)
+            print(sharekhan.requestHeaders())       # for printing request headers
             
             # Place order history
             
              orderparams={
              "customerId": "XXXXXXX",
              "scripCode": 2475,
              "tradingSymbol": "ONGC",
```

### Comparing `shareconnect-1.0.0.10/README.md` & `shareconnect-1.0.0.11/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,41 +19,42 @@
     
     api_key = "Your API-KEY"
     login = SharekhanConnect(api_key)
     vendor_key = "Vendor key" 
         """Pass the vendor key for vendor login otherwise keep it blank"""
     version_id = "Version Id"
         """Only null/1005/1006 version id is allowed to be passed"""
+    state=12345
     url = login.login_url(vendor_key=vendor_key, version_id=version_id)
     """This will provide you the redirect login url which can be used to login in the sharekhan account"""
     print(url)
 
     
     """After Successfully Login You will receive the request token value then you have to decrypt the token value by using secret key and then swap the request token which is a combination of RequestId and CustomerId.Then after that decrypt the request token value."""
     
     request_token = "Valid Request Token Value"
     secret_key = "Your Secret Key value"
 
-    """Use generate session method when you are passing version id """
+   """Use generate session method when you are passing version id """
     session=login.generate_session(request_token,secret_key)
+    # Generating access token for version id and pass parameters as it is passed below 
+    access_token=login.get_access_token(api_key,session,state,versionId=version_id)
     
     """Use generate session without version id method when you are not passing version id """
     sessionwithoutvesionId=login.generate_session_without_versionId(request_token,secret_key)
+    # Generating access token for without version id 
+    access_token=login.get_access_token(api_key,sessionwithoutvesionId,state)
     
-    # Generate access token
-    
-    """ You have to pass the encrypted request token after manipulation """
-    
-    requestToken="Your Encrypted request token value getting from generate session method"
-    access_token=login.get_access_token(apiKey=api_key,requestToken,userId=12345,versionId=1005)
     print(access_token)
     
     # Make a object for SharekhanConnect class
     """Here we are passing the api-key, access-token and vendor-key(when needed) as a request header parameters"""
-    sharekhan = SharekhanConnect(api_key,access_token=access_token,vendor_key=vendor_key)
+    access_token = "Your access token value"
+    sharekhan = SharekhanConnect(api_key,access_token)
+    print(sharekhan.requestHeaders())       # for printing request headers
     
     # Place order history
     
      orderparams={
      "customerId": "XXXXXXX",
      "scripCode": 2475,
      "tradingSymbol": "ONGC",
```

### Comparing `shareconnect-1.0.0.10/SharekhanApi/sharekhanConnect.py` & `shareconnect-1.0.0.11/SharekhanApi/sharekhanConnect.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,29 +33,16 @@
 
         "api.holdings": "/skapi/services/holdings/{customerId}",
 
         "api.master": "/skapi/services/master/{exchange}",
 
         "api.historical.data": "/skapi/services/historical/{exchange}/{scripcode}/{interval}"
     }
-    # try:
-    #     clientPublicIp = " " + get('https://api.ipify.org').text
-    #     if " " in clientPublicIp:
-    #         clientPublicIp = clientPublicIp.replace(" ", "") # Remove the space from the clientPublicIp string.
-    # except Exception as e:
-    #     print("Exception while retriving IP Address,using local host IP address", e)
-    # finally:
-    #     clientPublicIp = "106.193.147.98"
-    #     clientLocalIp = "127.0.0.1"
-    # # Retrieves the client's MAC address using the uuid.getnode() function and formats it as a colon-separated string
-    # clientMacAddress = ':'.join(re.findall('..', '%012x' % uuid.getnode()))
     accept = "application/json"
 
-    # userType = "USER"
-    # sourceID = "WEB"
     def __init__(self, api_key=None, state=None, vendor_key=None, access_token=None, refresh_token=None,
                  feed_token=None, userId=None, root=None,
                  debug=False, timeout=None, proxies=None, pool=None, disable_ssl=False, accept=None, userType=None,
                  sourceID=None, Authorization=None, clientPublicIP=None, clientMacAddress=None, clientLocalIP=None,
                  privateKey=None):
         self.refreshToken = None
         self.debug = debug
@@ -68,21 +55,16 @@
         self.refresh_token = refresh_token
         self.feed_token = feed_token
         self.userId = userId
         self.proxies = proxies if proxies else {}
         self.root = root or self._rootUrl
         self.timeout = timeout or self._default_timeout
         self.Authorization = None
-        # self.clientLocalIP = self.clientLocalIp
-        # self.clientPublicIP = self.clientPublicIp
-        # self.clientMacAddress = self.clientMacAddress
         self.privateKey = api_key
         self.accept = self.accept
-        # self.userType = self.userType
-        # self.sourceID = self.sourceID
 
         if pool:
             self.reqsession = requests.Session()
             reqadapter = requests.adapters.HTTPAdapter(**pool)
             self.reqsession.mount("https://", reqadapter)
             print("in pool")
         else:
@@ -202,15 +184,15 @@
         key = secret_key.encode('utf-8')
         iv = base64.b64decode("AAAAAAAAAAAAAAAAAAAAAA==")
 
         def encryptAPIString(plaintext):
             raw = plaintext.encode('utf-8')
             encryptor = Cipher(algorithms.AES(key), modes.GCM(iv, None, 16), default_backend()).encryptor()
             ciphertext = encryptor.update(raw) + encryptor.finalize()
-            return base64Encode(ciphertext + encryptor.tag)
+            return base64Encode(ciphertext + encryptor.tag).decode('utf-8')
 
         def decryptAPIString(ciphertext):
             enc = base64Decode(ciphertext)[:-16]
             decryptor = Cipher(algorithms.AES(key), modes.GCM(iv), default_backend()).decryptor()
             return decryptor.update(enc)
 
         def base64Encode(data):
@@ -239,25 +221,25 @@
             nonce = b'\x00' * 16
             skey_spec = AES.new(raw, AES.MODE_GCM, nonce=nonce)
             ciphertext, mac_tag = skey_spec.encrypt_and_digest(pad(non_encrypted_data.encode('utf-8'), AES.block_size))
             encrypted = ciphertext + mac_tag
             return base64.urlsafe_b64encode(encrypted).decode('utf-8')
 
         decrypted_code = decryption_method(secret_key, request_token)
-        print(decrypted_code)
+        # print(decrypted_code)
         result = decrypted_code.split('|')
         for s in result:
-            print(s)
+            s
+            # print(s)
         manipulated_code = result[1] + '|' + result[0]
-        print(manipulated_code)
+        # print(manipulated_code)
         msg = manipulated_code
         encStr = encryptAPIString(msg)
-        print("Encrypt :", encStr)
-        decStr = decryptAPIString(encStr)
-        print("Decrypt :", decStr)
+        # print("Encrypt :", encStr)
+        return encStr
 
     def generate_session(self, request_token, secret_key):
         import base64
         from Crypto.Cipher import AES
         from Crypto.Util.Padding import pad
         from cryptography.hazmat.backends import default_backend
         from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
@@ -267,20 +249,22 @@
         key = secret_key.encode('utf-8')
         iv = base64.b64decode("AAAAAAAAAAAAAAAAAAAAAA==")
 
         def encryptAPIString(plaintext):
             raw = plaintext.encode('utf-8')
             encryptor = Cipher(algorithms.AES(key), modes.GCM(iv, None, 16), default_backend()).encryptor()
             ciphertext = encryptor.update(raw) + encryptor.finalize()
-            return base64UrlEncode(ciphertext + encryptor.tag)
+            return base64UrlEncode(ciphertext + encryptor.tag).decode('utf-8')
 
         def decryptAPIString(ciphertext):
             enc = base64UrlDecode(ciphertext)[:-16]
             decryptor = Cipher(algorithms.AES(key), modes.GCM(iv), default_backend()).decryptor()
-            return decryptor.update(enc)
+            decrypted_bytes = decryptor.update(enc)
+            decrypted_string = decrypted_bytes.decode('utf-8')
+            return decrypted_string
 
         def base64UrlEncode(data):
             return urlsafe_b64encode(data).rstrip(b'=')
 
         def base64UrlDecode(base64Url):
             padding = b'=' * (4 - (len(base64Url) % 4))
             return urlsafe_b64decode(base64Url + padding)
@@ -306,42 +290,32 @@
             skey_spec = AES.new(raw, AES.MODE_GCM, nonce=nonce)
             ciphertext, mac_tag = skey_spec.encrypt_and_digest(pad(non_encrypted_data.encode('utf-8'), AES.block_size))
             encrypted = ciphertext + mac_tag
             return base64.urlsafe_b64encode(encrypted).decode('utf-8')
 
         request_token = urllib.parse.unquote(request_token)  # decode URL-encoded string
         decrypted_code = decryption_method(secret_key, request_token)
-        print(decrypted_code)
         result = decrypted_code.split('|')
-        for s in result:
-            print(s)
         manipulated_code = result[1] + '|' + result[0]
-        print(manipulated_code)
         msg = manipulated_code
         encStr = encryptAPIString(msg)
-        print("Encrypt :", encStr)
-        # return encStr
-        # decStr = decryptAPIString(encStr)
-        # print("Decrypt :", decStr)
+        # print("Encrypt :", encStr)
+        return encStr
 
-    def get_access_token(self, apiKey, requestToken, state, vendorkey=None, versionId=None):
+    def get_access_token(self, apiKey, encstr, state, vendorkey=None, versionId=None):
         url = f"{SharekhanConnect._rootUrl}{SharekhanConnect._routes['api.access.token']}"
         params = {
             'apiKey': apiKey,
-            'requestToken': requestToken,
+            'requestToken': encstr,
             'state': state
         }
         if vendorkey is not None:
             params['vendorkey'] = vendorkey
         if versionId is not None:
             params['versionId'] = versionId
-        # print(apiKey)
-        # print(requestToken)
-        # print(state)
-        # print(versionId)
         response = self._postRequest("api.access.token", params)
         return response
 
     def funds(self, exchange, customerId):
         fundsResponse = self._getRequest("api.fund.details", {"exchange": exchange, "customerId": customerId})
         return fundsResponse
```

### Comparing `shareconnect-1.0.0.10/SharekhanApi/sharekhanExceptions.py` & `shareconnect-1.0.0.11/SharekhanApi/sharekhanExceptions.py`

 * *Files identical despite different names*

### Comparing `shareconnect-1.0.0.10/SharekhanApi/sharekhanWebsocket.py` & `shareconnect-1.0.0.11/SharekhanApi/sharekhanWebsocket.py`

 * *Files identical despite different names*

### Comparing `shareconnect-1.0.0.10/setup.py` & `shareconnect-1.0.0.11/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         "requests>=2.18.4",
         "six>=1.11.0",
         "Crypto",
         "cryptography"
 ]
 setup(
     name='shareconnect',
-    version='1.0.0.10',
+    version='1.0.0.11',
     author='rg-sharekhanapi',
     author_email='shareconnect@sharekhan.com',
     description='Sharekhan Data Feed Trading Api Server',
     packages=find_packages(),
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requirements,
```

### Comparing `shareconnect-1.0.0.10/shareconnect.egg-info/PKG-INFO` & `shareconnect-1.0.0.11/shareconnect.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareconnect
-Version: 1.0.0.10
+Version: 1.0.0.11
 Summary: Sharekhan Data Feed Trading Api Server
 Home-page: UNKNOWN
 Author: rg-sharekhanapi
 Author-email: shareconnect@sharekhan.com
 License: UNKNOWN
 Description: # SHARECONNECT-PYTHON
         
@@ -27,41 +27,42 @@
             
             api_key = "Your API-KEY"
             login = SharekhanConnect(api_key)
             vendor_key = "Vendor key" 
                 """Pass the vendor key for vendor login otherwise keep it blank"""
             version_id = "Version Id"
                 """Only null/1005/1006 version id is allowed to be passed"""
+            state=12345
             url = login.login_url(vendor_key=vendor_key, version_id=version_id)
             """This will provide you the redirect login url which can be used to login in the sharekhan account"""
             print(url)
         
             
             """After Successfully Login You will receive the request token value then you have to decrypt the token value by using secret key and then swap the request token which is a combination of RequestId and CustomerId.Then after that decrypt the request token value."""
             
             request_token = "Valid Request Token Value"
             secret_key = "Your Secret Key value"
         
-            """Use generate session method when you are passing version id """
+           """Use generate session method when you are passing version id """
             session=login.generate_session(request_token,secret_key)
+            # Generating access token for version id and pass parameters as it is passed below 
+            access_token=login.get_access_token(api_key,session,state,versionId=version_id)
             
             """Use generate session without version id method when you are not passing version id """
             sessionwithoutvesionId=login.generate_session_without_versionId(request_token,secret_key)
+            # Generating access token for without version id 
+            access_token=login.get_access_token(api_key,sessionwithoutvesionId,state)
             
-            # Generate access token
-            
-            """ You have to pass the encrypted request token after manipulation """
-            
-            requestToken="Your Encrypted request token value getting from generate session method"
-            access_token=login.get_access_token(apiKey=api_key,requestToken,userId=12345,versionId=1005)
             print(access_token)
             
             # Make a object for SharekhanConnect class
             """Here we are passing the api-key, access-token and vendor-key(when needed) as a request header parameters"""
-            sharekhan = SharekhanConnect(api_key,access_token=access_token,vendor_key=vendor_key)
+            access_token = "Your access token value"
+            sharekhan = SharekhanConnect(api_key,access_token)
+            print(sharekhan.requestHeaders())       # for printing request headers
             
             # Place order history
             
              orderparams={
              "customerId": "XXXXXXX",
              "scripCode": 2475,
              "tradingSymbol": "ONGC",
```

### Comparing `shareconnect-1.0.0.10/test/test.py` & `shareconnect-1.0.0.11/test/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from SharekhanApi.sharekhanConnect import SharekhanConnect
 
-api_key = "Your API-KEY"
+api_key = "Your Api Key"
 login = SharekhanConnect(api_key)
-vendor_key = "Vendor key"
-version_id = "Version Id"
-url = login.login_url(vendor_key=vendor_key, version_id=version_id)
+vendor_key = ""         # vendor key for vendor login otherwise keep it null
+version_id = ""         # version id= 1005 or 1006 otherwise keep it null
+state=12345
+url = login.login_url(vendor_key, version_id)
 print(url)
 
 request_token="Your request token value after login"
-secret_key="Your secret key"
+secret_key="Your Secret key"
 
 """Use generate session method when you are passing version id """
 session=login.generate_session(request_token,secret_key)
+# Generating access token for version id and pass parameters as it is passed below
+access_token=login.get_access_token(api_key,session,state,versionId=version_id)
 
 """Use generate session without version id method when you are not passing version id """
 sessionwithoutvesionId=login.generate_session_without_versionId(request_token,secret_key)
+# Generating access token for without version id
+access_token=login.get_access_token(api_key,sessionwithoutvesionId,state)
 
-apiKey = api_key
-requestToken = "Your Encrypted request token value getting from generate session method"
-access_token=login.get_access_token(api_key,requestToken,state=12345, vendorkey=vendor_key, versionId=version_id)
 print(access_token)
-#
-access_token = "Your Access Token"
-sharekhan = SharekhanConnect(api_key,access_token=access_token,vendor_key=vendor_key)
-print(sharekhan.requestHeaders())
+access_token = "Your access token value"
+sharekhan = SharekhanConnect(api_key,access_token)
+print(sharekhan.requestHeaders())       # for printing request headers
 
 
 # Place order history
 
 orderparams={
  "customerId": "XXXXXXX",
  "scripCode": 2475,
@@ -148,26 +149,25 @@
 
 # # Historical Data
 
 exchange="BC"
 scripcode=500410
 interval="daily"
 order=sharekhan.historicaldata(exchange, scripcode, interval)
-print("Holdings Data: {}".format(order))
+print("Historical Data: {}".format(order))
 
 
 # websocket Programming Testing
 
 from SharekhanApi.sharekhanWebsocket import SharekhanWebSocket
 
 params = {
     "access_token": access_token
 }
 
-
 token_list = {"action": "subscribe", "key": ["feed"], "value": [""]}
 feed = {"action": "feed", "key": ["depth"], "value": ["MX250715"]}
 unsubscribefeed = {"action":"unsubscribe","key":["feed"],"value":["NC22,NF37833,NF37834,MX253461,RN7719"]}
 
 sws = SharekhanWebSocket(access_token)
```

