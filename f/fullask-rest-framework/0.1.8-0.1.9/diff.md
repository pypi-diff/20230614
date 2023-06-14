# Comparing `tmp/fullask-rest-framework-0.1.8.tar.gz` & `tmp/fullask-rest-framework-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullask-rest-framework-0.1.8.tar", last modified: Tue Jun 13 11:46:11 2023, max compression
+gzip compressed data, was "fullask-rest-framework-0.1.9.tar", last modified: Wed Jun 14 08:59:30 2023, max compression
```

## Comparing `fullask-rest-framework-0.1.8.tar` & `fullask-rest-framework-0.1.9.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.252270 fullask-rest-framework-0.1.8/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      175 2023-04-17 01:36:01.000000 fullask-rest-framework-0.1.8/AUTHORS.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1070 2023-04-17 01:40:34.000000 fullask-rest-framework-0.1.8/LICENSE
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      306 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/MANIFEST.in
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5399 2023-06-13 11:46:11.252270 fullask-rest-framework-0.1.8/PKG-INFO
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     4576 2023-06-05 17:51:33.000000 fullask-rest-framework-0.1.8/README.md
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.228269 fullask-rest-framework-0.1.8/docs/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      632 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/docs/Makefile
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.232269 fullask-rest-framework-0.1.8/docs/docfiles/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       31 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/docs/docfiles/authors.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5075 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/docs/docfiles/conf.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1997 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/docs/docfiles/contributing.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      313 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/docs/docfiles/index.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1246 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/docs/docfiles/installation.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       99 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/docs/docfiles/usage.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      829 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/docs/make.bat
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.232269 fullask-rest-framework-0.1.8/fullask_rest_framework/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      150 2023-06-13 11:45:54.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      604 2023-04-21 13:51:24.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/cli.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.236270 fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-18 18:19:58.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.236270 fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/admin/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/admin/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.236270 fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/admin/templates/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/admin/templates/index.html
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      851 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/admin/templates/login_form.html
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.240270 fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/admin/templates/static/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1146 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/admin/views.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.224269 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.240270 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/app_template/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/app_template/__init__.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/app_template/models.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/app_template/resources.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/app_template/schemas.txt
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.240270 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/project_template/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-08 13:47:33.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/project_template/__init__.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      112 2023-03-12 13:06:42.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/project_template/app.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      322 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/project_template/config.py.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      628 2023-04-18 19:16:45.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/project_template/factory.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       65 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/project_template/tests.txt
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.244270 fullask-rest-framework-0.1.8/fullask_rest_framework/entities/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-07 17:34:01.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/entities/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       49 2023-05-15 10:40:45.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/entities/base_entity.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      346 2023-05-08 13:47:35.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/entities/filtering.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      450 2023-06-05 16:00:39.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/entities/pagination.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      407 2023-05-15 10:15:36.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/entities/sorting.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.244270 fullask-rest-framework-0.1.8/fullask_rest_framework/factory/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-02 15:45:42.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/factory/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3875 2023-06-11 15:43:54.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/factory/app_factory.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      683 2023-06-12 15:50:25.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/factory/extensions.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.244270 fullask-rest-framework-0.1.8/fullask_rest_framework/orm/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:06:42.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/orm/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.244270 fullask-rest-framework-0.1.8/fullask_rest_framework/orm/sqlalchemy/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-13 16:25:47.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/orm/sqlalchemy/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      228 2023-06-05 16:15:54.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/orm/sqlalchemy/base_model.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1000 2023-06-12 14:52:13.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/orm/sqlalchemy/mixins.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.244270 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.248270 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/.pytest_cache/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       37 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/.pytest_cache/.gitignore
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      191 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/.pytest_cache/CACHEDIR.TAG
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      302 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/.pytest_cache/README.md
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.228269 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/.pytest_cache/v/
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.248270 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/.pytest_cache/v/cache/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       69 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/.pytest_cache/v/cache/lastfailed
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       63 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/.pytest_cache/v/cache/nodeids
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        2 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/.pytest_cache/v/cache/stepwise
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-20 07:40:30.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      427 2023-06-05 16:03:17.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/base.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     2852 2023-06-05 16:03:27.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/crud.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     8658 2023-06-12 13:24:52.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/sqlalchemy.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.248270 fullask-rest-framework-0.1.8/fullask_rest_framework/schemas/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/schemas/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1212 2023-05-15 07:28:57.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/schemas/fields.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      267 2023-06-05 16:08:35.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/schemas/filtering.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1033 2023-06-05 16:10:52.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/schemas/pagination.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      636 2023-06-05 16:11:02.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/schemas/sorting.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.248270 fullask-rest-framework-0.1.8/fullask_rest_framework/service/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-12 12:54:11.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/service/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.252270 fullask-rest-framework-0.1.8/fullask_rest_framework/utils/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/utils/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      572 2023-04-14 13:52:15.000000 fullask-rest-framework-0.1.8/fullask_rest_framework/utils/jwt.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.236270 fullask-rest-framework-0.1.8/fullask_rest_framework.egg-info/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5399 2023-06-13 11:46:11.000000 fullask-rest-framework-0.1.8/fullask_rest_framework.egg-info/PKG-INFO
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3189 2023-06-13 11:46:11.000000 fullask-rest-framework-0.1.8/fullask_rest_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-13 11:46:11.000000 fullask-rest-framework-0.1.8/fullask_rest_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       68 2023-06-13 11:46:11.000000 fullask-rest-framework-0.1.8/fullask_rest_framework.egg-info/entry_points.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-13 11:46:11.000000 fullask-rest-framework-0.1.8/fullask_rest_framework.egg-info/not-zip-safe
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      168 2023-06-13 11:46:11.000000 fullask-rest-framework-0.1.8/fullask_rest_framework.egg-info/requires.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       23 2023-06-13 11:46:11.000000 fullask-rest-framework-0.1.8/fullask_rest_framework.egg-info/top_level.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      869 2023-06-13 11:45:34.000000 fullask-rest-framework-0.1.8/pyproject.toml
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      394 2023-06-13 11:46:11.252270 fullask-rest-framework-0.1.8/setup.cfg
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1676 2023-06-13 11:46:05.000000 fullask-rest-framework-0.1.8/setup.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.252270 fullask-rest-framework-0.1.8/tests/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:34:17.000000 fullask-rest-framework-0.1.8/tests/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 11:46:11.252270 fullask-rest-framework-0.1.8/tests/repositories/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:35:54.000000 fullask-rest-framework-0.1.8/tests/repositories/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)    20125 2023-06-05 16:00:28.000000 fullask-rest-framework-0.1.8/tests/repositories/test_sqlalchemy_repository.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.365699 fullask-rest-framework-0.1.9/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      175 2023-04-17 01:36:01.000000 fullask-rest-framework-0.1.9/AUTHORS.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1070 2023-04-17 01:40:34.000000 fullask-rest-framework-0.1.9/LICENSE
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      306 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/MANIFEST.in
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5399 2023-06-14 08:59:30.365699 fullask-rest-framework-0.1.9/PKG-INFO
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     4576 2023-06-05 17:51:33.000000 fullask-rest-framework-0.1.9/README.md
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.341699 fullask-rest-framework-0.1.9/docs/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      632 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/docs/Makefile
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.345699 fullask-rest-framework-0.1.9/docs/docfiles/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       31 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/docs/docfiles/authors.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5075 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/docs/docfiles/conf.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1997 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/docs/docfiles/contributing.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      313 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/docs/docfiles/index.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1246 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/docs/docfiles/installation.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       99 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/docs/docfiles/usage.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      829 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/docs/make.bat
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.349699 fullask-rest-framework-0.1.9/fullask_rest_framework/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      150 2023-06-14 08:59:25.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      604 2023-04-21 13:51:24.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/cli.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.349699 fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-18 18:19:58.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.349699 fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/admin/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/admin/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.353699 fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/admin/templates/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/admin/templates/index.html
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      851 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/admin/templates/login_form.html
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.353699 fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/admin/templates/static/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1146 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/admin/views.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.337699 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.353699 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/app_template/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/app_template/__init__.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/app_template/models.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/app_template/resources.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/app_template/schemas.txt
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.353699 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/project_template/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-08 13:47:33.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/project_template/__init__.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      112 2023-03-12 13:06:42.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/project_template/app.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      322 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/project_template/config.py.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      628 2023-04-18 19:16:45.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/project_template/factory.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       65 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/project_template/tests.txt
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.357699 fullask-rest-framework-0.1.9/fullask_rest_framework/entities/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-07 17:34:01.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/entities/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       49 2023-06-13 17:54:22.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/entities/base_entity.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.357699 fullask-rest-framework-0.1.9/fullask_rest_framework/factory/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-02 15:45:42.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/factory/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3968 2023-06-13 14:17:47.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/factory/app_factory.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      683 2023-06-12 15:50:25.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/factory/extensions.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.357699 fullask-rest-framework-0.1.9/fullask_rest_framework/orm/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:06:42.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/orm/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.357699 fullask-rest-framework-0.1.9/fullask_rest_framework/orm/sqlalchemy/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-13 16:25:47.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/orm/sqlalchemy/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      228 2023-06-05 16:15:54.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/orm/sqlalchemy/base_model.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1000 2023-06-12 14:52:13.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/orm/sqlalchemy/mixins.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.361698 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.361698 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/.pytest_cache/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       37 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/.pytest_cache/.gitignore
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      191 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/.pytest_cache/CACHEDIR.TAG
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      302 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/.pytest_cache/README.md
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.337699 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/.pytest_cache/v/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.361698 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/.pytest_cache/v/cache/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       69 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/.pytest_cache/v/cache/lastfailed
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       63 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/.pytest_cache/v/cache/nodeids
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        2 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/.pytest_cache/v/cache/stepwise
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-20 07:40:30.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      243 2023-06-13 14:28:35.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/base.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     2821 2023-06-13 17:17:26.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/crud.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     8705 2023-06-14 08:58:03.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/sqlalchemy.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.365699 fullask-rest-framework-0.1.9/fullask_rest_framework/schemas/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/schemas/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1212 2023-05-15 07:28:57.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/schemas/fields.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      261 2023-06-13 17:17:24.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/schemas/filtering.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1014 2023-06-13 17:17:26.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/schemas/pagination.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      630 2023-06-13 17:17:25.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/schemas/sorting.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.365699 fullask-rest-framework-0.1.9/fullask_rest_framework/service/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-12 12:54:11.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/service/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.365699 fullask-rest-framework-0.1.9/fullask_rest_framework/utils/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/utils/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      572 2023-04-14 13:52:15.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/utils/jwt.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.365699 fullask-rest-framework-0.1.9/fullask_rest_framework/vo/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-06-13 17:07:42.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/vo/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      346 2023-05-08 13:47:35.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/vo/filtering.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      450 2023-06-05 16:00:39.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/vo/pagination.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      407 2023-05-15 10:15:36.000000 fullask-rest-framework-0.1.9/fullask_rest_framework/vo/sorting.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.349699 fullask-rest-framework-0.1.9/fullask_rest_framework.egg-info/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5399 2023-06-14 08:59:30.000000 fullask-rest-framework-0.1.9/fullask_rest_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3209 2023-06-14 08:59:30.000000 fullask-rest-framework-0.1.9/fullask_rest_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-14 08:59:30.000000 fullask-rest-framework-0.1.9/fullask_rest_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       68 2023-06-14 08:59:30.000000 fullask-rest-framework-0.1.9/fullask_rest_framework.egg-info/entry_points.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-14 08:59:30.000000 fullask-rest-framework-0.1.9/fullask_rest_framework.egg-info/not-zip-safe
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      168 2023-06-14 08:59:30.000000 fullask-rest-framework-0.1.9/fullask_rest_framework.egg-info/requires.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       23 2023-06-14 08:59:30.000000 fullask-rest-framework-0.1.9/fullask_rest_framework.egg-info/top_level.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      869 2023-06-13 11:45:34.000000 fullask-rest-framework-0.1.9/pyproject.toml
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      394 2023-06-14 08:59:30.369699 fullask-rest-framework-0.1.9/setup.cfg
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1676 2023-06-14 08:59:25.000000 fullask-rest-framework-0.1.9/setup.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.365699 fullask-rest-framework-0.1.9/tests/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:34:17.000000 fullask-rest-framework-0.1.9/tests/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-14 08:59:30.365699 fullask-rest-framework-0.1.9/tests/repositories/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:35:54.000000 fullask-rest-framework-0.1.9/tests/repositories/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)    18729 2023-06-13 18:36:44.000000 fullask-rest-framework-0.1.9/tests/repositories/test_sqlalchemy_repository.py
```

### Comparing `fullask-rest-framework-0.1.8/LICENSE` & `fullask-rest-framework-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/PKG-INFO` & `fullask-rest-framework-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fullask-rest-framework
-Version: 0.1.8
+Version: 0.1.9
 Summary: A fully-supported flask extension to build REST API.
 Home-page: https://github.com/tgoddessana/fullask-rest-framework
 Author: tgoddessana
 Author-email: twicegoddessana1229@gmail.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.1.8 Summary: A
+Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.1.9 Summary: A
 fully-supported flask extension to build REST API. Home-page: https://
 github.com/tgoddessana/fullask-rest-framework Author: tgoddessana Author-email:
 twicegoddessana1229@gmail.com License: MIT license Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fullask-rest-framework-0.1.8/README.md` & `fullask-rest-framework-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/docs/Makefile` & `fullask-rest-framework-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/docs/docfiles/conf.py` & `fullask-rest-framework-0.1.9/docs/docfiles/conf.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/docs/docfiles/contributing.rst` & `fullask-rest-framework-0.1.9/docs/docfiles/contributing.rst`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/docs/docfiles/installation.rst` & `fullask-rest-framework-0.1.9/docs/docfiles/installation.rst`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/docs/make.bat` & `fullask-rest-framework-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/cli.py` & `fullask-rest-framework-0.1.9/fullask_rest_framework/cli.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/admin/templates/login_form.html` & `fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/admin/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css` & `fullask-rest-framework-0.1.9/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/createproject_template/project_template/factory.txt` & `fullask-rest-framework-0.1.9/fullask_rest_framework/createproject_template/project_template/factory.txt`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/factory/app_factory.py` & `fullask-rest-framework-0.1.9/fullask_rest_framework/factory/app_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from flask import Flask
 from flask_smorest import Api
 
 
 class BaseApplicationFactory:
     FLASK_APP_NAME: Optional[str] = None
     APP_BASE_DIR: Optional[str] = None
-    CONFIG_FILE: Optional[str] = None
-    EXTENSION_FILE: Optional[str] = None
+    CONFIG_MODULE: Optional[str] = None
+    EXTENSION_MODULE: Optional[str] = None
     MICRO_APP_CONFIG: Optional[List[Dict[str, str]]] = None
     DOTENV_SETTINGS = {
         "dotenv_path": "./.env",
         "stream": None,
         "verbose": False,
         "override": False,
         "interpolate": True,
@@ -61,26 +61,26 @@
                 f"`FLASK_APP_NAME` class variable is not set in '{cls.__name__}'."
                 f"set `FLASK_APP_NAME` class variable, or naming the Factory class,"
                 f" like '`YourAppName`Factory'."
             )
 
     @classmethod
     def _load_config(cls, flask_app: Flask):
-        if cls.CONFIG_FILE:
-            flask_app.config.from_object(importlib.import_module(cls.CONFIG_FILE))
+        if cls.CONFIG_MODULE:
+            flask_app.config.from_object(importlib.import_module(cls.CONFIG_MODULE))
         else:
             pass
 
     @classmethod
     def _configure_extensions(cls, flask_app):
         """
         configure third-party extensions, with `EXTENSION_FILE`.
         """
 
-        extensions = importlib.import_module(cls.EXTENSION_FILE)
+        extensions = cls.get_extensions()
         extension_vars = [
             extension_var
             for extension_var in dir(extensions)
             if not extension_var.startswith("__")
             and not callable(getattr(extensions, extension_var))
         ]
         for var in extension_vars:
@@ -107,7 +107,11 @@
                     micro_app_container=app_package_module.MICROAPP_CONTAINER
                 )
 
     @classmethod
     def _setup_di_container(cls, micro_app_container):
         """wiring the DI Container."""
         micro_app_container.wire(packages=[cls.APP_BASE_DIR])
+
+    @classmethod
+    def get_extensions(cls):
+        return importlib.import_module(cls.EXTENSION_MODULE)
```

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/factory/extensions.py` & `fullask-rest-framework-0.1.9/fullask_rest_framework/factory/extensions.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/orm/sqlalchemy/mixins.py` & `fullask-rest-framework-0.1.9/fullask_rest_framework/orm/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/crud.py` & `fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/crud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Generic, List, Optional
 
-from fullask_rest_framework.entities.filtering import FilteringRequest
-from fullask_rest_framework.entities.pagination import (
-    PaginationRequest,
-    PaginationResponse,
-)
-from fullask_rest_framework.entities.sorting import SortingRequest
 from fullask_rest_framework.repositories.base import BaseRepository, T
+from fullask_rest_framework.vo.filtering import FilteringRequest
+from fullask_rest_framework.vo.pagination import PaginationRequest, PaginationResponse
+from fullask_rest_framework.vo.sorting import SortingRequest
 
 
 class CRUDRepositoryABC(BaseRepository, ABC, Generic[T]):
     """The Base CRUD Repository class."""
 
     @abstractmethod
     def save(self, entity: T) -> T:
```

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/repositories/sqlalchemy.py` & `fullask-rest-framework-0.1.9/fullask_rest_framework/repositories/sqlalchemy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,32 @@
 from functools import wraps
-from typing import Generic, List, Optional
+from typing import Generic, List, Optional, Type
 
 from flask_marshmallow.sqla import SQLAlchemyAutoSchema  # type: ignore[import]
 from flask_sqlalchemy.query import Query
 from sqlalchemy import inspect, select
 
-from fullask_rest_framework.entities.filtering import FilteringRequest
-from fullask_rest_framework.entities.pagination import (
-    PaginationRequest,
-    PaginationResponse,
-)
-from fullask_rest_framework.entities.sorting import SortingRequest
 from fullask_rest_framework.repositories.base import T
 from fullask_rest_framework.repositories.crud import CRUDRepositoryABC
+from fullask_rest_framework.vo.filtering import FilteringRequest
+from fullask_rest_framework.vo.pagination import PaginationRequest, PaginationResponse
+from fullask_rest_framework.vo.sorting import SortingRequest
 
 
 class SQLAlchemyFullRepository(CRUDRepositoryABC, Generic[T]):
     """
     The implementation of CRUDRepositoryABC, with SQLAlchemy.
     this implementation has dependency with flask-sqlalchemy's SQLAlchemy object.
     """
 
-    def __init__(self, entity, db, sqlalchemy_model):
-        """
-        :param db: flask-sqlalchemy.SQLAlchemy
-        :param sqlalchemy_model: the SQLAlchemy model
-        """
+    ENTITY_CLS: Type[T]
+
+    def __init__(self, db):
         self.db = db
-        self.sqlalchemy_model = sqlalchemy_model
-        super().__init__(entity=entity)
-        assert set(self.entity.__annotations__.keys()) == set(
-            [column.name for column in self.sqlalchemy_model.__table__.columns]
-        ), (
-            "sqlalchemy model fields not match entity fields."
-            f"{self.entity.__annotations__.keys()} "
-            f"!= "
-            f"{[column.name for column in self.sqlalchemy_model.__table__.columns]}"
-        )
+        self.sqlalchemy_model = self._configure_entity()
 
     def save(self, entity: T) -> T:
         if hasattr(entity, "id") and entity.id:
             model_instance = self.db.session.get(self.sqlalchemy_model, entity.id)
             if model_instance:
                 self._update_model_with_entity(model_instance, entity)
         else:
@@ -196,14 +182,33 @@
     @staticmethod
     def _update_model_with_entity(model_instance, entity):
         # Iterate over the fields of the entity object
         for field_name, field_value in entity.__dict__.items():
             if field_name != "id":
                 setattr(model_instance, field_name, field_value)
 
+    def _configure_entity(self) -> Type[T]:
+        """
+        This method will find if there is a SQLAlchemy model class defined based on the entity class name.
+
+        The rules to look for are as follows:
+        {entity class name - "Entity"} + "Model"
+
+        For example, if the entity is named "CarEntity", the method will try to find the "CarModel" class.
+        """
+        models = {
+            mapper.class_.__name__: mapper.class_
+            for mapper in self.db.Model.registry.mappers
+        }
+        print(models)
+        try:
+            pass
+        except Exception as e:
+            pass
+
 
 def read_by_fields(func):
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         field_name = func.__name__[len("read_by_") :]
         if field_name in kwargs:
             field_value = kwargs[field_name]
```

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/schemas/fields.py` & `fullask-rest-framework-0.1.9/fullask_rest_framework/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/schemas/pagination.py` & `fullask-rest-framework-0.1.9/fullask_rest_framework/schemas/pagination.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from marshmallow import Schema, fields, post_load
 from marshmallow.validate import Range
 
-from fullask_rest_framework.entities.pagination import (
-    PaginationRequest,
-    PaginationResponse,
-)
+from fullask_rest_framework.vo.pagination import PaginationRequest, PaginationResponse
 
 
 class PaginationRequestSchema(Schema):
     page = fields.Integer(
         validate=Range(min=1),
         metadata={"description": "The page number you want to look up."},
     )
```

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/schemas/sorting.py` & `fullask-rest-framework-0.1.9/fullask_rest_framework/schemas/sorting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from flask_marshmallow import Schema  # type: ignore[import]
 from marshmallow import post_load
 
-from fullask_rest_framework.entities.sorting import SortingRequest
 from fullask_rest_framework.schemas import fields
+from fullask_rest_framework.vo.sorting import SortingRequest
 
 
 class SortingRequestSchema(Schema):
     sort_by = fields.Sorting(
         metadata={
             "description": "The sort condition. It must conform to the format `fieldname:sortcondition (asc or desc)`."
         }
```

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework/utils/jwt.py` & `fullask-rest-framework-0.1.9/fullask_rest_framework/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework.egg-info/PKG-INFO` & `fullask-rest-framework-0.1.9/fullask_rest_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fullask-rest-framework
-Version: 0.1.8
+Version: 0.1.9
 Summary: A fully-supported flask extension to build REST API.
 Home-page: https://github.com/tgoddessana/fullask-rest-framework
 Author: tgoddessana
 Author-email: twicegoddessana1229@gmail.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.1.8 Summary: A
+Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.1.9 Summary: A
 fully-supported flask extension to build REST API. Home-page: https://
 github.com/tgoddessana/fullask-rest-framework Author: tgoddessana Author-email:
 twicegoddessana1229@gmail.com License: MIT license Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fullask-rest-framework-0.1.8/fullask_rest_framework.egg-info/SOURCES.txt` & `fullask-rest-framework-0.1.9/fullask_rest_framework.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,14 @@
 fullask_rest_framework/createproject_template/project_template/__init__.txt
 fullask_rest_framework/createproject_template/project_template/app.txt
 fullask_rest_framework/createproject_template/project_template/config.py.txt
 fullask_rest_framework/createproject_template/project_template/factory.txt
 fullask_rest_framework/createproject_template/project_template/tests.txt
 fullask_rest_framework/entities/__init__.py
 fullask_rest_framework/entities/base_entity.py
-fullask_rest_framework/entities/filtering.py
-fullask_rest_framework/entities/pagination.py
-fullask_rest_framework/entities/sorting.py
 fullask_rest_framework/factory/__init__.py
 fullask_rest_framework/factory/app_factory.py
 fullask_rest_framework/factory/extensions.py
 fullask_rest_framework/orm/__init__.py
 fullask_rest_framework/orm/sqlalchemy/__init__.py
 fullask_rest_framework/orm/sqlalchemy/base_model.py
 fullask_rest_framework/orm/sqlalchemy/mixins.py
@@ -63,10 +60,14 @@
 fullask_rest_framework/schemas/fields.py
 fullask_rest_framework/schemas/filtering.py
 fullask_rest_framework/schemas/pagination.py
 fullask_rest_framework/schemas/sorting.py
 fullask_rest_framework/service/__init__.py
 fullask_rest_framework/utils/__init__.py
 fullask_rest_framework/utils/jwt.py
+fullask_rest_framework/vo/__init__.py
+fullask_rest_framework/vo/filtering.py
+fullask_rest_framework/vo/pagination.py
+fullask_rest_framework/vo/sorting.py
 tests/__init__.py
 tests/repositories/__init__.py
 tests/repositories/test_sqlalchemy_repository.py
```

### Comparing `fullask-rest-framework-0.1.8/pyproject.toml` & `fullask-rest-framework-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.8/setup.py` & `fullask-rest-framework-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,10 +50,10 @@
     name="fullask-rest-framework",
     packages=find_packages(
         include=["fullask_rest_framework", "fullask_rest_framework.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/tgoddessana/fullask-rest-framework",
-    version="0.1.8",
+    version="0.1.9",
     zip_safe=False,
 )
```

### Comparing `fullask-rest-framework-0.1.8/tests/repositories/test_sqlalchemy_repository.py` & `fullask-rest-framework-0.1.9/tests/repositories/test_sqlalchemy_repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import pytest
 from flask import Flask
 from flask_sqlalchemy import SQLAlchemy
 
-from fullask_rest_framework.entities.filtering import FilteringRequest
-from fullask_rest_framework.entities.pagination import (
-    PaginationRequest,
-    PaginationResponse,
-)
-from fullask_rest_framework.entities.sorting import SortingRequest
 from fullask_rest_framework.repositories.sqlalchemy import SQLAlchemyFullRepository
+from fullask_rest_framework.vo.filtering import FilteringRequest
+from fullask_rest_framework.vo.pagination import PaginationRequest, PaginationResponse
+from fullask_rest_framework.vo.sorting import SortingRequest
 
 ###################
 # pytest fixtures #
 ###################
 
-
 db = SQLAlchemy()
 
 
 class UserModel(db.Model):  # type: ignore[name-defined]
     __tablename__ = "users"
     id = db.Column(db.Integer, primary_key=True)
     name = db.Column(db.String(50))
@@ -31,14 +27,22 @@
 class UserEntity:
     name: str
 
     id: Optional[int] = None
 
 
 @pytest.fixture
+def user_repository():
+    class UserRepository(SQLAlchemyFullRepository):
+        entity = UserEntity
+
+    yield UserRepository(db=db)
+
+
+@pytest.fixture
 def test_app():
     test_app = Flask("test_app")
     test_app.config["TESTING"] = True
     test_app.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:///:memory:"
     db.init_app(test_app)
 
     with test_app.app_context():
@@ -49,56 +53,50 @@
 
 
 # ##################
 # test code starts #
 # ##################
 
 
-def test_save_success_and_return_entity(test_app):
+def test_save_success_and_return_entity(test_app, user_repository):
     """
     save() 메서드가 저장을 잘 수행하는지를 테스트합니다.
     """
     user_fullask = UserEntity(name="mr_fullask")
     with test_app.test_request_context():
-        user_entity = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).save(user_fullask)
+        user_entity = user_repository.save(user_fullask)
         assert UserModel.query.count() == 1
         assert user_entity.id == 1
         assert user_entity.name == "mr_fullask"
 
 
-def test_get_id_and_save_success(test_app):
+def test_get_id_and_save_success(test_app, user_repository):
     """
     read_by_id 메서드로 엔티티를 가져온 다음, 수정을 진행한 후
     save() 메서드가 저장을 잘 수행하는지를 테스트합니다.
     """
 
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))
-        user_fullask = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).read_by_id(1)
+        user_fullask = user_repository.read_by_id(1)
         user_fullask.name = "mr_django"
-        SQLAlchemyFullRepository(UserEntity, db=db, sqlalchemy_model=UserModel).save(
-            user_fullask
-        )
+        user_repository.save(user_fullask)
 
 
-def test_save_all_success_and_return_entities(test_app):
+def test_save_all_success_and_return_entities(test_app, user_repository):
     """
     save_all() 메서드가 저장을 잘 수행하는지를 테스트합니다.
     """
     user_fullask = UserEntity(name="mr_fullask")
     user_django = UserEntity(name="mr_django")
     user_fastapi = UserEntity(name="mr_fastapi")
     with test_app.test_request_context():
-        user_entities = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).save_all([user_fullask, user_django, user_fastapi])
+        user_entities = user_repository.save_all(
+            [user_fullask, user_django, user_fastapi]
+        )
         assert UserModel.query.count() == 3
         assert isinstance(user_entities, list)
         assert user_entities[0].id == 1
         assert user_entities[0].name == "mr_fullask" and isinstance(
             user_entities[0], UserEntity
         )
         assert user_entities[1].id == 2
@@ -107,183 +105,161 @@
         )
         assert user_entities[2].id == 3
         assert user_entities[2].name == "mr_fastapi" and isinstance(
             user_entities[0], UserEntity
         )
 
 
-def test_read_by_id_should_return_none(test_app):
+def test_read_by_id_should_return_none(test_app, user_repository):
     """
     없는 id 로 사용자 조회를 수행하면,
     read_by_id 는 None 을 반환해야 합니다.
     """
     with test_app.test_request_context():
-        user = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).read_by_id(1)
+        user = user_repository.read_by_id(1)
     assert user is None
 
 
-def test_read_by_id_should_return_user_entity(test_app):
+def test_read_by_id_should_return_user_entity(test_app, user_repository):
     """
     데이터베이스 테이블에 사용자 정보가 적절하게 저장되었다면,
     read_by_id 는 UserEntity 객체를 반환해야 합니다.
     """
     # 데이터베이스에 사용자를 저장합니다.
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))
         db.session.add(UserModel(name="mr_django"))
         db.session.commit()
         # repository 를 이용해서 확인합니다.
-        user_fullask = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).read_by_id(1)
-        user_django = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).read_by_id(2)
+        user_fullask = user_repository.read_by_id(1)
+        user_django = user_repository.read_by_id(2)
     assert user_fullask.name == "mr_fullask" and isinstance(user_fullask, UserEntity)
     assert user_django.name == "mr_django" and isinstance(user_fullask, UserEntity)
 
 
-def test_is_exists_by_id_should_return_false(test_app):
+def test_is_exists_by_id_should_return_false(test_app, user_repository):
     """
     해당 id 로 찾을 수 없다면 False 를 반환해야 합니다.
     """
     with test_app.test_request_context():
-        assert (
-            SQLAlchemyFullRepository(
-                UserEntity, db=db, sqlalchemy_model=UserModel
-            ).is_exists_by_id(1)
-            is False
-        )
+        assert user_repository.is_exists_by_id(1) is False
 
 
-def test_is_exists_by_id_should_return_true(test_app):
+def test_is_exists_by_id_should_return_true(test_app, user_repository):
     """
     해당 id 로 찾을 수 있다면 True 를 반환해야 합니다.
     """
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))
         db.session.commit()
-        assert (
-            SQLAlchemyFullRepository(
-                UserEntity, db=db, sqlalchemy_model=UserModel
-            ).is_exists_by_id(1)
-            is True
-        )
+        assert user_repository.is_exists_by_id(1) is True
 
 
 ###################
 # read_all() TEST #
 ###################
 
 
-def test_read_all_return_empty_list(test_app):
+def test_read_all_return_empty_list(test_app, user_repository):
     """
     데이터베이스에 아무런 사용자도 저장되어있지 않다면, read_all() 은 비어있는 리스트를 반환해야 합니다.
     """
     with test_app.test_request_context():
-        read_all_result = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).read_all()
+        read_all_result = user_repository.read_all()
         assert isinstance(read_all_result, list)
         assert len(read_all_result) == 0
 
 
-def test_read_all_without_sorting_and_filtering_success(test_app):
+def test_read_all_without_sorting_and_filtering_success(test_app, user_repository):
     """
     정렬과 필터링 요청 객체가 없을 때, read_all() 메서드가 데이터를 잘 읽어오는지 테스트합니다.
     데이터베이스에 두 명의 사용자가 저장되어 있다면, read_list() 는 길이가 2인 리스트여야 합니다.
     아무런 정렬 요청 객체, 필터링 객체가 전달되지 않았다면 id의 오름차순, 모든 데이터가 페이지네이션 없이 반환되어야 합니다.
     그리고, 각각의 요소는 Entity 객체여야 합니다.
     """
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))
         db.session.add(UserModel(name="mr_django"))
         db.session.commit()
-        read_all_result = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).read_all()
+        read_all_result = user_repository.read_all()
         assert isinstance(read_all_result, list)
         assert len(read_all_result) == 2
         assert read_all_result[0].name == "mr_fullask" and isinstance(
             read_all_result[0], UserEntity
         )
         assert read_all_result[1].name == "mr_django" and isinstance(
             read_all_result[1], UserEntity
         )
 
 
-def test_read_all_with_pagination_return_paginated_list(test_app):
+def test_read_all_with_pagination_return_paginated_list(test_app, user_repository):
     """
     read_all_with_pagination() 메서드가 데이터를 잘 읽어오는지 테스트합니다.
     사용자 5명이 저장되어 있고, 2명씩 페이지네이션 처리한 다음 2페이지를 조회한다면 잘 수행되어야 합니다.
     """
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))
         db.session.add(UserModel(name="mr_django"))
         db.session.add(UserModel(name="mr_spring"))
         db.session.add(UserModel(name="mr_react"))
         db.session.add(UserModel(name="mr_fastapi"))
         db.session.commit()
-        read_all_result_with_pagination = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
+        read_all_result_with_pagination = user_repository(
+            sqlalchemy_model=UserModel
         ).read_all_with_pagination(PaginationRequest(page=2, per_page=2))
         assert isinstance(read_all_result_with_pagination, PaginationResponse)
         assert read_all_result_with_pagination.count == 5
         assert read_all_result_with_pagination.previous_page == 1
         assert read_all_result_with_pagination.next_page == 3
         assert len(read_all_result_with_pagination.results) == 2
         assert read_all_result_with_pagination.results[0].name == "mr_spring"
         assert read_all_result_with_pagination.results[1].name == "mr_react"
 
 
-def test_read_all_with_pagination_with_sorting_success(test_app):
+def test_read_all_with_pagination_with_sorting_success(test_app, user_repository):
     """
     read_all_with_pagination() 메서드가 정렬 객체가 있을 때 데이터를 잘 읽어오는지 테스트합니다.
     사용자 5명이 저장되어 있고, 2명씩 페이지네이션 처리한 다음 id의 내림차순으로 정렬 후 2페이지를 조회한다면 잘 수행되어야 합니다.
     """
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))
         db.session.add(UserModel(name="mr_django"))
         db.session.add(UserModel(name="mr_spring"))
         db.session.add(UserModel(name="mr_react"))
         db.session.add(UserModel(name="mr_fastapi"))
         db.session.commit()
-        read_all_result_with_pagination = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
+        read_all_result_with_pagination = user_repository(
+            sqlalchemy_model=UserModel
         ).read_all_with_pagination(
             PaginationRequest(page=2, per_page=2),
             SortingRequest({"id": "desc"}),
         )
 
         assert isinstance(read_all_result_with_pagination, PaginationResponse)
         assert read_all_result_with_pagination.count == 5
         assert read_all_result_with_pagination.previous_page == 1
         assert read_all_result_with_pagination.next_page == 3
         assert len(read_all_result_with_pagination.results) == 2
         assert read_all_result_with_pagination.results[0].name == "mr_spring"
         assert read_all_result_with_pagination.results[1].name == "mr_django"
 
 
-def test_read_all_with_pagination_with_filtering_success(test_app):
+def test_read_all_with_pagination_with_filtering_success(test_app, user_repository):
     """
     read_all_with_pagination() 메서드가 필터링 객체가 있을 때 데이터를 잘 읽어오는지 테스트합니다.
     사용자 5명이 저장되어 있고, 2명씩 페이지네이션 처리한 다음 "이름에 'pring' 이 들어 있는 필터링을 적용 후,
     1페이지를 조회한다면 잘 수행되어야 합니다.
     """
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))
         db.session.add(UserModel(name="mr_japring"))
         db.session.add(UserModel(name="mr_kopring"))
         db.session.add(UserModel(name="mr_fastapi"))
         db.session.commit()
-        read_all_result_with_pagination = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).read_all_with_pagination(
+        read_all_result_with_pagination = user_repository.read_all_with_pagination(
             pagination_request=PaginationRequest(page=1, per_page=2),
             filtering_request=FilteringRequest(name="pring"),
         )
 
         assert isinstance(read_all_result_with_pagination, PaginationResponse)
         assert (
             read_all_result_with_pagination.count == 2
@@ -291,29 +267,29 @@
         assert read_all_result_with_pagination.previous_page is None
         assert read_all_result_with_pagination.next_page is None
         assert len(read_all_result_with_pagination.results) == 2  # per_page is 2.
         assert read_all_result_with_pagination.results[0].name == "mr_japring"
         assert read_all_result_with_pagination.results[1].name == "mr_kopring"
 
 
-def test_read_all_with_pagination_with_filtering_sorting_success(test_app):
+def test_read_all_with_pagination_with_filtering_sorting_success(
+    test_app, user_repository
+):
     """
     read_all_with_pagination() 메서드가 필터링 객체와 정렬 객체가 있을 때 데이터를 잘 읽어오는지 테스트합니다.
     사용자 5명이 저장되어 있고, 2명씩 페이지네이션 처리한 다음 "이름에 'pring' 이 들어 있는 필터링을 적용 후,
     id의 역순으로 정렬하고 요청한 후 1페이지를 조회한다면 잘 수행되어야 합니다.
     """
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))
         db.session.add(UserModel(name="mr_japring"))
         db.session.add(UserModel(name="mr_kopring"))
         db.session.add(UserModel(name="mr_fastapi"))
         db.session.commit()
-        read_all_result_with_pagination = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).read_all_with_pagination(
+        read_all_result_with_pagination = user_repository.read_all_with_pagination(
             pagination_request=PaginationRequest(page=1, per_page=2),
             sorting_request=SortingRequest({"id": "desc"}),
             filtering_request=FilteringRequest(name="pring"),
         )
 
         assert isinstance(read_all_result_with_pagination, PaginationResponse)
         assert (
@@ -322,84 +298,73 @@
         assert read_all_result_with_pagination.previous_page is None
         assert read_all_result_with_pagination.next_page is None
         assert len(read_all_result_with_pagination.results) == 2  # per_page is 2.
         assert read_all_result_with_pagination.results[0].name == "mr_kopring"
         assert read_all_result_with_pagination.results[1].name == "mr_japring"
 
 
-def test_read_all_by_ids(test_app):
+def test_read_all_by_ids(test_app, user_repository):
     """
     read_all_by_ids() 메서드가 데이터를 잘 읽어오는지 테스트합니다.
     """
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))  # id should 1
         db.session.add(UserModel(name="mr_django"))  # id should 2
         db.session.add(UserModel(name="mr_spring"))  # id should 3
         db.session.commit()
-        read_all_result = SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).read_all_by_ids([1, 3])
+        read_all_result = user_repository.read_all_by_ids([1, 3])
         assert isinstance(read_all_result, list)
         assert len(read_all_result) == 2
         assert read_all_result[0].name == "mr_fullask" and isinstance(
             read_all_result[0], UserEntity
         )
         assert read_all_result[1].name == "mr_spring" and isinstance(
             read_all_result[1], UserEntity
         )
 
 
-def test_count_should_return_2(test_app):
+def test_count_should_return_2(test_app, user_repository):
     """
     count() 메서드가 정확한 값을 리턴하는지 테스트합니다.
     사용자 2명이 저장되어 있다면, count() 메서드는 2를 반환해야 합니다.
     """
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))
         db.session.add(UserModel(name="mr_django"))
         db.session.commit()
-        assert (
-            SQLAlchemyFullRepository(
-                UserEntity, db=db, sqlalchemy_model=UserModel
-            ).count()
-            == 2
-        )
+        assert user_repository.count() == 2
 
 
-def test_delete_by_id_should_success(test_app):
+def test_delete_by_id_should_success(test_app, user_repository):
     """
     delete_by_id() 메서드가 id를 받아 데이터 삭제를 잘 수행하는지 테스트합니다.
     """
     with test_app.test_request_context():
         db.session.add(UserModel(name="mr_fullask"))  # id should 1
         db.session.add(UserModel(name="mr_django"))  # id should 2
         db.session.commit()
         # 삭제 전에는 사용자가 2명이어야 함
         assert db.session.query(UserModel).count() == 2
         # delete_by_id() 메서드 호출
-        SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).delete_by_id(1)
+        user_repository.delete_by_id(1)
         assert db.session.query(UserModel).count() == 1
 
 
-def test_delete_by_id_with_unknown_id_should_fail(test_app):
+def test_delete_by_id_with_unknown_id_should_fail(test_app, user_repository):
     """
     delete_by_id() 메서드가 id를 받았지만, 데이터베이스에서 해당 id로 데이터를 찾을 수 없는 경우
     ValueError 를 발생시켜야 합니다.
     """
     with test_app.test_request_context():
         with pytest.raises(ValueError):
             # delete_by_id() 메서드 호출 시에는 ValueError 가 발생해야 한다.
-            SQLAlchemyFullRepository(
-                UserEntity, db=db, sqlalchemy_model=UserModel
-            ).delete_by_id(3)
+            user_repository.delete_by_id(3)
 
 
-def test_delete_by_entity_should_success(test_app):
+def test_delete_by_entity_should_success(test_app, user_repository):
     """
     delete() 메서드가 엔티티를 받아 데이터 삭제를 잘 수행하는지 테스트합니다.
     해당 엔티티를 데이터베이스에서 찾을 수 있다면, 삭제가 잘 이루어져야 합니다.
     """
     with test_app.test_request_context():
         # 먼저, 사용자를 저장
         db.session.add(UserModel(name="mr_fullask"))  # id is 1
@@ -408,36 +373,32 @@
         # 삭제 전에는 사용자가 1명이어야 함
         assert db.session.query(UserModel).count() == 1
 
         # entity 생성
         user = UserEntity(id=1, name="mr_fullask")
 
         # delete() 메서드 호출, 인자로는 entity 객체가 들어옴
-        SQLAlchemyFullRepository(UserEntity, db=db, sqlalchemy_model=UserModel).delete(
-            entity=user
-        )
+        user_repository.delete(entity=user)
         assert db.session.query(UserModel).count() == 0
 
 
-def test_delete_by_invalid_entity_should_fail(test_app):
+def test_delete_by_invalid_entity_should_fail(test_app, user_repository):
     """
     delete() 메서드가 엔티티를 받아 데이터 삭제를 잘 수행하는지 테스트합니다.
     해당 엔티티를 데이터베이스에서 찾을 수 없다면, 삭제는 실패해야 합니다.
     """
     with test_app.test_request_context():
         # 유효하지 않은 entity 생성
         invalid_user_entity = UserEntity(id=2, name="mr_fullask")
 
         with pytest.raises(ValueError):
-            SQLAlchemyFullRepository(
-                UserEntity, db=db, sqlalchemy_model=UserModel
-            ).delete(invalid_user_entity)
+            user_repository.delete(invalid_user_entity)
 
 
-def test_delete_by_valid_entity_should_success(test_app):
+def test_delete_by_valid_entity_should_success(test_app, user_repository):
     """
     delete() 메서드가 엔티티를 받아 데이터 삭제를 잘 수행하는지 테스트합니다.
     해당 엔티티를 데이터베이스에서 찾을 수 있다면, 삭제가 잘 이루어져야 합니다.
     """
     with test_app.test_request_context():
         # 먼저, 사용자를 저장
         db.session.add(UserModel(name="mr_fullask"))
@@ -445,54 +406,48 @@
 
         # 삭제 전에는 사용자가 1명이어야 함
         assert db.session.query(UserModel).count() == 1
 
         # 유효한 entity 생성
         valid_user_entity = UserEntity(id=1, name="mr_fullask")
 
-        SQLAlchemyFullRepository(UserEntity, db=db, sqlalchemy_model=UserModel).delete(
-            valid_user_entity
-        )
+        user_repository.delete(valid_user_entity)
 
         # 삭제 후에는 사용자가 0명이어야 함
         assert db.session.query(UserModel).count() == 0
 
 
-def test_delete_all_by_ids_should_success(test_app):
+def test_delete_all_by_ids_should_success(test_app, user_repository):
     """
     delete_all_by_ids() 메서드가 id 를 받아 데이터 삭제를 잘 수행하는지 테스트합니다.
     받은 id가 모두 데이터베이스에 존재하고 찾을 수 있다면, 삭제가 잘 이루어져야 합니다.
     """
     with test_app.test_request_context():
         # 먼저, 사용자를 저장
         db.session.add(UserModel(name="mr_fullask"))  # id should be 1
         db.session.add(UserModel(name="mr_django"))  # id should be 2
         db.session.add(UserModel(name="mr_fastapi"))  # id should be 3
         db.session.add(UserModel(name="mr_spring"))  # id should be 4
         db.session.commit()
 
-        SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).delete_all_by_ids([1, 3, 4])
+        user_repository.delete_all_by_ids([1, 3, 4])
 
         assert db.session.query(UserModel).count() == 1
 
 
-def test_delete_all_should_success(test_app):
+def test_delete_all_should_success(test_app, user_repository):
     """
     delete_all() 메서드가 데이터 삭제를 잘 수행하는지 테스트합니다.
     """
     with test_app.test_request_context():
         # 먼저, 사용자를 저장
         db.session.add(UserModel(name="mr_fullask"))
         db.session.add(UserModel(name="mr_django"))
         db.session.add(UserModel(name="mr_fastapi"))
         db.session.add(UserModel(name="mr_spring"))
         db.session.commit()
 
         assert db.session.query(UserModel).count() == 4
 
-        SQLAlchemyFullRepository(
-            UserEntity, db=db, sqlalchemy_model=UserModel
-        ).delete_all()
+        user_repository.delete_all()
 
         assert db.session.query(UserModel).count() == 0
```

