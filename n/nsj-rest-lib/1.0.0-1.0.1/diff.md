# Comparing `tmp/nsj_rest_lib-1.0.0.tar.gz` & `tmp/nsj_rest_lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-1.0.0.tar", last modified: Tue May 30 22:02:00 2023, max compression
+gzip compressed data, was "nsj_rest_lib-1.0.1.tar", last modified: Wed Jun 14 17:51:03 2023, max compression
```

## Comparing `nsj_rest_lib-1.0.0.tar` & `nsj_rest_lib-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.150052 nsj_rest_lib-1.0.0/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-05-30 22:02:00.150052 nsj_rest_lib-1.0.0/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2022-09-08 22:15:46.000000 nsj_rest_lib-1.0.0/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-05-30 22:02:00.150052 nsj_rest_lib-1.0.0/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.134053 nsj_rest_lib-1.0.0/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.142053 nsj_rest_lib-1.0.0/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.142053 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-01-06 22:06:31.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3131 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3700 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4349 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3684 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4094 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.142053 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    16608 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2022-12-19 18:04:42.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-03-20 12:54:19.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9038 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-01-02 23:27:01.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      195 2022-12-27 22:14:24.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-04-18 17:42:31.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2022-12-27 22:14:24.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2022-11-30 20:09:08.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-01-05 22:38:04.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2022-12-19 17:39:11.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    23264 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      582 2023-04-18 17:42:31.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.146052 nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-30 22:02:00.142053 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-05-30 22:02:00.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1609 2023-05-30 22:02:00.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-05-30 22:02:00.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-05-30 22:02:00.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-05-30 22:02:00.000000 nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.496348 nsj_rest_lib-1.0.1/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-14 17:51:03.496348 nsj_rest_lib-1.0.1/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2022-09-08 22:15:46.000000 nsj_rest_lib-1.0.1/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-06-14 17:51:03.496348 nsj_rest_lib-1.0.1/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.480347 nsj_rest_lib-1.0.1/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.488348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-01-06 22:06:31.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3131 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3700 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4349 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3684 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4094 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    16780 2023-06-14 17:50:21.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2022-12-19 18:04:42.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-03-20 12:54:19.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9827 2023-06-14 17:50:21.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-01-02 23:27:01.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      195 2022-12-27 22:14:24.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-04-18 17:42:31.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2022-12-27 22:14:24.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2022-11-30 20:09:08.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-01-05 22:38:04.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2022-12-19 17:39:11.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    23264 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      582 2023-04-18 17:42:31.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.496348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.488348 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-14 17:51:03.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1609 2023-06-14 17:51:03.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-06-14 17:51:03.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-06-14 17:51:03.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-06-14 17:51:03.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-1.0.0/PKG-INFO` & `nsj_rest_lib-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.0.0/setup.cfg` & `nsj_rest_lib-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 1.0.0
+version = 1.0.1
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/dao/dao_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,17 @@
 
                     # Storing condiction value
                     if condiction.value is not None and isinstance(condiction.value.__class__, enum.EnumMeta):
                         filter_values_map[condiction_alias] = condiction.value.value
                     else:
                         filter_values_map[condiction_alias] = condiction.value
 
+                    if operator == 'like' or operator == 'ilike':
+                        filter_values_map[condiction_alias] = f'%{filter_values_map[condiction_alias]}%'
+
                 # Formating condictions (with OR)
                 field_filter_where = ' or '.join(field_filter_where)
                 if field_filter_where.strip() != '':
                     field_filter_where = f"({field_filter_where})"
 
                 # Storing all condictions to a field
                 filters_where.append(field_filter_where)
```

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 from decimal import Decimal
 import uuid
 
 from nsj_rest_lib.descriptor.filter_operator import FilterOperator
 
 
 class DTOFieldFilter:
-
     def __init__(
-        self,
-        name: str = None,
-        operator: FilterOperator = FilterOperator.EQUALS
+        self, name: str = None, operator: FilterOperator = FilterOperator.EQUALS
     ):
         self.name = name
         self.operator = operator
         self.field_name = None
 
     def set_field_name(self, field_name: str):
         self.field_name = field_name
@@ -37,15 +34,15 @@
         validator: typing.Callable = None,
         strip: bool = False,
         entity_field: str = None,
         filters: typing.List[DTOFieldFilter] = None,
         pk: bool = False,
         use_default_validator: bool = True,
         default_value: typing.Union[typing.Callable, typing.Any] = None,
-        partition_data: bool = False
+        partition_data: bool = False,
     ):
         """
         -----------
         Parameters:
         -----------
         type: Expected type for the field. If it is an enum.Enum, the receive value (to set), will be converted.
         not_null: The field cannot be None (or empty, for strings).
@@ -93,95 +90,131 @@
 
     def validate(self, dto_field: "DTOField", value):
         """
         Default validator (ckecking default constraints: not null, type, min, max and enum types).
         """
 
         # Checking not null constraint
-        if (self.not_null) and (value is None or (isinstance(value, str) and len(value.strip()) <= 0)):
+        if (self.not_null) and (
+            value is None or (isinstance(value, str) and len(value.strip()) <= 0)
+        ):
             raise ValueError(
-                f"{self.storage_name} deve estar preenchido. Valor recebido: {value}.")
+                f"{self.storage_name} deve estar preenchido. Valor recebido: {value}."
+            )
 
         # Checking type constraint
         # TODO Ver como suportar typing
-        if self.expected_type is not None and not isinstance(value, self.expected_type) and value is not None:
+        if (
+            self.expected_type is not None
+            and not isinstance(value, self.expected_type)
+            and value is not None
+        ):
             value = self.validate_type(value)
 
         # Checking min constraint
         if self.min is not None:
             if isinstance(value, str) and (len(value) < self.min):
                 raise ValueError(
-                    f"{self.storage_name} deve conter no mínimo {self.min} caracteres. Valor recebido: {value}.")
-            elif (isinstance(value, int) or isinstance(value, float) or isinstance(value, Decimal)) and (value < self.min):
+                    f"{self.storage_name} deve conter no mínimo {self.min} caracteres. Valor recebido: {value}."
+                )
+            elif (
+                isinstance(value, int)
+                or isinstance(value, float)
+                or isinstance(value, Decimal)
+            ) and (value < self.min):
                 raise ValueError(
-                    f"{self.storage_name} deve ser maior ou igual a {self.min}. Valor recebido: {value}.")
+                    f"{self.storage_name} deve ser maior ou igual a {self.min}. Valor recebido: {value}."
+                )
 
         # Checking min constraint
         if self.max is not None:
             if isinstance(value, str) and (len(value) > self.max):
                 raise ValueError(
-                    f"{self.storage_name} deve conter no máximo {self.max} caracteres. Valor recebido: {value}.")
-            elif (isinstance(value, int) or isinstance(value, float) or isinstance(value, Decimal)) and (value > self.max):
+                    f"{self.storage_name} deve conter no máximo {self.max} caracteres. Valor recebido: {value}."
+                )
+            elif (
+                isinstance(value, int)
+                or isinstance(value, float)
+                or isinstance(value, Decimal)
+            ) and (value > self.max):
                 raise ValueError(
-                    f"{self.storage_name} deve ser menor ou igual a {self.max}. Valor recebido: {value}.")
+                    f"{self.storage_name} deve ser menor ou igual a {self.max}. Valor recebido: {value}."
+                )
 
         # Striping strings (if desired)
         if isinstance(value, str) and self.strip:
             value = value.strip()
 
         return value
 
     def validate_type(self, value):
         """
         Valida o value recebido, de acordo com o tipo esperado, e faz as conversões necessárias (se possível).
         """
 
         # Montando expressões regulares para as validações
         matcher_uuid = re.compile(
-            '^[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$')
+            "^[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$"
+        )
         matcher_datetime = re.compile(
-            '^(\d\d\d\d)-(\d\d)-(\d\d)[T,t](\d\d):(\d\d):(\d\d)$')
-        matcher_date = re.compile('^(\d\d\d\d)-(\d\d)-(\d\d)$')
+            "^(\d\d\d\d)-(\d\d)-(\d\d)[T,t](\d\d):(\d\d):(\d\d)$"
+        )
+        matcher_date = re.compile("^(\d\d\d\d)-(\d\d)-(\d\d)$")
 
         # Validação direta de tipos
         erro_tipo = False
         if self.expected_type is datetime.datetime and isinstance(value, str):
             match_datetime = matcher_datetime.search(value)
+            match_date = matcher_date.search(value)
 
             if match_datetime:
                 ano = int(match_datetime.group(1))
                 mes = int(match_datetime.group(2))
                 dia = int(match_datetime.group(3))
                 hora = int(match_datetime.group(4))
                 minuto = int(match_datetime.group(5))
                 segundo = int(match_datetime.group(6))
 
                 value = datetime.datetime(
-                    year=ano, month=mes, day=dia, hour=hora, minute=minuto, second=segundo)
+                    year=ano,
+                    month=mes,
+                    day=dia,
+                    hour=hora,
+                    minute=minuto,
+                    second=segundo,
+                )
+            elif match_date:
+                ano = int(match_date.group(1))
+                mes = int(match_date.group(2))
+                dia = int(match_date.group(3))
+
+                value = datetime.datetime(
+                    year=ano, month=mes, day=dia, hour=0, minute=0, second=0
+                )
             else:
-                erro_tipo=True
+                erro_tipo = True
         elif self.expected_type is datetime.date and isinstance(value, str):
-
             match_date = matcher_date.search(value)
 
             if match_date:
                 ano = int(match_date.group(1))
                 mes = int(match_date.group(2))
                 dia = int(match_date.group(3))
 
                 value = datetime.date(year=ano, month=mes, day=dia)
             else:
-                erro_tipo=True
+                erro_tipo = True
         elif isinstance(self.expected_type, enum.EnumMeta):
             # Enumerados
             try:
                 value = self.expected_type(value)
             except ValueError as e:
                 raise ValueError(
-                    f"{self.storage_name} não é um {self.expected_type.__name__} válido. Valor recebido: {value}.")
+                    f"{self.storage_name} não é um {self.expected_type.__name__} válido. Valor recebido: {value}."
+                )
         elif self.expected_type is bool and isinstance(value, int):
             # Booleanos
             # Converting int to bool (0 is False, otherwise is True)
             value = bool(value)
         elif self.expected_type is datetime.datetime and isinstance(value, datetime.date):
             # Datetime
             # Assumindo hora 0, minuto 0 e segundo 0 (quanto é recebida uma data para campo data + hora)
@@ -226,10 +259,11 @@
             except:
                 erro_tipo = True
         else:
             erro_tipo = True
 
         if erro_tipo:
             raise ValueError(
-                f"{self.storage_name} deve ser do tipo {self.expected_type.__name__}. Valor recebido: {value}.")
+                f"{self.storage_name} deve ser do tipo {self.expected_type.__name__}. Valor recebido: {value}."
+            )
 
         return value
```

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/dto/dto_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/service/service_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-rest-lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.0.0/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

