# Comparing `tmp/kadaster_kikinzage_client-0.1.1.tar.gz` & `tmp/kadaster_kikinzage_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kadaster_kikinzage_client-0.1.1.tar", max compression
+gzip compressed data, was "kadaster_kikinzage_client-0.1.2.tar", max compression
```

## Comparing `kadaster_kikinzage_client-0.1.1.tar` & `kadaster_kikinzage_client-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1071 2023-06-14 09:12:05.674396 kadaster_kikinzage_client-0.1.1/LICENSE
--rw-r--r--   0        0        0     2891 2023-06-14 09:12:05.674396 kadaster_kikinzage_client-0.1.1/README.md
--rw-r--r--   0        0        0     2084 2023-06-14 09:12:26.638627 kadaster_kikinzage_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       45 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/__init__.py
--rw-r--r--   0        0        0     2278 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/__main__.py
--rw-r--r--   0        0        0      302 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/client/__init__.py
--rw-r--r--   0        0        0     3024 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/client/asyncio.py
--rw-r--r--   0        0        0     9087 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/client/base.py
--rw-r--r--   0        0        0     6444 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/client/default.py
--rw-r--r--   0        0        0      610 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/client/errors.py
--rw-r--r--   0        0        0      182 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/client/utils.py
--rw-r--r--   0        0        0      145 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/models/__init__.py
--rw-r--r--   0        0        0    37698 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/models/generated.py
--rw-r--r--   0        0        0        0 2023-06-14 09:12:05.678396 kadaster_kikinzage_client-0.1.1/src/kikinzage/py.typed
--rw-r--r--   0        0        0     3897 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-14 09:39:27.090443 kadaster_kikinzage_client-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4027 2023-06-14 09:39:27.094443 kadaster_kikinzage_client-0.1.2/README.md
+-rw-r--r--   0        0        0     2084 2023-06-14 09:39:45.890788 kadaster_kikinzage_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-06-14 09:39:27.098443 kadaster_kikinzage_client-0.1.2/src/kikinzage/__init__.py
+-rw-r--r--   0        0        0     2274 2023-06-14 09:39:27.098443 kadaster_kikinzage_client-0.1.2/src/kikinzage/__main__.py
+-rw-r--r--   0        0        0      302 2023-06-14 09:39:27.098443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/__init__.py
+-rw-r--r--   0        0        0     3442 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/asyncio.py
+-rw-r--r--   0        0        0     9087 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/base.py
+-rw-r--r--   0        0        0     6428 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/default.py
+-rw-r--r--   0        0        0      610 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/errors.py
+-rw-r--r--   0        0        0      182 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/utils.py
+-rw-r--r--   0        0        0      145 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/models/__init__.py
+-rw-r--r--   0        0        0    37698 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/models/generated.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/py.typed
+-rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.2/PKG-INFO
```

### Comparing `kadaster_kikinzage_client-0.1.1/LICENSE` & `kadaster_kikinzage_client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.1/pyproject.toml` & `kadaster_kikinzage_client-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kadaster-kikinzage-client"
-version = "0.1.1"
+version = "0.1.2"
 description = " Kadaster - KIK Inzage API Python client"
 authors = ["Jelmer Draaijer <info@jelmert.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 repository = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 documentation = "https://kadaster-kik-inzage-api-python-client.readthedocs.io"
```

### Comparing `kadaster_kikinzage_client-0.1.1/src/kikinzage/__main__.py` & `kadaster_kikinzage_client-0.1.2/src/kikinzage/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     kik = DefaultClient(
         username=os.getenv("KIK_USERNAME", default="EMPTY"),
         password=os.getenv("KIK_PASSWORD", default="EMPTY"),
         event_hooks={"response": [log_response]},
     )
 
-    kik.eigendomsinformatie_postcode_get(
+    kik.eigendomsinformatie_postcode(
         postcode=postcode,
         huisnummer=huisnummer,
         formaat=Formaat.JSON,
         klantreferentie="onbekend",
     )
 
     with response_path.open("w+") as f:
```

### Comparing `kadaster_kikinzage_client-0.1.1/src/kikinzage/client/asyncio.py` & `kadaster_kikinzage_client-0.1.2/src/kikinzage/client/asyncio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from types import TracebackType
 from typing import Any
 from typing import Optional
 from typing import Type
 from typing import Union
 
 import httpx
 from httpx import USE_CLIENT_DEFAULT
@@ -47,15 +48,15 @@
         httpx_kwargs.setdefault("auth", (self.username, self.password))
 
         self.client = self.create_client(**httpx_kwargs)
 
     def create_client(self, **httpx_kwargs: Any) -> httpx.AsyncClient:
         return httpx.AsyncClient(**httpx_kwargs)
 
-    async def eigendomsinformatie_kadastraalobjectidentificatie_get(
+    async def eigendomsinformatie_kadastraalobjectidentificatie(
         self,
         kadastraalobjectidentificatie: str,
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
@@ -80,7 +81,19 @@
         request: httpx.Request,
         model: Type[ResponseType],
         status_code_success: int = 200,
     ) -> ResponseType:
         response = await self.client.send(request)
 
         return self.process_response(response, model, status_code_success)
+
+    async def __aenter__(self) -> "AsyncClient":
+        await self.client.__aenter__()
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_value: Optional[BaseException] = None,
+        traceback: Optional[TracebackType] = None,
+    ) -> None:
+        await self.client.__aexit__(exc_type, exc_value, traceback)
```

### Comparing `kadaster_kikinzage_client-0.1.1/src/kikinzage/client/base.py` & `kadaster_kikinzage_client-0.1.2/src/kikinzage/client/base.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.1/src/kikinzage/client/default.py` & `kadaster_kikinzage_client-0.1.2/src/kikinzage/client/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         httpx_kwargs.setdefault("auth", (self.username, self.password))
 
         self.client = self.create_client(**httpx_kwargs)
 
     def create_client(self, **httpx_kwargs: Any) -> httpx.Client:
         return httpx.Client(**httpx_kwargs)
 
-    def eigendomsinformatie_kadastraalobjectidentificatie_get(
+    def eigendomsinformatie_kadastraalobjectidentificatie(
         self,
         kadastraalobjectidentificatie: str,
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
@@ -71,15 +71,15 @@
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         return self.send(request, models.Eigendomsinformatie)
 
-    def eigendomsinformatie_kadastraleaanduiding_get(
+    def eigendomsinformatie_kadastraleaanduiding(
         self,
         kadastralegemeente: str,
         sectie: str,
         perceelnummer: int,
         appartementsrecht_volgnummer: Optional[int] = None,
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
@@ -99,15 +99,15 @@
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         return self.send(request, models.Eigendomsinformatie)
 
-    def eigendomsinformatie_postcode_get(
+    def eigendomsinformatie_postcode(
         self,
         postcode: str,
         huisnummer: str,
         huisletter: Optional[str] = None,
         huisnummertoevoeging: Optional[str] = None,
         *,
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
@@ -128,15 +128,15 @@
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         return self.send(request, models.Eigendomsinformatie)
 
-    def eigendomsinformatie_adres_get(
+    def eigendomsinformatie_adres(
         self,
         plaatsnaam: str,
         straatnaam: str,
         huisnummer: int,
         huisletter: Optional[str] = None,
         *,
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
```

### Comparing `kadaster_kikinzage_client-0.1.1/src/kikinzage/client/errors.py` & `kadaster_kikinzage_client-0.1.2/src/kikinzage/client/errors.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.1/src/kikinzage/models/generated.py` & `kadaster_kikinzage_client-0.1.2/src/kikinzage/models/generated.py`

 * *Files identical despite different names*

