# Comparing `tmp/mecapacktools-1.0.4.tar.gz` & `tmp/mecapacktools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecapacktools-1.0.4.tar", max compression
+gzip compressed data, was "mecapacktools-1.1.0.tar", max compression
```

## Comparing `mecapacktools-1.0.4.tar` & `mecapacktools-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.0.4/LICENSE
--rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.0.4/mecapacktools/__init__.py
--rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.0.4/mecapacktools/libCfg.py
--rw-r--r--   0        0        0     5025 2023-06-05 13:13:15.138222 mecapacktools-1.0.4/mecapacktools/libFTP.py
--rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.0.4/mecapacktools/libLog.py
--rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.0.4/mecapacktools/libMail.py
--rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.0.4/mecapacktools/libSql.py
--rw-r--r--   0        0        0    14859 2023-05-03 07:59:47.610440 mecapacktools-1.0.4/mecapacktools/libTool.py
--rw-r--r--   0        0        0    20493 2023-06-05 09:14:51.310848 mecapacktools-1.0.4/mecapacktools/libWebServices.py
--rw-r--r--   0        0        0     1160 2023-06-05 13:13:40.878210 mecapacktools-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      676 2023-06-05 11:21:37.250074 mecapacktools-1.0.4/README.md
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 mecapacktools-1.0.4/setup.py
--rw-r--r--   0        0        0     1697 1970-01-01 00:00:00.000000 mecapacktools-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.1.0/mecapacktools/__init__.py
+-rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.1.0/mecapacktools/libCfg.py
+-rw-r--r--   0        0        0     5025 2023-06-05 13:13:15.138222 mecapacktools-1.1.0/mecapacktools/libFTP.py
+-rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.1.0/mecapacktools/libLog.py
+-rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.1.0/mecapacktools/libMail.py
+-rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.1.0/mecapacktools/libSql.py
+-rw-r--r--   0        0        0    14859 2023-05-03 07:59:47.610440 mecapacktools-1.1.0/mecapacktools/libTool.py
+-rw-r--r--   0        0        0    20319 2023-06-07 08:51:38.798095 mecapacktools-1.1.0/mecapacktools/libWebServices.py
+-rw-r--r--   0        0        0     1161 2023-06-14 10:11:29.107682 mecapacktools-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      676 2023-06-05 11:21:37.250074 mecapacktools-1.1.0/README.md
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 mecapacktools-1.1.0/setup.py
+-rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 mecapacktools-1.1.0/PKG-INFO
```

### Comparing `mecapacktools-1.0.4/LICENSE` & `mecapacktools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.4/mecapacktools/libCfg.py` & `mecapacktools-1.1.0/mecapacktools/libCfg.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.4/mecapacktools/libFTP.py` & `mecapacktools-1.1.0/mecapacktools/libFTP.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.4/mecapacktools/libLog.py` & `mecapacktools-1.1.0/mecapacktools/libLog.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.4/mecapacktools/libMail.py` & `mecapacktools-1.1.0/mecapacktools/libMail.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.4/mecapacktools/libSql.py` & `mecapacktools-1.1.0/mecapacktools/libSql.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.4/mecapacktools/libTool.py` & `mecapacktools-1.1.0/mecapacktools/libTool.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.4/mecapacktools/libWebServices.py` & `mecapacktools-1.1.0/mecapacktools/libWebServices.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,15 +443,15 @@
                 </soap:Body>
             </soap:Envelope>
             """
         )
 
         self.hshParam.update(phshParam)
 
-    # pylint: disable-next=unused-argument
+    # pylint: disable=unused-argument,too-many-locals,broad-exception-caught,broad-exception-raised
     def Call(self, pqueryfilter, pbind=None, pparameters=None, **kw):
         """
         Lancement du web services avec infos à passer et résultats stockés dans data
 
         Args:
             pqueryfilter (str): filter string in queries dictionary
             pparameters (xml, optional): dict of key, value to send. Defaults to None.
@@ -500,31 +500,27 @@
             # prepared = self.session.prepare_request(req)
             # del prepared.headers["accept-encoding"]
             # resp = self.session.send(prepared)
             if resp.status_code != 200:
                 try:
                     # Récupérer le message contenu dans le xml
                     msg = xmltodict.parse(resp.text)["SOAP-ENV:Envelope"]["SOAP-ENV:Body"]["SOAP-ENV:Fault"]
-                # pylint: disable-next=broad-exception-caught
                 except Exception:
                     msg = resp.text
-                # pylint: disable-next=broad-exception-raised
                 raise Exception(f"get /{pqueryfilter}/ {resp.status_code} : {msg}")
             # Transcrire le XML et récupérer le contenu significatif
             content = xmltodict.parse(resp.text)["SOAP-ENV:Envelope"]["SOAP-ENV:Body"][f"ns1:{request}Response"][
                 "return"
             ]
-            if content["type_erreur"]["#text"] != "000":
+            if content["type_erreur"]["#text"] not in ["000", "251"]:
                 # ERREUR d'envoi
-                # pylint: disable-next=broad-exception-raised
                 raise Exception(f"retour /{pqueryfilter}/: {content['msg_erreur']['#text']}")
+            # décoder HTML
+            if "xml" in content:
+                self.__hshData[key] = xmltodict.parse(content["xml"]["#text"])
             else:
-                # décoder HTML
-                if "xml" in content:
-                    self.__hshData[key] = xmltodict.parse(content["xml"]["#text"])
-                else:
-                    res = {}
-                    for k, v in content.items():
-                        if "#text" in v:
-                            res[k] = v["#text"]
-                    self.__hshData[key] = res
+                res = {}
+                for k, v in content.items():
+                    if "#text" in v:
+                        res[k] = v["#text"]
+                self.__hshData[key] = res
             self.log.setStep = ""
```

### Comparing `mecapacktools-1.0.4/pyproject.toml` & `mecapacktools-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "mecapacktools"
-version = "1.0.4"
+version = "1.1.0"
 description = ""
 authors = ["Informatique Mecapack <informatique@mecapack.com>"]
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 exclude = ["mecapacktools/libExcel.py"]
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.11"
 arrow = "^1.2.3"
 sortedcontainers = "^2.4.0"
 requests = {version = "^2.28.2", optional = true}
 suds = {version = "^1.1.2", optional = true}
 xmltodict = {version = "^0.13.0", optional = true}
 pypyodbc = {version = "^1.3.6", optional = true}
 openpyxl = {version = "^3.1.2", optional = true}
```

### Comparing `mecapacktools-1.0.4/README.md` & `mecapacktools-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.4/setup.py` & `mecapacktools-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,24 +16,24 @@
  'sql': ['pypyodbc>=1.3.6,<2.0.0'],
  'webservices': ['requests>=2.28.2,<3.0.0',
                  'suds>=1.1.2,<2.0.0',
                  'xmltodict>=0.13.0,<0.14.0']}
 
 setup_kwargs = {
     'name': 'mecapacktools',
-    'version': '1.0.4',
+    'version': '1.1.0',
     'description': '',
     'long_description': '# Tools for Mecapack\n\nLa doc est disponible en Html ou en MD\n\n## installation par pip\n\n`pip install mecapacktools`\n\nInstaller les extensions :\n\n`pip install mecapacktools[excel,sql,webservices]`\n\n### Extensions diponibles :\n\n- excel \n- Sql \n- WebServices \n- FTP \n\n## Notes pour le développement:\n\n### Installation\n\n`poetry install --with dev --all-extras`\n\n### Génération de la doc\n\n`poetry run .\\make.bat html`\n`poetry run .\\make.bat markdown`\n\n### Publier une nouvelle version\n\nChanger la version :\nDans le fichier pyproject.toml modifier :\n```\n[tool.poetry]\nversion = "1.0.0"\n ```\n\nPublier sur pypi `poetry publish --build`\n\n\n\n',
     'author': 'Informatique Mecapack',
     'author_email': 'informatique@mecapack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.11,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mecapacktools-1.0.4/PKG-INFO` & `mecapacktools-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: mecapacktools
-Version: 1.0.4
+Version: 1.1.0
 Summary: 
 Author: Informatique Mecapack
 Author-email: informatique@mecapack.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: excel
 Provides-Extra: ftp
 Provides-Extra: sql
 Provides-Extra: webservices
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0) ; extra == "excel"
```

