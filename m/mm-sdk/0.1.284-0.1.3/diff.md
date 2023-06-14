# Comparing `tmp/mm_sdk-0.1.284.tar.gz` & `tmp/mm-sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mm_sdk-0.1.284.tar", max compression
+gzip compressed data, was "mm-sdk-0.1.3.tar", max compression
```

## Comparing `mm_sdk-0.1.284.tar` & `mm-sdk-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0      943 2023-06-14 08:32:38.541417 mm_sdk-0.1.284/pyproject.toml
--rw-r--r--   0        0        0     1523 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/__init__.py
--rw-r--r--   0        0        0     3260 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/admitad.py
--rw-r--r--   0        0        0     3235 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/analytics.py
--rw-r--r--   0        0        0      770 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/barcode_recognizer.py
--rw-r--r--   0        0        0      251 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/base.py
--rw-r--r--   0        0        0     3961 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/cash_register.py
--rw-r--r--   0        0        0     7989 2023-05-10 10:02:03.000000 mm_sdk-0.1.284/sdk/client.py
--rw-r--r--   0        0        0     2504 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/elk.py
--rw-r--r--   0        0        0     1661 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/face_detector.py
--rw-r--r--   0        0        0     1418 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/gift.py
--rw-r--r--   0        0        0    19444 2023-06-14 08:29:44.000000 mm_sdk-0.1.284/sdk/gigtest.py
--rw-r--r--   0        0        0        0 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/mis/__init__.py
--rw-r--r--   0        0        0     1789 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/mis/client.py
--rw-r--r--   0        0        0     3471 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/mis/crm.py
--rw-r--r--   0        0        0     3055 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/mis/lab.py
--rw-r--r--   0        0        0     2469 2023-03-07 11:16:58.000000 mm_sdk-0.1.284/sdk/mis/lmk.py
--rw-r--r--   0        0        0     1986 2023-06-14 08:29:44.000000 mm_sdk-0.1.284/sdk/mis/mobil.py
--rw-r--r--   0        0        0     1295 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/mis/standalone.py
--rw-r--r--   0        0        0      577 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/mis/widgets.py
--rw-r--r--   0        0        0     4158 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/mobile_backend.py
--rw-r--r--   0        0        0      858 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/notemaster.py
--rw-r--r--   0        0        0     2878 2023-06-14 08:29:44.000000 mm_sdk-0.1.284/sdk/notification.py
--rw-r--r--   0        0        0     5311 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/personal.py
--rw-r--r--   0        0        0    16921 2023-03-07 11:16:58.000000 mm_sdk-0.1.284/sdk/pre_record.py
--rw-r--r--   0        0        0     1740 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/prodoctorov.py
--rw-r--r--   0        0        0     1738 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/reestr.py
--rw-r--r--   0        0        0     1343 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/roistat.py
--rw-r--r--   0        0        0      961 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/site_mobilmed.py
--rw-r--r--   0        0        0      687 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/sms.py
--rw-r--r--   0        0        0     5349 2023-01-24 17:51:17.000000 mm_sdk-0.1.284/sdk/yandex_courier.py
--rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 mm_sdk-0.1.284/setup.py
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 mm_sdk-0.1.284/PKG-INFO
+-rw-r--r--   0        0        0      924 2022-07-05 08:57:45.794986 mm-sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1523 2021-11-03 10:47:40.140464 mm-sdk-0.1.3/sdk/__init__.py
+-rw-r--r--   0        0        0     3260 2021-03-27 09:11:45.803751 mm-sdk-0.1.3/sdk/admitad.py
+-rw-r--r--   0        0        0     3235 2021-06-22 10:55:14.651521 mm-sdk-0.1.3/sdk/analytics.py
+-rw-r--r--   0        0        0      770 2020-07-01 08:18:16.581104 mm-sdk-0.1.3/sdk/barcode_recognizer.py
+-rw-r--r--   0        0        0      251 2021-07-26 16:51:24.234761 mm-sdk-0.1.3/sdk/base.py
+-rw-r--r--   0        0        0     3961 2022-03-14 14:38:31.923386 mm-sdk-0.1.3/sdk/cash_register.py
+-rw-r--r--   0        0        0     7985 2022-06-15 12:33:23.914778 mm-sdk-0.1.3/sdk/client.py
+-rw-r--r--   0        0        0     2504 2020-11-05 06:57:38.236735 mm-sdk-0.1.3/sdk/elk.py
+-rw-r--r--   0        0        0     1661 2021-02-09 16:04:56.154361 mm-sdk-0.1.3/sdk/face_detector.py
+-rw-r--r--   0        0        0     1418 2022-05-12 16:33:40.037958 mm-sdk-0.1.3/sdk/gift.py
+-rw-r--r--   0        0        0    17068 2022-06-16 10:24:53.990974 mm-sdk-0.1.3/sdk/gigtest.py
+-rw-r--r--   0        0        0        0 2020-06-03 13:34:31.086579 mm-sdk-0.1.3/sdk/mis/__init__.py
+-rw-r--r--   0        0        0      950 2021-11-16 05:42:56.584617 mm-sdk-0.1.3/sdk/mis/client.py
+-rw-r--r--   0        0        0     3471 2020-11-05 06:57:38.237039 mm-sdk-0.1.3/sdk/mis/crm.py
+-rw-r--r--   0        0        0     3055 2022-05-30 14:25:59.736562 mm-sdk-0.1.3/sdk/mis/lab.py
+-rw-r--r--   0        0        0     2459 2022-07-04 14:20:40.906595 mm-sdk-0.1.3/sdk/mis/lmk.py
+-rw-r--r--   0        0        0     1295 2021-05-11 14:10:51.275246 mm-sdk-0.1.3/sdk/mis/standalone.py
+-rw-r--r--   0        0        0      577 2020-11-09 07:42:38.328729 mm-sdk-0.1.3/sdk/mis/widgets.py
+-rw-r--r--   0        0        0     4158 2022-06-11 08:11:00.162551 mm-sdk-0.1.3/sdk/mobile_backend.py
+-rw-r--r--   0        0        0      858 2020-07-25 17:36:48.003509 mm-sdk-0.1.3/sdk/notemaster.py
+-rw-r--r--   0        0        0     2873 2021-09-29 07:53:01.309319 mm-sdk-0.1.3/sdk/notification.py
+-rw-r--r--   0        0        0     5311 2021-09-29 13:25:05.138830 mm-sdk-0.1.3/sdk/personal.py
+-rw-r--r--   0        0        0    14908 2022-05-11 13:17:45.580093 mm-sdk-0.1.3/sdk/pre_record.py
+-rw-r--r--   0        0        0     1740 2021-04-19 15:09:24.056996 mm-sdk-0.1.3/sdk/prodoctorov.py
+-rw-r--r--   0        0        0     1738 2021-03-12 09:43:50.794504 mm-sdk-0.1.3/sdk/reestr.py
+-rw-r--r--   0        0        0     1343 2021-03-01 07:04:21.793697 mm-sdk-0.1.3/sdk/roistat.py
+-rw-r--r--   0        0        0      961 2021-08-31 06:33:29.400763 mm-sdk-0.1.3/sdk/site_mobilmed.py
+-rw-r--r--   0        0        0      687 2021-11-17 12:32:21.418758 mm-sdk-0.1.3/sdk/sms.py
+-rw-r--r--   0        0        0     5349 2022-06-20 06:07:11.764755 mm-sdk-0.1.3/sdk/yandex_courier.py
+-rw-r--r--   0        0        0      611 2022-07-05 08:57:46.425249 mm-sdk-0.1.3/setup.py
+-rw-r--r--   0        0        0      483 2022-07-05 08:57:46.425545 mm-sdk-0.1.3/PKG-INFO
```

### Comparing `mm_sdk-0.1.284/pyproject.toml` & `mm-sdk-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.poetry]
 name = "mm-sdk"
-version = "0.1.284"
+version = "0.1.3"
 description = ""
 authors = ["dyus <dyuuus@gmail.com>"]
 packages = [
     { include = "sdk" },
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pydantic = "^1.7.3"
-httpx = "^0.23.3"
+pydantic = "=1.7.3"
+httpx = "=0.13.3"
+pre-commit = "=2.9.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.4.3"
 pytest-cov = "^2.10.0"
 black = "^19.10b0"
-ipython = ">=7,<9"
-requests = "2.28.1"
 
 [tool.isort]
 line_length = 88
 atomic = true
 include_trailing_comma = true
 lines_after_imports = 2
 lines_between_types = 1
```

### Comparing `mm_sdk-0.1.284/sdk/__init__.py` & `mm-sdk-0.1.3/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/admitad.py` & `mm-sdk-0.1.3/sdk/admitad.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/analytics.py` & `mm-sdk-0.1.3/sdk/analytics.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/barcode_recognizer.py` & `mm-sdk-0.1.3/sdk/barcode_recognizer.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/cash_register.py` & `mm-sdk-0.1.3/sdk/cash_register.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/client.py` & `mm-sdk-0.1.3/sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     Typed http client with error handling.
 
-    # >>> import logging, pydantic
-    # >>> logging.basicConfig(level=logging.DEBUG)
-    # >>> client = SDKClient(connection_timeout=10, io_timeout=10, silent=True)
-    # >>> class UserAgent(pydantic.BaseModel):
-    # ...     user_agent: str = pydantic.Field(None, alias='user-agent')
-    # >>> response = client.get('http://httpbin.org/user-agent', UserAgent)
-    # >>> response
-    # SDKResponse[Union[List[sdk.client.UserAgent], UserAgent]](data=UserAgent(user_agent='mobil-sdk/0.0.1'), error=None)
-    #
-    # >>> response = client.get('http://httpbin.org/post', UserAgent)
-    # >>> response
-    # SDKResponse[str](data=None, error=Error(code=405, message='METHOD NOT ALLOWED', detail='<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2 Final//EN">\\n<title>405 Method Not Allowed</title>\\n<h1>Method Not Allowed</h1>\\n<p>The method is not allowed for the requested URL.</p>\\n'))
+    >>> import logging, pydantic
+    >>> logging.basicConfig(level=logging.DEBUG)
+    >>> client = SDKClient(connection_timeout=10, io_timeout=10, silent=True)
+    >>> class UserAgent(pydantic.BaseModel):
+    ...     user_agent: str = pydantic.Field(None, alias='user-agent')
+    >>> response = client.get('http://httpbin.org/user-agent', UserAgent)
+    >>> response
+    SDKResponse[typing.Union[typing.List[sdk.client.UserAgent], sdk.client.UserAgent]](data=UserAgent(user_agent='mobil-sdk/0.0.1'), error=None)
+
+    >>> response = client.get('http://httpbin.org/post', UserAgent)
+    >>> response
+    SDKResponse[str](data=None, error=Error(code=405, message='Method Not Allowed', detail='<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2 Final//EN">\\n<title>405 Method Not Allowed</title>\\n<h1>Method Not Allowed</h1>\\n<p>The method is not allowed for the requested URL.</p>\\n'))
 
 """
 import inspect
 import json
 import logging
 
 from http import HTTPStatus
@@ -94,15 +94,15 @@
     def __del__(self):
         self.close()
 
     @staticmethod
     def create_default_client(
         connection_timeout: Union[float, int, None], io_timeout: Union[float, int, None]
     ) -> Client:
-        timeout = Timeout(io_timeout, connect=connection_timeout)
+        timeout = Timeout(io_timeout, connect_timeout=connection_timeout)
         return Client(
             headers={"user-agent": "mobil-sdk/0.0.1"}, timeout=timeout, verify=False
         )
 
     def _update_request_parameters(self, params: dict) -> dict:
         kwargs = params.copy()
         if callable(self._headers):
@@ -124,24 +124,24 @@
     def request(
         self, method: str, url: HttpUrl, response_class: Type[BaseModel], **kwargs
     ) -> SDKResponse:
 
         try:
             params = self._update_request_parameters(kwargs)
 
-            logger.info(
+            logger.debug(
                 "~~~> HTTP request method=%s, url=%s, params=%s",
                 method,
                 url,
                 self._log_kwargs(params),
             )
 
             response = self._client.request(method, url, **params)
 
-            logger.info(
+            logger.debug(
                 "<~~~ HTTP response status_code=%s, url=%s content=%s",
                 response.status_code,
                 response.url,
                 response.content[: self._content_slice_size],
             )
 
         except Exception as ex:
@@ -234,15 +234,15 @@
     def patch(self, url, response_class: Type[BaseModel], **kwargs) -> SDKResponse:
         return self.request("PATCH", url, response_class, **kwargs)
 
     def delete(self, url, response_class: Type[BaseModel], **kwargs) -> SDKResponse:
         return self.request("DELETE", url, response_class, **kwargs)
 
     def close(self):
-        if hasattr(self, "_client"):
+        if self._client:
             self._client.close()
 
 
 if __name__ == "__main__":
     from doctest import testmod
 
     testmod(verbose=False)
```

### Comparing `mm_sdk-0.1.284/sdk/elk.py` & `mm-sdk-0.1.3/sdk/elk.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/face_detector.py` & `mm-sdk-0.1.3/sdk/face_detector.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/gift.py` & `mm-sdk-0.1.3/sdk/gift.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/gigtest.py` & `mm-sdk-0.1.3/sdk/gigtest.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     key: str = Field(description="unique key")
     parent_id: Optional[int] = Field(description="id of parent activity")
     title: str = Field(description="unique key")
 
 
 class SectionResponse(BaseModel):
     id: int = Field(description="id")
-    activity_key: Optional[str] = Field(description="Тип деятельности из activities.key")
+    activity_key: str = Field(description="Тип деятельности из activities.key")
     title: str = Field(description="Название")
     image_url: Optional[str] = Field(description="Картинка типа")
     recommended: bool = Field(description="Рекомендовано или нет")
 
 
 class CountryResponse(BaseModel):
     id: int = Field(description="id")
@@ -76,58 +76,39 @@
 
 
 class ClientInfo(BaseModel):
     home_address: Optional[str] = Field(description="Адрес")
     phone: Optional[str] = Field(description="Телефон")
     company_name: Optional[str] = Field(description="Название организации")
     position: Optional[str] = Field(description="Должность")
-    birthday: Optional[datetime_date] = Field(description="Дата рождения")
 
 
 class CreateClientRequest(ClientInfo):
     fio: str = Field(description="ФИО")
-    birthday: datetime_date = Field(description="Дата рождения")
+    birthday: str = Field(description="Дата рождения")
     country_id: int = Field(description="Id страны по справочнику")
 
 
 class UpdateClientRequest(ClientInfo):
     pass
 
 
 class ClientResponse(ClientInfo):
     id: int = Field(description="Id гигтест клиента")
-    birthday: Optional[str] = Field(description="Дата рождения")
 
 
 # МЕДКНИЖКА
 class MedicalBookRequest(BaseModel):
     number: str = Field(description="Номер ЛМК")
     regnum: str = Field(description="Рег.номер ЛМК")
     date: datetime_date = Field(description="Дата выдачи ЛМК")
     user_id: int = Field(description="Id гигтест клиента")
     activity_keys: list = Field(description="Ключи типов деятельности")
 
 
-class UserExtended(ClientInfo):
-    fio: str = Field(description="ФИО")
-    birth_date: str = Field(description="Дата рождения")
-
-
-class MedicalBookSearchResponseOther(BaseModel):
-    id: int = Field(description="Id ЛМК в гигтесте")
-    number: str = Field(description="Номер ЛМК")
-    regnum: str = Field(description="Рег. номер ЛМК")
-    date: str = Field(description="Дата выдачи ЛМК")
-    next_education_date: str = Field(description="Дата следующей аттестации")
-    status: str = Field(description="Статус ЛМК: new, accepted, returned, completed")
-    activity_names: list = Field(description="Тип деятельности")
-    user: UserExtended = Field(description="Гигтест клиент")
-    medical_direction_ids: list = Field(description="Гигтест id мед. направлений")
-
-
 class User(BaseModel):
     fio: str
 
 
 class MedicalBookSearchResponse(BaseModel):
     number: str = Field(description="Номер ЛМК")
     date: str = Field(description="Дата выдачи ЛМК")
@@ -192,38 +173,21 @@
 
 
 class MedicineCreateOrUpdateResponseResults(BaseModel):
     medical_research_id: int = Field(description="Id исследования в гигтест")
     id: int = Field(description="Id медобследования в гигтест")
 
 
-class MedicineCreateOrUpdateResponseResultsExtended(
-    MedicineCreateOrUpdateResponseResults
-):
-    medical_research_name: str = Field(description="Название услуги")
-    date_med_result: str = Field(description="Дата обследования")
-    medical_research_result: int = Field(
-        description="Результат обследования. Предположительно 1 - нет противопоказаний"
-    )
-    medical_research_key: str = Field(description="Код услуги по справочнику гигтест")
-
-
 class MedicineCreateResponse(BaseModel):
     id: int = Field(description="Id медобследования в гигтест")
     results: List[MedicineCreateOrUpdateResponseResults] = Field(
         description="Исследования"
     )
 
 
-class MedicineCreateResponseExtended(MedicineCreateResponse):
-    results: List[MedicineCreateOrUpdateResponseResultsExtended] = Field(
-        description="Исследования"
-    )
-
-
 class MedicineUpdateResponse(BaseModel):
     results: List[MedicineCreateOrUpdateResponseResults] = Field(
         description="Исследования"
     )
     sticker_links: Optional[list] = Field(description="Ссылки на исследования")
 
 
@@ -242,15 +206,14 @@
         self._get_countries_url = "/api/v2/countries"
         self._get_medical_researches_url = "/api/v2/medical-researches"
         # КЛИЕНТ
         self._search_client_url = "/api/v2/users/search"
         self._create_or_update_client_url = "/api/v2/users"
         # МЕДКНИЖКА
         self._medbook_url = "/api/v2/medical-books"
-        self._medbook_url_search = "/api/v2/medical-books/search"
         # АТТЕСТАЦИЯ
         self._attestation_url = "/api/v2/protocols"
         # МЕДИЦИНА
         self._create_update_medicine_url = "/api/v2/medical-directions"
         self._additional_medicine_results_url = "/api/v2/medical-research-results"
 
     # СПРАВОЧНИКИ
@@ -329,24 +292,14 @@
                 self._create_or_update_client_url + "/" + str(client_gig_test_id)
             ),
             Empty,
             timeout=LONG_GIGTEST_TIMEOUT,
         )
 
     # МЕДКНИЖКИ
-    def search_medbook_when_other_department(
-        self, medbook_number: int
-    ) -> SDKResponse[MedicalBookSearchResponseOther]:
-        return self._client.get(
-            self._full_url(self._medbook_url_search),
-            MedicalBookSearchResponseOther,
-            params={"number": medbook_number},
-            timeout=COMMON_GIGTEST_TIMEOUT,
-        )
-
     def search_medbook(
         self, medbook_number: int
     ) -> SDKResponse[List[MedicalBookSearchResponse]]:
         return self._client.get(
             self._full_url(self._medbook_url),
             MedicalBookSearchResponse,
             params={"MedicalBooksSearch[number]": medbook_number},
@@ -403,22 +356,21 @@
         return self._client.delete(
             self._full_url(self._attestation_url + "/" + str(gigtest_att_id)),
             Empty,
             timeout=LONG_GIGTEST_TIMEOUT,
         )
 
     # МЕДИЦИНА
-    def get_med_direction(
-        self, gigtest_med_direction_id: int
-    ) -> SDKResponse[MedicineCreateResponseExtended]:
+    # этот метод не используется. Для проверки
+    def get_med_direction(self, gigtest_med_direction_id: int) -> SDKResponse[Empty]:
         return self._client.get(
             self._full_url(
                 self._create_update_medicine_url + "/" + str(gigtest_med_direction_id)
             ),
-            MedicineCreateResponseExtended,
+            Empty,
             timeout=COMMON_GIGTEST_TIMEOUT,
         )
 
     def create_med_direction(
         self, query: MedicineCreateRequest
     ) -> SDKResponse[MedicineCreateResponse]:
         return self._client.post(
@@ -447,15 +399,14 @@
             self._full_url(
                 self._create_update_medicine_url + "/" + str(gigtest_med_direction_id)
             ),
             Empty,
             timeout=LONG_GIGTEST_TIMEOUT,
         )
 
-    # TODO выше метод get_med_direction объединить с этим, проверив апи
     def search_med_direction(
         self, gigtest_med_direction_id: int
     ) -> SDKResponse[MedicineUpdateResponse]:
         return self._client.get(
             self._full_url(
                 self._create_update_medicine_url + "/" + str(gigtest_med_direction_id)
             ),
```

### Comparing `mm_sdk-0.1.284/sdk/mis/client.py` & `mm-sdk-0.1.3/sdk/roistat.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,57 @@
-import datetime
-
-from typing import Optional
+from typing import List, Optional
 from urllib.parse import urljoin
 
 from pydantic import BaseModel, Field, HttpUrl
 
-from .. import Gender
-from ..client import SDKClient, SDKResponse
-
+from .client import Empty, SDKClient
 
-MC_URL_BY_ID = {
-    1: "https://sm.mm/",
-    2: "https://dm.mm/",
-    3: "https://tm.mm/",
-    4: "https://fm.mm/",
-}
 
+class AdditionalFields(BaseModel):
+    mc_code: str
+    pre_record_number: Optional[str]
 
-class GetClient(BaseModel):
-    uuid: str
 
+class Product(BaseModel):
+    id: str
+    name: str
+    quantity: int = 1
+    price: int
 
-class Client(BaseModel):
-    uuid: str
-    phone: str
-    last_name: str = Field(alias="lname")
-    first_name: str = Field(alias="fname")
-    middle_name: Optional[str] = Field(alias="mname", default="")
-    birth: datetime.date
-    email: Optional[str]
-    sex: Gender
 
-    class Config:
-        use_enum_values = True
+class Order(BaseModel):
+    id: str
+    name: str
+    date_create: str
+    status: str = "1"  # взял из примера, нет описания что такое статус
+    price: str
+    client_id: str
+    roistat: Optional[str]
+    additional_fields: AdditionalFields = Field(alias="fields")
+    products: List[Product]
 
 
-class ClientResultsRequest(BaseModel):
-    client_uuid: str
-    mc_id: int
-    pre_record_number: int
-    lab_number: int
+class Orders(BaseModel):
+    __root__: List[Order]
 
 
-class ClientResultsResponse(BaseModel):
-    lab_results_url: Optional[str]
-    covid_results_url: Optional[str]
-    flg_results_url: Optional[str]
+class Auth(BaseModel):
+    project: str
+    key: str
 
 
-class ClientService:
-    def __init__(self, client: SDKClient, url: HttpUrl):
+class RoistatService:
+    def __init__(self, client: SDKClient, url: HttpUrl, auth: Auth):
+        assert url.endswith("/")
         self._client = client
         self._url = url
+        self._auth = auth
 
-    def get_client(self, query: GetClient, timeout=3) -> SDKResponse[Client]:
-        return self._client.get(
-            urljoin(str(self._url), f"mobil/rest/client/{query.uuid}/"),
-            Client,
-            timeout=timeout,
-        )
-
-    def get_results(self, query: ClientResultsRequest, timeout=3):
-        params = {
-            "lab_number": query.lab_number,
-            "pre_record_number": query.pre_record_number,
-        }
-        return self._client.get(
-            urljoin(
-                MC_URL_BY_ID[query.mc_id], f"mobil/client/{query.client_uuid}/results/"
-            ),
-            ClientResultsResponse,
-            params=params,
+    def add_orders(self, query: Orders, timeout: int = 3):
+        return self._client.post(
+            urljoin(str(self._url), "api/v1/project/add-orders"),
+            Empty,
+            params=self._auth.dict(),
+            data=query.json(by_alias=True),
             timeout=timeout,
+            headers={"Content-Type": "application/json"},
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mm_sdk-0.1.284/sdk/mis/crm.py` & `mm-sdk-0.1.3/sdk/mis/crm.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/mis/lab.py` & `mm-sdk-0.1.3/sdk/mis/lab.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/mis/lmk.py` & `mm-sdk-0.1.3/sdk/mis/lmk.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 class Medicine(BaseModel):
     latest_date: datetime.date
     next_date: Optional[datetime.date]
     nearest_expired_date: Optional[datetime.date]
 
 
 class Attestation(BaseModel):
-    latest_date: Optional[datetime.date]
+    latest_date: datetime.date
     next_date: Optional[datetime.date]
     reg_date: Optional[datetime.date]
 
 
 class Lmk(BaseModel):
     reg_number: Optional[str]
     blank_number: str
```

### Comparing `mm_sdk-0.1.284/sdk/mis/mobil.py` & `mm-sdk-0.1.3/sdk/notification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,106 @@
-from typing import Optional, List
-from urllib.parse import urljoin
+from typing import Optional
 
-from pydantic import BaseModel, HttpUrl
+from pydantic import BaseModel
 
-from ..client import SDKClient, SDKResponse
+from .client import HttpUrl, SDKClient, SDKResponse
 
 
-class UserRequest(BaseModel):
+class EmailConfigRequest(BaseModel):
+    name: str
+    host_name: str
+    host_port: str
     username: str
+    password: str
+    test: str
+
 
-class OrgRequest(BaseModel):
-    ids: Optional[List[int]]
-    name: Optional[str]
+class EmailConfigResponse(BaseModel):
+    created: str
 
-class OrgResponse(BaseModel):
-    id: int
+
+class TelegramConfigRequest(BaseModel):
     name: str
-    base_org_id: Optional[int]
+    bot_name: str
+    token: str
 
-class OrgResponsePaginated(BaseModel):
-    results: List[OrgResponse]
-    count: int
-    next: Optional[str]
-    previous: Optional[str]
-    page_size: int
 
+class TelegramConfigResponse(BaseModel):
+    created: str
 
-class MobilOrgService:
-    def __init__(self, client: SDKClient, url: HttpUrl):
-        self._client = client
-        self._url = url
 
-    def get_orgs_by_user(
-        self, query: UserRequest, timeout=3
-    ) -> SDKResponse[OrgResponse]:
-        return self._client.get(
-            urljoin(str(self._url), f"mobil/api/org_by_user/"),
-            OrgResponse,
-            params=query.dict(),
-            timeout=timeout,
-        )
+class NotificationConfigRequest(BaseModel):
+    service: str
+    notification_type: str
+    email_config: Optional[int] = None
+    telegram_config: Optional[int] = None
 
-    def get_orgs(self, query: OrgRequest, timeout=3) -> SDKResponse[OrgResponsePaginated]:
-        return self._client.get(
-            f"{self._url}/mobil/rest/external_orgs/",
-            OrgResponsePaginated,
-            timeout=timeout,
-            params=query.dict(exclude_unset=True),
-            headers={"Content-Type": "application/json"},
-        )
 
+class NotificationConfigResponse(BaseModel):
+    created: str
+    error: Optional[str] = None
 
-class GetManagerRequest(UserRequest):
-    name: str
 
+class NotificationRequest(BaseModel):
+    msg: str
+    receiver: str
+    subject: Optional[str] = None
+    service: str
+    notification_type: str
+    spam_countdown: Optional[int] = None  # время в секундах
 
-class GetManagerResponse(BaseModel):
-    username: str
-    name: str
-    email: Optional[str]
-    groups: List[str] = []
-    is_active: bool
+
+class NotificationResponse(BaseModel):
+    status: str
+    error: Optional[str] = None
 
 
-class ManagerService:
+class NotificationService:
     def __init__(self, client: SDKClient, url: HttpUrl):
         self._client = client
         self._url = url
+        self._url_email_config = self._url + "api/email_config"
+        self._url_telegram_config = self._url + "api/telegram_config"
+        self._url_notification_config = self._url + "api/notification_config"
+        self._url_notification = self._url + "api/notification"
+
+    def create_email_config(
+        self, query: EmailConfigRequest, timeout=3
+    ) -> SDKResponse[EmailConfigResponse]:
+        return self._client.post(
+            self._url_email_config,
+            response_class=EmailConfigResponse,
+            data=query.json(),
+            headers={"Content-Type": "application/json"},
+            timeout=timeout,
+        )
+
+    def create_telegram_config(
+        self, query: TelegramConfigRequest, timeout=3
+    ) -> SDKResponse[TelegramConfigResponse]:
+        return self._client.post(
+            self._url_telegram_config,
+            response_class=TelegramConfigResponse,
+            data=query.json(),
+            headers={"Content-Type": "application/json"},
+            timeout=timeout,
+        )
+
+    def create_notification_config(
+        self, query: NotificationConfigRequest, timeout=3
+    ) -> SDKResponse[NotificationConfigResponse]:
+        return self._client.post(
+            self._url_notification_config,
+            response_class=NotificationConfigResponse,
+            data=query.json(),
+            timeout=timeout,
+        )
 
-    def get_superuser_managers(
-        self, query: GetManagerRequest, timeout=3
-    ) -> SDKResponse[GetManagerResponse]:
-        return self._client.get(
-            urljoin(str(self._url), f"mobil/api/user/search/"),
-            GetManagerResponse,
-            params=query.dict(),
+    def create_notification(
+        self, query: NotificationRequest, timeout=3
+    ) -> SDKResponse[NotificationResponse]:
+        return self._client.post(
+            self._url_notification,
+            response_class=NotificationResponse,
+            data=query.json(),
             timeout=timeout,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mm_sdk-0.1.284/sdk/mis/standalone.py` & `mm-sdk-0.1.3/sdk/mis/standalone.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/mis/widgets.py` & `mm-sdk-0.1.3/sdk/mis/widgets.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/mobile_backend.py` & `mm-sdk-0.1.3/sdk/mobile_backend.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/notemaster.py` & `mm-sdk-0.1.3/sdk/notemaster.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/personal.py` & `mm-sdk-0.1.3/sdk/personal.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/pre_record.py` & `mm-sdk-0.1.3/sdk/pre_record.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 class ServiceForOrder(int, Enum):
     LAB = 5
     LMK = 4
     PROF = 3
     CERT = 1
-    OUT = 6
 
 
 class PaySystem(str, Enum):
     OTHER = ""  # когда наличка, не передается система оплаты
     TINKOFF_PAYMENT = "tinkoff"
     YOOKASSA_PAYMENT = "yookassa"
     # деньги платятся яндексу. Мис считает заказ полностью оплаченным
@@ -49,20 +48,20 @@
     passport_type: Optional[PassportType]
     passport_date: Optional[datetime.date]
     passport_code: Optional[str]
     passport_series: Optional[str]
     passport_number: Optional[str]
     oms: Optional[str]
     snils: Optional[str]
-    is_moscow: Optional[bool]
-    registration_region: Optional[str] = ""
-    registration_city: Optional[str]
-    registration_street: Optional[str]
-    registration_building: Optional[str] = ""
-    registration_quarter: Optional[str] = ""
+    is_moscow: bool
+    registration_region: str = ""
+    registration_city: str
+    registration_street: str
+    registration_building: str = ""
+    registration_quarter: str = ""
     fact_country: Optional[str]
     fact_republic: Optional[str]
     fact_region: Optional[str]
     fact_city: Optional[str]
     fact_street: Optional[str]
     fact_building: Optional[str]
     fact_quarter: Optional[str]
@@ -71,20 +70,14 @@
     vaccine_covid_second: Optional[datetime.date]
     vaccine_covid_second_name: Optional[str]
 
     class Config:
         use_enum_values = True
 
 
-class OutData(BaseModel):
-    address: str
-    lat: Optional[str]
-    long: Optional[str]
-
-
 class LabExtraFields(BaseModel):
     gender: Optional[Gender]
     nationality: Optional[str]
     passport_type: Optional[PassportType]
     passport_date: Optional[str]
     passport_code: Optional[str]
     passport_series: Optional[str]
@@ -99,25 +92,23 @@
     pregnancy_week: Optional[int]
     cycle_day: Optional[int]
     cycle_phase: Optional[CyclePhase]
     work_place: Optional[str]
     work_place_phone: Optional[str]
     work_place_address: Optional[str]
     trip: Optional[str]
-    out: Optional[OutData]
 
     class Config:
         use_enum_values = True
 
 
 class Source(str, Enum):
     site = "site"
     call_center = "call_center"
     delivery = "delivery"
-    mobile = "mobile"
 
 
 class PayType(str, Enum):
     cashless_prepayment = "cashless_prepayment"
     med_center = "med_center"
     delivery = "delivery"
 
@@ -148,20 +139,26 @@
 class WorkSchedule(BaseModel):
     week_day: int
     time_from: datetime.time
     time_to: datetime.time
     week_day_name: str
 
 
+class PlacesServices(BaseModel):
+    service: Service
+    work_schedule: List[WorkSchedule]
+
+
 class PlacesResponse(BaseModel):
     id: int
     name: str
     med_center_id: int
     metro: str
     extra_metro: List[str]
+    place_services: List[PlacesServices]
     subnet: IPvAnyAddress
     med_center_extra_info: Union[Dict, Json]
     lat: Decimal
     lng: Decimal
 
 
 class RecordTime(BaseModel):
@@ -199,15 +196,14 @@
     admitad_code: Optional[str]
     pay_system: Optional[PaySystem]
     roistat: Optional[str]
     # игнорирую, потому что пока ненужно. Но в апи передают
     roistat_first: Optional[str]
     with_discount: bool = True
     gift_code: str = ""
-    initial_cost: Optional[int]
 
     class Config:
         use_enum_values = True
 
     def convert_to_request(self):
         """Преобразовывает данные в формат, который принимает предварительная запись."""
         data = {
@@ -231,17 +227,14 @@
                 {"price_code": price_code} for price_code in self.analysis
             ],
             "source": self.source,
             "pay_type": self.pay_type,
             "with_discount": self.with_discount,
             "gift_code": self.gift_code,
         }
-        if self.initial_cost:
-            data["initial_cost"] = self.initial_cost
-
         if self.lab_extra_fields:
             data["extra_fields"] = self.lab_extra_fields.dict(exclude_none=True)
         if self.covid_fields:
             # преобразую, в json и обратно, потому что иначе datetime остается в
             # словаре и http json дампер не переваривает
             data["covid_fields"] = json.loads(self.covid_fields.json(exclude_none=True))
         if self.called_from_number:
@@ -272,93 +265,58 @@
     phone: str
     covid_fields: CovidFields
 
     class Config:
         use_enum_values = True
 
 
-class PreRecordTickRequest(BaseModel):
-    # забрал со старого апи, это результат json.dumps() примерный набор полей
-    # phone/cost/lab_services(cost/price_code
-    external_data: bytes
-    lmk_order_uuid: Optional[str]
-    lab_order_uuid: Optional[str]
-    prof_order_uuid: Optional[str]
-    certificate_order_uuid: Optional[str]
-    client_uuid: Optional[str]
-    lname: Optional[str]
-    mname: Optional[str]
-    fname: Optional[str]
-    birth: Optional[datetime.date]
-
-
 class ClientPreRecordsRequest(BaseModel):
     client_uuid: Optional[str]
     phone: Optional[str]
-    d_to: Optional[datetime.date]
-    lname: Optional[str]
-    services: Optional[List[ServiceForOrder]]
     limit: int = 10
     offset: int = 0
 
-    class Config:
-        use_enum_values = True
-
     @root_validator(pre=True)
     def one_of(cls, values):
         client_uuid = values.get("client_uuid")
         phone = values.get("phone")
         if not client_uuid and not phone:
-            raise ValueError("phone or client_uuid is required")
+            raise ValueError("All fields are empty")
         return values
 
 
 class PreRecordGetRequest(BaseModel):
     number: int
-    client_uuid: Optional[str]
-    phone: Optional[str]
 
 
 class LabService(BaseModel):
     price_code: str
 
 
-class OrderResults(BaseModel):
-    lab_results_url: Optional[str]
-    covid_results_url: Optional[str]
-    flg_results_url: Optional[str]
-
-
 class PreRecordResponse(BaseModel):
     number: int
     phone: str
     services: List[Service]
     lab_services: Optional[List[Optional[LabService]]]
     d_from: datetime.datetime
     d_to: datetime.datetime
     prepayment_is_paid: bool
     prepayment_cost: Optional[int]
     pay_type: PayType
     visit_cost: Optional[int]
-    initial_cost: Optional[int]
     pay_system: Optional[PaySystem]
     pay_service_id: Optional[str]
     med_center_id: int
     lname: str
     fname: str
     mname: str
-    birth: Optional[datetime.date]
     client_uuid: Optional[str]
     email: Optional[str]
     gift_code: Optional[str]
     place: int
-    extra_fields: Optional[LabExtraFields]
-    covid_fields: Optional[CovidFields]
-    results: Optional[OrderResults]
-    dc: datetime.datetime
 
     class Config:
         use_enum_values = True
 
 
 class PaginatedPreRecordResponse(BaseModel):
     count: int
@@ -508,56 +466,36 @@
             PreRecordResponse,
             data=json.dumps({"roistat": query.roistat}),
             timeout=timeout,
             headers={"Content-Type": "application/json"},
         )
 
     def get_pre_record(
-        self, query: PreRecordGetRequest, timeout=10, strict: bool = False
+        self, query: PreRecordGetRequest, timeout=10
     ) -> SDKResponse[PreRecordResponse]:
-        url = f"{self._url}rest/pre_record/{query.number}"
-        params = query.dict()
-        del params["number"]
-        if strict:
-            url = f"{self._url}rest/pre_record_strict/{query.number}"
         return self._client.get(
-            url,
+            f"{self._url}rest/pre_record/{query.number}",
             PreRecordResponse,
-            params=params,
             timeout=timeout,
             headers={"Content-Type": "application/json"},
         )
 
     def get_client_pre_records(
         self,
         query: ClientPreRecordsRequest,
         with_pagination: bool = False,
         timeout: int = 10,
-        strict: bool = False,
     ) -> SDKResponse[Union[List[PreRecordResponse], PaginatedPreRecordResponse]]:
-        url = f"{self._url}rest/pre_record/"
-        if strict:
-            url = f"{self._url}rest/pre_record_strict/"
+        print(query.dict())
         resp: SDKResponse[PaginatedPreRecordResponse] = self._client.get(
-            url,
+            f"{self._url}rest/pre_record/",
             PaginatedPreRecordResponse,
             timeout=timeout,
             params=query.dict(),
             headers={"Content-Type": "application/json"},
         )
         if with_pagination:
             return resp
         else:
             # старый формат
             resp = SDKResponse[List[PreRecordResponse]](data=resp.data.results)
             return resp
-
-    def set_tick(
-        self, number: int, query: PreRecordTickRequest, timeout: int = 2
-    ) -> SDKResponse[PreRecordResponse]:
-        return self._client.patch(
-            f"{self._url}rest/pre_record/{number}/set_tick/",
-            PreRecordResponse,
-            timeout=timeout,
-            params=query.dict(exclude_unset=True),
-            headers={"Content-Type": "application/json"},
-        )
```

### Comparing `mm_sdk-0.1.284/sdk/prodoctorov.py` & `mm-sdk-0.1.3/sdk/prodoctorov.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/reestr.py` & `mm-sdk-0.1.3/sdk/reestr.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/site_mobilmed.py` & `mm-sdk-0.1.3/sdk/site_mobilmed.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/sms.py` & `mm-sdk-0.1.3/sdk/sms.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.284/sdk/yandex_courier.py` & `mm-sdk-0.1.3/sdk/yandex_courier.py`

 * *Files identical despite different names*

