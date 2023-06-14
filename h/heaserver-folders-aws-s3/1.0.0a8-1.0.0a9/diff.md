# Comparing `tmp/heaserver-folders-aws-s3-1.0.0a8.tar.gz` & `tmp/heaserver-folders-aws-s3-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-folders-aws-s3-1.0.0a8.tar", last modified: Thu Jun 30 20:17:43 2022, max compression
+gzip compressed data, was "heaserver-folders-aws-s3-1.0.0a9.tar", last modified: Tue Aug 16 20:03:01 2022, max compression
```

## Comparing `heaserver-folders-aws-s3-1.0.0a8.tar` & `heaserver-folders-aws-s3-1.0.0a9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.245484 heaserver-folders-aws-s3-1.0.0a8/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.0a8/.editorconfig
--rw-rw-rw-   0        0        0      286 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.0a8/.gitignore
--rw-rw-rw-   0        0        0     1694 2022-06-30 19:52:09.000000 heaserver-folders-aws-s3-1.0.0a8/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.0a8/LICENSE
--rw-rw-rw-   0        0        0      272 2022-06-10 03:29:54.000000 heaserver-folders-aws-s3-1.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0     4791 2022-06-30 20:17:43.245484 heaserver-folders-aws-s3-1.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     3599 2022-06-30 19:52:09.000000 heaserver-folders-aws-s3-1.0.0a8/README.md
--rw-rw-rw-   0        0        0     1768 2022-03-11 17:53:59.000000 heaserver-folders-aws-s3-1.0.0a8/RELEASING.md
--rw-rw-rw-   0        0        0      415 2022-04-14 23:47:43.000000 heaserver-folders-aws-s3-1.0.0a8/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.184652 heaserver-folders-aws-s3-1.0.0a8/integrationtests/
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.184652 heaserver-folders-aws-s3-1.0.0a8/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.215350 heaserver-folders-aws-s3-1.0.0a8/integrationtests/heaserver/folderawss3integrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.0a8/integrationtests/heaserver/folderawss3integrationtest/__init__.py
--rw-rw-rw-   0        0        0    32005 2022-06-30 19:58:55.000000 heaserver-folders-aws-s3-1.0.0a8/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
--rw-rw-rw-   0        0        0      722 2022-06-08 00:07:47.000000 heaserver-folders-aws-s3-1.0.0a8/integrationtests/heaserver/folderawss3integrationtest/test_items_all.py
--rw-rw-rw-   0        0        0       92 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.0a8/pytest.ini
--rw-rw-rw-   0        0        0      432 2022-06-30 19:52:09.000000 heaserver-folders-aws-s3-1.0.0a8/requirements_dev.txt
--rw-rw-rw-   0        0        0     6995 2022-06-10 03:28:47.000000 heaserver-folders-aws-s3-1.0.0a8/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2022-06-30 20:17:43.245484 heaserver-folders-aws-s3-1.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0     2418 2022-06-30 19:53:20.000000 heaserver-folders-aws-s3-1.0.0a8/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.184652 heaserver-folders-aws-s3-1.0.0a8/src/
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.184652 heaserver-folders-aws-s3-1.0.0a8/src/heaserver/
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.225373 heaserver-folders-aws-s3-1.0.0a8/src/heaserver/folderawss3/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.0a8/src/heaserver/folderawss3/__init__.py
--rw-rw-rw-   0        0        0    29499 2022-06-30 20:01:28.000000 heaserver-folders-aws-s3-1.0.0a8/src/heaserver/folderawss3/service.py
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.225373 heaserver-folders-aws-s3-1.0.0a8/src/heaserver/folderawss3/wstl/
--rw-rw-rw-   0        0        0    12623 2022-06-30 19:52:09.000000 heaserver-folders-aws-s3-1.0.0a8/src/heaserver/folderawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.235422 heaserver-folders-aws-s3-1.0.0a8/src/heaserver_folders_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     4791 2022-06-30 20:17:43.000000 heaserver-folders-aws-s3-1.0.0a8/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      990 2022-06-30 20:17:43.000000 heaserver-folders-aws-s3-1.0.0a8/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-30 20:17:43.000000 heaserver-folders-aws-s3-1.0.0a8/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2022-06-30 20:17:43.000000 heaserver-folders-aws-s3-1.0.0a8/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2022-06-30 20:17:43.000000 heaserver-folders-aws-s3-1.0.0a8/src/heaserver_folders_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-06-30 20:17:43.000000 heaserver-folders-aws-s3-1.0.0a8/src/heaserver_folders_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.184652 heaserver-folders-aws-s3-1.0.0a8/tests/
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.184652 heaserver-folders-aws-s3-1.0.0a8/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.245484 heaserver-folders-aws-s3-1.0.0a8/tests/heaserver/folderawss3test/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.0a8/tests/heaserver/folderawss3test/__init__.py
--rw-rw-rw-   0        0        0    29131 2022-06-30 19:59:12.000000 heaserver-folders-aws-s3-1.0.0a8/tests/heaserver/folderawss3test/folderawss3testcase.py
--rw-rw-rw-   0        0        0     1077 2022-06-08 00:07:47.000000 heaserver-folders-aws-s3-1.0.0a8/tests/heaserver/folderawss3test/test_all.py
-drwxrwxrwx   0        0        0        0 2022-06-30 20:17:43.245484 heaserver-folders-aws-s3-1.0.0a8/tests/heaserver/folderawss3test/wstl/
--rw-rw-rw-   0        0        0    14496 2022-06-08 00:07:47.000000 heaserver-folders-aws-s3-1.0.0a8/tests/heaserver/folderawss3test/wstl/all.json
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.146299 heaserver-folders-aws-s3-1.0.0a9/
+-rw-rw-rw-   0        0        0      261 2022-04-12 21:56:16.000000 heaserver-folders-aws-s3-1.0.0a9/.editorconfig
+-rw-rw-rw-   0        0        0      286 2022-04-12 21:56:16.000000 heaserver-folders-aws-s3-1.0.0a9/.gitignore
+-rw-rw-rw-   0        0        0     1694 2022-08-16 19:53:40.000000 heaserver-folders-aws-s3-1.0.0a9/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-04-12 21:56:16.000000 heaserver-folders-aws-s3-1.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0      272 2022-06-15 20:25:32.000000 heaserver-folders-aws-s3-1.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4791 2022-08-16 20:03:01.145304 heaserver-folders-aws-s3-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     3599 2022-08-16 19:53:40.000000 heaserver-folders-aws-s3-1.0.0a9/README.md
+-rw-rw-rw-   0        0        0     1768 2022-04-12 21:56:16.000000 heaserver-folders-aws-s3-1.0.0a9/RELEASING.md
+-rw-rw-rw-   0        0        0      422 2022-08-16 19:57:36.000000 heaserver-folders-aws-s3-1.0.0a9/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.034297 heaserver-folders-aws-s3-1.0.0a9/integrationtests/
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.035297 heaserver-folders-aws-s3-1.0.0a9/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.088297 heaserver-folders-aws-s3-1.0.0a9/integrationtests/heaserver/folderawss3integrationtest/
+-rw-rw-rw-   0        0        0        0 2022-04-12 21:56:16.000000 heaserver-folders-aws-s3-1.0.0a9/integrationtests/heaserver/folderawss3integrationtest/__init__.py
+-rw-rw-rw-   0        0        0    33494 2022-08-16 19:53:40.000000 heaserver-folders-aws-s3-1.0.0a9/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    10401 2022-08-16 19:53:40.000000 heaserver-folders-aws-s3-1.0.0a9/integrationtests/heaserver/folderawss3integrationtest/test_items_all.py
+-rw-rw-rw-   0        0        0       92 2022-04-12 21:56:16.000000 heaserver-folders-aws-s3-1.0.0a9/pytest.ini
+-rw-rw-rw-   0        0        0      432 2022-08-16 19:53:40.000000 heaserver-folders-aws-s3-1.0.0a9/requirements_dev.txt
+-rw-rw-rw-   0        0        0     7207 2022-08-16 19:53:40.000000 heaserver-folders-aws-s3-1.0.0a9/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2022-08-16 20:03:01.146299 heaserver-folders-aws-s3-1.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     2418 2022-08-16 19:59:46.000000 heaserver-folders-aws-s3-1.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.036298 heaserver-folders-aws-s3-1.0.0a9/src/
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.035297 heaserver-folders-aws-s3-1.0.0a9/src/heaserver/
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.099298 heaserver-folders-aws-s3-1.0.0a9/src/heaserver/folderawss3/
+-rw-rw-rw-   0        0        0        0 2022-04-12 21:56:16.000000 heaserver-folders-aws-s3-1.0.0a9/src/heaserver/folderawss3/__init__.py
+-rw-rw-rw-   0        0        0    29649 2022-08-16 19:53:40.000000 heaserver-folders-aws-s3-1.0.0a9/src/heaserver/folderawss3/service.py
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.104297 heaserver-folders-aws-s3-1.0.0a9/src/heaserver/folderawss3/wstl/
+-rw-rw-rw-   0        0        0    12623 2022-08-16 19:53:40.000000 heaserver-folders-aws-s3-1.0.0a9/src/heaserver/folderawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.125300 heaserver-folders-aws-s3-1.0.0a9/src/heaserver_folders_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     4791 2022-08-16 20:03:00.000000 heaserver-folders-aws-s3-1.0.0a9/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2022-08-16 20:03:00.000000 heaserver-folders-aws-s3-1.0.0a9/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-16 20:03:00.000000 heaserver-folders-aws-s3-1.0.0a9/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2022-08-16 20:03:00.000000 heaserver-folders-aws-s3-1.0.0a9/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2022-08-16 20:03:00.000000 heaserver-folders-aws-s3-1.0.0a9/src/heaserver_folders_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-08-16 20:03:00.000000 heaserver-folders-aws-s3-1.0.0a9/src/heaserver_folders_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.036298 heaserver-folders-aws-s3-1.0.0a9/tests/
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.037298 heaserver-folders-aws-s3-1.0.0a9/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.138297 heaserver-folders-aws-s3-1.0.0a9/tests/heaserver/folderawss3test/
+-rw-rw-rw-   0        0        0        0 2022-04-12 21:56:16.000000 heaserver-folders-aws-s3-1.0.0a9/tests/heaserver/folderawss3test/__init__.py
+-rw-rw-rw-   0        0        0    29984 2022-08-16 19:53:40.000000 heaserver-folders-aws-s3-1.0.0a9/tests/heaserver/folderawss3test/folderawss3testcase.py
+-rw-rw-rw-   0        0        0     1177 2022-08-16 19:53:40.000000 heaserver-folders-aws-s3-1.0.0a9/tests/heaserver/folderawss3test/test_all.py
+drwxrwxrwx   0        0        0        0 2022-08-16 20:03:01.144297 heaserver-folders-aws-s3-1.0.0a9/tests/heaserver/folderawss3test/wstl/
+-rw-rw-rw-   0        0        0    14496 2022-06-15 20:25:32.000000 heaserver-folders-aws-s3-1.0.0a9/tests/heaserver/folderawss3test/wstl/all.json
```

### Comparing `heaserver-folders-aws-s3-1.0.0a8/Dockerfile` & `heaserver-folders-aws-s3-1.0.0a9/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.0a8/LICENSE` & `heaserver-folders-aws-s3-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.0a8/PKG-INFO` & `heaserver-folders-aws-s3-1.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `heaserver-folders-aws-s3-1.0.0a8/README.md` & `heaserver-folders-aws-s3-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.0a8/RELEASING.md` & `heaserver-folders-aws-s3-1.0.0a9/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.0a8/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py` & `heaserver-folders-aws-s3-1.0.0a9/tests/heaserver/folderawss3test/folderawss3testcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Runs integration tests for the HEA folder service.
 
 Note that each test opens an aiohttp server listening on port 8080.
 """
 
-from heaserver.service.testcase import expectedvalues, awss3microservicetestcase
+from heaserver.service.testcase import expectedvalues, microservicetestcase
 from heaserver.folderawss3 import service
-from heaserver.service.testcase.mockaws import MockS3Manager
+from heaserver.service.testcase.mockaws import MockS3ManagerWithMockMongo
 from heaobject import user
-
+from base64 import b64encode
 
 db_values = {'awss3folders_items': [
     {
         'created': '2022-05-17T00:00:00+00:00',
         'derived_by': None,
         'derived_from': [],
         'description': None,
@@ -25,15 +25,15 @@
         'shares': [],
         'source': 'AWS Simple Cloud Storage (S3)',
         'type': 'heaobject.folder.AWSS3Item',
         'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
         'actual_object_id': 'VGVzdEZvbGRlci8=',
         'actual_object_uri': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlci8=',
         'version': None,
-        's3_uri':'s3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
+        's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
         'storage_class': 'STANDARD',
         'mime_type': 'application/x.item',
         'size': None,
         'human_readable_size': None,
         'volume_id': None,
         'folder_id': 'root'
     },
@@ -51,15 +51,15 @@
         'shares': [],
         'source': 'AWS Simple Cloud Storage (S3)',
         'type': 'heaobject.folder.AWSS3Item',
         'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
         'actual_object_id': 'VGVzdEZvbGRlcjIv',
         'actual_object_uri': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlcjIv',
         'version': None,
-        's3_uri':'s3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
+        's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
         'storage_class': 'STANDARD',
         'mime_type': 'application/x.item',
         'size': None,
         'human_readable_size': None,
         'volume_id': None,
         'folder_id': 'root'
     }
@@ -118,15 +118,15 @@
         'source': None,
         'type': 'heaobject.volume.Volume',
         'version': None,
         'file_system_name': 'amazon_web_services',
         'file_system_type': 'heaobject.volume.AWSFileSystem',
         'credential_id': None  # Let boto3 try to find the user's credentials.
     }],
-'buckets': [ {
+    'buckets': [{
         "arn": None,
         "created": '2022-05-17T00:00:00+00:00',
         "derived_by": None,
         "derived_from": [],
         "description": None,
         "display_name": "arp-scale-2-cloud-bucket-with-tags11",
         "encrypted": True,
@@ -144,15 +144,15 @@
         "shares": [],
         "size": None,
         "source": None,
         "tags": [],
         "type": "heaobject.bucket.AWSBucket",
         "version": None,
         "versioned": False
-  }],
+    }],
     'awsaccounts': [
         {
             'email_address': 'no-reply@example.com',
             'alternate_contact_name': None,
             "alternate_email_address": None,
             "alternate_phone_number": None,
             "created": '2022-05-17T00:00:00+00:00',
@@ -170,15 +170,15 @@
             "phone_number": None,
             "shares": [],
             "source": None,
             "type": "heaobject.account.AWSAccount",
             "version": None
         }
     ],
-'awss3folders': [{
+    'awss3folders': [{
         'created': '2022-05-17T00:00:00+00:00',
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'TestFolder',
         'id': 'VGVzdEZvbGRlci8=',
         'invites': [],
@@ -189,34 +189,34 @@
         'source': 'AWS Simple Cloud Storage (S3)',
         'type': 'heaobject.folder.AWSS3Folder',
         'version': None,
         'mime_type': 'application/x.folder',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
         'storage_class': 'STANDARD'
     },
-    {
-        'created': '2022-05-17T00:00:00+00:00',
-        'derived_by': None,
-        'derived_from': [],
-        'description': None,
-        'display_name': 'TestFolder2',
-        'id': 'VGVzdEZvbGRlcjIv',
-        'invites': [],
-        'modified': '2022-05-17T00:00:00+00:00',
-        'name': 'VGVzdEZvbGRlcjIv',
-        'owner': user.NONE_USER,
-        'shares': [],
-        'source': 'AWS Simple Cloud Storage (S3)',
-        'type': 'heaobject.folder.AWSS3Folder',
-        'version': None,
-        'mime_type': 'application/x.folder',
-        's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
-        'storage_class': 'STANDARD'
-    }
-]
+        {
+            'created': '2022-05-17T00:00:00+00:00',
+            'derived_by': None,
+            'derived_from': [],
+            'description': None,
+            'display_name': 'TestFolder2',
+            'id': 'VGVzdEZvbGRlcjIv',
+            'invites': [],
+            'modified': '2022-05-17T00:00:00+00:00',
+            'name': 'VGVzdEZvbGRlcjIv',
+            'owner': user.NONE_USER,
+            'shares': [],
+            'source': 'AWS Simple Cloud Storage (S3)',
+            'type': 'heaobject.folder.AWSS3Folder',
+            'version': None,
+            'mime_type': 'application/x.folder',
+            's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
+            'storage_class': 'STANDARD'
+        }
+    ]
 
 }
 
 content_ = [{'collection': {'version': '1.0', 'href': 'http://localhost:8080/folders/root/items/', 'items': [{'data': [
     {'name': 'created', 'value': None, 'prompt': 'created', 'display': True},
     {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
     {'name': 'derived_from', 'value': [], 'prompt': 'derived_from', 'display': True},
@@ -485,88 +485,104 @@
                                     'readOnly': True, 'pattern': ''},
                                    {'name': 'derived_from', 'value': [], 'prompt': 'Derived from', 'required': False,
                                     'readOnly': True, 'pattern': ''},
                                    {'name': 'items', 'value': None, 'prompt': 'Items', 'required': False,
                                     'readOnly': True, 'pattern': ''}]}}}]
 
 content = {
-    'folders': {
+    'awss3folders': {
         '666f6f2d6261722d71757579': content_
     }
 }
 
-
 AWSS3FolderTestCase = \
-    awss3microservicetestcase.get_test_case_cls_default(href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/',
-                                                   wstl_package=service.__package__,
-                                                   coll='awss3folders',
-                                                   fixtures=db_values,
-                                                   db_manager_cls=MockS3Manager,
-                                                   get_all_actions=[
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-folder-get-open-choices',
-                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/opener',
-                                                           rel=['hea-opener-choices']),
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-folder-duplicate',
-                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/duplicator',
-                                                           rel=['hea-duplicator']),
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-folder-get-properties',
-                                                           rel=['hea-properties']
-                                                       )
-                                                   ],
-                                                   get_actions=[
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-folder-get-open-choices',
-                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/opener',
-                                                           rel=['hea-opener-choices']),
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-folder-duplicate',
-                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/duplicator',
-                                                           rel=['hea-duplicator']),
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-folder-get-properties',
-                                                           rel=['hea-properties']
-                                                       )
-                                                   ],
-                                                   duplicate_action_name='heaserver-awss3folders-folder-duplicate-form',
-                                                   exclude=['body_put', 'body_post'])
+    microservicetestcase.get_test_case_cls_default(
+        href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/',
+        wstl_package=service.__package__,
+        coll='awss3folders',
+        fixtures=db_values,
+        db_manager_cls=MockS3ManagerWithMockMongo,
+        get_all_actions=[
+            expectedvalues.Action(
+                name='heaserver-awss3folders-folder-get-open-choices',
+                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/opener',
+                rel=['hea-opener-choices']),
+            expectedvalues.Action(
+                name='heaserver-awss3folders-folder-duplicate',
+                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/duplicator',
+                rel=['hea-duplicator']),
+            expectedvalues.Action(
+                name='heaserver-awss3folders-folder-get-properties',
+                rel=['hea-properties']
+            )
+        ],
+        get_actions=[
+            expectedvalues.Action(
+                name='heaserver-awss3folders-folder-get-open-choices',
+                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/opener',
+                rel=['hea-opener-choices']),
+            expectedvalues.Action(
+                name='heaserver-awss3folders-folder-duplicate',
+                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/duplicator',
+                rel=['hea-duplicator']),
+            expectedvalues.Action(
+                name='heaserver-awss3folders-folder-get-properties',
+                rel=['hea-properties']
+            )
+        ],
+        duplicate_action_name='heaserver-awss3folders-folder-duplicate-form',
+        exclude=['body_put', 'body_post'])
+
 
-AWSS3ItemTestCase = \
-    awss3microservicetestcase.get_test_case_cls_default(href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/items/',
-                                                   wstl_package=service.__package__,
-                                                   coll='awss3folders_items',
-                                                   fixtures=db_values,
-                                                   db_manager_cls=MockS3Manager,
-                                                   get_all_actions=[
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-item-get-actual',
-                                                           url='http://localhost:8080{+actual_object_uri}',
-                                                           rel=['hea-actual']),
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-item-duplicate',
-                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/duplicator',
-                                                           rel=['hea-duplicator']),
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-item-move',
-                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/mover',
-                                                           rel=['hea-mover']
-                                                       )
-                                                   ],
-                                                   get_actions=[
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-item-duplicate',
-                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/duplicator',
-                                                           rel=['hea-duplicator']),
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-item-move',
-                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/mover',
-                                                           rel=['hea-mover']
-                                                       ),
-                                                       expectedvalues.Action(
-                                                           name='heaserver-awss3folders-item-get-actual',
-                                                           url='http://localhost:8080{+actual_object_uri}',
-                                                           rel=['hea-actual'])
-                                                   ],
-                                                   duplicate_action_name='heaserver-awss3folders-item-duplicate-form',
-                                                   exclude=['body_put'])
+class AWSS3ItemTestCase(
+    microservicetestcase.get_test_case_cls_default(
+        href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/items/',
+        wstl_package=service.__package__,
+        coll='awss3folders_items',
+        fixtures=db_values,
+        db_manager_cls=MockS3ManagerWithMockMongo,
+        get_all_actions=[
+            expectedvalues.Action(
+                name='heaserver-awss3folders-item-duplicate',
+                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/duplicator',
+                rel=['hea-duplicator']),
+            expectedvalues.Action(
+                name='heaserver-awss3folders-item-get-actual',
+                url='http://localhost:8080{+actual_object_uri}',
+                rel=['hea-actual']),
+            expectedvalues.Action(
+                name='heaserver-awss3folders-item-move',
+                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/mover',
+                rel=['hea-mover']
+            )
+        ],
+        get_actions=[
+            expectedvalues.Action(
+                name='heaserver-awss3folders-item-duplicate',
+                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/duplicator',
+                rel=['hea-duplicator']),
+            expectedvalues.Action(
+                name='heaserver-awss3folders-item-get-actual',
+                url='http://localhost:8080{+actual_object_uri}',
+                rel=['hea-actual']),
+            expectedvalues.Action(
+                name='heaserver-awss3folders-item-move',
+                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/mover',
+                rel=['hea-mover']
+            )
+        ],
+        duplicate_action_name='heaserver-awss3folders-item-duplicate-form',
+        exclude=['body_put'])
+):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if self._body_post:
+            encoded = b64encode(b'Tritimus/').decode('utf-8')
+            modified_data = {**db_values[self._coll][0],
+                             'display_name': 'Tritimus',
+                             'actual_object_id': encoded,
+                             'actual_object_uri': '/'.join(db_values[self._coll][0]['actual_object_uri'].split('/')[:-1] + [encoded]),
+                             'name': encoded,
+                             's3_uri': '/'.join(db_values[self._coll][0]['s3_uri'].split('/')[:-2] + ['Tritimus', ''])}
+            if 'id' in modified_data:
+                del modified_data['id']
+            self._body_post = expectedvalues._create_template(modified_data)
```

### Comparing `heaserver-folders-aws-s3-1.0.0a8/run-swaggerui.py` & `heaserver-folders-aws-s3-1.0.0a9/run-swaggerui.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python3
 
 from heaserver.folderawss3 import service
 from heaserver.service.testcase import swaggerui
 from heaserver.service.testcase.docker import DockerContainerConfig
+from heaserver.service.testcase.collection import CollectionKey
 from heaserver.service.db.aws import S3Manager
 from heaserver.service.db.mongo import MongoManager
 from heaserver.service.wstl import builder_factory
 from aiohttp.web import get, post, delete, view, options
 from heaobject.registry import Resource
 from heaobject.volume import DEFAULT_FILE_SYSTEM
 from heaobject.volume import AWSFileSystem
 from heaobject import user
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 db_values = {
-    'components': [
+    CollectionKey(name='components', db_manager_cls=MongoManager): [
         {
             'id': '666f6f2d6261722d71757578',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'Reximus',
@@ -35,15 +36,15 @@
             'base_url': 'http://localhost:8080',
             'resources': [{'type': 'heaobject.registry.Resource', 'resource_type_name': 'heaobject.folder.AWSS3Folder',
                            'base_path': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders'},
                           {'type': 'heaobject.registry.Resource', 'resource_type_name': 'heaobject.folder.AWSS3Item',
                            'base_path': '/items'}]
         }
     ],
-    'filesystems': [{
+    CollectionKey(name='filesystems', db_manager_cls=MongoManager): [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'Amazon Web Services',
         'invited': [],
@@ -51,15 +52,15 @@
         'name': 'amazon_web_services',
         'owner': user.NONE_USER,
         'shared_with': [],
         'source': None,
         'type': 'heaobject.volume.AWSFileSystem',
         'version': None
     }],
-    'volumes': [{
+    CollectionKey(name='volumes', db_manager_cls=MongoManager): [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'My Amazon Web Services',
         'invited': [],
```

### Comparing `heaserver-folders-aws-s3-1.0.0a8/setup.py` & `heaserver-folders-aws-s3-1.0.0a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaserver-folders-aws-s3',
-                 version='1.0.0a8',
+                 version='1.0.0a9',
                  description='The HEA AWS S3 bucket folder service.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
                  package_dir={'': 'src'},
                  packages=['heaserver.folderawss3'],
                  package_data={'heaserver.folderawss3': ['wstl/*.json']},
                  install_requires=[
-                     'heaserver>=1.0.0a73, < 1.0.0a74'
+                     'heaserver>=1.0.0a76, < 1.0.0a77'
                  ],
                  classifiers=[
                      'Development Status :: 2 - Pre-Alpha',
                      'Intended Audience :: Developers',
                      'Intended Audience :: Science/Research',
                      'License :: OSI Approved :: Apache Software License',
                      'Framework :: AsyncIO',
```

### Comparing `heaserver-folders-aws-s3-1.0.0a8/src/heaserver/folderawss3/service.py` & `heaserver-folders-aws-s3-1.0.0a9/src/heaserver/folderawss3/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,14 +462,18 @@
                       {
                         "name": "actual_object_type_name",
                         "value": "heaobject.data.AWSS3FileObject"
                       },
                       {
                         "name": "actual_object_uri",
                         "value": "/volumes/666f6f2d6261722d71757578/buckets/my-bucket/folders/666f6f2d6261722d71757578"
+                      },
+                      {
+                        "name": "type",
+                        "value": "heaobject.folder.Item"
                       }]
                     }
                   }
             application/json:
               schema:
                 type: object
               examples:
```

### Comparing `heaserver-folders-aws-s3-1.0.0a8/src/heaserver/folderawss3/wstl/all.json` & `heaserver-folders-aws-s3-1.0.0a9/src/heaserver/folderawss3/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.0a8/src/heaserver_folders_aws_s3.egg-info/PKG-INFO` & `heaserver-folders-aws-s3-1.0.0a9/src/heaserver_folders_aws_s3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `heaserver-folders-aws-s3-1.0.0a8/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt` & `heaserver-folders-aws-s3-1.0.0a9/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.0a8/tests/heaserver/folderawss3test/folderawss3testcase.py` & `heaserver-folders-aws-s3-1.0.0a9/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 """
 Runs integration tests for the HEA folder service.
 
 Note that each test opens an aiohttp server listening on port 8080.
 """
 
-from heaserver.service.testcase import expectedvalues, microservicetestcase
+from heaserver.service.testcase import expectedvalues, awss3microservicetestcase
+from heaserver.service.testcase.dockermongo import DockerMongoManager
+
 from heaserver.folderawss3 import service
-from heaserver.service.testcase.mockaws import MockS3ManagerWithMockMongo
+from heaserver.service.testcase.mockaws import MockS3Manager
+from heaserver.service.testcase.collection import CollectionKey
 from heaobject import user
+from base64 import b64encode
 
-db_values = {'awss3folders_items': [
-    {
-        'created': '2022-05-17T00:00:00+00:00',
-        'derived_by': None,
-        'derived_from': [],
-        'description': None,
-        'display_name': 'TestFolder',
-        'id': 'VGVzdEZvbGRlci8=',
-        'invites': [],
-        'modified': '2022-05-17T00:00:00+00:00',
-        'name': 'VGVzdEZvbGRlci8=',
-        'owner': user.NONE_USER,
-        'shares': [],
-        'source': 'AWS Simple Cloud Storage (S3)',
-        'type': 'heaobject.folder.AWSS3Item',
-        'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
-        'actual_object_id': 'VGVzdEZvbGRlci8=',
-        'actual_object_uri': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlci8=',
-        'version': None,
-        's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
-        'storage_class': 'STANDARD',
-        'mime_type': 'application/x.item',
-        'size': None,
-        'human_readable_size': None,
-        'volume_id': None,
-        'folder_id': 'root'
-    },
-    {
-        'created': '2022-05-17T00:00:00+00:00',
-        'derived_by': None,
-        'derived_from': [],
-        'description': None,
-        'display_name': 'TestFolder2',
-        'id': 'VGVzdEZvbGRlcjIv',
-        'invites': [],
-        'modified': '2022-05-17T00:00:00+00:00',
-        'name': 'VGVzdEZvbGRlcjIv',
-        'owner': user.NONE_USER,
-        'shares': [],
-        'source': 'AWS Simple Cloud Storage (S3)',
-        'type': 'heaobject.folder.AWSS3Item',
-        'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
-        'actual_object_id': 'VGVzdEZvbGRlcjIv',
-        'actual_object_uri': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlcjIv',
-        'version': None,
-        's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
-        'storage_class': 'STANDARD',
-        'mime_type': 'application/x.item',
-        'size': None,
-        'human_readable_size': None,
-        'volume_id': None,
-        'folder_id': 'root'
-    }
-],
-    'components': [
+
+db_values = {
+    'awss3folders_items': [
         {
+            'created': '2022-05-17T00:00:00+00:00',
+            'derived_by': None,
+            'derived_from': [],
+            'description': None,
+            'display_name': 'TestFolder',
+            'id': 'VGVzdEZvbGRlci8=',
+            'invites': [],
+            'modified': '2022-05-17T00:00:00+00:00',
+            'name': 'VGVzdEZvbGRlci8=',
+            'owner': user.NONE_USER,
+            'shares': [],
+            'source': 'AWS Simple Cloud Storage (S3)',
+            'type': 'heaobject.folder.AWSS3Item',
+            'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
+            'actual_object_id': 'VGVzdEZvbGRlci8=',
+            'actual_object_uri': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlci8=',
+            'version': None,
+            's3_uri':'s3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
+            'storage_class': 'STANDARD',
+            'mime_type': 'application/x.item',
+            'size': None,
+            'human_readable_size': None,
+            'volume_id': None,
+            'folder_id': 'root'
+        },
+        {
+            'created': '2022-05-17T00:00:00+00:00',
+            'derived_by': None,
+            'derived_from': [],
+            'description': None,
+            'display_name': 'TestFolder2',
+            'id': 'VGVzdEZvbGRlcjIv',
+            'invites': [],
+            'modified': '2022-05-17T00:00:00+00:00',
+            'name': 'VGVzdEZvbGRlcjIv',
+            'owner': user.NONE_USER,
+            'shares': [],
+            'source': 'AWS Simple Cloud Storage (S3)',
+            'type': 'heaobject.folder.AWSS3Item',
+            'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
+            'actual_object_id': 'VGVzdEZvbGRlcjIv',
+            'actual_object_uri': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlcjIv',
+            'version': None,
+            's3_uri':'s3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
+            'storage_class': 'STANDARD',
+            'mime_type': 'application/x.item',
+            'size': None,
+            'human_readable_size': None,
+            'volume_id': None,
+            'folder_id': 'root'
+        }
+    ],
+    CollectionKey(name='components', db_manager_cls=DockerMongoManager): [{
             'id': '666f6f2d6261722d71757578',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'Reximus',
             'invited': [],
@@ -80,17 +85,16 @@
             'type': 'heaobject.registry.Component',
             'version': None,
             'base_url': 'http://localhost:8080',
             'resources': [{'type': 'heaobject.registry.Resource', 'resource_type_name': 'heaobject.folder.AWSS3Folder',
                            'base_path': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders'},
                           {'type': 'heaobject.registry.Resource', 'resource_type_name': 'heaobject.folder.AWSS3Item',
                            'base_path': '/items'}]
-        }
-    ],
-    'filesystems': [{
+    }],
+    CollectionKey(name='filesystems', db_manager_cls=DockerMongoManager): [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'Amazon Web Services',
         'invited': [],
@@ -98,15 +102,15 @@
         'name': 'amazon_web_services',
         'owner': user.NONE_USER,
         'shared_with': [],
         'source': None,
         'type': 'heaobject.volume.AWSFileSystem',
         'version': None
     }],
-    'volumes': [{
+    CollectionKey(name='volumes', db_manager_cls=DockerMongoManager): [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'My Amazon Web Services',
         'invited': [],
@@ -144,16 +148,15 @@
         "size": None,
         "source": None,
         "tags": [],
         "type": "heaobject.bucket.AWSBucket",
         "version": None,
         "versioned": False
     }],
-    'awsaccounts': [
-        {
+    'awsaccounts': [{
             'email_address': 'no-reply@example.com',
             'alternate_contact_name': None,
             "alternate_email_address": None,
             "alternate_phone_number": None,
             "created": '2022-05-17T00:00:00+00:00',
             "derived_by": None,
             "derived_from": [],
@@ -167,35 +170,34 @@
             "name": "311813441058",
             "owner": "system|none",
             "phone_number": None,
             "shares": [],
             "source": None,
             "type": "heaobject.account.AWSAccount",
             "version": None
-        }
-    ],
+        }],
     'awss3folders': [{
-        'created': '2022-05-17T00:00:00+00:00',
-        'derived_by': None,
-        'derived_from': [],
-        'description': None,
-        'display_name': 'TestFolder',
-        'id': 'VGVzdEZvbGRlci8=',
-        'invites': [],
-        'modified': '2022-05-17T00:00:00+00:00',
-        'name': 'VGVzdEZvbGRlci8=',
-        'owner': user.NONE_USER,
-        'shares': [],
-        'source': 'AWS Simple Cloud Storage (S3)',
-        'type': 'heaobject.folder.AWSS3Folder',
-        'version': None,
-        'mime_type': 'application/x.folder',
-        's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
-        'storage_class': 'STANDARD'
-    },
+            'created': '2022-05-17T00:00:00+00:00',
+            'derived_by': None,
+            'derived_from': [],
+            'description': None,
+            'display_name': 'TestFolder',
+            'id': 'VGVzdEZvbGRlci8=',
+            'invites': [],
+            'modified': '2022-05-17T00:00:00+00:00',
+            'name': 'VGVzdEZvbGRlci8=',
+            'owner': user.NONE_USER,
+            'shares': [],
+            'source': 'AWS Simple Cloud Storage (S3)',
+            'type': 'heaobject.folder.AWSS3Folder',
+            'version': None,
+            'mime_type': 'application/x.folder',
+            's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
+            'storage_class': 'STANDARD'
+        },
         {
             'created': '2022-05-17T00:00:00+00:00',
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'TestFolder2',
             'id': 'VGVzdEZvbGRlcjIv',
@@ -206,17 +208,15 @@
             'shares': [],
             'source': 'AWS Simple Cloud Storage (S3)',
             'type': 'heaobject.folder.AWSS3Folder',
             'version': None,
             'mime_type': 'application/x.folder',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
             'storage_class': 'STANDARD'
-        }
-    ]
-
+        }]
 }
 
 content_ = [{'collection': {'version': '1.0', 'href': 'http://localhost:8080/folders/root/items/', 'items': [{'data': [
     {'name': 'created', 'value': None, 'prompt': 'created', 'display': True},
     {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
     {'name': 'derived_from', 'value': [], 'prompt': 'derived_from', 'display': True},
     {'name': 'description', 'value': None, 'prompt': 'description', 'display': True},
@@ -484,89 +484,102 @@
                                     'readOnly': True, 'pattern': ''},
                                    {'name': 'derived_from', 'value': [], 'prompt': 'Derived from', 'required': False,
                                     'readOnly': True, 'pattern': ''},
                                    {'name': 'items', 'value': None, 'prompt': 'Items', 'required': False,
                                     'readOnly': True, 'pattern': ''}]}}}]
 
 content = {
-    'awss3folders': {
+    'folders': {
         '666f6f2d6261722d71757579': content_
     }
 }
 
+
 AWSS3FolderTestCase = \
-    microservicetestcase.get_test_case_cls_default(
-        href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/',
-        wstl_package=service.__package__,
-        coll='awss3folders',
-        fixtures=db_values,
-        db_manager_cls=MockS3ManagerWithMockMongo,
-        get_all_actions=[
-            expectedvalues.Action(
-                name='heaserver-awss3folders-folder-get-open-choices',
-                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/opener',
-                rel=['hea-opener-choices']),
-            expectedvalues.Action(
-                name='heaserver-awss3folders-folder-duplicate',
-                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/duplicator',
-                rel=['hea-duplicator']),
-            expectedvalues.Action(
-                name='heaserver-awss3folders-folder-get-properties',
-                rel=['hea-properties']
-            )
-        ],
-        get_actions=[
-            expectedvalues.Action(
-                name='heaserver-awss3folders-folder-get-open-choices',
-                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/opener',
-                rel=['hea-opener-choices']),
-            expectedvalues.Action(
-                name='heaserver-awss3folders-folder-duplicate',
-                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/duplicator',
-                rel=['hea-duplicator']),
-            expectedvalues.Action(
-                name='heaserver-awss3folders-folder-get-properties',
-                rel=['hea-properties']
-            )
-        ],
-        duplicate_action_name='heaserver-awss3folders-folder-duplicate-form',
-        exclude=['body_put', 'body_post'])
+    awss3microservicetestcase.get_test_case_cls_default(href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/',
+                                                   wstl_package=service.__package__,
+                                                   coll='awss3folders',
+                                                   fixtures=db_values,
+                                                   db_manager_cls=MockS3Manager,
+                                                   get_all_actions=[
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-folder-get-open-choices',
+                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/opener',
+                                                           rel=['hea-opener-choices']),
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-folder-duplicate',
+                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/duplicator',
+                                                           rel=['hea-duplicator']),
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-folder-get-properties',
+                                                           rel=['hea-properties']
+                                                       )
+                                                   ],
+                                                   get_actions=[
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-folder-get-open-choices',
+                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/opener',
+                                                           rel=['hea-opener-choices']),
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-folder-duplicate',
+                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/duplicator',
+                                                           rel=['hea-duplicator']),
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-folder-get-properties',
+                                                           rel=['hea-properties']
+                                                       )
+                                                   ],
+                                                   duplicate_action_name='heaserver-awss3folders-folder-duplicate-form',
+                                                   exclude=['body_put', 'body_post'])
 
-AWSS3ItemTestCase = \
-    microservicetestcase.get_test_case_cls_default(
-        href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/items/',
-        wstl_package=service.__package__,
-        coll='awss3folders_items',
-        fixtures=db_values,
-        db_manager_cls=MockS3ManagerWithMockMongo,
-        get_all_actions=[
-            expectedvalues.Action(
-                name='heaserver-awss3folders-item-duplicate',
-                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/duplicator',
-                rel=['hea-duplicator']),
-            expectedvalues.Action(
-                name='heaserver-awss3folders-item-get-actual',
-                url='http://localhost:8080{+actual_object_uri}',
-                rel=['hea-actual']),
-            expectedvalues.Action(
-                name='heaserver-awss3folders-item-move',
-                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/mover',
-                rel=['hea-mover']
-            )
-        ],
-        get_actions=[
-            expectedvalues.Action(
-                name='heaserver-awss3folders-item-duplicate',
-                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/duplicator',
-                rel=['hea-duplicator']),
-            expectedvalues.Action(
-                name='heaserver-awss3folders-item-get-actual',
-                url='http://localhost:8080{+actual_object_uri}',
-                rel=['hea-actual']),
-            expectedvalues.Action(
-                name='heaserver-awss3folders-item-move',
-                url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/mover',
-                rel=['hea-mover']
-            )
-        ],
-        duplicate_action_name='heaserver-awss3folders-item-duplicate-form',
-        exclude=['body_put'])
+class AWSS3ItemTestCase(
+    awss3microservicetestcase.get_test_case_cls_default(href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/items/',
+                                                   wstl_package=service.__package__,
+                                                   coll='awss3folders_items',
+                                                   fixtures=db_values,
+                                                   db_manager_cls=MockS3Manager,
+                                                   get_all_actions=[
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-item-get-actual',
+                                                           url='http://localhost:8080{+actual_object_uri}',
+                                                           rel=['hea-actual']),
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-item-duplicate',
+                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/duplicator',
+                                                           rel=['hea-duplicator']),
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-item-move',
+                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/mover',
+                                                           rel=['hea-mover']
+                                                       )
+                                                   ],
+                                                   get_actions=[
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-item-duplicate',
+                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/duplicator',
+                                                           rel=['hea-duplicator']),
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-item-move',
+                                                           url='http://localhost:8080/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/items/{id}/mover',
+                                                           rel=['hea-mover']
+                                                       ),
+                                                       expectedvalues.Action(
+                                                           name='heaserver-awss3folders-item-get-actual',
+                                                           url='http://localhost:8080{+actual_object_uri}',
+                                                           rel=['hea-actual'])
+                                                   ],
+                                                   duplicate_action_name='heaserver-awss3folders-item-duplicate-form',
+                                                   exclude=['body_put'])
+):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if self._body_post:
+            encoded = b64encode(b'Tritimus/').decode('utf-8')
+            modified_data = {**db_values[self._coll][0],
+                             'display_name': 'Tritimus',
+                             'actual_object_id': encoded,
+                             'actual_object_uri': '/'.join(db_values[self._coll][0]['actual_object_uri'].split('/')[:-1] + [encoded]),
+                             'name': encoded,
+                             's3_uri': '/'.join(db_values[self._coll][0]['s3_uri'].split('/')[:-2] + ['Tritimus', ''])}
+            if 'id' in modified_data:
+                del modified_data['id']
+            self._body_post = expectedvalues._create_template(modified_data)
```

### Comparing `heaserver-folders-aws-s3-1.0.0a8/tests/heaserver/folderawss3test/test_all.py` & `heaserver-folders-aws-s3-1.0.0a9/tests/heaserver/folderawss3test/test_all.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 class TestPutAWSS3Folder(AWSS3FolderTestCase, PutMixin):  # type: ignore
     pass
 
 
 class TestDeleteAWSS3Folder(AWSS3FolderTestCase, DeleteMixin):  # type: ignore
     pass
 
-#
 
 class TestGetAWSS3Item(AWSS3ItemTestCase, GetOneMixin):  # type: ignore
-    pass
+    async def test_get_by_name(self) -> None:
+        self.skipTest('folder items do not support get by name')
 
 
 class TestGetAllAWSS3Items(AWSS3ItemTestCase, GetAllMixin):  # type: ignore
     pass
 
 
 class TestPostAWSS3Item(AWSS3ItemTestCase, PostMixin):  # type: ignore
```

### Comparing `heaserver-folders-aws-s3-1.0.0a8/tests/heaserver/folderawss3test/wstl/all.json` & `heaserver-folders-aws-s3-1.0.0a9/tests/heaserver/folderawss3test/wstl/all.json`

 * *Files identical despite different names*

