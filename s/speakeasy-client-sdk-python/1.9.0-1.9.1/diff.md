# Comparing `tmp/speakeasy-client-sdk-python-1.9.0.tar.gz` & `tmp/speakeasy-client-sdk-python-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakeasy-client-sdk-python-1.9.0.tar", last modified: Fri Mar 10 00:11:55 2023, max compression
+gzip compressed data, was "speakeasy-client-sdk-python-1.9.1.tar", last modified: Sat Mar 11 00:10:40 2023, max compression
```

## Comparing `speakeasy-client-sdk-python-1.9.0.tar` & `speakeasy-client-sdk-python-1.9.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 00:11:54.999496 speakeasy-client-sdk-python-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-03-10 00:11:54.999496 speakeasy-client-sdk-python-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 00:11:54.999496 speakeasy-client-sdk-python-1.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1039 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 00:11:54.991496 speakeasy-client-sdk-python-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 00:11:54.995496 speakeasy-client-sdk-python-1.9.0/src/speakeasy/
--rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12386 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/apiendpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9477 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/apis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4710 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/embeds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4835 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 00:11:54.995496 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 00:11:54.999496 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      884 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/deleteapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/deleteapiendpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/deleteschema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1194 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/deleteversionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      966 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/downloadschema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/downloadschemarevision.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1193 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/findapiendpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1135 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/generateopenapispec.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/generatepostmancollection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      925 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/generaterequestpostmancollection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getallapiendpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1510 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getallapiversions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getallforversionapiendpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1194 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getapiendpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1194 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getapis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getembedaccesstoken.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getplugins.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      984 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getrequestfromeventlog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getschema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1335 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getschemadiff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getschemarevision.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getschemas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getvalidembedaccesstokens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getversionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/insertversionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/queryeventlog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/registerschema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/revokeembedaccesstoken.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/runplugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      971 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/upsertapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1335 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/upsertapiendpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/upsertplugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/validateapikey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 00:11:54.999496 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      752 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2634 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3074 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/apiendpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2802 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/boundedrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/embedaccesstokenresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2379 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/embedtoken.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/error.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      839 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/filters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/generateopenapispecdiff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1716 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      685 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/requestmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1061 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/schemadiff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      246 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/unboundedrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/versionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4675 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/plugins.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4986 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/requests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11893 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/schemas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4989 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 00:11:54.999496 speakeasy-client-sdk-python-1.9.0/src/speakeasy/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23642 2023-03-10 00:11:46.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 00:11:54.999496 speakeasy-client-sdk-python-1.9.0/src/speakeasy_client_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-03-10 00:11:54.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-03-10 00:11:54.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 00:11:54.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-10 00:11:54.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy_client_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-10 00:11:54.000000 speakeasy-client-sdk-python-1.9.0/src/speakeasy_client_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:10:40.477289 speakeasy-client-sdk-python-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-03-11 00:10:40.477289 speakeasy-client-sdk-python-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 00:10:40.477289 speakeasy-client-sdk-python-1.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1039 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:10:40.469289 speakeasy-client-sdk-python-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:10:40.469289 speakeasy-client-sdk-python-1.9.1/src/speakeasy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12386 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/apiendpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9477 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/apis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4710 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/embeds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4835 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:10:40.469289 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:10:40.473289 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      884 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/deleteapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/deleteapiendpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/deleteschema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1194 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/deleteversionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      966 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/downloadschema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/downloadschemarevision.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1193 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/findapiendpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1135 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/generateopenapispec.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/generatepostmancollection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      925 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/generaterequestpostmancollection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getallapiendpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1510 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getallapiversions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getallforversionapiendpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1194 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getapiendpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1194 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getapis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getembedaccesstoken.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getplugins.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      984 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getrequestfromeventlog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getschema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1335 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getschemadiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getschemarevision.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getschemas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getvalidembedaccesstokens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getversionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/insertversionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/queryeventlog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/registerschema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/revokeembedaccesstoken.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/runplugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      971 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/upsertapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1335 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/upsertapiendpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/upsertplugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/validateapikey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:10:40.477289 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      752 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2634 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3074 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/apiendpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2802 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/boundedrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/embedaccesstokenresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2379 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/embedtoken.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/error.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      839 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/filters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/generateopenapispecdiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1716 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      685 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/requestmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1061 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/schemadiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      246 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/unboundedrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/versionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4675 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/plugins.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4986 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/requests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11893 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/schemas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4989 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:10:40.477289 speakeasy-client-sdk-python-1.9.1/src/speakeasy/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23642 2023-03-11 00:10:28.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:10:40.477289 speakeasy-client-sdk-python-1.9.1/src/speakeasy_client_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-03-11 00:10:40.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-03-11 00:10:40.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 00:10:40.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-11 00:10:40.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy_client_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-11 00:10:40.000000 speakeasy-client-sdk-python-1.9.1/src/speakeasy_client_sdk_python.egg-info/top_level.txt
```

### Comparing `speakeasy-client-sdk-python-1.9.0/PKG-INFO` & `speakeasy-client-sdk-python-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 1.9.0
+Version: 1.9.1
 Summary: Speakeasy API Client SDK for Python
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `speakeasy-client-sdk-python-1.9.0/README.md` & `speakeasy-client-sdk-python-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/setup.py` & `speakeasy-client-sdk-python-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="speakeasy-client-sdk-python",
-    version="1.9.0",
+    version="1.9.1",
     author="Speakeasy",
     description="Speakeasy API Client SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/apiendpoints.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/apiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/apis.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/apis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/embeds.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/embeds.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/metadata.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/metadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/__init__.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/deleteapi.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/deleteapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/deleteapiendpoint.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/deleteapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/deleteschema.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/deleteschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/deleteversionmetadata.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/deleteversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/downloadschema.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/downloadschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/downloadschemarevision.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/downloadschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/findapiendpoint.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/findapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/generateopenapispec.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/generateopenapispec.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/generatepostmancollection.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/generatepostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/generaterequestpostmancollection.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/generaterequestpostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getallapiendpoints.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getallapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getallapiversions.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getallapiversions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getallforversionapiendpoints.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getallforversionapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getapiendpoint.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getapis.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getapis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getembedaccesstoken.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getplugins.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getplugins.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getrequestfromeventlog.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getrequestfromeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getschema.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getschemadiff.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getschemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getschemarevision.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getschemas.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getschemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getvalidembedaccesstokens.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getvalidembedaccesstokens.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/getversionmetadata.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/getversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/insertversionmetadata.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/insertversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/queryeventlog.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/queryeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/registerschema.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/registerschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/revokeembedaccesstoken.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/revokeembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/runplugin.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/runplugin.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/upsertapi.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/upsertapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/upsertapiendpoint.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/upsertapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/operations/upsertplugin.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/operations/upsertplugin.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/__init__.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/api.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/api.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/apiendpoint.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/apiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/boundedrequest.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/boundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/embedaccesstokenresponse.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/embedaccesstokenresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/embedtoken.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/embedtoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/error.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/error.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/filter.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/filter.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/filters.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/filters.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/plugin.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/plugin.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/requestmetadata.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/requestmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/schema.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/schemadiff.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/schemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/unboundedrequest.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/unboundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/models/shared/versionmetadata.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/models/shared/versionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/plugins.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/plugins.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/requests.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/requests.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/schemas.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/schemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/sdk.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     schemas: Schemas
     
     _client: requests_http.Session
     _security_client: requests_http.Session
     _security: shared.Security
     _server_url: str = SERVERS[SERVER_PROD]
     _language: str = "python"
-    _sdk_version: str = "1.9.0"
-    _gen_version: str = "1.9.1"
+    _sdk_version: str = "1.9.1"
+    _gen_version: str = "1.9.2"
 
     def __init__(self) -> None:
         self._client = requests_http.Session()
         self._security_client = requests_http.Session()
         self._init_sdks()
 
     def config_server_url(self, server_url: str, params: dict[str, str] = None):
```

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/utils/retries.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/utils/retries.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy/utils/utils.py` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy_client_sdk_python.egg-info/PKG-INFO` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy_client_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 1.9.0
+Version: 1.9.1
 Summary: Speakeasy API Client SDK for Python
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `speakeasy-client-sdk-python-1.9.0/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt` & `speakeasy-client-sdk-python-1.9.1/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

