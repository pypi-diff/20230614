# Comparing `tmp/xmlschema-2.3.0.tar.gz` & `tmp/xmlschema-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlschema-2.3.0.tar", last modified: Thu May 18 20:19:54 2023, max compression
+gzip compressed data, was "xmlschema-2.3.1.tar", last modified: Wed Jun 14 07:04:26 2023, max compression
```

## Comparing `xmlschema-2.3.0.tar` & `xmlschema-2.3.1.tar`

### file list

```diff
@@ -1,493 +1,496 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.688786 xmlschema-2.3.0/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-2.3.0/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    25053 2023-05-18 20:18:16.000000 xmlschema-2.3.0/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2022-09-26 10:47:27.000000 xmlschema-2.3.0/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-2.3.0/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7377 2023-05-18 20:19:54.688786 xmlschema-2.3.0/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6045 2022-08-26 15:33:28.000000 xmlschema-2.3.0/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.545786 xmlschema-2.3.0/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-2.3.0/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11613 2022-10-01 13:42:01.000000 xmlschema-2.3.0/doc/api.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-2.3.0/doc/components.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5474 2023-05-18 20:18:16.000000 xmlschema-2.3.0/doc/conf.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-2.3.0/doc/converters.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-2.3.0/doc/extras.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7488 2022-06-24 14:13:22.000000 xmlschema-2.3.0/doc/features.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-2.3.0/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-2.3.0/doc/intro.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-2.3.0/doc/testing.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)    27730 2022-10-01 13:42:01.000000 xmlschema-2.3.0/doc/usage.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-2.3.0/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2023-05-18 20:18:16.000000 xmlschema-2.3.0/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-05-18 20:19:54.688786 xmlschema-2.3.0/setup.cfg
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2764 2023-05-18 20:18:16.000000 xmlschema-2.3.0/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.552785 xmlschema-2.3.0/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-2.3.0/tests/__init__.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     4934 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/check_memory.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.529785 xmlschema-2.3.0/tests/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.552785 xmlschema-2.3.0/tests/templates/demo/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/demo/demo_type_filter_test.jinja
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.555786 xmlschema-2.3.0/tests/templates/filters/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/namespace_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/python_type_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/sort_types_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-2.3.0/tests/templates/filters/type_name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/type_qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/templates/filters/unknown_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/wrong-template.jinja
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3484 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_all.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.555786 xmlschema-2.3.0/tests/test_cases/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.529785 xmlschema-2.3.0/tests/test_cases/examples/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.558786 xmlschema-2.3.0/tests/test_cases/examples/collection/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection-default.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2023-05-18 20:17:39.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection3bis.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection3bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection4.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection5.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.559786 xmlschema-2.3.0/tests/test_cases/examples/stockquote/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquote.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.568786 xmlschema-2.3.0/tests/test_cases/examples/vehicles/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/bikes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/cars.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-1_error.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-3_errors.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-max.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles2.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles2.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.530785 xmlschema-2.3.0/tests/test_cases/features/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.569786 xmlschema-2.3.0/tests/test_cases/features/attributes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/attributes/default_attributes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.570786 xmlschema-2.3.0/tests/test_cases/features/builtins/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/builtins/builtins.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/builtins/builtins.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.572786 xmlschema-2.3.0/tests/test_cases/features/decoder/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/data.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/data2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/data3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/data4-mixed.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/long-sequence-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/mixed-content.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/simple-types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.575786 xmlschema-2.3.0/tests/test_cases/features/derivations/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/complex-extensions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/complex11-restrictions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/list_types.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/list_types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.577786 xmlschema-2.3.0/tests/test_cases/features/elements/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/elements/test_alternatives-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/elements/type_alternatives.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.583786 xmlschema-2.3.0/tests/test_cases/features/models/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/billion_laughs_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/circular_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/illegal-attributes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/illegal-declarations.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/illegal-occurs.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/invalid_models1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/invalid_models2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/model1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-2.3.0/tests/test_cases/features/models/models.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/other-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/recursive-groups.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-2.3.0/tests/test_cases/features/models/valid_model1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.591786 xmlschema-2.3.0/tests/test_cases/features/namespaces/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/chameleon1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/chameleon2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/chameleon3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/default_ns_invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/default_ns_valid1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/default_ns_valid2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case5a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case5b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case5c.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case1bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case2bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case5.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case6.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/included3-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/included4-invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/included5-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/included6-invalid.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.592786 xmlschema-2.3.0/tests/test_cases/features/patterns/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/patterns/patterns.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-2.3.0/tests/test_cases/features/patterns/patterns.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.594786 xmlschema-2.3.0/tests/test_cases/features/wsdl/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.536785 xmlschema-2.3.0/tests/test_cases/issues/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.594786 xmlschema-2.3.0/tests/test_cases/issues/issue_008/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_008/issue_008.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_008/issue_008.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.594786 xmlschema-2.3.0/tests/test_cases/issues/issue_009/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_009/issue_009.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.596786 xmlschema-2.3.0/tests/test_cases/issues/issue_013/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.596786 xmlschema-2.3.0/tests/test_cases/issues/issue_014/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_014/issue014.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.597786 xmlschema-2.3.0/tests/test_cases/issues/issue_018/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_018/issue_018-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_018/issue_018.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.600786 xmlschema-2.3.0/tests/test_cases/issues/issue_022/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_022/README.md
--rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_022/xml_string_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_022/xml_string_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_022/xsd_string.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.601786 xmlschema-2.3.0/tests/test_cases/issues/issue_026/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_026/issue_026-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_026/issue_026-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_026/issue_026-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_026/issue_026.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.602786 xmlschema-2.3.0/tests/test_cases/issues/issue_028/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_028/issue_028-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_028/issue_028-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_028/issue_028.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.603786 xmlschema-2.3.0/tests/test_cases/issues/issue_029/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_029/issue_029-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_029/issue_029-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_029/issue_029-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_029/issue_029.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.604786 xmlschema-2.3.0/tests/test_cases/issues/issue_035/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_035/dates.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_035/dates.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.604786 xmlschema-2.3.0/tests/test_cases/issues/issue_041/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_041/issue_041.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_041/issue_041.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.604786 xmlschema-2.3.0/tests/test_cases/issues/issue_045/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_045/issue_045.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.605786 xmlschema-2.3.0/tests/test_cases/issues/issue_046/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_046/issue_046.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_046/issue_046.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.605786 xmlschema-2.3.0/tests/test_cases/issues/issue_051/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_051/issue_051.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_051/issue_051.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.606786 xmlschema-2.3.0/tests/test_cases/issues/issue_073/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_073/issue_073-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_073/issue_073-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_073/issue_073.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.607786 xmlschema-2.3.0/tests/test_cases/issues/issue_086/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_086/issue_086-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_086/issue_086-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_086/issue_086.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.607786 xmlschema-2.3.0/tests/test_cases/issues/issue_105/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_105/issue_105.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.608786 xmlschema-2.3.0/tests/test_cases/issues/issue_111/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_111/issue_111.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.609786 xmlschema-2.3.0/tests/test_cases/issues/issue_115/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_115/Rotation.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.610786 xmlschema-2.3.0/tests/test_cases/issues/issue_171/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_171/issue_171.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_171/issue_171b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_171/issue_171c.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.611786 xmlschema-2.3.0/tests/test_cases/issues/issue_187/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_187/issue_187_1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_187/issue_187_2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.611786 xmlschema-2.3.0/tests/test_cases/issues/issue_190/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_190/issue_190.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_190/issue_190.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.612786 xmlschema-2.3.0/tests/test_cases/issues/issue_200/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_200/issue_200.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_200/issue_200.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.613786 xmlschema-2.3.0/tests/test_cases/issues/issue_203/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_203/issue_203.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_203/issue_203.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_203/issue_203alt.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.614786 xmlschema-2.3.0/tests/test_cases/issues/issue_204/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_204/issue_204.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_204/issue_204_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_204/issue_204_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_204/issue_204_3.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.615786 xmlschema-2.3.0/tests/test_cases/issues/issue_208/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_208/issue_208.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_208/issue_208.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.615786 xmlschema-2.3.0/tests/test_cases/issues/issue_222/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_222/issue_222.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_222/issue_222.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.616786 xmlschema-2.3.0/tests/test_cases/issues/issue_223/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_223/issue_223.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_223/issue_223.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.534786 xmlschema-2.3.0/tests/test_cases/issues/issue_237/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.617786 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.620786 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.620786 xmlschema-2.3.0/tests/test_cases/issues/issue_243/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_243/issue_243.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_243/issue_243.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.621786 xmlschema-2.3.0/tests/test_cases/issues/issue_245/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.621786 xmlschema-2.3.0/tests/test_cases/issues/issue_259/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_259/issue_259-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_259/issue_259-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.622786 xmlschema-2.3.0/tests/test_cases/issues/issue_265/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_265/issue_265-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.623786 xmlschema-2.3.0/tests/test_cases/issues/issue_266/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-2.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.624786 xmlschema-2.3.0/tests/test_cases/issues/issue_273/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_273/issue_273.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_273/issue_273.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.624786 xmlschema-2.3.0/tests/test_cases/issues/issue_276/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_276/dummy.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_276/schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.625786 xmlschema-2.3.0/tests/test_cases/issues/issue_298/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_298/issue_298-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_298/issue_298-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_298/issue_298.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.626786 xmlschema-2.3.0/tests/test_cases/issues/issue_306/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306-invalid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306-valid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.627786 xmlschema-2.3.0/tests/test_cases/issues/issue_311/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_311/correct_no_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.627786 xmlschema-2.3.0/tests/test_cases/issues/issue_314/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_314/issue_314.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_314/issue_314.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.629786 xmlschema-2.3.0/tests/test_cases/issues/issue_315/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315-3.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315-4.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315-5.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315_simple.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.631786 xmlschema-2.3.0/tests/test_cases/issues/issue_322/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_322/issue_322.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_322/issue_322.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.633786 xmlschema-2.3.0/tests/test_cases/issues/issue_324/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324-invalid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324b.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.634786 xmlschema-2.3.0/tests/test_cases/issues/issue_334/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.zip
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.635786 xmlschema-2.3.0/tests/test_cases/issues/issue_341/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_341/issue_341.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_341/issue_341.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.636786 xmlschema-2.3.0/tests/test_cases/mypy/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-2.3.0/tests/test_cases/mypy/extra_validator.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-2.3.0/tests/test_cases/mypy/schema_source.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-2.3.0/tests/test_cases/mypy/simple_types.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.637786 xmlschema-2.3.0/tests/test_cases/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/dummy file #2.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/dummy file.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/malformed.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/resources/unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/unused_external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/resources/unused_unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/with_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6429 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/testfiles
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11973 2021-03-04 20:38:45.000000 xmlschema-2.3.0/tests/test_cli.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-2.3.0/tests/test_codegen.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28857 2022-08-26 15:33:28.000000 xmlschema-2.3.0/tests/test_converters.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26556 2023-02-06 08:55:27.000000 xmlschema-2.3.0/tests/test_dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24554 2023-02-06 06:20:42.000000 xmlschema-2.3.0/tests/test_documents.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-2.3.0/tests/test_files.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    26065 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_helpers.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5745 2021-12-08 22:11:41.000000 xmlschema-2.3.0/tests/test_memory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9099 2023-02-11 10:41:50.000000 xmlschema-2.3.0/tests/test_namespaces.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-03-05 21:16:57.000000 xmlschema-2.3.0/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    70653 2023-02-06 06:20:42.000000 xmlschema-2.3.0/tests/test_resources.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-2.3.0/tests/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3600 2022-05-20 20:00:14.000000 xmlschema-2.3.0/tests/test_translations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2022 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_typing.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-2.3.0/tests/test_validation.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    27317 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_w3c_suite.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2023-02-11 10:41:50.000000 xmlschema-2.3.0/tests/test_xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.639786 xmlschema-2.3.0/tests/validation/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.3.0/tests/validation/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    66088 2023-04-14 13:49:05.000000 xmlschema-2.3.0/tests/validation/test_decoding.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    33339 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validation/test_encoding.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16337 2022-10-01 13:42:01.000000 xmlschema-2.3.0/tests/validation/test_validation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.647786 xmlschema-2.3.0/tests/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.3.0/tests/validators/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-2.3.0/tests/validators/test_builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33116 2023-03-05 20:30:24.000000 xmlschema-2.3.0/tests/validators/test_complex_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-2.3.0/tests/validators/test_elements.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     9464 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_exceptions.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60271 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_facets.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2022-03-07 13:26:41.000000 xmlschema-2.3.0/tests/validators/test_global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    13500 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/validators/test_groups.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19187 2023-02-06 06:20:42.000000 xmlschema-2.3.0/tests/validators/test_identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    52697 2023-04-14 13:49:05.000000 xmlschema-2.3.0/tests/validators/test_models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_notations.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    41506 2022-10-01 13:42:01.000000 xmlschema-2.3.0/tests/validators/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_simple_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_wildcards.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    33897 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1569 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tox.ini
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.656786 xmlschema-2.3.0/xmlschema/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2857 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5515 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/aliases.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11669 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/cli.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.661786 xmlschema-2.3.0/xmlschema/converters/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      813 2022-07-18 14:19:15.000000 xmlschema-2.3.0/xmlschema/converters/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5977 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/abdera.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7228 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/badgerfish.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7587 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/columnar.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19819 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/default.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4769 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/jsonml.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5840 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/parker.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5711 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/unordered.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23717 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35712 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/documents.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-2.3.0/xmlschema/exceptions.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.662786 xmlschema-2.3.0/xmlschema/extras/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-2.3.0/xmlschema/extras/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    21930 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/extras/codegen.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.538786 xmlschema-2.3.0/xmlschema/extras/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.663786 xmlschema-2.3.0/xmlschema/extras/templates/python/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-2.3.0/xmlschema/extras/templates/python/bindings.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-2.3.0/xmlschema/extras/templates/python/sample.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24454 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/extras/wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11097 2022-08-26 15:33:28.000000 xmlschema-2.3.0/xmlschema/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-2.3.0/xmlschema/limits.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.538786 xmlschema-2.3.0/xmlschema/locale/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.538786 xmlschema-2.3.0/xmlschema/locale/en/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.665786 xmlschema-2.3.0/xmlschema/locale/en/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-2.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    64464 2022-05-20 20:00:14.000000 xmlschema-2.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.538786 xmlschema-2.3.0/xmlschema/locale/it/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.667786 xmlschema-2.3.0/xmlschema/locale/it/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-2.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-2.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.538786 xmlschema-2.3.0/xmlschema/locale/ru/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.667786 xmlschema-2.3.0/xmlschema/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-2.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-2.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8827 2020-12-23 12:38:37.000000 xmlschema-2.3.0/xmlschema/names.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9907 2023-02-04 20:00:06.000000 xmlschema-2.3.0/xmlschema/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-2.3.0/xmlschema/py.typed
--rw-r--r--   0 brunato   (1000) brunato   (1000)    55658 2023-04-14 13:49:05.000000 xmlschema-2.3.0/xmlschema/resources.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.539785 xmlschema-2.3.0/xmlschema/schemas/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.668786 xmlschema-2.3.0/xmlschema/schemas/HFP/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.668786 xmlschema-2.3.0/xmlschema/schemas/VC/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.669786 xmlschema-2.3.0/xmlschema/schemas/WSDL/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/WSDL/soap-encoding.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/WSDL/soap-envelope.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/WSDL/wsdl-soap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/WSDL/wsdl.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.669786 xmlschema-2.3.0/xmlschema/schemas/XHTML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.670786 xmlschema-2.3.0/xmlschema/schemas/XLINK/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XLINK/xlink.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.670786 xmlschema-2.3.0/xmlschema/schemas/XML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XML/xml_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.671786 xmlschema-2.3.0/xmlschema/schemas/XSD_1.0/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-2.3.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XSD_1.0/datatypes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.672786 xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/datatypes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.672786 xmlschema-2.3.0/xmlschema/schemas/XSI/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.675786 xmlschema-2.3.0/xmlschema/testing/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2116 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/testing/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    29742 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/testing/_builders.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7950 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/testing/_case_class.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/testing/_factory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6911 2022-09-08 10:16:11.000000 xmlschema-2.3.0/xmlschema/testing/_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4891 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/testing/_observers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-2.3.0/xmlschema/translation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.687786 xmlschema-2.3.0/xmlschema/validators/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3557 2021-11-11 15:30:24.000000 xmlschema-2.3.0/xmlschema/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6619 2023-05-07 06:35:13.000000 xmlschema-2.3.0/xmlschema/validators/assertions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34132 2022-09-24 15:52:22.000000 xmlschema-2.3.0/xmlschema/validators/attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-2.3.0/xmlschema/validators/builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    46791 2023-05-07 06:33:55.000000 xmlschema-2.3.0/xmlschema/validators/complex_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    64166 2023-03-28 06:38:11.000000 xmlschema-2.3.0/xmlschema/validators/elements.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14970 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/validators/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31723 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/validators/facets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33050 2023-05-05 13:39:50.000000 xmlschema-2.3.0/xmlschema/validators/global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    63595 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/validators/groups.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     6655 2022-05-20 16:16:20.000000 xmlschema-2.3.0/xmlschema/validators/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    18740 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/validators/identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23474 2023-04-14 13:49:05.000000 xmlschema-2.3.0/xmlschema/validators/models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-2.3.0/xmlschema/validators/notations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6684 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/validators/particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)   103598 2023-05-07 06:48:48.000000 xmlschema-2.3.0/xmlschema/validators/schemas.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    61468 2023-05-08 10:45:15.000000 xmlschema-2.3.0/xmlschema/validators/simple_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38290 2022-09-25 07:58:42.000000 xmlschema-2.3.0/xmlschema/validators/wildcards.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    41151 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/validators/xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    13135 2023-02-11 10:41:50.000000 xmlschema-2.3.0/xmlschema/xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.657786 xmlschema-2.3.0/xmlschema.egg-info/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7377 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/PKG-INFO
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    17121 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/SOURCES.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/dependency_links.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/entry_points.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/requires.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/top_level.txt
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.663356 xmlschema-2.3.1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-2.3.1/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    25333 2023-06-14 07:04:00.000000 xmlschema-2.3.1/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2022-09-26 10:47:27.000000 xmlschema-2.3.1/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-2.3.1/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7377 2023-06-14 07:04:26.663356 xmlschema-2.3.1/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6045 2022-08-26 15:33:28.000000 xmlschema-2.3.1/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.628356 xmlschema-2.3.1/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-2.3.1/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11613 2022-10-01 13:42:01.000000 xmlschema-2.3.1/doc/api.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-2.3.1/doc/components.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5474 2023-06-14 07:04:00.000000 xmlschema-2.3.1/doc/conf.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-2.3.1/doc/converters.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-2.3.1/doc/extras.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7488 2022-06-24 14:13:22.000000 xmlschema-2.3.1/doc/features.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-2.3.1/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-2.3.1/doc/intro.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-2.3.1/doc/testing.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27730 2022-10-01 13:42:01.000000 xmlschema-2.3.1/doc/usage.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-2.3.1/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2023-05-18 20:18:16.000000 xmlschema-2.3.1/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-06-14 07:04:26.663356 xmlschema-2.3.1/setup.cfg
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2764 2023-06-14 07:04:00.000000 xmlschema-2.3.1/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.630356 xmlschema-2.3.1/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-2.3.1/tests/__init__.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     4934 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/check_memory.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.621356 xmlschema-2.3.1/tests/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.630356 xmlschema-2.3.1/tests/templates/demo/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/demo/demo_type_filter_test.jinja
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.631356 xmlschema-2.3.1/tests/templates/filters/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/namespace_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/python_type_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/sort_types_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-2.3.1/tests/templates/filters/type_name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/type_qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/templates/filters/unknown_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/wrong-template.jinja
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3484 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_all.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.631356 xmlschema-2.3.1/tests/test_cases/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.622356 xmlschema-2.3.1/tests/test_cases/examples/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.632356 xmlschema-2.3.1/tests/test_cases/examples/collection/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection-default.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2023-06-14 06:39:51.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection3bis.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection3bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection4.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection5.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.632356 xmlschema-2.3.1/tests/test_cases/examples/stockquote/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquote.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.634356 xmlschema-2.3.1/tests/test_cases/examples/vehicles/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/bikes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/cars.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-1_error.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-3_errors.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-max.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles2.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles2.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.622356 xmlschema-2.3.1/tests/test_cases/features/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.634356 xmlschema-2.3.1/tests/test_cases/features/attributes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/attributes/default_attributes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.634356 xmlschema-2.3.1/tests/test_cases/features/builtins/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/builtins/builtins.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/builtins/builtins.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.635356 xmlschema-2.3.1/tests/test_cases/features/decoder/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/data.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/data2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/data3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/data4-mixed.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/long-sequence-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/mixed-content.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/simple-types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.635356 xmlschema-2.3.1/tests/test_cases/features/derivations/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/complex-extensions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/complex11-restrictions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-restrictions1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-restrictions2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/list_types.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/list_types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.636356 xmlschema-2.3.1/tests/test_cases/features/elements/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/elements/test_alternatives-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/elements/type_alternatives.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.637356 xmlschema-2.3.1/tests/test_cases/features/models/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/billion_laughs_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/circular_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/illegal-attributes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/illegal-declarations.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/illegal-occurs.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/invalid_models1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/invalid_models2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/model1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-2.3.1/tests/test_cases/features/models/models.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/other-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/recursive-groups.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-2.3.1/tests/test_cases/features/models/valid_model1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.639356 xmlschema-2.3.1/tests/test_cases/features/namespaces/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/chameleon1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/chameleon2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/chameleon3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/default_ns_invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/default_ns_valid1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/default_ns_valid2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case5a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case5b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case5c.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case1bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case2bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case5.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case6.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/included3-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/included4-invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/included5-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/included6-invalid.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.640356 xmlschema-2.3.1/tests/test_cases/features/patterns/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/patterns/patterns.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-2.3.1/tests/test_cases/features/patterns/patterns.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.640356 xmlschema-2.3.1/tests/test_cases/features/wsdl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/tests/test_cases/issues/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.641356 xmlschema-2.3.1/tests/test_cases/issues/issue_008/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_008/issue_008.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_008/issue_008.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.641356 xmlschema-2.3.1/tests/test_cases/issues/issue_009/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_009/issue_009.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.641356 xmlschema-2.3.1/tests/test_cases/issues/issue_013/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.641356 xmlschema-2.3.1/tests/test_cases/issues/issue_014/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_014/issue014.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.641356 xmlschema-2.3.1/tests/test_cases/issues/issue_018/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_018/issue_018-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_018/issue_018.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.642356 xmlschema-2.3.1/tests/test_cases/issues/issue_022/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_022/README.md
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_022/xml_string_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_022/xml_string_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_022/xsd_string.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.642356 xmlschema-2.3.1/tests/test_cases/issues/issue_026/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_026/issue_026-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_026/issue_026-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_026/issue_026-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_026/issue_026.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.642356 xmlschema-2.3.1/tests/test_cases/issues/issue_028/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_028/issue_028-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_028/issue_028-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_028/issue_028.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.643356 xmlschema-2.3.1/tests/test_cases/issues/issue_029/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_029/issue_029-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_029/issue_029-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_029/issue_029-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_029/issue_029.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.643356 xmlschema-2.3.1/tests/test_cases/issues/issue_035/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_035/dates.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_035/dates.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.643356 xmlschema-2.3.1/tests/test_cases/issues/issue_041/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_041/issue_041.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_041/issue_041.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.643356 xmlschema-2.3.1/tests/test_cases/issues/issue_045/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_045/issue_045.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.643356 xmlschema-2.3.1/tests/test_cases/issues/issue_046/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_046/issue_046.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_046/issue_046.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_051/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_051/issue_051.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_051/issue_051.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_073/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_073/issue_073-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_073/issue_073-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_073/issue_073.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_086/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_086/issue_086-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_086/issue_086-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_086/issue_086.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_105/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_105/issue_105.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_111/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_111/issue_111.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_115/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_115/Rotation.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.645356 xmlschema-2.3.1/tests/test_cases/issues/issue_171/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_171/issue_171.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_171/issue_171b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_171/issue_171c.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.645356 xmlschema-2.3.1/tests/test_cases/issues/issue_187/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_187/issue_187_1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_187/issue_187_2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.645356 xmlschema-2.3.1/tests/test_cases/issues/issue_190/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_190/issue_190.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_190/issue_190.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.645356 xmlschema-2.3.1/tests/test_cases/issues/issue_200/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_200/issue_200.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_200/issue_200.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.646356 xmlschema-2.3.1/tests/test_cases/issues/issue_203/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_203/issue_203.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_203/issue_203.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_203/issue_203alt.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.646356 xmlschema-2.3.1/tests/test_cases/issues/issue_204/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_204/issue_204.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_204/issue_204_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_204/issue_204_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_204/issue_204_3.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.646356 xmlschema-2.3.1/tests/test_cases/issues/issue_208/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_208/issue_208.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_208/issue_208.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.646356 xmlschema-2.3.1/tests/test_cases/issues/issue_222/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_222/issue_222.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_222/issue_222.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.646356 xmlschema-2.3.1/tests/test_cases/issues/issue_223/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_223/issue_223.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_223/issue_223.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.624356 xmlschema-2.3.1/tests/test_cases/issues/issue_237/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.647356 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.647356 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.647356 xmlschema-2.3.1/tests/test_cases/issues/issue_243/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_243/issue_243.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_243/issue_243.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.647356 xmlschema-2.3.1/tests/test_cases/issues/issue_245/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.648356 xmlschema-2.3.1/tests/test_cases/issues/issue_259/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_259/issue_259-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_259/issue_259-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.648356 xmlschema-2.3.1/tests/test_cases/issues/issue_265/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_265/issue_265-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.648356 xmlschema-2.3.1/tests/test_cases/issues/issue_266/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-2.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266b-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266b-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.649356 xmlschema-2.3.1/tests/test_cases/issues/issue_273/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_273/issue_273.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_273/issue_273.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.649356 xmlschema-2.3.1/tests/test_cases/issues/issue_276/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_276/dummy.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_276/schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.649356 xmlschema-2.3.1/tests/test_cases/issues/issue_298/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_298/issue_298-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_298/issue_298-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_298/issue_298.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.649356 xmlschema-2.3.1/tests/test_cases/issues/issue_306/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306-alt.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306-invalid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306-valid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.650356 xmlschema-2.3.1/tests/test_cases/issues/issue_311/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_311/correct_no_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_311/incorrect_with_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.650356 xmlschema-2.3.1/tests/test_cases/issues/issue_314/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_314/issue_314.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_314/issue_314.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.651356 xmlschema-2.3.1/tests/test_cases/issues/issue_315/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315-3.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315-4.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315-5.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315_simple.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.651356 xmlschema-2.3.1/tests/test_cases/issues/issue_322/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_322/issue_322.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_322/issue_322.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.651356 xmlschema-2.3.1/tests/test_cases/issues/issue_324/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324-invalid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324b.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.652356 xmlschema-2.3.1/tests/test_cases/issues/issue_334/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.zip
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.652356 xmlschema-2.3.1/tests/test_cases/issues/issue_341/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_341/issue_341-ext.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_341/issue_341.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_341/issue_341.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.652356 xmlschema-2.3.1/tests/test_cases/issues/issue_349/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      329 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_349/issue_349.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      574 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_349/issue_349.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.652356 xmlschema-2.3.1/tests/test_cases/mypy/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-2.3.1/tests/test_cases/mypy/extra_validator.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-2.3.1/tests/test_cases/mypy/schema_source.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-2.3.1/tests/test_cases/mypy/simple_types.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.653356 xmlschema-2.3.1/tests/test_cases/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/dummy file #2.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/dummy file.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/malformed.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/resources/unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/unused_external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/resources/unused_unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/with_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6534 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/test_cases/testfiles
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11973 2021-03-04 20:38:45.000000 xmlschema-2.3.1/tests/test_cli.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-2.3.1/tests/test_codegen.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28857 2022-08-26 15:33:28.000000 xmlschema-2.3.1/tests/test_converters.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26556 2023-02-06 08:55:27.000000 xmlschema-2.3.1/tests/test_dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24557 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/test_documents.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-2.3.1/tests/test_files.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    26065 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_helpers.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5745 2021-12-08 22:11:41.000000 xmlschema-2.3.1/tests/test_memory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9099 2023-02-11 10:41:50.000000 xmlschema-2.3.1/tests/test_namespaces.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-03-05 21:16:57.000000 xmlschema-2.3.1/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    70653 2023-02-06 06:20:42.000000 xmlschema-2.3.1/tests/test_resources.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-2.3.1/tests/test_schemas.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3600 2022-05-20 20:00:14.000000 xmlschema-2.3.1/tests/test_translations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2101 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/test_typing.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-2.3.1/tests/test_validation.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    27317 2023-06-12 10:20:33.000000 xmlschema-2.3.1/tests/test_w3c_suite.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2023-02-11 10:41:50.000000 xmlschema-2.3.1/tests/test_xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.653356 xmlschema-2.3.1/tests/validation/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.3.1/tests/validation/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    66088 2023-04-14 13:49:05.000000 xmlschema-2.3.1/tests/validation/test_decoding.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    33339 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validation/test_encoding.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17401 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/validation/test_validation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.655356 xmlschema-2.3.1/tests/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.3.1/tests/validators/__init__.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-2.3.1/tests/validators/test_builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33116 2023-03-05 20:30:24.000000 xmlschema-2.3.1/tests/validators/test_complex_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-2.3.1/tests/validators/test_elements.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     9464 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_exceptions.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60271 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_facets.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2022-03-07 13:26:41.000000 xmlschema-2.3.1/tests/validators/test_global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13500 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/validators/test_groups.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19187 2023-02-06 06:20:42.000000 xmlschema-2.3.1/tests/validators/test_identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    52697 2023-04-14 13:49:05.000000 xmlschema-2.3.1/tests/validators/test_models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_notations.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41506 2022-10-01 13:42:01.000000 xmlschema-2.3.1/tests/validators/test_schemas.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_simple_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_wildcards.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    33897 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1569 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.656356 xmlschema-2.3.1/xmlschema/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2857 2023-06-14 07:04:00.000000 xmlschema-2.3.1/xmlschema/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5515 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/aliases.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11669 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/cli.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.658356 xmlschema-2.3.1/xmlschema/converters/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      813 2022-07-18 14:19:15.000000 xmlschema-2.3.1/xmlschema/converters/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5977 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/abdera.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7228 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/badgerfish.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7587 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/columnar.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19819 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/default.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4769 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/jsonml.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5840 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/parker.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5711 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/unordered.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23717 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35730 2023-06-14 07:04:00.000000 xmlschema-2.3.1/xmlschema/documents.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-2.3.1/xmlschema/exceptions.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.658356 xmlschema-2.3.1/xmlschema/extras/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-2.3.1/xmlschema/extras/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    21930 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/extras/codegen.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/xmlschema/extras/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.658356 xmlschema-2.3.1/xmlschema/extras/templates/python/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-2.3.1/xmlschema/extras/templates/python/bindings.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-2.3.1/xmlschema/extras/templates/python/sample.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24454 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/extras/wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11097 2022-08-26 15:33:28.000000 xmlschema-2.3.1/xmlschema/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-2.3.1/xmlschema/limits.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/xmlschema/locale/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/xmlschema/locale/en/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.658356 xmlschema-2.3.1/xmlschema/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-2.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    64464 2022-05-20 20:00:14.000000 xmlschema-2.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/xmlschema/locale/it/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.658356 xmlschema-2.3.1/xmlschema/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-2.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-2.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/xmlschema/locale/ru/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.659356 xmlschema-2.3.1/xmlschema/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-2.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-2.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8827 2020-12-23 12:38:37.000000 xmlschema-2.3.1/xmlschema/names.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9907 2023-02-04 20:00:06.000000 xmlschema-2.3.1/xmlschema/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-2.3.1/xmlschema/py.typed
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    55658 2023-04-14 13:49:05.000000 xmlschema-2.3.1/xmlschema/resources.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.626356 xmlschema-2.3.1/xmlschema/schemas/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.659356 xmlschema-2.3.1/xmlschema/schemas/HFP/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.659356 xmlschema-2.3.1/xmlschema/schemas/VC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/VC/XMLSchema-versioning.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.659356 xmlschema-2.3.1/xmlschema/schemas/WSDL/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/WSDL/soap-encoding.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/WSDL/soap-envelope.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/WSDL/wsdl-soap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/WSDL/wsdl.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.659356 xmlschema-2.3.1/xmlschema/schemas/XHTML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XHTML/xhtml1-strict.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.660356 xmlschema-2.3.1/xmlschema/schemas/XLINK/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XLINK/xlink.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.660356 xmlschema-2.3.1/xmlschema/schemas/XML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XML/xml_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.660356 xmlschema-2.3.1/xmlschema/schemas/XSD_1.0/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-2.3.1/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XSD_1.0/datatypes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.660356 xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/datatypes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.660356 xmlschema-2.3.1/xmlschema/schemas/XSI/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.661356 xmlschema-2.3.1/xmlschema/testing/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2116 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/testing/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30214 2023-06-14 07:04:00.000000 xmlschema-2.3.1/xmlschema/testing/_builders.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7950 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/testing/_case_class.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/testing/_factory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6911 2022-09-08 10:16:11.000000 xmlschema-2.3.1/xmlschema/testing/_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4891 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/testing/_observers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-2.3.1/xmlschema/translation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.663356 xmlschema-2.3.1/xmlschema/validators/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3557 2021-11-11 15:30:24.000000 xmlschema-2.3.1/xmlschema/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6619 2023-05-07 06:35:13.000000 xmlschema-2.3.1/xmlschema/validators/assertions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34132 2022-09-24 15:52:22.000000 xmlschema-2.3.1/xmlschema/validators/attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-2.3.1/xmlschema/validators/builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    46791 2023-05-07 06:33:55.000000 xmlschema-2.3.1/xmlschema/validators/complex_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    64310 2023-06-14 07:04:00.000000 xmlschema-2.3.1/xmlschema/validators/elements.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14970 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/validators/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31723 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/validators/facets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33050 2023-06-10 06:00:33.000000 xmlschema-2.3.1/xmlschema/validators/global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    63815 2023-06-14 07:04:00.000000 xmlschema-2.3.1/xmlschema/validators/groups.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     6655 2022-05-20 16:16:20.000000 xmlschema-2.3.1/xmlschema/validators/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    18740 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/validators/identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23474 2023-04-14 13:49:05.000000 xmlschema-2.3.1/xmlschema/validators/models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-2.3.1/xmlschema/validators/notations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6684 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/validators/particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)   103598 2023-06-09 17:48:42.000000 xmlschema-2.3.1/xmlschema/validators/schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    61468 2023-05-08 10:45:15.000000 xmlschema-2.3.1/xmlschema/validators/simple_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38290 2022-09-25 07:58:42.000000 xmlschema-2.3.1/xmlschema/validators/wildcards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41151 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/validators/xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13135 2023-02-11 10:41:50.000000 xmlschema-2.3.1/xmlschema/xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.657356 xmlschema-2.3.1/xmlschema.egg-info/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7377 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/PKG-INFO
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    17217 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/entry_points.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/requires.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/top_level.txt
```

### Comparing `xmlschema-2.3.0/CHANGELOG.rst` & `xmlschema-2.3.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v2.3.1`_ (2023-06-14)
+======================
+* Meta-schema elements and groups ignore xsi:type attributes (issue #350)
+* Use the meta-schemas only for validating XSD sources otherwise create dummy schemas
+
 `v2.3.0`_ (2023-05-18)
 ======================
 * Improve sequence/all restriction checks for XSD 1.1
 * Add *schema* argument to `Wsdl11Document`
 
 `v2.2.3`_ (2023-04-14)
 ======================
@@ -618,7 +623,8 @@
 .. _v2.1.0: https://github.com/brunato/xmlschema/compare/v2.0.4...v2.1.0
 .. _v2.1.1: https://github.com/brunato/xmlschema/compare/v2.1.0...v2.1.1
 .. _v2.2.0: https://github.com/brunato/xmlschema/compare/v2.1.1...v2.2.0
 .. _v2.2.1: https://github.com/brunato/xmlschema/compare/v2.2.0...v2.2.1
 .. _v2.2.2: https://github.com/brunato/xmlschema/compare/v2.2.1...v2.2.2
 .. _v2.2.3: https://github.com/brunato/xmlschema/compare/v2.2.2...v2.2.3
 .. _v2.3.0: https://github.com/brunato/xmlschema/compare/v2.2.3...v2.3.0
+.. _v2.3.1: https://github.com/brunato/xmlschema/compare/v2.3.0...v2.3.1
```

### Comparing `xmlschema-2.3.0/LICENSE` & `xmlschema-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/PKG-INFO` & `xmlschema-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 2.3.0
+Version: 2.3.1
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-2.3.0/README.rst` & `xmlschema-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/doc/Makefile` & `xmlschema-2.3.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/doc/api.rst` & `xmlschema-2.3.1/doc/api.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/doc/components.rst` & `xmlschema-2.3.1/doc/components.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/doc/conf.py` & `xmlschema-2.3.1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '2.3'
 # The full version, including alpha/beta/rc tags.
-release = '2.3.0'
+release = '2.3.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 # language = None
```

### Comparing `xmlschema-2.3.0/doc/converters.rst` & `xmlschema-2.3.1/doc/converters.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/doc/extras.rst` & `xmlschema-2.3.1/doc/extras.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/doc/features.rst` & `xmlschema-2.3.1/doc/features.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/doc/testing.rst` & `xmlschema-2.3.1/doc/testing.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/doc/usage.rst` & `xmlschema-2.3.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/setup.py` & `xmlschema-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with Path(__file__).parent.joinpath('README.rst').open() as readme:
     long_description = readme.read()
 
 
 setup(
     name='xmlschema',
-    version='2.3.0',
+    version='2.3.1',
     packages=find_packages(include=['xmlschema*']),
     package_data={
         'xmlschema': ['py.typed', 'locale/**/*.mo', 'locale/**/*.po', 'schemas/*/*.xsd'],
         'xmlschema.extras': ['templates/*/*.jinja'],
     },
     entry_points={
         'console_scripts': [
```

### Comparing `xmlschema-2.3.0/tests/check_memory.py` & `xmlschema-2.3.1/tests/check_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_all.py` & `xmlschema-2.3.1/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection-1_error.xml` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection-1_error.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection-default.xml` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection-default.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection.py` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection.xml` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection.xsd` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection2.xml` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection2.xsd` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection3.xml` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection3.xsd` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection3bis.xml` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection3bis.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection3bis.xsd` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection3bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection4.xml` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection4.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection4.xsd` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection4.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/collection/collection5.xsd` & `xmlschema-2.3.1/tests/test_cases/examples/collection/collection5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquote.wsdl` & `xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquote.xsd` & `xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl` & `xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/vehicles/invalid.xsd` & `xmlschema-2.3.1/tests/test_cases/examples/vehicles/invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-max.xsd` & `xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-max.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip` & `xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles.xsd` & `xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd` & `xmlschema-2.3.1/tests/test_cases/features/attributes/default_attributes-missing_group.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/attributes/default_attributes.xsd` & `xmlschema-2.3.1/tests/test_cases/features/attributes/default_attributes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/builtins/builtins.xml` & `xmlschema-2.3.1/tests/test_cases/features/builtins/builtins.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/builtins/builtins.xsd` & `xmlschema-2.3.1/tests/test_cases/features/builtins/builtins.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/decoder/data.xml` & `xmlschema-2.3.1/tests/test_cases/features/decoder/data.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/decoder/data2.xml` & `xmlschema-2.3.1/tests/test_cases/features/decoder/data2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/decoder/data3.xml` & `xmlschema-2.3.1/tests/test_cases/features/decoder/data3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/decoder/long-sequence-1.xsd` & `xmlschema-2.3.1/tests/test_cases/features/decoder/long-sequence-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/decoder/mixed-content.xsd` & `xmlschema-2.3.1/tests/test_cases/features/decoder/mixed-content.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/decoder/simple-types.xsd` & `xmlschema-2.3.1/tests/test_cases/features/decoder/simple-types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/derivations/complex-extensions.xsd` & `xmlschema-2.3.1/tests/test_cases/features/derivations/complex-extensions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd` & `xmlschema-2.3.1/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/derivations/complex11-restrictions.xsd` & `xmlschema-2.3.1/tests/test_cases/features/derivations/complex11-restrictions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd` & `xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd` & `xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-restrictions1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd` & `xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-restrictions2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/derivations/list_types.xsd` & `xmlschema-2.3.1/tests/test_cases/features/derivations/list_types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd` & `xmlschema-2.3.1/tests/test_cases/features/elements/type_alternatives-no-ns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/elements/type_alternatives.xsd` & `xmlschema-2.3.1/tests/test_cases/features/elements/type_alternatives.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/models/billion_laughs_model.xsd` & `xmlschema-2.3.1/tests/test_cases/features/models/billion_laughs_model.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/models/illegal-declarations.xsd` & `xmlschema-2.3.1/tests/test_cases/features/models/illegal-declarations.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/models/illegal-occurs.xsd` & `xmlschema-2.3.1/tests/test_cases/features/models/illegal-occurs.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/models/invalid_models1.xsd` & `xmlschema-2.3.1/tests/test_cases/features/models/invalid_models1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/models/invalid_models2.xsd` & `xmlschema-2.3.1/tests/test_cases/features/models/invalid_models2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/models/models.xsd` & `xmlschema-2.3.1/tests/test_cases/features/models/models.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/models/recursive-groups.xsd` & `xmlschema-2.3.1/tests/test_cases/features/models/recursive-groups.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/models/valid_model1.xsd` & `xmlschema-2.3.1/tests/test_cases/features/models/valid_model1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case1.xsd` & `xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case2.xsd` & `xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4a.xsd` & `xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4a.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4b.xsd` & `xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case2.xsd` & `xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case2bis.xsd` & `xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case2bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case3.xsd` & `xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case5.xsd` & `xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/patterns/patterns.xml` & `xmlschema-2.3.1/tests/test_cases/features/patterns/patterns.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/patterns/patterns.xsd` & `xmlschema-2.3.1/tests/test_cases/features/patterns/patterns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl` & `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl` & `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl` & `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl` & `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example4.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl` & `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl` & `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl` & `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl` & `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_008/issue_008.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_008/issue_008.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013-1.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_014/issue014.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_014/issue014.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_018/issue_018.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_018/issue_018.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_022/README.md` & `xmlschema-2.3.1/tests/test_cases/issues/issue_022/README.md`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_022/xsd_string.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_022/xsd_string.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_026/issue_026.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_026/issue_026.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_035/dates.xml` & `xmlschema-2.3.1/tests/test_cases/issues/issue_035/dates.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_035/dates.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_035/dates.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_041/issue_041.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_041/issue_041.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_051/issue_051.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_051/issue_051.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_073/issue_073.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_073/issue_073.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_086/issue_086.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_086/issue_086.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_105/issue_105.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_105/issue_105.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_111/issue_111.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_111/issue_111.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_115/Rotation.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_115/Rotation.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_171/issue_171.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_171/issue_171.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_171/issue_171b.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_171/issue_171b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_187/issue_187_1.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_187/issue_187_1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_187/issue_187_2.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_187/issue_187_2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_190/issue_190.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_190/issue_190.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_200/issue_200.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_200/issue_200.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_203/issue_203.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_203/issue_203.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_203/issue_203alt.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_203/issue_203alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_204/issue_204.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_204/issue_204.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_208/issue_208.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_208/issue_208.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_222/issue_222.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_222/issue_222.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl` & `xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl` & `xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_243/issue_243.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_243/issue_243.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245-valid.xml` & `xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245-valid.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245.xml` & `xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_259/issue_259-1.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_259/issue_259-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_259/issue_259-2.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_259/issue_259-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_265/issue_265-1.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_265/issue_265-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-1.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-2.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266b-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266b-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_273/issue_273.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_273/issue_273.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_298/issue_298.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_298/issue_298.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306-alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_311/correct_no_list.xml` & `xmlschema-2.3.1/tests/test_cases/issues/issue_311/correct_no_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml` & `xmlschema-2.3.1/tests/test_cases/issues/issue_311/incorrect_with_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_314/issue_314.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_314/issue_314.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315_mixed.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324.zip` & `xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.xml` & `xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.zip` & `xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_341/issue_341-ext.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/issues/issue_341/issue_341.xsd` & `xmlschema-2.3.1/tests/test_cases/issues/issue_341/issue_341.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/mypy/extra_validator.py` & `xmlschema-2.3.1/tests/test_cases/mypy/extra_validator.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/mypy/schema_source.py` & `xmlschema-2.3.1/tests/test_cases/mypy/schema_source.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/mypy/simple_types.py` & `xmlschema-2.3.1/tests/test_cases/mypy/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_cases/testfiles` & `xmlschema-2.3.1/tests/test_cases/testfiles`

 * *Files 2% similar despite different names*

```diff
@@ -143,7 +143,9 @@
 issues/issue_298/issue_298-2.xml -L 'http://xmlschema.test/ns' issue_298.xsd
 issues/issue_306/issue_306.xsd
 issues/issue_306/issue_306-alt.xsd
 issues/issue_311/correct_no_list.xml --version=1.1 --validation-only \
     -L 'http://www.ludd21.com/kPartModel' kPartModel_reduit_issue.xsd
 issues/issue_311/incorrect_with_list.xml --version=1.1 --validation-only \
     -L 'http://www.ludd21.com/kPartModel' kPartModel_reduit_issue.xsd
+issues/issue_349/issue_349.xml --errors=1 --validation-only
+issues/issue_349/issue_349.xml --version=1.1
```

### Comparing `xmlschema-2.3.0/tests/test_cli.py` & `xmlschema-2.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_codegen.py` & `xmlschema-2.3.1/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_converters.py` & `xmlschema-2.3.1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_dataobjects.py` & `xmlschema-2.3.1/tests/test_dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_documents.py` & `xmlschema-2.3.1/tests/test_documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     def test_get_context_without_schema(self):
         xml_data = '<text xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"\n' \
                    '      xmlns:xs="http://www.w3.org/2001/XMLSchema"\n' \
                    '      xsi:type="xs:string">foo</text>'
 
         source, schema = get_context(xml_data)
         self.assertIsInstance(source, XMLResource)
-        self.assertIs(schema, XMLSchema10.meta_schema)
+        self.assertIsNot(schema, XMLSchema10.meta_schema)
         self.assertEqual(source.root.tag, 'text')
         self.assertTrue(schema.is_valid(source))
 
         with self.assertRaises(ValueError) as ctx:
             get_context('<empty/>')
         self.assertEqual(str(ctx.exception),
                          "cannot get a schema for XML data, provide a schema argument")
```

### Comparing `xmlschema-2.3.0/tests/test_files.py` & `xmlschema-2.3.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_helpers.py` & `xmlschema-2.3.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_memory.py` & `xmlschema-2.3.1/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_namespaces.py` & `xmlschema-2.3.1/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_package.py` & `xmlschema-2.3.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_resources.py` & `xmlschema-2.3.1/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_schemas.py` & `xmlschema-2.3.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_translations.py` & `xmlschema-2.3.1/tests/test_translations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_typing.py` & `xmlschema-2.3.1/tests/test_typing.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 """Tests about static typing of xmlschema objects."""
 
 import unittest
 import importlib
+import sys
 from pathlib import Path
 
 try:
     from mypy import api as mypy_api
 except ImportError:
     mypy_api = None
 
@@ -23,14 +24,15 @@
     lxml_stubs_module = importlib.import_module('lxml-stubs')
 except ImportError:
     lxml_stubs_module = None
 
 
 @unittest.skipIf(mypy_api is None, "mypy is not installed")
 @unittest.skipIf(lxml_stubs_module is None, "lxml-stubs is not installed")
+@unittest.skipIf(sys.version_info < (3, 8), "Python version < 3.8")
 class TestTyping(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.cases_dir = Path(__file__).parent.joinpath('test_cases/mypy')
         cls.config_file = Path(__file__).parent.parent.joinpath('mypy.ini')
```

### Comparing `xmlschema-2.3.0/tests/test_validation.py` & `xmlschema-2.3.1/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_w3c_suite.py` & `xmlschema-2.3.1/tests/test_w3c_suite.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_wsdl.py` & `xmlschema-2.3.1/tests/test_wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/test_xpath.py` & `xmlschema-2.3.1/tests/test_xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validation/test_decoding.py` & `xmlschema-2.3.1/tests/validation/test_decoding.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validation/test_encoding.py` & `xmlschema-2.3.1/tests/validation/test_encoding.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validation/test_validation.py` & `xmlschema-2.3.1/tests/validation/test_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -324,14 +324,41 @@
 
         with open(self.col_xml_file, 'rb') as fp:
             col_xml_data = fp.read()
 
         self.assertIsInstance(col_xml_data, bytes)
         self.assertTrue(self.col_schema.is_valid(col_xml_data))
 
+    def test_issue_350__ignore_xsi_type_for_schema_validation(self):
+        schema = xmlschema.XMLSchema(dedent("""\
+            <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema"
+                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
+
+                <xs:element name="root" xsi:type="non-empty-string" />
+
+                <xs:simpleType name="non-empty-string">
+                  <xs:restriction base="xs:string">
+                    <xs:minLength value="1" />
+                  </xs:restriction>
+                </xs:simpleType>
+
+            </xs:schema>"""))
+
+        self.assertTrue(schema.is_valid('<root></root>'))
+        self.assertTrue(schema.is_valid('<root>foo</root>'))
+
+        self.assertFalse(schema.is_valid(
+            '<root xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+            'xsi:type="non-empty-string"></root>'
+        ))
+        self.assertTrue(schema.is_valid(
+            '<root xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+            'xsi:type="non-empty-string">foo</root>'
+        ))
+
 
 class TestValidation11(TestValidation):
     schema_class = XMLSchema11
 
     def test_default_attributes(self):
         xs = self.schema_class(self.casepath('features/attributes/default_attributes.xsd'))
         self.assertTrue(xs.is_valid("<tree xmlns='ns'>\n"
```

### Comparing `xmlschema-2.3.0/tests/validators/test_attributes.py` & `xmlschema-2.3.1/tests/validators/test_attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_builtins.py` & `xmlschema-2.3.1/tests/validators/test_builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_complex_types.py` & `xmlschema-2.3.1/tests/validators/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_elements.py` & `xmlschema-2.3.1/tests/validators/test_elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_exceptions.py` & `xmlschema-2.3.1/tests/validators/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_facets.py` & `xmlschema-2.3.1/tests/validators/test_facets.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_global_maps.py` & `xmlschema-2.3.1/tests/validators/test_global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_groups.py` & `xmlschema-2.3.1/tests/validators/test_groups.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_identities.py` & `xmlschema-2.3.1/tests/validators/test_identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_models.py` & `xmlschema-2.3.1/tests/validators/test_models.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_notations.py` & `xmlschema-2.3.1/tests/validators/test_notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_particles.py` & `xmlschema-2.3.1/tests/validators/test_particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_schemas.py` & `xmlschema-2.3.1/tests/validators/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_simple_types.py` & `xmlschema-2.3.1/tests/validators/test_simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_wildcards.py` & `xmlschema-2.3.1/tests/validators/test_wildcards.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tests/validators/test_xsdbase.py` & `xmlschema-2.3.1/tests/validators/test_xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/tox.ini` & `xmlschema-2.3.1/tox.ini`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/__init__.py` & `xmlschema-2.3.1/xmlschema/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     XMLSchemaModelError, XMLSchemaModelDepthError, XMLSchemaValidationError,
     XMLSchemaDecodeError, XMLSchemaEncodeError, XMLSchemaChildrenValidationError,
     XMLSchemaIncludeWarning, XMLSchemaImportWarning, XMLSchemaTypeTableWarning,
     XsdGlobals, XMLSchemaBase, XMLSchema, XMLSchema10, XMLSchema11,
     XsdComponent, XsdType, XsdElement, XsdAttribute
 )
 
-__version__ = '2.3.0'
+__version__ = '2.3.1'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2016-2023, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 __all__ = [
```

### Comparing `xmlschema-2.3.0/xmlschema/aliases.py` & `xmlschema-2.3.1/xmlschema/aliases.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/cli.py` & `xmlschema-2.3.1/xmlschema/cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/converters/__init__.py` & `xmlschema-2.3.1/xmlschema/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/converters/abdera.py` & `xmlschema-2.3.1/xmlschema/converters/abdera.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/converters/badgerfish.py` & `xmlschema-2.3.1/xmlschema/converters/badgerfish.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/converters/columnar.py` & `xmlschema-2.3.1/xmlschema/converters/columnar.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/converters/default.py` & `xmlschema-2.3.1/xmlschema/converters/default.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/converters/jsonml.py` & `xmlschema-2.3.1/xmlschema/converters/jsonml.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/converters/parker.py` & `xmlschema-2.3.1/xmlschema/converters/parker.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/converters/unordered.py` & `xmlschema-2.3.1/xmlschema/converters/unordered.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/dataobjects.py` & `xmlschema-2.3.1/xmlschema/dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/documents.py` & `xmlschema-2.3.1/xmlschema/documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,18 +70,18 @@
             kwargs = dict(locations=locations, defuse=defuse, timeout=timeout)
             if schema is None or isinstance(schema, XMLSchemaBase):
                 return resource, cls(schema_location, **kwargs)
             else:
                 return resource, cls(schema, **kwargs)
 
     if schema is None:
-        if cls.meta_schema is not None and \
-                (XSI_TYPE in resource.root.attrib or XSD_NAMESPACE in resource.namespace):
+        if XSD_NAMESPACE == resource.namespace:
+            assert cls.meta_schema is not None
             return resource, cls.meta_schema
-        elif dummy_schema:
+        elif dummy_schema or XSI_TYPE in resource.root.attrib:
             return resource, get_dummy_schema(resource.root.tag, cls)
         else:
             msg = "cannot get a schema for XML data, provide a schema argument"
             raise XMLSchemaValueError(msg)
 
     elif isinstance(schema, XMLSchemaBase):
         return resource, schema
@@ -598,20 +598,20 @@
                         allow=allow,
                         defuse=defuse,
                         timeout=timeout,
                     )
 
             if self.schema is None:
                 if XSI_TYPE in self._root.attrib:
-                    self.schema = cls.meta_schema
+                    self.schema = get_dummy_schema(self._root.tag, cls)
                 elif validation != 'skip':
                     msg = "cannot get a schema for XML data, provide a schema argument"
                     raise XMLSchemaValueError(msg)
                 else:
-                    self._fallback_schema = get_dummy_schema(self.root.tag, cls)
+                    self._fallback_schema = get_dummy_schema(self._root.tag, cls)
 
         if self.schema is None:
             pass
         elif validation == 'strict':
             self.schema.validate(self, namespaces=self.namespaces)
         elif validation == 'lax':
             self.errors = [e for e in self.schema.iter_errors(self, namespaces=self.namespaces)]
```

### Comparing `xmlschema-2.3.0/xmlschema/exceptions.py` & `xmlschema-2.3.1/xmlschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/extras/codegen.py` & `xmlschema-2.3.1/xmlschema/extras/codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/extras/templates/python/bindings.py.jinja` & `xmlschema-2.3.1/xmlschema/extras/templates/python/bindings.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/extras/templates/python/sample.py.jinja` & `xmlschema-2.3.1/xmlschema/extras/templates/python/sample.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/extras/wsdl.py` & `xmlschema-2.3.1/xmlschema/extras/wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/helpers.py` & `xmlschema-2.3.1/xmlschema/helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/limits.py` & `xmlschema-2.3.1/xmlschema/limits.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po` & `xmlschema-2.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po` & `xmlschema-2.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po` & `xmlschema-2.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/names.py` & `xmlschema-2.3.1/xmlschema/names.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/namespaces.py` & `xmlschema-2.3.1/xmlschema/namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/resources.py` & `xmlschema-2.3.1/xmlschema/resources.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd` & `xmlschema-2.3.1/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd` & `xmlschema-2.3.1/xmlschema/schemas/VC/XMLSchema-versioning.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/WSDL/soap-encoding.xsd` & `xmlschema-2.3.1/xmlschema/schemas/WSDL/soap-encoding.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/WSDL/soap-envelope.xsd` & `xmlschema-2.3.1/xmlschema/schemas/WSDL/soap-envelope.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/WSDL/wsdl-soap.xsd` & `xmlschema-2.3.1/xmlschema/schemas/WSDL/wsdl-soap.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/WSDL/wsdl.xsd` & `xmlschema-2.3.1/xmlschema/schemas/WSDL/wsdl.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd` & `xmlschema-2.3.1/xmlschema/schemas/XHTML/xhtml1-strict.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/XLINK/xlink.xsd` & `xmlschema-2.3.1/xmlschema/schemas/XLINK/xlink.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/XML/xml_minimal.xsd` & `xmlschema-2.3.1/xmlschema/schemas/XML/xml_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd` & `xmlschema-2.3.1/xmlschema/schemas/XSD_1.0/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/XSD_1.0/datatypes.xsd` & `xmlschema-2.3.1/xmlschema/schemas/XSD_1.0/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd` & `xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/datatypes.xsd` & `xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd` & `xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/testing/__init__.py` & `xmlschema-2.3.1/xmlschema/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/testing/_builders.py` & `xmlschema-2.3.1/xmlschema/testing/_builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # @author Davide Brunato <brunato@sissa.it>
 #
 # mypy: ignore-errors
 import pdb
 import os
 import ast
 import pickle
+import re
 import time
 import logging
 import importlib
 import tempfile
 import warnings
 from xml.etree import ElementTree
 
@@ -45,14 +46,17 @@
     PythonGenerator = None
 
 from ._helpers import iter_nested_items, etree_elements_assert_equal
 from ._case_class import XsdValidatorTestCase
 from ._observers import SchemaObserver
 
 
+OBJ_ID_PATTERN = re.compile(r" at 0x[0-9a-fA-F]+")
+
+
 def make_schema_test_class(test_file, test_args, test_num, schema_class, check_with_lxml):
     """
     Creates a schema test class.
 
     :param test_file: the schema test file path.
     :param test_args: line arguments for test case.
     :param test_num: a positive integer number associated with the test case.
@@ -538,28 +542,38 @@
                 with self.assertRaises(XMLSchemaValidationError, msg=xml_file):
                     self.schema.validate(xml_file)
             else:
                 self.assertTrue(self.schema.is_valid(xml_file), msg=xml_file)
                 self.assertIsNone(self.schema.validate(xml_file), msg=xml_file)
 
         def check_iter_errors(self):
+            def compare_error_reasons(reason, other_reason):
+                if ' at 0x' in reason:
+                    self.assertEqual(
+                        OBJ_ID_PATTERN.sub(' at 0xff', reason),
+                        OBJ_ID_PATTERN.sub(' at 0xff', other_reason),
+                        msg=xml_file
+                    )
+                else:
+                    self.assertEqual(reason, other_reason, msg=xml_file)
+
             errors = list(self.schema.iter_errors(xml_file))
             for e in errors:
                 self.assertIsInstance(e.reason, str, msg=xml_file)
             self.assertEqual(len(errors), expected_errors, msg=xml_file)
 
             module_api_errors = list(xmlschema.iter_errors(xml_file, schema=self.schema))
             self.assertEqual(len(errors), len(module_api_errors), msg=xml_file)
             for e, api_error in zip(errors, module_api_errors):
-                self.assertEqual(e.reason, api_error.reason, msg=xml_file)
+                compare_error_reasons(e.reason, api_error.reason)
 
             lazy_errors = list(xmlschema.iter_errors(xml_file, schema=self.schema, lazy=True))
             self.assertEqual(len(errors), len(lazy_errors), msg=xml_file)
             for e, lazy_error in zip(errors, lazy_errors):
-                self.assertEqual(e.reason, lazy_error.reason, msg=xml_file)
+                compare_error_reasons(e.reason, lazy_error.reason)
 
             # TODO: Test also lazy validation with lazy=2.
             #  This needs two fixes in XPath:
             #   1) find has to retrieve also element substitutes
             #   2) multiple XSD type match on tokens that have wildcard parent (eg. /root/*/name)
 
         def check_lxml_validation(self):
```

### Comparing `xmlschema-2.3.0/xmlschema/testing/_case_class.py` & `xmlschema-2.3.1/xmlschema/testing/_case_class.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/testing/_factory.py` & `xmlschema-2.3.1/xmlschema/testing/_factory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/testing/_helpers.py` & `xmlschema-2.3.1/xmlschema/testing/_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/testing/_observers.py` & `xmlschema-2.3.1/xmlschema/testing/_observers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/translation.py` & `xmlschema-2.3.1/xmlschema/translation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/__init__.py` & `xmlschema-2.3.1/xmlschema/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/assertions.py` & `xmlschema-2.3.1/xmlschema/validators/assertions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/attributes.py` & `xmlschema-2.3.1/xmlschema/validators/attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/builtins.py` & `xmlschema-2.3.1/xmlschema/validators/builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/complex_types.py` & `xmlschema-2.3.1/xmlschema/validators/complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/elements.py` & `xmlschema-2.3.1/xmlschema/validators/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,15 +653,16 @@
 
         inherited = kwargs.get('inherited')
         value = content = attributes = None
         nilled = False
 
         # Get the instance effective type
         xsd_type = self.get_type(obj, inherited)
-        if XSI_TYPE in obj.attrib:
+        if XSI_TYPE in obj.attrib and self.schema.meta_schema is not None:
+            # Meta-schema elements ignore xsi:type (issue #350)
             type_name = obj.attrib[XSI_TYPE].strip()
             try:
                 xsd_type = self.maps.get_instance_type(type_name, xsd_type, namespaces)
             except (KeyError, TypeError) as err:
                 yield self.validation_error(validation, err, obj, **kwargs)
             else:
                 if self.identities:
@@ -970,15 +971,15 @@
                     return
 
         text = None
         children = element_data.content
         attributes = ()
 
         xsd_type = self.get_type(element_data)
-        if XSI_TYPE in element_data.attributes:
+        if XSI_TYPE in element_data.attributes and self.schema.meta_schema is not None:
             type_name = element_data.attributes[XSI_TYPE].strip()
             try:
                 xsd_type = self.maps.get_instance_type(type_name, xsd_type, converter)
             except (KeyError, TypeError) as err:
                 errors.append(err)
             else:
                 default_namespace = converter.get('')
```

### Comparing `xmlschema-2.3.0/xmlschema/validators/exceptions.py` & `xmlschema-2.3.1/xmlschema/validators/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/facets.py` & `xmlschema-2.3.1/xmlschema/validators/facets.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/global_maps.py` & `xmlschema-2.3.1/xmlschema/validators/global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/groups.py` & `xmlschema-2.3.1/xmlschema/validators/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -800,14 +800,18 @@
         if isinstance(xsd_element, XsdAnyElement):
             if xsd_element.process_contents == 'skip':
                 return
 
             try:
                 xsd_element = self.maps.lookup_element(elem.tag)
             except LookupError:
+                if self.schema.meta_schema is None:
+                    # Meta-schema groups ignore xsi:type (issue #350)
+                    return
+
                 try:
                     type_name = elem.attrib[XSI_TYPE].strip()
                 except KeyError:
                     return
                 else:
                     xsd_type = self.maps.get_instance_type(
                         type_name, self.any_type, namespaces
@@ -820,15 +824,15 @@
                     xsd_type = xsd_element.type
                 else:
                     xsd_type = self.maps.get_instance_type(
                         type_name, xsd_element.type, namespaces
                     )
 
         else:
-            if XSI_TYPE not in elem.attrib:
+            if XSI_TYPE not in elem.attrib or self.schema.meta_schema is None:
                 xsd_type = xsd_element.type
             else:
                 alternatives = xsd_element.alternatives
                 try:
                     type_name = elem.attrib[XSI_TYPE].strip()
                 except KeyError:
                     xsd_type = xsd_element.type
@@ -842,15 +846,15 @@
                 for derivation in model_element.block.split():
                     if xsd_type is not model_element.type and \
                             xsd_type.is_derived(model_element.type, derivation):
                         reason = _("usage of {0!r} with type {1} is blocked by "
                                    "head element").format(xsd_element, derivation)
                         raise XMLSchemaValidationError(self, elem, reason)
 
-            if XSI_TYPE not in elem.attrib:
+            if XSI_TYPE not in elem.attrib or self.schema.meta_schema is None:
                 return
 
         # If it's a restriction the context is the base_type's group
         group = self.restriction if self.restriction is not None else self
 
         # Dynamic EDC check of matched element
         for e in group.iter_elements():
```

### Comparing `xmlschema-2.3.0/xmlschema/validators/helpers.py` & `xmlschema-2.3.1/xmlschema/validators/helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/identities.py` & `xmlschema-2.3.1/xmlschema/validators/identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/models.py` & `xmlschema-2.3.1/xmlschema/validators/models.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/notations.py` & `xmlschema-2.3.1/xmlschema/validators/notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/particles.py` & `xmlschema-2.3.1/xmlschema/validators/particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/schemas.py` & `xmlschema-2.3.1/xmlschema/validators/schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/simple_types.py` & `xmlschema-2.3.1/xmlschema/validators/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/wildcards.py` & `xmlschema-2.3.1/xmlschema/validators/wildcards.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/validators/xsdbase.py` & `xmlschema-2.3.1/xmlschema/validators/xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema/xpath.py` & `xmlschema-2.3.1/xmlschema/xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.0/xmlschema.egg-info/PKG-INFO` & `xmlschema-2.3.1/xmlschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 2.3.0
+Version: 2.3.1
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-2.3.0/xmlschema.egg-info/SOURCES.txt` & `xmlschema-2.3.1/xmlschema.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -276,14 +276,16 @@
 tests/test_cases/issues/issue_324/issue_324b.xsd
 tests/test_cases/issues/issue_334/issue_334.xml
 tests/test_cases/issues/issue_334/issue_334.xsd
 tests/test_cases/issues/issue_334/issue_334.zip
 tests/test_cases/issues/issue_341/issue_341-ext.xsd
 tests/test_cases/issues/issue_341/issue_341.xml
 tests/test_cases/issues/issue_341/issue_341.xsd
+tests/test_cases/issues/issue_349/issue_349.xml
+tests/test_cases/issues/issue_349/issue_349.xsd
 tests/test_cases/mypy/extra_validator.py
 tests/test_cases/mypy/schema_source.py
 tests/test_cases/mypy/simple_types.py
 tests/test_cases/resources/dummy file #2.txt
 tests/test_cases/resources/dummy file.txt
 tests/test_cases/resources/external_entity.xml
 tests/test_cases/resources/malformed.xml
```

