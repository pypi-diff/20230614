# Comparing `tmp/severino-0.9.1.tar.gz` & `tmp/severino-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "severino-0.9.1.tar", max compression
+gzip compressed data, was "severino-0.9.2.tar", max compression
```

## Comparing `severino-0.9.1.tar` & `severino-0.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      460 2022-09-16 13:46:46.988562 severino-0.9.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-16 13:46:46.988562 severino-0.9.1/severino/__init__.py
--rw-r--r--   0        0        0      555 2022-09-16 13:46:46.988562 severino-0.9.1/severino/sdk/__init__.py
--rw-r--r--   0        0        0       49 2022-09-16 13:46:46.988562 severino-0.9.1/severino/sdk/airflow/__init__.py
--rw-r--r--   0        0        0      940 2022-09-16 13:46:46.988562 severino-0.9.1/severino/sdk/airflow/airflow.py
--rw-r--r--   0        0        0        0 2022-09-16 13:46:46.988562 severino-0.9.1/severino/sdk/helpers/__init__.py
--rw-r--r--   0        0        0     1609 2022-09-16 13:46:46.988562 severino-0.9.1/severino/sdk/helpers/http_requests.py
--rw-r--r--   0        0        0     1718 2022-09-16 13:46:46.988562 severino-0.9.1/severino/sdk/helpers/pagination.py
--rw-r--r--   0        0        0       79 2022-09-16 13:46:46.988562 severino-0.9.1/severino/sdk/hub_distance/__init__.py
--rw-r--r--   0        0        0     2852 2022-09-16 13:46:46.988562 severino-0.9.1/severino/sdk/hub_distance/hub_distance.py
--rw-r--r--   0        0        0      119 2022-09-16 13:46:46.988562 severino-0.9.1/severino/sdk/internal_recruitment/__init__.py
--rw-r--r--   0        0        0     4336 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/internal_recruitment/internal_recruitment.py
--rw-r--r--   0        0        0       84 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/mail_carrier/__init__.py
--rw-r--r--   0        0        0     7328 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/mail_carrier/mail_carrier.py
--rw-r--r--   0        0        0      125 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/reports_of_pcds_in_admission/__init__.py
--rw-r--r--   0        0        0     2528 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/reports_of_pcds_in_admission/reports_of_pcds_in_admission.py
--rw-r--r--   0        0        0       84 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/rescission_workflow/__init__.py
--rw-r--r--   0        0        0     8115 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/rescission_workflow/rescission_workflow.py
--rw-r--r--   0        0        0      121 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/store_data/__init__.py
--rw-r--r--   0        0        0     1044 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/store_data/store_data.py
--rw-r--r--   0        0        0      514 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/store_data/store_data_tmp.py
--rw-r--r--   0        0        0       89 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/vagas_dot_com/__init__.py
--rw-r--r--   0        0        0     3949 2022-09-16 13:46:46.990563 severino-0.9.1/severino/sdk/vagas_dot_com/bot.py
--rw-r--r--   0        0        0      115 2022-09-16 13:46:46.990563 severino-0.9.1/severino/settings.py
--rw-r--r--   0        0        0     1027 2022-09-16 14:06:02.701257 severino-0.9.1/setup.py
--rw-r--r--   0        0        0      483 2022-09-16 14:06:02.701631 severino-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      460 2022-09-20 19:56:48.581178 severino-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-20 19:56:48.581178 severino-0.9.2/severino/__init__.py
+-rw-r--r--   0        0        0      555 2022-09-20 19:56:48.581178 severino-0.9.2/severino/sdk/__init__.py
+-rw-r--r--   0        0        0       49 2022-09-20 19:56:48.581178 severino-0.9.2/severino/sdk/airflow/__init__.py
+-rw-r--r--   0        0        0      940 2022-09-20 19:56:48.581178 severino-0.9.2/severino/sdk/airflow/airflow.py
+-rw-r--r--   0        0        0        0 2022-09-20 19:56:48.581178 severino-0.9.2/severino/sdk/helpers/__init__.py
+-rw-r--r--   0        0        0     1609 2022-09-20 19:56:48.581178 severino-0.9.2/severino/sdk/helpers/http_requests.py
+-rw-r--r--   0        0        0     1718 2022-09-20 19:56:48.581178 severino-0.9.2/severino/sdk/helpers/pagination.py
+-rw-r--r--   0        0        0       79 2022-09-20 19:56:48.581178 severino-0.9.2/severino/sdk/hub_distance/__init__.py
+-rw-r--r--   0        0        0     2852 2022-09-20 19:56:48.581178 severino-0.9.2/severino/sdk/hub_distance/hub_distance.py
+-rw-r--r--   0        0        0      119 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/internal_recruitment/__init__.py
+-rw-r--r--   0        0        0     4336 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/internal_recruitment/internal_recruitment.py
+-rw-r--r--   0        0        0       84 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/mail_carrier/__init__.py
+-rw-r--r--   0        0        0     7328 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/mail_carrier/mail_carrier.py
+-rw-r--r--   0        0        0      125 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/reports_of_pcds_in_admission/__init__.py
+-rw-r--r--   0        0        0     2528 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/reports_of_pcds_in_admission/reports_of_pcds_in_admission.py
+-rw-r--r--   0        0        0       84 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/rescission_workflow/__init__.py
+-rw-r--r--   0        0        0     8115 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/rescission_workflow/rescission_workflow.py
+-rw-r--r--   0        0        0      121 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/store_data/__init__.py
+-rw-r--r--   0        0        0     1044 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/store_data/store_data.py
+-rw-r--r--   0        0        0      514 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/store_data/store_data_tmp.py
+-rw-r--r--   0        0        0       89 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/vagas_dot_com/__init__.py
+-rw-r--r--   0        0        0     4088 2022-09-20 19:56:48.583178 severino-0.9.2/severino/sdk/vagas_dot_com/bot.py
+-rw-r--r--   0        0        0      115 2022-09-20 19:56:48.583178 severino-0.9.2/severino/settings.py
+-rw-r--r--   0        0        0     1027 2022-09-20 19:58:18.245098 severino-0.9.2/setup.py
+-rw-r--r--   0        0        0      483 2022-09-20 19:58:18.245514 severino-0.9.2/PKG-INFO
```

### Comparing `severino-0.9.1/severino/sdk/__init__.py` & `severino-0.9.2/severino/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/airflow/airflow.py` & `severino-0.9.2/severino/sdk/airflow/airflow.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/helpers/http_requests.py` & `severino-0.9.2/severino/sdk/helpers/http_requests.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/helpers/pagination.py` & `severino-0.9.2/severino/sdk/helpers/pagination.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/hub_distance/hub_distance.py` & `severino-0.9.2/severino/sdk/hub_distance/hub_distance.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/internal_recruitment/internal_recruitment.py` & `severino-0.9.2/severino/sdk/internal_recruitment/internal_recruitment.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/mail_carrier/mail_carrier.py` & `severino-0.9.2/severino/sdk/mail_carrier/mail_carrier.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/reports_of_pcds_in_admission/reports_of_pcds_in_admission.py` & `severino-0.9.2/severino/sdk/reports_of_pcds_in_admission/reports_of_pcds_in_admission.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/rescission_workflow/rescission_workflow.py` & `severino-0.9.2/severino/sdk/rescission_workflow/rescission_workflow.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/store_data/store_data.py` & `severino-0.9.2/severino/sdk/store_data/store_data.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/store_data/store_data_tmp.py` & `severino-0.9.2/severino/sdk/store_data/store_data_tmp.py`

 * *Files identical despite different names*

### Comparing `severino-0.9.1/severino/sdk/vagas_dot_com/bot.py` & `severino-0.9.2/severino/sdk/vagas_dot_com/bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,30 +67,32 @@
         )
 
 
 class VagasDotComCandidateMigration:
     def __init__(self):
         self.http = Http()
         self.severino_api_url = SEVERINO_API_URL
-        self.path = "/vagas-dot-com/candidate-migration/"
+        self.path = "/vagas-dot-com/candidate-migration"
 
     def create(
         self,
+        migration_uuid: UUID,
         name: str,
         city: str = "",
         most_recent_professional_experience: str = "",
         vagas_candidate_id: str = "",
     ):
         return self.http.post(
             url=f"{self.severino_api_url}{self.path}/",
             data={
                 "name": name,
                 "city": city,
                 "most_recent_professional_experience": most_recent_professional_experience,
                 "vagas_candidate_id": vagas_candidate_id,
+                "migration_uuid": migration_uuid,
             },
         )
 
     def read(self, candidate_migration_uuid: str):
         return self.http.get(
             url=f"{self.severino_api_url}{self.path}/{candidate_migration_uuid}/"
         )
@@ -105,26 +107,28 @@
             _type_: _description_
         """
         return self.http.get(url=f"{self.severino_api_url}{self.path}/", params=filters)
 
     def update(
         self,
         candidate_migration_uuid: UUID,
+        migration_uuid: UUID,
         name: str,
-        city: str = "",
-        most_recent_professional_experience: str = "",
-        vagas_candidate_id: str = "",
+        city: str,
+        most_recent_professional_experience: str,
+        vagas_candidate_id: str,
     ):
         return self.http.put(
             url=f"{self.severino_api_url}{self.path}/{candidate_migration_uuid}/",
             data={
                 "name": name,
                 "city": city,
                 "most_recent_professional_experience": most_recent_professional_experience,
                 "vagas_candidate_id": vagas_candidate_id,
+                "migration": migration_uuid,
             },
         )
 
     def delete(self, candidate_migration_uuid):
         return self.http.delete(
             url=f"{self.severino_api_url}{self.path}/{candidate_migration_uuid}/"
         )
```

### Comparing `severino-0.9.1/setup.py` & `severino-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Jinja2==3.0.3', 'requests>=2.27.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'severino',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'O Severino é utilizado para facilitar as integrações e também a reutilização de código',
     'long_description': None,
     'author': 'Stone People Analytics',
     'author_email': 'systems-techpeople@stone.com.br',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

