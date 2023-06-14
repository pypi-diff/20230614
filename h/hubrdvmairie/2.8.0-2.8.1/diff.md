# Comparing `tmp/hubrdvmairie-2.8.0.tar.gz` & `tmp/hubrdvmairie-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubrdvmairie-2.8.0.tar", last modified: Mon Feb 13 09:22:03 2023, max compression
+gzip compressed data, was "hubrdvmairie-2.8.1.tar", last modified: Wed Mar  8 22:19:08 2023, max compression
```

## Comparing `hubrdvmairie-2.8.0.tar` & `hubrdvmairie-2.8.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.961598 hubrdvmairie-2.8.0/
--rw-rw-rw-   0        0        0     1098 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.0/LICENSE
--rw-rw-rw-   0        0        0     1821 2023-02-13 09:22:03.959754 hubrdvmairie-2.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1265 2023-02-06 18:32:04.000000 hubrdvmairie-2.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-13 09:22:03.962874 hubrdvmairie-2.8.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.485574 hubrdvmairie-2.8.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.516405 hubrdvmairie-2.8.0/src/hubrdvmairie/
--rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.591287 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/
--rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/__init__.py
--rw-rw-rw-   0        0        0      450 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/controller.py
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.605481 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/dependencies/
--rw-rw-rw-   0        0        0      584 2023-01-13 12:55:59.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/dependencies/auth_token.py
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.685048 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/routes/
--rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/routes/__init__.py
--rw-rw-rw-   0        0        0     9377 2023-01-11 09:44:08.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/routes/external.py
--rw-rw-rw-   0        0        0     5819 2023-01-06 13:48:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/routes/internal.py
--rw-rw-rw-   0        0        0     5531 2023-02-10 10:19:06.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/routes/time_slots.py
--rw-rw-rw-   0        0        0     4221 2023-02-10 10:19:06.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/routes/websocket.py
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.717527 hubrdvmairie-2.8.0/src/hubrdvmairie/core/
--rw-rw-rw-   0        0        0      149 2022-11-28 13:35:51.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/core/__init__.py
--rw-rw-rw-   0        0        0      599 2022-11-10 16:30:03.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/core/config.py
--rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/core/errors.py
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.732705 hubrdvmairie-2.8.0/src/hubrdvmairie/db/
--rw-rw-rw-   0        0        0     1723 2022-12-26 11:40:19.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/db/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.765523 hubrdvmairie-2.8.0/src/hubrdvmairie/logging/
--rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/logging/__init__.py
--rw-rw-rw-   0        0        0     3054 2023-01-06 13:48:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/logging/app_logger.py
--rw-rw-rw-   0        0        0     1515 2022-12-22 15:37:17.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/logging/app_logger_formatter.py
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.881595 hubrdvmairie-2.8.0/src/hubrdvmairie/models/
--rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/models/__init__.py
--rw-rw-rw-   0        0        0      128 2022-12-13 08:27:01.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/models/announcement.py
--rw-rw-rw-   0        0        0      194 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/models/application.py
--rw-rw-rw-   0        0        0      153 2022-11-16 16:37:28.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/models/available_time_slot.py
--rw-rw-rw-   0        0        0    19014 2023-02-06 00:32:54.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/models/editor.py
--rw-rw-rw-   0        0        0      150 2023-01-06 13:48:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/models/editor_model.py
--rw-rw-rw-   0        0        0      705 2022-12-27 13:11:22.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/models/municipality.py
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.957695 hubrdvmairie-2.8.0/src/hubrdvmairie/services/
--rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/services/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-02-10 10:19:06.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/services/data_validator.py
--rw-rw-rw-   0        0        0     7840 2022-12-22 15:37:17.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/services/mock_data.py
--rw-rw-rw-   0        0        0      943 2023-01-28 13:31:23.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/services/scheduled_functions.py
--rw-rw-rw-   0        0        0     1520 2023-01-28 13:31:23.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/services/search_meeting_points.py
--rw-rw-rw-   0        0        0     2613 2023-02-10 10:19:06.000000 hubrdvmairie-2.8.0/src/hubrdvmairie/services/search_time_slots.py
-drwxrwxrwx   0        0        0        0 2023-02-13 09:22:03.571478 hubrdvmairie-2.8.0/src/hubrdvmairie.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-02-13 09:22:03.000000 hubrdvmairie-2.8.0/src/hubrdvmairie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1429 2023-02-13 09:22:03.000000 hubrdvmairie-2.8.0/src/hubrdvmairie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 09:22:03.000000 hubrdvmairie-2.8.0/src/hubrdvmairie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      291 2023-02-13 09:22:03.000000 hubrdvmairie-2.8.0/src/hubrdvmairie.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-13 09:22:03.000000 hubrdvmairie-2.8.0/src/hubrdvmairie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.568486 hubrdvmairie-2.8.1/
+-rw-rw-rw-   0        0        0     1098 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.1/LICENSE
+-rw-rw-rw-   0        0        0     1821 2023-03-08 22:19:08.566139 hubrdvmairie-2.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1420 2023-03-08 22:18:01.000000 hubrdvmairie-2.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-08 22:19:08.569606 hubrdvmairie-2.8.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.183138 hubrdvmairie-2.8.1/src/
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.265109 hubrdvmairie-2.8.1/src/hubrdvmairie/
+-rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.376649 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/
+-rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/__init__.py
+-rw-rw-rw-   0        0        0      450 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/controller.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.382400 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/dependencies/
+-rw-rw-rw-   0        0        0      584 2023-02-22 16:10:51.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/dependencies/auth_token.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.415027 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/routes/
+-rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/routes/__init__.py
+-rw-rw-rw-   0        0        0     9377 2023-02-22 16:10:51.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/routes/external.py
+-rw-rw-rw-   0        0        0     7862 2023-03-08 18:14:44.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/routes/internal.py
+-rw-rw-rw-   0        0        0     5531 2023-02-22 16:10:51.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/routes/time_slots.py
+-rw-rw-rw-   0        0        0     4221 2023-02-22 16:10:51.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/routes/websocket.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.434322 hubrdvmairie-2.8.1/src/hubrdvmairie/core/
+-rw-rw-rw-   0        0        0      149 2022-11-28 13:35:51.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/core/__init__.py
+-rw-rw-rw-   0        0        0      636 2023-03-08 18:14:44.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/core/config.py
+-rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/core/errors.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.439758 hubrdvmairie-2.8.1/src/hubrdvmairie/db/
+-rw-rw-rw-   0        0        0     4745 2023-03-08 18:14:44.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/db/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.455659 hubrdvmairie-2.8.1/src/hubrdvmairie/logging/
+-rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/logging/__init__.py
+-rw-rw-rw-   0        0        0     3054 2023-02-22 16:10:51.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/logging/app_logger.py
+-rw-rw-rw-   0        0        0     1515 2022-12-22 15:37:17.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/logging/app_logger_formatter.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.506013 hubrdvmairie-2.8.1/src/hubrdvmairie/models/
+-rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/models/__init__.py
+-rw-rw-rw-   0        0        0      128 2022-12-13 08:27:01.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/models/announcement.py
+-rw-rw-rw-   0        0        0      194 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/models/application.py
+-rw-rw-rw-   0        0        0      153 2022-11-16 16:37:28.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/models/available_time_slot.py
+-rw-rw-rw-   0        0        0    19390 2023-03-08 21:34:09.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/models/editor.py
+-rw-rw-rw-   0        0        0      150 2023-02-22 16:10:51.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/models/editor_model.py
+-rw-rw-rw-   0        0        0     1076 2023-03-08 18:14:44.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/models/municipality.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.560261 hubrdvmairie-2.8.1/src/hubrdvmairie/services/
+-rw-rw-rw-   0        0        0        0 2022-11-04 09:15:48.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/services/__init__.py
+-rw-rw-rw-   0        0        0     1628 2023-02-22 16:10:51.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/services/data_validator.py
+-rw-rw-rw-   0        0        0      632 2023-03-08 18:14:45.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/services/excel_helper.py
+-rw-rw-rw-   0        0        0     7840 2022-12-22 15:37:17.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/services/mock_data.py
+-rw-rw-rw-   0        0        0      943 2023-02-22 16:10:51.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/services/scheduled_functions.py
+-rw-rw-rw-   0        0        0     2938 2023-03-08 18:14:45.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/services/search_meeting_points.py
+-rw-rw-rw-   0        0        0     2613 2023-02-22 16:10:51.000000 hubrdvmairie-2.8.1/src/hubrdvmairie/services/search_time_slots.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:19:08.360732 hubrdvmairie-2.8.1/src/hubrdvmairie.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-03-08 22:19:08.000000 hubrdvmairie-2.8.1/src/hubrdvmairie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1471 2023-03-08 22:19:08.000000 hubrdvmairie-2.8.1/src/hubrdvmairie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-08 22:19:08.000000 hubrdvmairie-2.8.1/src/hubrdvmairie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      385 2023-03-08 22:19:08.000000 hubrdvmairie-2.8.1/src/hubrdvmairie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-03-08 22:19:08.000000 hubrdvmairie-2.8.1/src/hubrdvmairie.egg-info/top_level.txt
```

### Comparing `hubrdvmairie-2.8.0/LICENSE` & `hubrdvmairie-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/PKG-INFO` & `hubrdvmairie-2.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubrdvmairie
-Version: 2.8.0
+Version: 2.8.1
 Summary: API de la plateforme de recherche de rendez-vous mairies
 Author-email: ANTS <ants-rdvmairie@interieur.gouv.fr>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `hubrdvmairie-2.8.0/pyproject.toml` & `hubrdvmairie-2.8.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hubrdvmairie"
-version = "2.8.0"
+version = "2.8.1"
 description = "API de la plateforme de recherche de rendez-vous mairies"
 readme = "README.md"
 authors = [{ name = "ANTS", email = "ants-rdvmairie@interieur.gouv.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["rendez-vous", "mairie", "proxy", "pré-demande", "passeport", "CNI"]
 dependencies = [
-    "asyncio >= 3.4.3",
-    "fastapi >= 0.79.0",
-    "fastapi-utils >= 0.2.1",
-    "geopy >= 2.2.0",
-    "pydantic >= 1.9.1",
-    "python-dotenv >= 0.20.0",
-    "requests >= 2.28.1",
-    "requests-async >= 0.6.2",
-    "uvicorn >= 0.18.2",
-    "websockets >= 10.3",
-    "pytest-mock >= 3.8.2"
+    "asyncio == 3.4.3",
+    "fastapi == 0.87.0",
+    "fastapi-utils == 0.2.1",
+    "geopy == 2.2.0",
+    "pydantic == 1.9.1",
+    "python-dotenv == 0.20.0",
+    "slowapi == 0.1.6", 
+    "uvicorn == 0.18.2",
+    "websockets == 10.3",
+    "pytest-mock == 3.8.2",
+    "secweb == 1.6.0",
+    "markdown == 3.4.1",
+    "unidecode == 1.3.6",
+    "httpx == 0.23.3",
+    "requests == 2.28.1",
+    "msoffcrypto-tool == 5.0.1",
+    "openpyxl == 3.1.1"
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black", "flake8", "isort", "autoflake", "bandit", "pytest", "pytest-asyncio", "pytest-mock", "pytest-cov", "coverage"]
 
 [project.urls]
```

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/dependencies/auth_token.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/dependencies/auth_token.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/routes/external.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/routes/external.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/routes/internal.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/routes/internal.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,28 +3,40 @@
 
 from fastapi import APIRouter, Query, Request, Response
 from markdown import markdown
 from pydantic import Required
 from slowapi import Limiter
 from slowapi.util import get_remote_address
 
-from ...db.utils import get_all_editors, get_all_meeting_points
+from ...db.utils import (
+    get_all_editors,
+    get_all_meeting_points,
+    get_all_offline_meeting_points,
+)
 from ...models.announcement import Announcement
 from ...models.editor_model import Editor
-from ...models.municipality import MuncipalityWithDistance, Municipality
-from ...services.search_meeting_points import search_close_meeting_points
+from ...models.municipality import (
+    Municipality,
+    MunicipalityWithDistance,
+    OfflineMunicipality,
+    OfflineMunicipalityWithDistance,
+)
+from ...services.search_meeting_points import (
+    search_close_meeting_points,
+    search_close_offline_meeting_points,
+)
 
 router = APIRouter()
 
 limiter = Limiter(key_func=get_remote_address)
 
 
 @router.get(
     "/MeetingPointsFromPosition",
-    response_model=List[MuncipalityWithDistance],
+    response_model=List[MunicipalityWithDistance],
     responses={
         200: {
             "description": "Meeting Points successfully found",
             "content": {
                 "application/json": {
                     "example": [
                         {
@@ -47,20 +59,20 @@
 )
 @limiter.limit("30/minute")
 def meeting_points_from_position(
     request: Request,
     longitude: float = Query(default=Required, example=2.352222),
     latitude: float = Query(default=Required, example=48.856613),
     radius_km: int = Query(default=20, enum=[20, 40, 60]),
-) -> List[MuncipalityWithDistance]:
+) -> List[MunicipalityWithDistance]:
     """
     Search Meeting Point from position.
     """
     all_points: List[Municipality] = get_all_meeting_points()
-    meeting_points: List[MuncipalityWithDistance] = search_close_meeting_points(
+    meeting_points: List[MunicipalityWithDistance] = search_close_meeting_points(
         all_points, latitude, longitude, radius_km
     )
     return meeting_points
 
 
 @router.get(
     "/Announcement",
@@ -166,7 +178,54 @@
 )
 @limiter.limit("30/minute")
 def get_editors(request: Request) -> List[Editor]:
     """
     Get editor detail.
     """
     return {"editors": get_all_editors()}
+
+
+@router.get(
+    "/searchOfflineMeetingPoints",
+    response_model=List[OfflineMunicipalityWithDistance],
+    responses={
+        200: {
+            "description": "Search for offline meeting points completed",
+            "content": {
+                "application/json": {
+                    "example": [
+                        {
+                            "id": "201",
+                            "name": "Paris 10",
+                            "longitude": 2.357828,
+                            "latitude": 48.8717442,
+                            "public_entry_address": "72 Rue du Faubourg Saint-Martin",
+                            "zip_code": "75010",
+                            "city_name": "Paris",
+                            "decoded_city_name": "paris",
+                            "website": "https://mairie10.paris.fr",
+                            "city_logo": "https://b1425524.smushcdn.com/1425524/wp-content/uploads/Creation-logo-paris.png?lossy=1&strip=1&webp=1",
+                            "distance_km": 1.56,
+                        }
+                    ]
+                }
+            },
+        }
+    },
+)
+@limiter.limit("30/minute")
+def search_offline_meeting_points(
+    request: Request,
+    longitude: float = Query(default=Required, example=2.352222),
+    latitude: float = Query(default=Required, example=48.856613),
+    radius_km: int = Query(default=20, enum=[20, 40, 60]),
+) -> List[OfflineMunicipalityWithDistance]:
+    """
+    Search surrounding offline meeting points.
+    """
+    all_offline_points: List[OfflineMunicipality] = get_all_offline_meeting_points()
+    meeting_points: List[
+        OfflineMunicipalityWithDistance
+    ] = search_close_offline_meeting_points(
+        all_offline_points, latitude, longitude, radius_km
+    )
+    return meeting_points
```

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/routes/time_slots.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/routes/time_slots.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/controllers/routes/websocket.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/controllers/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/core/config.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/core/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     project_name: str = "HUB RDV"
 
     logging_level: int = logging.DEBUG if debug else logging.INFO
     loggers: Set[str] = {"uvicorn.asgi", "uvicorn.access"}
 
     editors_list = []
     meeting_point_list = []
+    offline_meeting_point_list = []
     ws_use_rates = {}
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
```

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/logging/app_logger.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/logging/app_logger.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/logging/app_logger_formatter.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/logging/app_logger_formatter.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/models/editor.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/models/editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+# pylint: disable=C0415
 import asyncio
 import json
 import logging
 import os
 import random
 import threading
 import time
 from datetime import date, datetime, timedelta
 
 import httpx
 from fastapi import WebSocket
 from httpx import ConnectTimeout, ReadTimeout
 from pydantic import ValidationError
 
-from ..db import utils
 from ..logging.app_logger import write_external_service_data
 from ..services.mock_data import get_mock_managed_meeting_points, get_mock_slots
 from .application import Application
 from .municipality import Municipality
 
 
 class Editor:
@@ -370,17 +370,22 @@
 
         counter = 0
         while counter < 60 * 20:
             time.sleep(1 * 60)
             try:
                 meeting_points = self.get_managed_meeting_points()
                 if meeting_points:
-                    all_meeting_points = utils.get_all_meeting_points()
+                    from ..db.utils import (
+                        get_all_meeting_points,
+                        set_all_meeting_points,
+                    )
+
+                    all_meeting_points = get_all_meeting_points()
                     all_meeting_points += meeting_points
-                    utils.set_all_meeting_points(all_meeting_points)
+                    set_all_meeting_points(all_meeting_points)
                     break
                 else:
                     raise Exception(f"No meeting points found for editor {self.name}")
             except Exception as retry_get_managed_meeting_points_e:
                 _logger.error(
                     "Error while retrying to get managed meeting for editor %s : %s",
                     self.name,
@@ -425,14 +430,21 @@
     )
     numesia_editor = Editor(
         "numesia", "Numesia", "https://rdvs.numesia.fr/api", False, True
     )
     info_local_editor = Editor(
         "infolocal", "InfoLocale", "https://api.rdvenmairie.fr/api", False, True
     )
+    agglocompiegne_editor = Editor(
+        "agglocompiegne",
+        "AggloCompiegne",
+        "https://demarches.agglo-compiegne.fr/api",
+        False,
+        True,
+    )
     mega_editor = Editor("mega", "Mega", "https://www.mega.com", True, True)
     orionRDV_editor = Editor(
         "orionRDV", "OrionRDV", "https://orionrdv.com/", True, True
     )
     if os.environ.get("MOCK_EDITORS") in ["True", True]:
         return [citopia_editor, mega_editor, orionRDV_editor, synbird_editor]
     else:
@@ -443,8 +455,9 @@
             # troov_editor,
             rdv_360_editor,
             ypok_editor,
             solocal_editor,
             smartagenda_editor,
             numesia_editor,
             info_local_editor,
+            agglocompiegne_editor,
         ]
```

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/models/municipality.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/models/municipality.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,13 +19,30 @@
     city_logo: Optional[str]
     _editor_name: Optional[str]
 
     class Config:
         underscore_attrs_are_private = True
 
 
-class MuncipalityWithDistance(Municipality):
+class MunicipalityWithDistance(Municipality):
     distance_km: float
 
 
-class MunicipalityWithSlots(MuncipalityWithDistance):
+class MunicipalityWithSlots(MunicipalityWithDistance):
     available_slots: List[AvailableTimeSlot]
+
+
+class OfflineMunicipality(BaseModel):
+    id: str
+    name: str
+    longitude: float
+    latitude: float
+    public_entry_address: str
+    zip_code: str
+    city_name: str
+    decoded_city_name: Optional[str]
+    website: Optional[str]
+    city_logo: Optional[str]
+
+
+class OfflineMunicipalityWithDistance(OfflineMunicipality):
+    distance_km: float
```

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/services/data_validator.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/services/data_validator.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/services/mock_data.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/services/mock_data.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/services/scheduled_functions.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/services/scheduled_functions.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie/services/search_time_slots.py` & `hubrdvmairie-2.8.1/src/hubrdvmairie/services/search_time_slots.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie.egg-info/PKG-INFO` & `hubrdvmairie-2.8.1/src/hubrdvmairie.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubrdvmairie
-Version: 2.8.0
+Version: 2.8.1
 Summary: API de la plateforme de recherche de rendez-vous mairies
 Author-email: ANTS <ants-rdvmairie@interieur.gouv.fr>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `hubrdvmairie-2.8.0/src/hubrdvmairie.egg-info/SOURCES.txt` & `hubrdvmairie-2.8.1/src/hubrdvmairie.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,11 +26,12 @@
 src/hubrdvmairie/models/application.py
 src/hubrdvmairie/models/available_time_slot.py
 src/hubrdvmairie/models/editor.py
 src/hubrdvmairie/models/editor_model.py
 src/hubrdvmairie/models/municipality.py
 src/hubrdvmairie/services/__init__.py
 src/hubrdvmairie/services/data_validator.py
+src/hubrdvmairie/services/excel_helper.py
 src/hubrdvmairie/services/mock_data.py
 src/hubrdvmairie/services/scheduled_functions.py
 src/hubrdvmairie/services/search_meeting_points.py
 src/hubrdvmairie/services/search_time_slots.py
```

