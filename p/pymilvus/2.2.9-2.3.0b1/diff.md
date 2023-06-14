# Comparing `tmp/pymilvus-2.2.9.tar.gz` & `tmp/pymilvus-2.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilvus-2.2.9.tar", last modified: Fri Jun  2 11:00:59 2023, max compression
+gzip compressed data, was "pymilvus-2.3.0b1.tar", last modified: Mon Mar 20 10:23:59 2023, max compression
```

## Comparing `pymilvus-2.2.9.tar` & `pymilvus-2.3.0b1.tar`

### file list

```diff
@@ -1,175 +1,163 @@
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.884827 pymilvus-2.2.9/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      246 2023-05-16 07:00:46.000000 pymilvus-2.2.9/.env.example
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.868826 pymilvus-2.2.9/.github/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.872826 pymilvus-2.2.9/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2045 2023-05-16 07:00:46.000000 pymilvus-2.2.9/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       27 2023-05-16 07:00:46.000000 pymilvus-2.2.9/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1371 2023-05-16 07:00:46.000000 pymilvus-2.2.9/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      633 2023-05-16 07:00:46.000000 pymilvus-2.2.9/.github/ISSUE_TEMPLATE/general-question.yaml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      817 2023-06-02 10:59:50.000000 pymilvus-2.2.9/.github/mergify.yml
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.872826 pymilvus-2.2.9/.github/workflows/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      723 2023-06-02 10:59:50.000000 pymilvus-2.2.9/.github/workflows/check_milvus_proto.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      685 2023-06-02 10:59:50.000000 pymilvus-2.2.9/.github/workflows/code_checker.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      919 2023-05-16 07:00:46.000000 pymilvus-2.2.9/.github/workflows/doc_update_event.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2046 2023-05-16 07:00:46.000000 pymilvus-2.2.9/.github/workflows/nightly_ci.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1067 2023-06-02 10:59:50.000000 pymilvus-2.2.9/.github/workflows/publish_dev_package.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      783 2023-06-02 10:59:50.000000 pymilvus-2.2.9/.github/workflows/pull_request.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      778 2023-05-16 07:00:46.000000 pymilvus-2.2.9/.github/workflows/release_event.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      264 2023-05-16 07:00:46.000000 pymilvus-2.2.9/.gitignore
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      137 2023-05-22 07:05:30.000000 pymilvus-2.2.9/.gitmodules
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4996 2023-05-16 07:00:46.000000 pymilvus-2.2.9/CONTRIBUTING.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4620 2023-05-16 07:00:46.000000 pymilvus-2.2.9/CONTRIBUTING_CN.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       77 2023-05-16 07:00:46.000000 pymilvus-2.2.9/Dockerfile
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11336 2023-04-10 06:47:08.000000 pymilvus-2.2.9/LICENSE
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      552 2023-05-16 07:00:46.000000 pymilvus-2.2.9/Makefile
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      176 2023-05-16 07:00:46.000000 pymilvus-2.2.9/OWNERS
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3916 2023-06-02 11:00:59.884827 pymilvus-2.2.9/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3369 2023-06-02 10:59:50.000000 pymilvus-2.2.9/README.md
--rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1306 2023-05-16 07:00:46.000000 pymilvus-2.2.9/check_proto_product.sh
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.868826 pymilvus-2.2.9/ci/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.868826 pymilvus-2.2.9/ci/docker/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.872826 pymilvus-2.2.9/ci/docker/milvus/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1169 2023-05-16 07:00:46.000000 pymilvus-2.2.9/ci/docker/milvus/docker-compose.yml
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.872826 pymilvus-2.2.9/ci/scripts/
--rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     7597 2023-05-16 07:00:46.000000 pymilvus-2.2.9/ci/scripts/docker_image_find_tag.sh
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.872826 pymilvus-2.2.9/docs/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      638 2022-11-09 07:08:42.000000 pymilvus-2.2.9/docs/Makefile
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1858 2022-11-09 07:08:42.000000 pymilvus-2.2.9/docs/README.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      799 2022-11-09 07:08:42.000000 pymilvus-2.2.9/docs/make.bat
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.872826 pymilvus-2.2.9/docs/source/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.872826 pymilvus-2.2.9/docs/source/_templates/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       97 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/_templates/autosummaryclass.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      389 2022-11-09 07:08:42.000000 pymilvus-2.2.9/docs/source/_templates/layout.html
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      122 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/about.rst
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.872826 pymilvus-2.2.9/docs/source/api/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      169 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/api/api.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8038 2023-06-02 10:59:50.000000 pymilvus-2.2.9/docs/source/api/collection.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3644 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/api/connections.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2580 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/api/future.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2122 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/api/milvus_index.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4010 2023-06-02 10:59:50.000000 pymilvus-2.2.9/docs/source/api/partition.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3199 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/api/schema.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4749 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/api/search.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7557 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/api/utility.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       24 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/changes.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3236 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/conf.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3255 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/contribute.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      575 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/faq.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      931 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/index.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2115 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/install.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       60 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/param.rst
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.872826 pymilvus-2.2.9/docs/source/res/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     9091 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/res/Intro_to_Indexes.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      544 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/res/about_documentation.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1448 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/results.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7429 2023-05-16 07:00:46.000000 pymilvus-2.2.9/docs/source/tutorial.rst
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.876826 pymilvus-2.2.9/examples/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2316 2023-06-01 03:26:50.000000 pymilvus-2.2.9/examples/binary_example.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.876826 pymilvus-2.2.9/examples/cert/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1326 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/cert/ca.pem
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1704 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/cert/client.key
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/cert/client.pem
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/cert/server.pem
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11523 2023-06-02 10:59:50.000000 pymilvus-2.2.9/examples/collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4171 2023-05-26 03:18:53.000000 pymilvus-2.2.9/examples/database.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3269 2023-06-02 10:59:50.000000 pymilvus-2.2.9/examples/dynamic_field.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4302 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/example.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    15138 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/example_bulkinsert.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5512 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/example_index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4437 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/example_str.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4120 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/example_tls1.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4230 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/example_tls2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)  1070736 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/films.csv
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    12007 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/hello_milvus.ipynb
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7380 2023-05-29 02:44:04.000000 pymilvus-2.2.9/examples/hello_milvus.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2690 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/multithreading_hello_milvus.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3452 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/old_style_example.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5612 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/old_style_example_index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3779 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/old_style_example_str.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1874 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/old_style_query.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4676 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/partition.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2977 2023-06-02 10:59:50.000000 pymilvus-2.2.9/examples/resource_group.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7110 2023-05-26 03:18:53.000000 pymilvus-2.2.9/examples/role_and_privilege.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3310 2023-05-16 07:00:46.000000 pymilvus-2.2.9/examples/user.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19554 2023-05-16 07:00:46.000000 pymilvus-2.2.9/pylint.conf
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.876826 pymilvus-2.2.9/pymilvus/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3318 2023-05-26 03:18:53.000000 pymilvus-2.2.9/pymilvus/__init__.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.880826 pymilvus-2.2.9/pymilvus/client/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1790 2023-05-16 07:00:46.000000 pymilvus-2.2.9/pymilvus/client/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    27311 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/client/abstract.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10417 2023-06-01 03:26:50.000000 pymilvus-2.2.9/pymilvus/client/asynch.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      738 2023-05-16 07:00:46.000000 pymilvus-2.2.9/pymilvus/client/blob.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10227 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/client/check.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      283 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/client/constants.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     9303 2023-06-01 03:26:50.000000 pymilvus-2.2.9/pymilvus/client/entity_helper.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    61317 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/client/grpc_handler.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3522 2023-06-01 03:26:50.000000 pymilvus-2.2.9/pymilvus/client/interceptor.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    41717 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/client/prepare.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      355 2023-05-16 07:00:46.000000 pymilvus-2.2.9/pymilvus/client/singleton_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    58708 2023-05-25 07:52:56.000000 pymilvus-2.2.9/pymilvus/client/stub.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3254 2023-06-01 03:26:50.000000 pymilvus-2.2.9/pymilvus/client/ts_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19545 2023-05-26 03:18:53.000000 pymilvus-2.2.9/pymilvus/client/types.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7072 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/client/utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7508 2023-06-01 03:26:50.000000 pymilvus-2.2.9/pymilvus/decorators.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6993 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/exceptions.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.880826 pymilvus-2.2.9/pymilvus/grpc_gen/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    15346 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/grpc_gen/common_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14269 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/grpc_gen/common_pb2.pyi
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    69848 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/grpc_gen/milvus_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    87574 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/grpc_gen/milvus_pb2.pyi
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)   119361 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/grpc_gen/milvus_pb2_grpc.py
--rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1356 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/grpc_gen/python_gen.sh
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7255 2023-05-29 14:14:31.000000 pymilvus-2.2.9/pymilvus/grpc_gen/schema_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10702 2023-05-29 14:14:31.000000 pymilvus-2.2.9/pymilvus/grpc_gen/schema_pb2.pyi
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.880826 pymilvus-2.2.9/pymilvus/milvus_client/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        0 2023-05-23 09:41:28.000000 pymilvus-2.2.9/pymilvus/milvus_client/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      550 2023-05-23 09:41:28.000000 pymilvus-2.2.9/pymilvus/milvus_client/defaults.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    34990 2023-05-25 07:52:56.000000 pymilvus-2.2.9/pymilvus/milvus_client/milvus_client.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11900 2023-05-23 09:41:28.000000 pymilvus-2.2.9/pymilvus/milvus_client/milvus_client_tests.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.884827 pymilvus-2.2.9/pymilvus/orm/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      593 2023-05-16 07:00:46.000000 pymilvus-2.2.9/pymilvus/orm/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    50824 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/orm/collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    17628 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/orm/connections.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      909 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/orm/constants.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1101 2023-05-26 03:18:53.000000 pymilvus-2.2.9/pymilvus/orm/db.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1553 2023-05-16 07:00:46.000000 pymilvus-2.2.9/pymilvus/orm/future.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5650 2023-05-16 07:00:46.000000 pymilvus-2.2.9/pymilvus/orm/index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1887 2023-05-16 07:00:46.000000 pymilvus-2.2.9/pymilvus/orm/mutation.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    23037 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/orm/partition.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3482 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/orm/prepare.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8327 2023-05-26 03:18:53.000000 pymilvus-2.2.9/pymilvus/orm/role.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    17774 2023-06-02 10:59:50.000000 pymilvus-2.2.9/pymilvus/orm/schema.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7437 2023-05-16 07:00:46.000000 pymilvus-2.2.9/pymilvus/orm/search.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4379 2023-05-23 09:41:28.000000 pymilvus-2.2.9/pymilvus/orm/types.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    47584 2023-05-16 07:00:46.000000 pymilvus-2.2.9/pymilvus/orm/utility.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2554 2023-05-29 03:06:06.000000 pymilvus-2.2.9/pymilvus/settings.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.876826 pymilvus-2.2.9/pymilvus.egg-info/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3916 2023-06-02 11:00:59.000000 pymilvus-2.2.9/pymilvus.egg-info/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3937 2023-06-02 11:00:59.000000 pymilvus-2.2.9/pymilvus.egg-info/SOURCES.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        1 2023-06-02 11:00:59.000000 pymilvus-2.2.9/pymilvus.egg-info/dependency_links.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      101 2023-06-02 11:00:59.000000 pymilvus-2.2.9/pymilvus.egg-info/requires.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        9 2023-06-02 11:00:59.000000 pymilvus-2.2.9/pymilvus.egg-info/top_level.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      118 2022-11-09 07:08:42.000000 pymilvus-2.2.9/pyproject.toml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      620 2023-06-02 10:59:50.000000 pymilvus-2.2.9/requirements.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       38 2023-06-02 11:00:59.884827 pymilvus-2.2.9/setup.cfg
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1131 2023-05-30 03:28:20.000000 pymilvus-2.2.9/setup.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       97 2023-05-16 07:00:46.000000 pymilvus-2.2.9/test_requirements.txt
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-02 11:00:59.884827 pymilvus-2.2.9/tests/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      830 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/conftest.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8443 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/mock_milvus.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      570 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/mock_result.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      275 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/pytest.ini
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4514 2023-06-02 10:59:50.000000 pymilvus-2.2.9/tests/test_check.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6200 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/test_collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14735 2023-05-29 03:06:06.000000 pymilvus-2.2.9/tests/test_connections.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4398 2023-05-29 14:14:31.000000 pymilvus-2.2.9/tests/test_create_collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6114 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/test_decorators.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5523 2023-06-01 03:26:50.000000 pymilvus-2.2.9/tests/test_grpc_handler.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1557 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/test_index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2768 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/test_partition.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7382 2023-06-02 10:59:50.000000 pymilvus-2.2.9/tests/test_prepare.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6553 2023-06-02 10:59:50.000000 pymilvus-2.2.9/tests/test_schema.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1201 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/test_ts_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4548 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/test_types.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      423 2023-06-02 10:59:50.000000 pymilvus-2.2.9/tests/test_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4810 2023-05-16 07:00:46.000000 pymilvus-2.2.9/tests/utils.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/.github/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2045 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       27 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1371 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      633 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/general-question.yaml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      823 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/mergify.yml
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/.github/workflows/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      733 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/check_milvus_proto.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      596 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/code_checker.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      919 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/workflows/doc_update_event.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2046 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/workflows/nightly_ci.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1067 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/publish_dev_package.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      747 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/pull_request.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      778 2022-11-21 06:54:31.000000 pymilvus-2.3.0b1/.github/workflows/release_event.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      264 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.gitignore
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      137 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/.gitmodules
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4996 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/CONTRIBUTING.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4620 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/CONTRIBUTING_CN.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       77 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/Dockerfile
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11336 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/LICENSE
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      552 2022-12-06 08:37:06.000000 pymilvus-2.3.0b1/Makefile
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      176 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/OWNERS
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3816 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/PKG-INFO
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3369 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/README.md
+-rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1306 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/check_proto_product.sh
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.240631 pymilvus-2.3.0b1/ci/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.240631 pymilvus-2.3.0b1/ci/docker/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/ci/docker/milvus/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1169 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/ci/docker/milvus/docker-compose.yml
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/ci/scripts/
+-rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     7597 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/ci/scripts/docker_image_find_tag.sh
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/docs/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      638 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/Makefile
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1858 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/README.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      799 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/make.bat
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/_templates/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       97 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/_templates/autosummaryclass.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      389 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/_templates/layout.html
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      122 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/about.rst
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/api/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      169 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/docs/source/api/api.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8339 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/docs/source/api/collection.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3644 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/connections.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2580 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/future.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2122 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/milvus_index.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4253 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/docs/source/api/partition.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3199 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/schema.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4749 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/search.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7557 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/docs/source/api/utility.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       24 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/changes.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3236 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/docs/source/conf.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3255 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/contribute.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      575 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/faq.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      931 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/index.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2115 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/install.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       60 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/param.rst
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/res/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     9091 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/res/Intro_to_Indexes.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      544 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/res/about_documentation.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1448 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/results.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7429 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/tutorial.rst
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/examples/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/examples/cert/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1326 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/ca.pem
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1704 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/client.key
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/client.pem
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/server.pem
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11469 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/examples/collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4302 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/examples/example.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    15138 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/examples/example_bulkinsert.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5512 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/examples/example_index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4437 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/example_str.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4120 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/example_tls1.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4230 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/example_tls2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)  1070736 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/films.csv
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    12007 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/hello_milvus.ipynb
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7380 2023-02-20 09:16:24.000000 pymilvus-2.3.0b1/examples/hello_milvus.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2690 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/multithreading_hello_milvus.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3452 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_example.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5612 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_example_index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3779 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_example_str.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1874 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_query.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4676 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/examples/partition.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2701 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/examples/resource_group.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6680 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/examples/role_and_privilege.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3310 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/examples/user.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19554 2023-02-09 06:48:27.000000 pymilvus-2.3.0b1/pylint.conf
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/pymilvus/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3188 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/__init__.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.256630 pymilvus-2.3.0b1/pymilvus/client/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1790 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    28616 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/pymilvus/client/abstract.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10675 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/asynch.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      738 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/blob.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11932 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/check.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      242 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/configs.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      200 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pymilvus/client/constants.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3144 2023-03-17 10:58:42.000000 pymilvus-2.3.0b1/pymilvus/client/entity_helper.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    59059 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/grpc_handler.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3522 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/interceptor.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    37767 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/prepare.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      355 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/singleton_utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    58555 2023-02-09 06:48:27.000000 pymilvus-2.3.0b1/pymilvus/client/stub.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2781 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/ts_utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19426 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/client/types.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6421 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6414 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/pymilvus/decorators.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6423 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/exceptions.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.256630 pymilvus-2.3.0b1/pymilvus/grpc_gen/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      116 2023-03-17 10:56:09.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    23471 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/common_pb2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)   120931 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/milvus_pb2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)   109919 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/milvus_pb2_grpc.py
+-rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)      967 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/python_gen.sh
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10854 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/schema_pb2.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.256630 pymilvus-2.3.0b1/pymilvus/orm/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      593 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pymilvus/orm/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    52636 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14956 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/orm/connections.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      909 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/pymilvus/orm/constants.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      842 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/orm/default_config.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1553 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pymilvus/orm/future.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5680 2023-03-01 03:03:27.000000 pymilvus-2.3.0b1/pymilvus/orm/index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1887 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/orm/mutation.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    28312 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/partition.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3691 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/prepare.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7911 2023-03-01 03:03:27.000000 pymilvus-2.3.0b1/pymilvus/orm/role.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14893 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/schema.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7478 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/orm/search.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4318 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/orm/types.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    44273 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/orm/utility.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1926 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/pymilvus/settings.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/pymilvus.egg-info/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3816 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/PKG-INFO
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3622 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/SOURCES.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        1 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/dependency_links.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      175 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/requires.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        9 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/top_level.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      118 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pyproject.toml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      617 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/requirements.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       38 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/setup.cfg
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1096 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/setup.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/tests/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      830 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/conftest.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8443 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/mock_milvus.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      570 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/mock_result.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      275 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/tests/pytest.ini
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5828 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_check.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6200 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    13787 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_connections.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4283 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_create_collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6114 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_decorators.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4163 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_grpc_handler.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1557 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2768 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_partition.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4490 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_prepare.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5437 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_schema.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1201 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_ts_utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4292 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_types.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4810 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/utils.py
```

### Comparing `pymilvus-2.2.9/.github/ISSUE_TEMPLATE/bug_report.yaml` & `pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/.github/ISSUE_TEMPLATE/feature_request.yaml` & `pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/.github/ISSUE_TEMPLATE/general-question.yaml` & `pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/general-question.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/.github/mergify.yml` & `pymilvus-2.3.0b1/.github/mergify.yml`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,28 @@
       label:
         add:
           - ci-passed
   - name: Add needs-dco label when DCO check failed
     conditions:
       - or:
         - base=master
-        - base=2.0
+        - base~=2\.\d
       - -status-success=DCO
     actions:
       label:
         remove:
           - dco-passed
         add:
           - needs-dco
 
   - name: Add dco-passed label when DCO check passed
     conditions:
       - or:
         - base=master
-        - base=2.0
+        - base~=2\.\d
       - status-success=DCO
     actions:
       label:
         remove:
           - needs-dco
         add:
           - dco-passed
```

### Comparing `pymilvus-2.2.9/.github/workflows/check_milvus_proto.yml` & `pymilvus-2.3.0b1/.github/workflows/check_milvus_proto.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Check proto on pull request
 
 on:
   pull_request:
     branches:
-      - 2.2
+      - master
 
 jobs:
   build:
     name: Run Check Proto
     runs-on: ubuntu-latest
     strategy:
       matrix:
@@ -23,14 +23,14 @@
     - name: Fetch tags
       run: |
         git fetch --prune --unshallow --tags
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -e .
+        python setup.py install
 
     - name: Try generate proto
       run: |
         git submodule update --init
         make check_proto_product
```

### Comparing `pymilvus-2.2.9/.github/workflows/code_checker.yml` & `pymilvus-2.3.0b1/.github/workflows/pull_request.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-name: Code checker on pull request
+name: Test on pull request
 
 on:
   pull_request:
     branches:
-      - 2.2
+      - master
 
 jobs:
-  code-lint:
-    name: Code lint check
+  build:
+    name: Run Python Tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.11]
+        python-version: [3.8]
+
     steps:
-      - name: Checkout code
-        uses: actions/checkout@v2
-      - name: Set up python
-        uses: actions/setup-python@v2
-        with:
-          python-version: ${{ matrix.python-version }}
-      - name: check setup.py install
-        run: |
-          python setup.py install
-      - name: Install requirements
-        run: |
-          pip install -r requirements.txt
-      - name: Run pylint
-        shell: bash
-        run: |
-          make lint
+    - uses: actions/checkout@v2
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v2
+      with:
+        python-version: ${{ matrix.python-version }}
+
+    - name: Fetch tags
+      run: |
+        git fetch --prune --unshallow --tags
+
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install pytest
+        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+
+    - name: Test with pytest
+      run: |
+        make unittest
```

### Comparing `pymilvus-2.2.9/.github/workflows/doc_update_event.yml` & `pymilvus-2.3.0b1/.github/workflows/doc_update_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/.github/workflows/nightly_ci.yml` & `pymilvus-2.3.0b1/.github/workflows/nightly_ci.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/.github/workflows/pull_request.yml` & `pymilvus-2.3.0b1/.github/workflows/code_checker.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-name: Test on pull request
+name: Code checker on pull request
 
 on:
   pull_request:
     branches:
-      - 2.2
+      - master
 
 jobs:
-  build:
-    name: Run Python Tests
+  code-lint:
+    name: Code lint check
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.11]
-
+        python-version: [3.8]
     steps:
       - name: Checkout code
         uses: actions/checkout@v2
-      - name: Set up Python ${{ matrix.python-version }}
+      - name: Set up python
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
-
-      - name: Fetch tags
+      - name: Install requirements
         run: |
-          git fetch --prune --unshallow --tags
-
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python setup.py install
-          pip install -r test_requirements.txt
-
-      - name: Test with pytest
+          pip install -r requirements.txt
+      - name: Run pylint
+        shell: bash
         run: |
-          make unittest
+          make lint
```

### Comparing `pymilvus-2.2.9/.github/workflows/release_event.yml` & `pymilvus-2.3.0b1/.github/workflows/release_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/CONTRIBUTING.md` & `pymilvus-2.3.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/CONTRIBUTING_CN.md` & `pymilvus-2.3.0b1/CONTRIBUTING_CN.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/LICENSE` & `pymilvus-2.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/Makefile` & `pymilvus-2.3.0b1/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/PKG-INFO` & `pymilvus-2.3.0b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.2.9
+Version: 2.3.0b1
 Summary: Python Sdk for Milvus
 Home-page: https://github.com/milvus-io/pymilvus
 Author: Milvus Team
 Author-email: milvus-team@zilliz.com
 License: Apache-2.0
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
```

### Comparing `pymilvus-2.2.9/README.md` & `pymilvus-2.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/check_proto_product.sh` & `pymilvus-2.3.0b1/check_proto_product.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/ci/docker/milvus/docker-compose.yml` & `pymilvus-2.3.0b1/ci/docker/milvus/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/ci/scripts/docker_image_find_tag.sh` & `pymilvus-2.3.0b1/ci/scripts/docker_image_find_tag.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/Makefile` & `pymilvus-2.3.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/README.md` & `pymilvus-2.3.0b1/docs/README.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/make.bat` & `pymilvus-2.3.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/api/collection.rst` & `pymilvus-2.3.0b1/docs/source/api/collection.rst`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `insert() <#pymilvus.Collection.insert>`_                     | Insert data into collection.                                             |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `delete() <#pymilvus.Collection.delete>`_                     | Delete entities with an expression condition.                            |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `search() <#pymilvus.Collection.search>`_                     | Vector similarity search with an optional boolean expression as filters. |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
+| `upsert() <#pymilvus.Collection.upsert>`_                     | Upsert data of collection.                                                                  |
++---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `query() <#pymilvus.Collection.query>`_                       | Query with a set of criteria.                                            |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `partition() <#pymilvus.Collection.partition>`_               | Return the partition corresponding to name.                              |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `create_partition() <#pymilvus.Collection.create_partition>`_ | Create the partition for the collection.                                 |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `has_partition() <#pymilvus.Collection.has_partition>`_       | Checks if a specified partition exists.                                  |
```

### Comparing `pymilvus-2.2.9/docs/source/api/connections.rst` & `pymilvus-2.3.0b1/docs/source/api/connections.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/api/future.rst` & `pymilvus-2.3.0b1/docs/source/api/future.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/api/milvus_index.rst` & `pymilvus-2.3.0b1/docs/source/api/milvus_index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/api/partition.rst` & `pymilvus-2.3.0b1/docs/source/api/partition.rst`

 * *Files 15% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `release() <#pymilvus.Partition.release>`_ | Release the Partition from memory.                                       |
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `insert() <#pymilvus.Partition.insert>`_   | Insert data into partition.                                              |
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `delete() <#pymilvus.Partition.delete>`_   | Delete entities with an expression condition.                            |
 +--------------------------------------------+--------------------------------------------------------------------------+
+| `upsert() <#pymilvus.Collection.upsert>`_  |Upsert data of collection.                                               |
++--------------------------------------------+--------------------------------------------------------------------------+
 | `search() <#pymilvus.Partition.search>`_   | Vector similarity search with an optional boolean expression as filters. |
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `query() <#pymilvus.Partition.query>`_     | Query with a set of criteria.                                            |
 +--------------------------------------------+--------------------------------------------------------------------------+
 
 API Refereences
 ---------------
```

### Comparing `pymilvus-2.2.9/docs/source/api/schema.rst` & `pymilvus-2.3.0b1/docs/source/api/schema.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/api/search.rst` & `pymilvus-2.3.0b1/docs/source/api/search.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/api/utility.rst` & `pymilvus-2.3.0b1/docs/source/api/utility.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/conf.py` & `pymilvus-2.3.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/contribute.rst` & `pymilvus-2.3.0b1/docs/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/faq.rst` & `pymilvus-2.3.0b1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/index.rst` & `pymilvus-2.3.0b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/install.rst` & `pymilvus-2.3.0b1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/res/Intro_to_Indexes.md` & `pymilvus-2.3.0b1/docs/source/res/Intro_to_Indexes.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/res/about_documentation.md` & `pymilvus-2.3.0b1/docs/source/res/about_documentation.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/results.rst` & `pymilvus-2.3.0b1/docs/source/results.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/docs/source/tutorial.rst` & `pymilvus-2.3.0b1/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/cert/ca.pem` & `pymilvus-2.3.0b1/examples/cert/ca.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/cert/client.key` & `pymilvus-2.3.0b1/examples/cert/client.key`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/cert/client.pem` & `pymilvus-2.3.0b1/examples/cert/client.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/cert/server.pem` & `pymilvus-2.3.0b1/examples/cert/server.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/collection.py` & `pymilvus-2.3.0b1/examples/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,14 @@
 
     print("\nlist collections:")
     print(utility.list_collections())
     assert utility.has_collection(old_collection)
 
     utility.rename_collection(old_collection, new_collection)
     assert utility.has_collection(new_collection)
-    assert not utility.has_collection(old_collection)
 
 
 if __name__ == "__main__":
     print("test collection and get an existing collection")
     name = test_create_collection()
     print("test an existing collection")
     test_exist_collection(name)
```

### Comparing `pymilvus-2.2.9/examples/database.py` & `pymilvus-2.3.0b1/examples/example_tls2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,166 @@
 import random
 
 from pymilvus import (
     connections,
     FieldSchema, CollectionSchema, DataType,
     Collection,
-    db,
+    utility
 )
-from pymilvus.orm import utility
+
+# This example shows how to:
+#   1. connect to Milvus server
+#   2. create a collection
+#   3. insert entities
+#   4. create index
+#   5. search
+
 
 _HOST = '127.0.0.1'
 _PORT = '19530'
-_ROOT = "root"
-_ROOT_PASSWORD = "Milvus"
-_METRIC_TYPE = 'IP'
-_INDEX_TYPE = 'IVF_FLAT'
-_NLIST = 1024
-_NPROBE = 16
-_TOPK = 3
+
+# Const names
+_COLLECTION_NAME = 'demo'
+_ID_FIELD_NAME = 'id_field'
+_VECTOR_FIELD_NAME = 'float_vector_field'
 
 # Vector parameters
 _DIM = 128
 _INDEX_FILE_SIZE = 32  # max file size of stored index
 
+# Index parameters
+_METRIC_TYPE = 'L2'
+_INDEX_TYPE = 'IVF_FLAT'
+_NLIST = 1024
+_NPROBE = 16
+_TOPK = 3
 
-def connect_to_milvus(db_name="default"):
-    print(f"connect to milvus\n")
-    connections.connect(host=_HOST,
-                        port=_PORT,
-                        user=_ROOT,
-                        password=_ROOT_PASSWORD,
-                        db_name=db_name,
-                        )
-
-
-def connect_to_milvus_with_uri(db_name="default"):
-    print(f"connect to milvus\n")
-    connections.connect(
-        alias="uri-connection",
-        uri="http://{}:{}/{}".format(_HOST, _PORT, db_name),
-    )
-
-
-def create_collection(collection_name, db_name):
-    default_fields = [
-        FieldSchema(name="id", dtype=DataType.INT64, is_primary=True),
-        FieldSchema(name="double", dtype=DataType.DOUBLE),
-        FieldSchema(name="fv", dtype=DataType.FLOAT_VECTOR, dim=128)
-    ]
-    default_schema = CollectionSchema(fields=default_fields)
-    print(f"Create collection:{collection_name} within db:{db_name}")
-    return Collection(name=collection_name, schema=default_schema)
+
+# Create a Milvus connection
+def create_connection():
+    print(f"\nCreate connection...")
+    connections.connect(host=_HOST, port=_PORT, secure=True, client_pem_path="cert/client.pem",
+                        client_key_path="cert/client.key",
+                        ca_pem_path="cert/ca.pem", server_name="localhost")
+    print(f"\nList connections:")
+    print(connections.list_connections())
+
+
+# Create a collection named 'demo'
+def create_collection(name, id_field, vector_field):
+    field1 = FieldSchema(name=id_field, dtype=DataType.INT64, description="int64", is_primary=True)
+    field2 = FieldSchema(name=vector_field, dtype=DataType.FLOAT_VECTOR, description="float vector", dim=_DIM,
+                         is_primary=False)
+    schema = CollectionSchema(fields=[field1, field2], description="collection description")
+    collection = Collection(name=name, data=None, schema=schema)
+    print("\ncollection created:", name)
+    return collection
+
+
+def has_collection(name):
+    return utility.has_collection(name)
+
+
+# Drop a collection in Milvus
+def drop_collection(name):
+    collection = Collection(name)
+    collection.drop()
+    print("\nDrop collection: {}".format(name))
+
+
+# List all collections in Milvus
+def list_collections():
+    print("\nlist collections:")
+    print(utility.list_collections())
 
 
 def insert(collection, num, dim):
     data = [
         [i for i in range(num)],
-        [float(i) for i in range(num)],
         [[random.random() for _ in range(dim)] for _ in range(num)],
     ]
     collection.insert(data)
-    return data[2]
+    return data[1]
+
+
+def get_entity_num(collection):
+    print("\nThe number of entity:")
+    print(collection.num_entities)
+
+
+def create_index(collection, filed_name):
+    index_param = {
+        "index_type": _INDEX_TYPE,
+        "params": {"nlist": _NLIST},
+        "metric_type": _METRIC_TYPE}
+    collection.create_index(filed_name, index_param)
+    print("\nCreated index:\n{}".format(collection.index().params))
 
 
 def drop_index(collection):
     collection.drop_index()
     print("\nDrop index sucessfully")
 
 
+def load_collection(collection):
+    collection.load()
+
+
+def release_collection(collection):
+    collection.release()
+
+
 def search(collection, vector_field, id_field, search_vectors):
     search_param = {
         "data": search_vectors,
         "anns_field": vector_field,
         "param": {"metric_type": _METRIC_TYPE, "params": {"nprobe": _NPROBE}},
         "limit": _TOPK,
-        "expr": "id >= 0"}
+        "expr": "id_field > 0"}
     results = collection.search(**search_param)
     for i, result in enumerate(results):
         print("\nSearch result for {}th vector: ".format(i))
         for j, res in enumerate(result):
             print("Top {}: {}".format(j, res))
 
 
-def collection_read_write(collection, db_name):
-    col_name = "{}:{}".format(db_name, collection.name)
+def main():
+    # create a connection
+    create_connection()
+
+    # drop collection if the collection exists
+    if has_collection(_COLLECTION_NAME):
+        drop_collection(_COLLECTION_NAME)
+
+    # create collection
+    collection = create_collection(_COLLECTION_NAME, _ID_FIELD_NAME, _VECTOR_FIELD_NAME)
+
+    # show collections
+    list_collections()
+
+    # insert 10000 vectors with 128 dimension
     vectors = insert(collection, 10000, _DIM)
-    collection.flush()
-    print("\nInsert {} rows data into collection:{}".format(collection.num_entities, col_name))
+
+    # get the number of entities
+    get_entity_num(collection)
 
     # create index
-    index_param = {
-        "index_type": _INDEX_TYPE,
-        "params": {"nlist": _NLIST},
-        "metric_type": _METRIC_TYPE}
-    collection.create_index("fv", index_param)
-    print("\nCreated index:{} for collection:{}".format(collection.index().params, col_name))
+    create_index(collection, _VECTOR_FIELD_NAME)
 
     # load data to memory
-    print("\nLoad collection:{}".format(col_name))
-    collection.load()
+    load_collection(collection)
+
     # search
-    print("\nSearch collection:{}".format(col_name))
-    search(collection, "fv", "id", vectors[:3])
+    search(collection, _VECTOR_FIELD_NAME, _ID_FIELD_NAME, vectors[:3])
 
-    # release memory
-    collection.release()
     # drop collection index
-    collection.drop_index()
-    print("\nDrop collection:{}".format(col_name))
+    drop_index(collection)
 
+    # release memory
+    release_collection(collection)
 
-if __name__ == '__main__':
-    # connect to milvus and using database db1
-    # there will not check db1 already exists during connect
-    connect_to_milvus(db_name="default")
-
-    # create collection within default
-    col1_db1 = create_collection("col1_db1", "default")
-
-    # create db1
-    if "db1" not in db.list_database():
-        print("\ncreate database: db1")
-        db.create_database(db_name="db1")
-
-    # use database db1
-    db.using_database(db_name="db1")
-    # create collection within default
-    col2_db1 = create_collection("col1_db1", "db1")
+    # drop collection
+    drop_collection(_COLLECTION_NAME)
 
-    # verify read and write
-    collection_read_write(col2_db1, "db1")
 
-    # list collections within db1
-    print("\nlist collections of database db1:")
-    print(utility.list_collections())
-
-    print("\ndrop collection: col1_db2 from db1")
-    col2_db1.drop()
-    print("\ndrop database: db1")
-    db.drop_database(db_name="db1")
-
-    # list database
-    print("\nlist databases:")
-    print(db.list_database())
+if __name__ == '__main__':
+    main()
```

### Comparing `pymilvus-2.2.9/examples/dynamic_field.py` & `pymilvus-2.3.0b1/examples/multithreading_hello_milvus.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,77 @@
 import time
+
 import numpy as np
 from pymilvus import (
     connections,
     utility,
     FieldSchema, CollectionSchema, DataType,
     Collection,
 )
 
-fmt = "\n=== {:30} ===\n"
-dim = 8
+import threading
+import concurrent
+
+fmt = "\n=== {:30} ==="
+search_latency_fmt = "search latency = {:.4f}s"
+num_entities, dim = 3000, 8
 
 print(fmt.format("start connecting to Milvus"))
 connections.connect("default", host="localhost", port="19530")
 
-has = utility.has_collection("hello_milvus")
-print(f"Does collection hello_milvus exist in Milvus: {has}")
-if has:
+if utility.has_collection("hello_milvus"):
     utility.drop_collection("hello_milvus")
+    print(f"Dropping existing collection hello_milvus")
 
 fields = [
-    FieldSchema(name="pk", dtype=DataType.VARCHAR, is_primary=True, auto_id=False, max_length=100),
+    FieldSchema(name="pk", dtype=DataType.INT64, is_primary=True, auto_id=False),
     FieldSchema(name="random", dtype=DataType.DOUBLE),
     FieldSchema(name="embeddings", dtype=DataType.FLOAT_VECTOR, dim=dim)
 ]
 
-schema = CollectionSchema(fields, "hello_milvus is the simplest demo to introduce the APIs", enable_dynamic_field=True)
+schema = CollectionSchema(fields, "hello_milvus is the simplest demo to introduce the APIs")
 
 print(fmt.format("Create collection `hello_milvus`"))
 hello_milvus = Collection("hello_milvus", schema, consistency_level="Strong")
 
-################################################################################
-# 3. insert data
-hello_milvus2 = Collection("hello_milvus")
-print(fmt.format("Start inserting entities"))
-rng = np.random.default_rng(seed=19530)
-
-rows = [
-        {"pk": "1", "random": 1.0, "embeddings": rng.random((1, dim))[0], "a": 1},
-        {"pk": "2", "random": 1.0, "embeddings": rng.random((1, dim))[0], "b": 1},
-        {"pk": "3", "random": 1.0, "embeddings": rng.random((1, dim))[0], "c": 1},
-        {"pk": "4", "random": 1.0, "embeddings": rng.random((1, dim))[0], "d": 1},
-        {"pk": "5", "random": 1.0, "embeddings": rng.random((1, dim))[0], "e": 1},
-        {"pk": "6", "random": 1.0, "embeddings": rng.random((1, dim))[0], "f": 1},
-        ]
-
-insert_result = hello_milvus.insert(rows)
-
-hello_milvus.insert({"pk": "7", "random": 1.0, "embeddings": rng.random((1, dim))[0], "g": 1})
-hello_milvus.flush()
-print(f"Number of entities in Milvus: {hello_milvus.num_entities}")  # check the num_entites
-
-# 4. create index
-print(fmt.format("Start Creating index IVF_FLAT"))
-index = {
-    "index_type": "IVF_FLAT",
-    "metric_type": "L2",
-    "params": {"nlist": 128},
-}
-
-hello_milvus.create_index("embeddings", index)
-
-print(fmt.format("Start loading"))
-hello_milvus.load()
-# -----------------------------------------------------------------------------
-# search based on vector similarity
-print(fmt.format("Start searching based on vector similarity"))
-
-rng = np.random.default_rng(seed=19530)
-vectors_to_search = rng.random((1, dim))
-search_params = {
-    "metric_type": "L2",
-    "params": {"nprobe": 10},
-}
-
-start_time = time.time()
-
-print(fmt.format(f"Start search with retrieve all $meta fields."))
-result = hello_milvus.search(vectors_to_search, "embeddings", search_params, limit=3, output_fields=["pk", "$meta"])
-end_time = time.time()
-
-for hits in result:
-    for hit in hits:
-        print(f"hit: {hit}")
-
-
-expr = f'pk in ["1" , "2"] || g == 1'
-
-print(fmt.format(f"Start query with expr `{expr}`"))
-result = hello_milvus.query(expr=expr, output_fields=["random", "a", "g"])
-for hit in result:
-    print("hit:", hit)
 
+class MilvusMultiThreadingInsert:
+    def __init__(self, collection_name: str, number_of_batch: int):
 
+        self.thread_local = threading.local()
+        self.collection_name = collection_name
+        self.batchs = [i for i in range(number_of_batch)]
+
+    def get_thread_local_collection(self):
+        if not hasattr(self.thread_local, "collection"):
+            self.thread_local.collection = Collection(self.collection_name)
+        return self.thread_local.collection
+
+    def insert_data(self, number: int):
+        print(fmt.format(f"No.{number:2}: Start inserting entities"))
+        rng = np.random.default_rng(seed=number)
+        entities = [
+            [i for i in range(num_entities)],
+            rng.random(num_entities).tolist(),
+            rng.random((num_entities, dim)),
+        ]
 
-###############################################################################
-# 7. drop collection
-print(fmt.format("Drop collection `hello_milvus`"))
-utility.drop_collection("hello_milvus")
+        insert_result = hello_milvus.insert(entities)
+        assert len(insert_result.primary_keys) == num_entities
+        print(fmt.format(f"No.{number:2}: Finish inserting entities"))
+
+    def insert_all_batches(self):
+        with concurrent.futures.ThreadPoolExecutor(max_workers=12) as executor:
+            executor.map(self.insert_data, self.batchs)
+
+    def run(self):
+        start_time = time.time()
+        self.insert_all_batches()
+        duration = time.time() - start_time
+        print(f'Inserted {len(self.batchs)} batches of {num_entities} entities in {duration} seconds')
+        print(f"Expected num_entities: {len(self.batchs)*num_entities}. \
+                Acutal num_entites: {self.get_thread_local_collection().num_entities}")
+
+
+if __name__ == "__main__":
+    multithreading_insert = MilvusMultiThreadingInsert("hello_milvus", 10)
+    multithreading_insert.run()
```

### Comparing `pymilvus-2.2.9/examples/example.py` & `pymilvus-2.3.0b1/examples/example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/example_bulkinsert.py` & `pymilvus-2.3.0b1/examples/example_bulkinsert.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/example_index.py` & `pymilvus-2.3.0b1/examples/example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/example_str.py` & `pymilvus-2.3.0b1/examples/example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/example_tls1.py` & `pymilvus-2.3.0b1/examples/example_tls1.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/films.csv` & `pymilvus-2.3.0b1/examples/films.csv`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/hello_milvus.ipynb` & `pymilvus-2.3.0b1/examples/hello_milvus.ipynb`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/hello_milvus.py` & `pymilvus-2.3.0b1/examples/hello_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/old_style_example.py` & `pymilvus-2.3.0b1/examples/old_style_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/old_style_example_index.py` & `pymilvus-2.3.0b1/examples/old_style_example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/old_style_example_str.py` & `pymilvus-2.3.0b1/examples/old_style_example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/old_style_query.py` & `pymilvus-2.3.0b1/examples/old_style_query.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/partition.py` & `pymilvus-2.3.0b1/examples/partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/examples/resource_group.py` & `pymilvus-2.3.0b1/examples/resource_group.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,22 +49,20 @@
 
 def transfer_replica(source, target, collection_name, num_replica):
     print(
         f"transfer {num_replica} replicas in {collection_name} from {source} to {target}")
     utility.transfer_replica(
         source, target, collection_name, num_replica, using=_CONNECTION_NAME)
     
-
 def run(): 
     create_connection("root", "123456")
     coll = create_collection(_COLLECTION_NAME, _ID_FIELD_NAME, _VECTOR_FIELD_NAME)
     vectors = insert(coll, 10000, _DIM)
     coll.flush()
     create_index(coll, _VECTOR_FIELD_NAME)
-    load_collection(coll)
     
     create_resource_group("rg")
     list_resource_groups()
     describe_resource_group("rg")
     transfer_node(DEFAULT_RESOURCE_GROUP, "rg", 1)
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
@@ -76,20 +74,14 @@
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
     
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
     transfer_replica("rg", DEFAULT_RESOURCE_GROUP, _COLLECTION_NAME, 1)
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
-    describe_resource_group("rg")
-    
-    describe_resource_group(DEFAULT_RESOURCE_GROUP)
-    describe_resource_group("rg")
-    transfer_replica("rg", DEFAULT_RESOURCE_GROUP, _COLLECTION_NAME, 1)
-    describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
    
     drop_resource_group("rg")
     release_collection(coll)
     drop_collection(_COLLECTION_NAME)
 
 if __name__ == "__main__":
```

### Comparing `pymilvus-2.2.9/examples/role_and_privilege.py` & `pymilvus-2.3.0b1/examples/role_and_privilege.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 from pymilvus.orm.role import Role
 
 import random
 from sklearn import preprocessing
 
 _CONNECTION = "demo"
 _FOO_CONNECTION = "foo_connection"
-_DB_NAME = "foo_db"
 _HOST = '127.0.0.1'
 _PORT = '19530'
 _ROOT = "root"
 _ROOT_PASSWORD = "Milvus"
 _COLLECTION_NAME = "foocol2"
 
 
-def connect_to_milvus(connection=_CONNECTION, user=_ROOT, password=_ROOT_PASSWORD, db_name="default"):
+def connect_to_milvus(connection=_CONNECTION, user=_ROOT, password=_ROOT_PASSWORD):
     print(f"connect to milvus\n")
     connections.connect(alias=connection,
                         host=_HOST,
                         port=_PORT,
                         user=user,
                         password=password,
-                        db_name=db_name,
                         )
 
 
 def create_credential(user, password, connection=_CONNECTION):
     print(f"create credential, user: {user}, password: {password}")
     utility.create_user(user, password, using=connection)
     print(f"create credential down\n")
@@ -131,17 +129,17 @@
     try:
         select_all_user(connection=connection)
     except Exception as e:
         print(e)
         is_exception = True
     assert is_exception
     role = Role(role_name, using=_CONNECTION)
-    role.grant("User", "*", "SelectUser", db_name=_DB_NAME)
+    role.grant("User", "*", "SelectUser")
     print(select_all_user(connection))
-    role.revoke("User", "*", "SelectUser", db_name=_DB_NAME)
+    role.revoke("User", "*", "SelectUser")
 
 
 def role_example():
     role_name = "role_test5"
     role = Role(role_name, using=_CONNECTION)
     print(f"create role, role_name: {role_name}")
     role.create()
@@ -180,39 +178,34 @@
     create_credential(username, password)
     role = Role(role_name, using=_CONNECTION)
     print(f"create role, role_name: {role_name}")
     role.create()
     print(f"add user")
     role.add_user(username)
     print(f"grant privilege")
-    role.grant("Global", "*", privilege_create, db_name=_DB_NAME)
-    role.grant("Collection", object_name, privilege_insert, db_name=_DB_NAME)
-    # role.grant("Collection", object_name, "*", db_name=_DB_NAME)
-    # role.grant("Collection", "*", privilege_insert, db_name=_DB_NAME)
-
-    print(f"list grants")
-    print(role.list_grants(db_name=_DB_NAME))
-    print(f"list grant")
-    print(role.list_grant("Collection", object_name, db_name=_DB_NAME))
+    role.grant("Global", "*", privilege_create)
+    role.grant("Collection", object_name, privilege_insert)
+    # role.grant("Collection", object_name, "*")
+    # role.grant("Collection", "*", privilege_insert)
 
     print(f"list grants")
     print(role.list_grants())
     print(f"list grant")
     print(role.list_grant("Collection", object_name))
 
-    connect_to_milvus(connection=_FOO_CONNECTION, user=username, password=password, db_name=_DB_NAME)
+    connect_to_milvus(connection=_FOO_CONNECTION, user=username, password=password)
     has_collection(_COLLECTION_NAME, connection=_FOO_CONNECTION)
     rbac_collection(connection=_FOO_CONNECTION)
     rbac_user(username, password, role_name, connection=_FOO_CONNECTION)
 
     print(f"revoke privilege")
     role.revoke("Global", "*", privilege_create)
-    role.revoke("Collection", object_name, privilege_insert, db_name=_DB_NAME)
-    # role.revoke("Collection", object_name, "*", db_name=_DB_NAME)
-    # role.revoke("Collection", "*", privilege_insert, db_name=_DB_NAME)
+    role.revoke("Collection", object_name, privilege_insert)
+    # role.revoke("Collection", object_name, "*")
+    # role.revoke("Collection", "*", privilege_insert)
     print(f"remove user")
     role.remove_user(username)
     role.drop()
     drop_credential(username)
 
 
 def run():
```

### Comparing `pymilvus-2.2.9/examples/user.py` & `pymilvus-2.3.0b1/examples/user.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/pylint.conf` & `pymilvus-2.3.0b1/pylint.conf`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/pymilvus/__init__.py` & `pymilvus-2.3.0b1/pymilvus/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,24 +27,15 @@
     ParamError,
     MilvusException,
     MilvusUnavailableException,
     ExceptionsMessage
 )
 from .client import __version__
 
-from .settings import (
-    DEBUG_LOG_LEVEL,
-    INFO_LOG_LEVEL,
-    WARN_LOG_LEVEL,
-    ERROR_LOG_LEVEL,
-)
-# Compatiable
-from .settings import Config as DefaultConfig
-
-from .client.constants import DEFAULT_RESOURCE_GROUP
+from .settings import DEBUG_LOG_LEVEL, INFO_LOG_LEVEL, WARN_LOG_LEVEL, ERROR_LOG_LEVEL
 
 from .orm.collection import Collection
 from .orm.connections import connections, Connections
 
 from .orm.index import Index
 from .orm.partition import Partition
 from .orm.utility import (
@@ -62,38 +53,35 @@
     hybridts_to_unixtime, hybridts_to_datetime,
     do_bulk_insert, get_bulk_insert_state, list_bulk_insert_tasks,
     reset_password, create_user, update_password, delete_user, list_usernames,
     create_resource_group, drop_resource_group, describe_resource_group,
     list_resource_groups, transfer_node, transfer_replica
 )
 
-from .orm import utility, db
+from .orm import utility
+from .orm.default_config import DefaultConfig, ENV_CONNECTION_CONF, DEFAULT_RESOURCE_GROUP
 
 from .orm.search import SearchResult, Hits, Hit
 from .orm.schema import FieldSchema, CollectionSchema
 from .orm.future import SearchFuture, MutationFuture
 from .orm.role import Role
 
-from .milvus_client.milvus_client import MilvusClient
-
 __all__ = [
     'Collection', 'Index', 'Partition',
     'connections',
     'loading_progress', 'index_building_progress', 'wait_for_loading_complete', 'has_collection', 'has_partition',
     'list_collections', 'wait_for_loading_complete', 'wait_for_index_building_complete', 'drop_collection',
     'mkts_from_hybridts', 'mkts_from_unixtime', 'mkts_from_datetime',
     'hybridts_to_unixtime', 'hybridts_to_datetime',
     'reset_password', 'create_user', 'update_password', 'delete_user', 'list_usernames',
     'SearchResult', 'Hits', 'Hit', 'Replica', 'Group', 'Shard',
     'FieldSchema', 'CollectionSchema',
     'SearchFuture', 'MutationFuture',
-    'utility', 'db', 'DefaultConfig', 'ExceptionsMessage', 'MilvusUnavailableException', 'BulkInsertState',
+    'utility', 'DefaultConfig', 'ExceptionsMessage', 'MilvusUnavailableException', 'BulkInsertState',
     'Role',
     'create_resource_group', 'drop_resource_group', 'describe_resource_group',
     'list_resource_groups', 'transfer_node', 'transfer_replica',
 
     'Milvus', 'Prepare', 'Status', 'DataType',
     'MilvusException',
-    '__version__',
-
-    'MilvusClient'
+    '__version__'
 ]
```

### Comparing `pymilvus-2.2.9/pymilvus/client/__init__.py` & `pymilvus-2.3.0b1/pymilvus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/pymilvus/client/abstract.py` & `pymilvus-2.3.0b1/pymilvus/client/abstract.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 
-from ..settings import Config
+import numpy as np
+from .configs import DefaultConfigs
 from .types import DataType
 from .constants import DEFAULT_CONSISTENCY_LEVEL
 from ..grpc_gen import schema_pb2
 from ..exceptions import MilvusException
-from . import entity_helper
 
 
 class LoopBase:
     def __init__(self):
         self.__index = 0
 
     def __iter__(self):
@@ -64,43 +64,35 @@
         self.name = None
         self.is_primary = False
         self.description = None
         self.auto_id = False
         self.type = DataType.UNKNOWN
         self.indexes = []
         self.params = {}
-        self.is_partition_key = False
-        self.is_dynamic = False
 
         ##
         self.__pack(self._raw)
 
     def __pack(self, raw):
         self.field_id = raw.fieldID
         self.name = raw.name
         self.is_primary = raw.is_primary_key
         self.description = raw.description
         self.auto_id = raw.autoID
         self.type = raw.data_type
-        self.is_partition_key = raw.is_partition_key
-        try:
-            self.is_dynamic = raw.is_dynamic
-        except Exception:
-            self.is_dynamic = False
-
         # self.type = DataType(int(raw.type))
 
         for type_param in raw.type_params:
             if type_param.key == "params":
                 import json
                 self.params[type_param.key] = json.loads(type_param.value)
             else:
                 self.params[type_param.key] = type_param.value
                 # maybe we'd better not to check these fields in ORM.
-                if type_param.key in ["dim", Config.MaxVarCharLengthKey]:
+                if type_param.key in ["dim", DefaultConfigs.MaxVarCharLengthKey]:
                     self.params[type_param.key] = int(type_param.value)
 
         index_dict = {}
         for index_param in raw.index_params:
             if index_param.key == "params":
                 import json
                 index_dict[index_param.key] = json.loads(index_param.value)
@@ -114,16 +106,14 @@
             "field_id": self.field_id,
             "name": self.name,
             "description": self.description,
             "type": self.type,
             "params": self.params or {},
             "is_primary": self.is_primary,
             "auto_id": self.auto_id,
-            "is_partition_key": self.is_partition_key,
-            "is_dynamic": self.is_dynamic,
         }
         return _dict
 
 
 class CollectionSchema:
     def __init__(self, raw):
         self._raw = raw
@@ -135,41 +125,31 @@
         self.fields = []
         self.statistics = {}
         self.auto_id = False  # auto_id is not in collection level any more later
         self.aliases = []
         self.collection_id = 0
         self.consistency_level = DEFAULT_CONSISTENCY_LEVEL  # by default
         self.properties = {}
-        self.num_shards = 0
-        self.num_partitions = 0
-        self.enable_dynamic_field = False
 
         #
         if self._raw:
             self.__pack(self._raw)
 
     def __pack(self, raw):
         self.collection_name = raw.schema.name
         self.description = raw.schema.description
         self.aliases = raw.aliases
         self.collection_id = raw.collectionID
-        self.num_shards = raw.shards_num
-        self.num_partitions = raw.num_partitions
 
         # keep compatible with older Milvus
         try:
             self.consistency_level = raw.consistency_level
         except Exception:
             self.consistency_level = DEFAULT_CONSISTENCY_LEVEL
 
-        try:
-            self.enable_dynamic_field = raw.schema.enable_dynamic_field
-        except Exception:
-            self.enable_dynamic_field = False
-
         # self.params = dict()
         # TODO: extra_params here
         # for kv in raw.extra_params:
         #     par = ujson.loads(kv.value)
         #     self.params.update(par)
         #     # self.params[kv.key] = kv.value
 
@@ -182,23 +162,20 @@
 
     def dict(self):
         if not self._raw:
             return {}
         _dict = {
             "collection_name": self.collection_name,
             "auto_id": self.auto_id,
-            "num_shards": self.num_shards,
             "description": self.description,
             "fields": [f.dict() for f in self.fields],
             "aliases": self.aliases,
             "collection_id": self.collection_id,
             "consistency_level": self.consistency_level,
             "properties": self.properties,
-            "num_partitions": self.num_partitions,
-            "enable_dynamic_field": self.enable_dynamic_field,
         }
         return _dict
 
     def __str__(self):
         return self.dict().__str__()
 
 
@@ -240,17 +217,15 @@
     def __init__(self, entity_id, entity_row_data, entity_score):
         self._id = entity_id
         self._row_data = entity_row_data
         self._score = entity_score
         self._distance = entity_score
 
     def __str__(self):
-        return str(self.entity)
-
-    __repr__ = __str__
+        return f"(distance: {self._distance}, score: {self._score}, id: {self._id})"
 
     @property
     def entity(self):
         return Entity(self._id, self._row_data, self._score)
 
     @property
     def id(self):
@@ -262,44 +237,76 @@
 
     @property
     def score(self):
         return self._score
 
 
 class Hits(LoopBase):
-    def __init__(self, raw, round_decimal=-1):
+    def __init__(self, raw, auto_id, round_decimal=-1):
         super().__init__()
         self._raw = raw
+        self._auto_id = auto_id
         if round_decimal != -1:
             self._distances = [round(x, round_decimal) for x in self._raw.scores]
         else:
             self._distances = self._raw.scores
 
-        self._dynamic_field_name = None
-        self._dynamic_fields = set()
-        self._dynamic_field_name, self._dynamic_fields = entity_helper.extract_dynamic_field_from_result(self._raw)
-
-
     def __len__(self):
         if self._raw.ids.HasField("int_id"):
             return len(self._raw.ids.int_id.data)
         if self._raw.ids.HasField("str_id"):
             return len(self._raw.ids.str_id.data)
         return 0
 
     def get__item(self, item):
         if self._raw.ids.HasField("int_id"):
             entity_id = self._raw.ids.int_id.data[item]
         elif self._raw.ids.HasField("str_id"):
             entity_id = self._raw.ids.str_id.data[item]
         else:
             raise MilvusException(message="Unsupported ids type")
-
-        entity_row_data = entity_helper.extract_row_data_from_fields_data(self._raw.fields_data, item,
-                                                                          self._dynamic_fields)
+        entity_row_data = {}
+        if self._raw.fields_data:
+            for field_data in self._raw.fields_data:
+                if field_data.type == DataType.BOOL:
+                    if len(field_data.scalars.bool_data.data) >= item:
+                        entity_row_data[field_data.field_name] = field_data.scalars.bool_data.data[item]
+                elif field_data.type in (DataType.INT8, DataType.INT16, DataType.INT32):
+                    if len(field_data.scalars.int_data.data) >= item:
+                        entity_row_data[field_data.field_name] = field_data.scalars.int_data.data[item]
+                elif field_data.type == DataType.INT64:
+                    if len(field_data.scalars.long_data.data) >= item:
+                        entity_row_data[field_data.field_name] = field_data.scalars.long_data.data[item]
+                elif field_data.type == DataType.FLOAT:
+                    if len(field_data.scalars.float_data.data) >= item:
+                        entity_row_data[field_data.field_name] = np.single(field_data.scalars.float_data.data[item])
+                elif field_data.type == DataType.DOUBLE:
+                    if len(field_data.scalars.double_data.data) >= item:
+                        entity_row_data[field_data.field_name] = field_data.scalars.double_data.data[item]
+                elif field_data.type == DataType.VARCHAR:
+                    if len(field_data.scalars.string_data.data) >= item:
+                        entity_row_data[field_data.field_name] = field_data.scalars.string_data.data[item]
+                elif field_data.type == DataType.STRING:
+                    raise MilvusException(message="Not support string yet")
+                    # result[field_data.field_name] = field_data.scalars.string_data.data[index]
+                elif field_data.type == DataType.FLOAT_VECTOR:
+                    dim = field_data.vectors.dim
+                    if len(field_data.vectors.float_vector.data) >= item * dim:
+                        start_pos = item * dim
+                        end_pos = item * dim + dim
+                        entity_row_data[field_data.field_name] = [np.single(x) for x in
+                                                                  field_data.vectors.float_vector.data[
+                                                                  start_pos:end_pos]]
+                elif field_data.type == DataType.BINARY_VECTOR:
+                    dim = field_data.vectors.dim
+                    if len(field_data.vectors.binary_vector.data) >= item * (dim / 8):
+                        start_pos = item * (dim / 8)
+                        end_pos = (item + 1) * (dim / 8)
+                        entity_row_data[field_data.field_name] = [
+                            field_data.vectors.binary_vector.data[start_pos:end_pos]]
         entity_score = self._distances[item]
         return Hit(entity_id, entity_row_data, entity_score)
 
     @property
     def ids(self):
         if self._raw.ids.HasField("int_id"):
             return self._raw.ids.int_id.data
@@ -387,17 +394,18 @@
         self._upsert_cnt = raw.upsert_cnt
         self._timestamp = raw.timestamp
         self._succ_index = raw.succ_index
         self._err_index = raw.err_index
 
 
 class QueryResult(LoopBase):
-    def __init__(self, raw):
+    def __init__(self, raw, auto_id=True):
         super().__init__()
         self._raw = raw
+        self._auto_id = auto_id
         self._pack(raw.hits)
 
     def __len__(self):
         return self._nq
 
     def _pack(self, raw):
         self._nq = raw.results.num_queries
@@ -428,16 +436,14 @@
                 elif field_data.type == DataType.DOUBLE:
                     field.scalars.double_data.data.extend(field_data.scalars.double_data.data[start_pos: end_pos])
                 elif field_data.type == DataType.VARCHAR:
                     field.scalars.string_data.data.extend(field_data.scalars.string_data.data[start_pos: end_pos])
                 elif field_data.type == DataType.STRING:
                     raise MilvusException(message="Not support string yet")
                     # result[field_data.field_name] = field_data.scalars.string_data.data[index]
-                elif field_data.type == DataType.JSON:
-                    field.scalars.json_data.data.extend(field_data.scalars.json_data.data[start_pos: end_pos])
                 elif field_data.type == DataType.FLOAT_VECTOR:
                     dim = field.vectors.dim
                     field.vectors.dim = dim
                     field.vectors.float_vector.data.extend(
                         field_data.vectors.float_data.data[start_pos * dim: end_pos * dim])
                 elif field_data.type == DataType.BINARY_VECTOR:
                     dim = field_data.vectors.dim
@@ -445,21 +451,22 @@
                     field.vectors.binary_vector.data.extend(field_data.vectors.binary_vector.data[
                                                             start_pos * (dim / 8): end_pos * (dim / 8)])
                 hit.fields_data.append(field)
             self._hits.append(hit)
             offset += raw.results.topks[i]
 
     def get__item(self, item):
-        return Hits(self._hits[item])
+        return Hits(self._hits[item], self._auto_id)
 
 
 class ChunkedQueryResult(LoopBase):
-    def __init__(self, raw_list, round_decimal=-1):
+    def __init__(self, raw_list, auto_id=True, round_decimal=-1):
         super().__init__()
         self._raw_list = raw_list
+        self._auto_id = auto_id
         self._nq = 0
         self.round_decimal = round_decimal
 
         self._pack(self._raw_list)
 
     def __len__(self):
         return self._nq
@@ -476,20 +483,18 @@
                 start_pos = offset
                 end_pos = offset + raw.results.topks[i]
                 hit.scores.extend(raw.results.scores[start_pos: end_pos])
                 if raw.results.ids.HasField("int_id"):
                     hit.ids.int_id.data.extend(raw.results.ids.int_id.data[start_pos: end_pos])
                 elif raw.results.ids.HasField("str_id"):
                     hit.ids.str_id.data.extend(raw.results.ids.str_id.data[start_pos: end_pos])
-                hit.output_fields.extend(raw.results.output_fields)
                 for field_data in raw.results.fields_data:
                     field = schema_pb2.FieldData()
                     field.type = field_data.type
                     field.field_name = field_data.field_name
-                    field.is_dynamic = field_data.is_dynamic
                     if field_data.type == DataType.BOOL:
                         field.scalars.bool_data.data.extend(field_data.scalars.bool_data.data[start_pos: end_pos])
                     elif field_data.type in (DataType.INT8, DataType.INT16, DataType.INT32):
                         field.scalars.int_data.data.extend(field_data.scalars.int_data.data[start_pos: end_pos])
                     elif field_data.type == DataType.INT64:
                         field.scalars.long_data.data.extend(field_data.scalars.long_data.data[start_pos: end_pos])
                     elif field_data.type == DataType.FLOAT:
@@ -497,16 +502,14 @@
                     elif field_data.type == DataType.DOUBLE:
                         field.scalars.double_data.data.extend(field_data.scalars.double_data.data[start_pos: end_pos])
                     elif field_data.type == DataType.VARCHAR:
                         field.scalars.string_data.data.extend(field_data.scalars.string_data.data[start_pos: end_pos])
                     elif field_data.type == DataType.STRING:
                         raise MilvusException(message="Not support string yet")
                         # result[field_data.field_name] = field_data.scalars.string_data.data[index]
-                    elif field_data.type == DataType.JSON:
-                        field.scalars.json_data.data.extend(field_data.scalars.json_data.data[start_pos: end_pos])
                     elif field_data.type == DataType.FLOAT_VECTOR:
                         dim = field_data.vectors.dim
                         field.vectors.dim = dim
                         field.vectors.float_vector.data.extend(field_data.vectors.float_vector.data[
                                                                start_pos * dim: end_pos * dim])
                     elif field_data.type == DataType.BINARY_VECTOR:
                         dim = field_data.vectors.dim
@@ -514,15 +517,15 @@
                         field.vectors.binary_vector.data.extend(field_data.vectors.binary_vector.data[
                                                                 start_pos * (dim / 8): end_pos * (dim / 8)])
                     hit.fields_data.append(field)
                 self._hits.append(hit)
                 offset += raw.results.topks[i]
 
     def get__item(self, item):
-        return Hits(self._hits[item], self.round_decimal)
+        return Hits(self._hits[item], self._auto_id, self.round_decimal)
 
 
 def _abstract():
     raise NotImplementedError('You need to override this function')
 
 
 class ConnectIntf:
```

### Comparing `pymilvus-2.2.9/pymilvus/client/asynch.py` & `pymilvus-2.3.0b1/pymilvus/client/asynch.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,27 +152,32 @@
         if self._exception:
             raise self._exception
         if self._future:
             self._future.exception()
 
 
 class SearchFuture(Future):
+    def __init__(self, future, done_callback=None, auto_id=True, pre_exception=None):
+        super().__init__(future, done_callback, pre_exception)
+        self._auto_id = auto_id
+
     def on_response(self, response):
         if response.status.error_code == 0:
-            return QueryResult(response)
+            return QueryResult(response, self._auto_id)
 
         status = response.status
         raise MilvusException(status.error_code, status.reason)
 
 
 # TODO: if ChunkedFuture is more common later, consider using ChunkedFuture as Base Class,
 #       then Future(future, done_cb, pre_exception) equal to ChunkedFuture([future], done_cb, pre_exception)
 class ChunkedSearchFuture(Future):
-    def __init__(self, future_list, done_callback=None, pre_exception=None):
+    def __init__(self, future_list, done_callback=None, auto_id=True, pre_exception=None):
         super().__init__(None, done_callback, pre_exception)
+        self._auto_id = auto_id
         self._future_list = future_list
         self._response = []
 
     def result(self, **kwargs):
         self.exception()
         with self._condition:
             to = kwargs.get("timeout", None)
@@ -235,15 +240,15 @@
                 future.exception()
 
     def on_response(self, response):
         for raw in response:
             if raw.status.error_code != 0:
                 raise MilvusException(raw.status.error_code, raw.status.reason)
 
-        return ChunkedQueryResult(response)
+        return ChunkedQueryResult(response, self._auto_id)
 
 
 class MutationFuture(Future):
     def on_response(self, response):
         status = response.status
         if status.error_code == 0:
             return MutationResult(response)
```

### Comparing `pymilvus-2.2.9/pymilvus/client/blob.py` & `pymilvus-2.3.0b1/pymilvus/client/blob.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/pymilvus/client/check.py` & `pymilvus-2.3.0b1/pymilvus/client/check.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import sys
 import datetime
 from typing import Any, Union
 from ..exceptions import ParamError
 from ..grpc_gen import milvus_pb2 as milvus_types
 from .singleton_utils import Singleton
+from .utils import (
+    valid_index_types,
+    valid_binary_index_types,
+    valid_index_params_keys,
+)
 
 
 def is_legal_address(addr: Any) -> bool:
     if not isinstance(addr, str):
         return False
 
     a = addr.split(":")
@@ -91,19 +96,14 @@
     return isinstance(index_size, int)
 
 
 def is_legal_table_name(table_name: Any) -> bool:
     return table_name and isinstance(table_name, str)
 
 
-def is_legal_db_name(db_name: Any) -> bool:
-    # you can connect to the default database "".
-    return isinstance(db_name, str)
-
-
 def is_legal_field_name(field_name: Any) -> bool:
     return field_name and isinstance(field_name, str)
 
 
 def is_legal_nlist(nlist: Any) -> bool:
     return not isinstance(nlist, bool) and isinstance(nlist, int)
 
@@ -164,16 +164,18 @@
 def is_legal_partition_name(tag: Any) -> bool:
     return tag is not None and isinstance(tag, str)
 
 
 def is_legal_limit(limit: Any) -> bool:
     return isinstance(limit, int) and limit > 0
 
+
 def is_legal_anns_field(field: Any) -> bool:
-    return field is None or isinstance(field, str)
+    return field and isinstance(field, str)
+
 
 def is_legal_search_data(data: Any) -> bool:
     import numpy as np
     if not isinstance(data, (list, np.ndarray)):
         return False
 
     for vector in data:
@@ -213,25 +215,26 @@
     return True
 
 def is_legal_replica_number(replica_number: int) -> bool:
     return isinstance(replica_number, int)
 
 # https://milvus.io/cn/docs/v1.0.0/metric.md#floating
 def is_legal_index_metric_type(index_type: str, metric_type: str) -> bool:
-    if index_type not in ("FLAT",
+    if index_type not in ("GPU_FLAT",
+                          "GPU_IVF_FLAT",
+                          "GPU_IVF_SQ8",
+                          "GPU_IVF_PQ",
+                          "RAFT_IVF_FLAT",
+                          "RAFT_IVF_PQ",
+                          "FLAT",
                           "IVF_FLAT",
                           "IVF_SQ8",
-                          # "IVF_SQ8_HYBRID",
                           "IVF_PQ",
                           "HNSW",
-                          # "NSG",
                           "ANNOY",
-                          "RHNSW_FLAT",
-                          "RHNSW_PQ",
-                          "RHNSW_SQ",
                           "AUTOINDEX",
                           "DISKANN"):
         return False
     if metric_type not in ("L2", "IP"):
         return False
     return True
 
@@ -256,15 +259,16 @@
 
 
 def is_legal_travel_timestamp(ts: Any) -> bool:
     return isinstance(ts, int) and ts >= 0
 
 
 def is_legal_guarantee_timestamp(ts: Any) -> bool:
-    return ts is None or isinstance(ts, int) and ts >= 0
+    return isinstance(ts, int) and ts >= 0
+
 
 def is_legal_user(user) -> bool:
     return isinstance(user, str)
 
 
 def is_legal_password(password) -> bool:
     return isinstance(password, str)
@@ -307,15 +311,14 @@
     return operate_privilege_type in \
             (milvus_types.OperatePrivilegeType.Grant, milvus_types.OperatePrivilegeType.Revoke)
 
 
 class ParamChecker(metaclass=Singleton):
     def __init__(self) -> None:
         self.check_dict = {
-            "db_name": is_legal_db_name,
             "collection_name": is_legal_table_name,
             "field_name": is_legal_field_name,
             "dimension": is_legal_dimension,
             "index_file_size": is_legal_index_size,
             "topk": is_legal_topk,
             "ids": is_legal_ids,
             "nprobe": is_legal_nprobe,
@@ -348,18 +351,46 @@
     def check(self, key, value):
         if key in self.check_dict:
             if not self.check_dict[key](value):
                 _raise_param_error(key, value)
         else:
             raise ParamError(message=f"unknown param `{key}`")
 
-
 def _get_param_checker():
     return ParamChecker()
 
-
 def check_pass_param(*_args: Any, **kwargs: Any) -> None:  # pylint: disable=too-many-statements
     if kwargs is None:
         raise ParamError(message="Param should not be None")
     checker = _get_param_checker()
     for key, value in kwargs.items():
         checker.check(key, value)
+
+
+def check_index_params(params):
+    params = params or {}
+    if not isinstance(params, dict):
+        raise ParamError(message="Params must be a dictionary type")
+    # params preliminary validate
+    if 'index_type' not in params:
+        raise ParamError(message="Params must contains key: 'index_type'")
+    if 'params' not in params:
+        raise ParamError(message="Params must contains key: 'params'")
+    if 'metric_type' not in params:
+        raise ParamError(message="Params must contains key: 'metric_type'")
+    if not isinstance(params['params'], dict):
+        raise ParamError(message="Params['params'] must be a dictionary type")
+    if params['index_type'] not in valid_index_types:
+        raise ParamError(message=f"Invalid index_type: {params['index_type']}, which must be one of: {str(valid_index_types)}")
+    for k in params['params'].keys():
+        if k not in valid_index_params_keys:
+            raise ParamError(message=f"Invalid params['params'].key: {k}")
+    for v in params['params'].values():
+        if not isinstance(v, int):
+            raise ParamError(message=f"Invalid params['params'].value: {v}, which must be an integer")
+    # filter invalid metric type
+    if params['index_type'] in valid_binary_index_types:
+        if not is_legal_binary_index_metric_type(params['index_type'], params['metric_type']):
+            raise ParamError(message=f"Invalid metric_type: {params['metric_type']}, which does not match the index type: {params['index_type']}")
+    else:
+        if not is_legal_index_metric_type(params['index_type'], params['metric_type']):
+            raise ParamError(message=f"Invalid metric_type: {params['metric_type']}, which does not match the index type: {params['index_type']}")
```

### Comparing `pymilvus-2.2.9/pymilvus/client/grpc_handler.py` & `pymilvus-2.3.0b1/pymilvus/client/grpc_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 import time
 import json
 import copy
 import base64
 from urllib import parse
-import socket
+
 import grpc
+import numpy as np
 from grpc._cython import cygrpc
 
 from ..grpc_gen import milvus_pb2_grpc
 from ..grpc_gen import milvus_pb2 as milvus_types
 from ..grpc_gen import common_pb2
 
 from .abstract import CollectionSchema, ChunkedQueryResult, MutationResult
 from .check import (
     is_legal_host,
     is_legal_port,
     check_pass_param,
+    check_index_params,
 )
 from .prepare import Prepare
 from .types import (
     Status,
     IndexState,
     LoadState,
     DataType,
     CompactionState,
     State,
     CompactionPlans,
     Plan,
+    get_consistency_level,
     Replica, Shard, Group,
     GrantInfo, UserInfo, RoleInfo,
     BulkInsertState,
     ResourceGroupInfo,
 )
 
 from .utils import (
     check_invalid_binary_vector,
-    len_of,
-    get_server_type,
+    len_of
 )
 
-from ..settings import Config
+from ..settings import DefaultConfig as config
+from .configs import DefaultConfigs
 from . import ts_utils
 from . import interceptor
-from . import entity_helper
 
 from .asynch import (
     SearchFuture,
     MutationFuture,
     CreateIndexFuture,
     FlushFuture,
     LoadPartitionsFuture,
@@ -57,32 +59,27 @@
     ExceptionsMessage,
     ParamError,
     DescribeCollectionException,
     MilvusException,
     AmbiguousIndexName,
 )
 
-from ..decorators import retry_on_rpc_failure, upgrade_reminder
+from ..decorators import retry_on_rpc_failure
 
 
 class GrpcHandler:
-
-    # pylint: disable=too-many-instance-attributes
-
-    def __init__(self, uri=Config.GRPC_URI, host="", port="", channel=None, **kwargs):
+    def __init__(self, uri=config.GRPC_URI, host="", port="", channel=None, **kwargs):
         self._stub = None
         self._channel = channel
 
         addr = kwargs.get("address")
         self._address = addr if addr is not None else self.__get_address(uri, host, port)
         self._log_level = None
         self._request_id = None
-        self._user = kwargs.get("user", None)
         self._set_authorization(**kwargs)
-        self._setup_db_interceptor(kwargs.get("db_name", None))
         self._setup_grpc_channel()
 
     def __get_address(self, uri: str, host: str, port: str) -> str:
         if host != "" and port != "" and is_legal_host(host) and is_legal_port(port):
             return f"{host}:{port}"
 
         try:
@@ -99,64 +96,41 @@
         self._client_pem_path = kwargs.get("client_pem_path", "")
         self._client_key_path = kwargs.get("client_key_path", "")
         self._ca_pem_path = kwargs.get("ca_pem_path", "")
         self._server_pem_path = kwargs.get("server_pem_path", "")
         self._server_name = kwargs.get("server_name", "")
 
         self._authorization_interceptor = None
-        self._setup_authorization_interceptor(kwargs.get("user", None),
-                                              kwargs.get("password", None),
-                                              kwargs.get("token", None))
+        self._setup_authorization_interceptor(kwargs.get("user", None), kwargs.get("password", None))
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
     def _wait_for_channel_ready(self, timeout=10):
         if self._channel is not None:
             try:
                 grpc.channel_ready_future(self._channel).result(timeout=timeout)
-                self._setup_identifier_interceptor(self._user)
                 return
-            except (grpc.FutureTimeoutError,  MilvusException) as e:
+            except grpc.FutureTimeoutError as e:
                 raise MilvusException(Status.CONNECT_FAILED,
                                       f'Fail connecting to server on {self._address}. Timeout') from e
 
         raise MilvusException(Status.CONNECT_FAILED, 'No channel in handler, please setup grpc channel first')
 
     def close(self):
         self._channel.close()
 
-    def reset_db_name(self, db_name):
-        self._setup_db_interceptor(db_name)
-        self._setup_grpc_channel()
-        self._setup_identifier_interceptor(self._user)
-
-    def _setup_authorization_interceptor(self, user, password, token):
-        keys = []
-        values = []
-        if token:
-            authorization = base64.b64encode(f"{token}".encode('utf-8'))
-            keys.append("authorization")
-            values.append(authorization)
-        elif user and password:
+    def _setup_authorization_interceptor(self, user, password):
+        if user and password:
             authorization = base64.b64encode(f"{user}:{password}".encode('utf-8'))
-            keys.append("authorization")
-            values.append(authorization)
-        if len(keys) > 0 and len(values) > 0:
-            self._authorization_interceptor = interceptor.header_adder_interceptor(keys, values)
-
-    def _setup_db_interceptor(self, db_name):
-        if db_name is None:
-            self._db_interceptor = None
-        else:
-            check_pass_param(db_name=db_name)
-            self._db_interceptor = interceptor.header_adder_interceptor(["dbname"], [db_name])
+            key = "authorization"
+            self._authorization_interceptor = interceptor.header_adder_interceptor(key, authorization)
 
     def _setup_grpc_channel(self):
         """ Create a ddl grpc channel """
         if self._channel is None:
             opts = [(cygrpc.ChannelArgKey.max_send_message_length, -1),
                     (cygrpc.ChannelArgKey.max_receive_message_length, -1),
                     ('grpc.enable_retries', 1),
@@ -191,61 +165,48 @@
                     creds,
                     options=opts
                 )
         # avoid to add duplicate headers.
         self._final_channel = self._channel
         if self._authorization_interceptor:
             self._final_channel = grpc.intercept_channel(self._final_channel, self._authorization_interceptor)
-        if self._db_interceptor:
-            self._final_channel = grpc.intercept_channel(self._final_channel, self._db_interceptor)
         if self._log_level:
-            log_level_interceptor = interceptor.header_adder_interceptor(["log_level"], [self._log_level])
+            log_level_interceptor = interceptor.header_adder_interceptor("log_level", self._log_level)
             self._final_channel = grpc.intercept_channel(self._final_channel, log_level_interceptor)
             self._log_level = None
         if self._request_id:
-            request_id_interceptor = interceptor.header_adder_interceptor(["client_request_id"], [self._request_id])
+            request_id_interceptor = interceptor.header_adder_interceptor("client_request_id", self._request_id)
             self._final_channel = grpc.intercept_channel(self._final_channel, request_id_interceptor)
             self._request_id = None
         self._stub = milvus_pb2_grpc.MilvusServiceStub(self._final_channel)
 
     def set_onetime_loglevel(self, log_level):
         self._log_level = log_level
         self._setup_grpc_channel()
 
     def set_onetime_request_id(self, req_id):
         self._request_id = req_id
         self._setup_grpc_channel()
 
-    def _setup_identifier_interceptor(self, user):
-        host = socket.gethostname()
-        self._identifier = self.__internal_register(user, host)
-        self._identifier_interceptor = interceptor.header_adder_interceptor(["identifier"], [str(self._identifier)])
-        self._final_channel = grpc.intercept_channel(self._final_channel, self._identifier_interceptor)
-        self._stub = milvus_pb2_grpc.MilvusServiceStub(self._final_channel)
-
     @property
     def server_address(self):
         """ Server network address """
         return self._address
 
-    def get_server_type(self):
-        return get_server_type(self.server_address.split(':')[0])
-
     def reset_password(self, user, old_password, new_password, timeout=None):
         """
         reset password and then setup the grpc channel.
         """
         self.update_password(user, old_password, new_password, timeout=timeout)
-        self._setup_authorization_interceptor(user, new_password, None)
+        self._setup_authorization_interceptor(user, new_password)
         self._setup_grpc_channel()
 
     @retry_on_rpc_failure()
-    def create_collection(self, collection_name, fields, timeout=None, **kwargs):
-        check_pass_param(collection_name=collection_name)
-        request = Prepare.create_collection_request(collection_name, fields, **kwargs)
+    def create_collection(self, collection_name, fields, shards_num=2, timeout=None, **kwargs):
+        request = Prepare.create_collection_request(collection_name, fields, shards_num=shards_num, **kwargs)
 
         rf = self._stub.CreateCollection.future(request, timeout=timeout)
         if kwargs.get("_async", False):
             return rf
         status = rf.result()
         if status.error_code != 0:
             raise MilvusException(status.error_code, status.reason)
@@ -388,75 +349,47 @@
         response = future.result()
         status = response.status
         if status.error_code == 0:
             return response.stats
 
         raise MilvusException(status.error_code, status.reason)
 
-    def _prepare_row_insert_or_upsert_request(self, collection_name, rows, partition_name=None, timeout=None,
-                                              is_insert=True, **kwargs):
-        if not isinstance(rows, list):
-            raise ParamError(message="None rows, please provide valid row data.")
+    def _prepare_batch_insert_or_upsert_request(self, collection_name, entities, partition_name=None, timeout=None, isInsert=True, **kwargs):
+        param = kwargs.get('insert_param', None)
 
-        collection_schema = kwargs.get("schema", None)
-        if not collection_schema:
-            collection_schema = self.describe_collection(
-                collection_name, timeout=timeout, **kwargs)
+        if not isInsert:
+            param = kwargs.get('upsert_param', None)
 
-        fields_info = collection_schema["fields"]
-        enable_dynamic = collection_schema.get("enable_dynamic_field", False)
-        request = Prepare.row_insert_or_upsert_param(collection_name, rows, partition_name, fields_info, is_insert,
-                                                     enable_dynamic=enable_dynamic)
-        return request
-
-    def _prepare_batch_insert_request(self, collection_name, entities, partition_name=None, timeout=None, **kwargs):
-        insert_param = kwargs.get('insert_param', None)
-
-        if insert_param and not isinstance(insert_param, milvus_types.RowBatch):
-            raise ParamError(message="The value of key 'insert_param' is invalid")
+        if param and not isinstance(param, milvus_types.RowBatch):
+            if isInsert:
+                raise ParamError(message="The value of key 'insert_param' is invalid")
+            raise ParamError(message="The value of key 'upsert_param' is invalid")
         if not isinstance(entities, list):
             raise ParamError(message="None entities, please provide valid entities.")
 
         collection_schema = kwargs.get("schema", None)
         if not collection_schema:
-            collection_schema = self.describe_collection(collection_name, timeout=timeout, **kwargs)
+            collection_schema = self.describe_collection(
+                collection_name, timeout=timeout, **kwargs)
 
         fields_info = collection_schema["fields"]
 
-        request = insert_param if insert_param \
-            else Prepare.batch_insert_param(collection_name, entities, partition_name, fields_info)
+        request = param if param \
+            else Prepare.batch_insert_or_upsert_param(collection_name, entities, partition_name, fields_info, isInsert)
 
         return request
 
-
-    @retry_on_rpc_failure()
-    def insert_rows(self, collection_name, entities, partition_name=None, timeout=None, **kwargs):
-        if isinstance(entities, dict):
-            entities = [entities]
-        try:
-            request = self._prepare_row_insert_or_upsert_request(
-                collection_name, entities, partition_name, timeout, **kwargs)
-            rf = self._stub.Insert.future(request, timeout=timeout)
-            response = rf.result()
-            if response.status.error_code == 0:
-                m = MutationResult(response)
-                ts_utils.update_collection_ts(collection_name, m.timestamp)
-                return m
-
-            raise MilvusException(response.status.error_code, response.status.reason)
-        except Exception as err:
-            raise err
-
     @retry_on_rpc_failure()
     def batch_insert(self, collection_name, entities, partition_name=None, timeout=None, **kwargs):
         if not check_invalid_binary_vector(entities):
             raise ParamError(message="Invalid binary vector data exists")
 
         try:
-            request = self._prepare_batch_insert_request(collection_name, entities, partition_name, timeout, **kwargs)
+            request = self._prepare_batch_insert_or_upsert_request(
+                collection_name, entities, partition_name, timeout, **kwargs)
             rf = self._stub.Insert.future(request, timeout=timeout)
             if kwargs.get("_async", False) is True:
                 cb = kwargs.get("_callback", None)
                 f = MutationFuture(rf, cb, timeout=timeout, **kwargs)
                 f.add_callback(ts_utils.update_ts_on_mutation(collection_name))
                 return f
 
@@ -493,59 +426,100 @@
 
             raise MilvusException(response.status.error_code, response.status.reason)
         except Exception as err:
             if kwargs.get("_async", False):
                 return MutationFuture(None, None, err)
             raise err
 
+    @retry_on_rpc_failure()
+    def upsert(self, collection_name, entities, partition_name=None, timeout=None, **kwargs):
+        if not check_invalid_binary_vector(entities):
+            raise ParamError(message="Invalid binary vector data exists")
+
+        try:
+            request = self._prepare_batch_insert_or_upsert_request(
+                collection_name, entities, partition_name, timeout, False, **kwargs)
+            rf = self._stub.Upsert.future(request, timeout=timeout)
+            if kwargs.get("_async", False) is True:
+                cb = kwargs.get("_callback", None)
+                f = MutationFuture(rf, cb, timeout=timeout, **kwargs)
+                f.add_callback(ts_utils.update_ts_on_mutation(collection_name))
+                return f
+
+            response = rf.result()
+            if response.status.error_code == 0:
+                m = MutationResult(response)
+                ts_utils.update_collection_ts(collection_name, m.timestamp)
+                return m
+
+            raise MilvusException(
+                response.status.error_code, response.status.reason)
+        except Exception as err:
+            if kwargs.get("_async", False):
+                return MutationFuture(None, None, err)
+            raise err
+
     def _execute_search_requests(self, requests, timeout=None, **kwargs):
+        auto_id = kwargs.get("auto_id", True)
+
         try:
             if kwargs.get("_async", False):
                 futures = []
                 for request in requests:
                     ft = self._stub.Search.future(request, timeout=timeout)
                     futures.append(ft)
                 func = kwargs.get("_callback", None)
-                return ChunkedSearchFuture(futures, func)
+                return ChunkedSearchFuture(futures, func, auto_id)
 
             raws = []
             for request in requests:
                 response = self._stub.Search(request, timeout=timeout)
 
                 if response.status.error_code != 0:
                     raise MilvusException(response.status.error_code, response.status.reason)
 
                 raws.append(response)
             round_decimal = kwargs.get("round_decimal", -1)
-            return ChunkedQueryResult(raws, round_decimal)
+            return ChunkedQueryResult(raws, auto_id, round_decimal)
 
         except Exception as pre_err:
             if kwargs.get("_async", False):
-                return SearchFuture(None, None, pre_err)
+                return SearchFuture(None, None, True, pre_err)
             raise pre_err
 
     @retry_on_rpc_failure(retry_on_deadline=False)
     def search(self, collection_name, data, anns_field, param, limit,
                expression=None, partition_names=None, output_fields=None,
-               round_decimal=-1, timeout=None, **kwargs):
+               round_decimal=-1, timeout=None, schema=None, **kwargs):
         check_pass_param(
             limit=limit,
             round_decimal=round_decimal,
             anns_field=anns_field,
             search_data=data,
             partition_name_array=partition_names,
             output_fields=output_fields,
             travel_timestamp=kwargs.get("travel_timestamp", 0),
-            guarantee_timestamp=kwargs.get("guarantee_timestamp", None)
+            guarantee_timestamp=kwargs.get("guarantee_timestamp", 0)
         )
 
-        requests = Prepare.search_requests_with_expr(collection_name, data, anns_field, param, limit,
+        if schema is None:
+            schema = self.describe_collection(collection_name, timeout=timeout, **kwargs)
+
+        consistency_level = schema["consistency_level"]
+        # overwrite the consistency level defined when user created the collection
+        consistency_level = get_consistency_level(kwargs.get("consistency_level", consistency_level))
+
+        ts_utils.construct_guarantee_ts(consistency_level, collection_name, kwargs)
+
+        requests = Prepare.search_requests_with_expr(collection_name, data, anns_field, param, limit, schema,
                                                      expression, partition_names, output_fields, round_decimal,
                                                      **kwargs)
-        return self._execute_search_requests(requests, timeout, round_decimal=round_decimal, **kwargs)
+
+        auto_id = schema["auto_id"]
+        return self._execute_search_requests(requests, timeout, round_decimal=round_decimal, auto_id=auto_id, **kwargs)
 
     @retry_on_rpc_failure()
     def get_query_segment_info(self, collection_name, timeout=30, **kwargs):
         req = Prepare.get_query_segment_info_request(collection_name)
         future = self._stub.GetQuerySegmentInfo.future(req, timeout=timeout)
         response = future.result()
         status = response.status
@@ -578,26 +552,28 @@
         response = rf.result()
         if response.error_code != 0:
             raise MilvusException(response.error_code, response.reason)
 
     @retry_on_rpc_failure()
     def create_index(self, collection_name, field_name, params, timeout=None, **kwargs):
         # for historical reason, index_name contained in kwargs.
-        index_name = kwargs.pop("index_name", Config.IndexName)
+        index_name = kwargs.pop("index_name", DefaultConfigs.IndexName)
         copy_kwargs = copy.deepcopy(kwargs)
 
         collection_desc = self.describe_collection(collection_name, timeout=timeout, **copy_kwargs)
 
         valid_field = False
         for fields in collection_desc["fields"]:
             if field_name != fields["name"]:
                 continue
             valid_field = True
             if fields["type"] != DataType.FLOAT_VECTOR and fields["type"] != DataType.BINARY_VECTOR:
                 break
+            # check index params on vector field.
+            check_index_params(params)
 
         if not valid_field:
             raise MilvusException(message=f"cannot create index on non-existed field: {field_name}")
 
         # sync flush
         _async = kwargs.get("_async", False)
         kwargs["_async"] = False
@@ -676,16 +652,15 @@
         request = Prepare.describe_index_request(collection_name, index_name)
         rf = self._stub.DescribeIndex.future(request, timeout=timeout)
         response = rf.result()
         status = response.status
         if status.error_code == 0:
             if len(response.index_descriptions) == 1:
                 index_desc = response.index_descriptions[0]
-                return {'total_rows': index_desc.total_rows, 'indexed_rows': index_desc.indexed_rows,
-                        "pending_index_rows": index_desc.pending_index_rows}
+                return {'total_rows': index_desc.total_rows, 'indexed_rows': index_desc.indexed_rows}
             raise AmbiguousIndexName(message=ExceptionsMessage.AmbiguousIndexName)
         raise MilvusException(status.error_code, status.reason)
 
     @retry_on_rpc_failure()
     def get_index_state(self, collection_name: str, index_name: str, timeout=None, **kwargs):
         request = Prepare.describe_index_request(collection_name, index_name)
         rf = self._stub.DescribeIndex.future(request, timeout=timeout)
@@ -749,15 +724,15 @@
         def can_loop(t) -> bool:
             return True if timeout is None else t <= (start + timeout)
 
         while can_loop(time.time()):
             progress = self.get_loading_progress(collection_name, timeout=timeout)
             if progress >= 100:
                 return
-            time.sleep(Config.WaitTimeDurationWhenLoad)
+            time.sleep(DefaultConfigs.WaitTimeDurationWhenLoad)
         raise MilvusException(message=f"wait for loading collection timeout, collection: {collection_name}")
 
     @retry_on_rpc_failure()
     def release_collection(self, collection_name, timeout=None):
         check_pass_param(collection_name=collection_name)
         request = Prepare.release_collection("", collection_name)
         rf = self._stub.ReleaseCollection.future(request, timeout=timeout)
@@ -805,48 +780,26 @@
         def can_loop(t) -> bool:
             return True if timeout is None else t <= (start + timeout)
 
         while can_loop(time.time()):
             progress = self.get_loading_progress(collection_name, partition_names, timeout=timeout)
             if progress >= 100:
                 return
-            time.sleep(Config.WaitTimeDurationWhenLoad)
+            time.sleep(DefaultConfigs.WaitTimeDurationWhenLoad)
         raise MilvusException(message=f"wait for loading partition timeout, collection: {collection_name}, partitions: {partition_names}")
 
     @retry_on_rpc_failure()
     def get_loading_progress(self, collection_name, partition_names=None, timeout=None):
         request = Prepare.get_loading_progress(collection_name, partition_names)
         response = self._stub.GetLoadingProgress.future(request, timeout=timeout).result()
         if response.status.error_code != 0:
             raise MilvusException(response.status.error_code, response.status.reason)
         return response.progress
 
     @retry_on_rpc_failure()
-    def create_database(self, db_name, timeout=None):
-        request = Prepare.create_database_req(db_name)
-        status = self._stub.CreateDatabase(request, timeout=timeout)
-        if status.error_code != 0:
-            raise MilvusException(status.error_code, status.reason)
-
-    @retry_on_rpc_failure()
-    def drop_database(self, db_name, timeout=None):
-        request = Prepare.drop_database_req(db_name)
-        status = self._stub.DropDatabase(request, timeout=timeout)
-        if status.error_code != 0:
-            raise MilvusException(status.error_code, status.reason)
-
-    @retry_on_rpc_failure()
-    def list_database(self, timeout=None):
-        request = Prepare.list_database_req()
-        response = self._stub.ListDatabases(request, timeout=timeout)
-        if response.status.error_code != 0:
-            raise MilvusException(response.status.error_code, response.status.reason)
-        return list(response.db_names)
-
-    @retry_on_rpc_failure()
     def get_load_state(self, collection_name, partition_names=None, timeout=None):
         request = Prepare.get_load_state(collection_name, partition_names)
         response = self._stub.GetLoadState.future(request, timeout=timeout).result()
         if response.status.error_code != 0:
             raise MilvusException(response.status.error_code, response.status.reason)
         return LoadState(response.state)
 
@@ -974,14 +927,22 @@
         future = self._stub.Retrieve.future(request, timeout=timeout)
         return future.result()
 
     @retry_on_rpc_failure()
     def query(self, collection_name, expr, output_fields=None, partition_names=None, timeout=None, **kwargs):
         if output_fields is not None and not isinstance(output_fields, (list,)):
             raise ParamError(message="Invalid query format. 'output_fields' must be a list")
+        collection_schema = kwargs.get("schema", None)
+        if not collection_schema:
+            collection_schema = self.describe_collection(collection_name, timeout)
+        consistency_level = collection_schema["consistency_level"]
+        # overwrite the consistency level defined when user created the collection
+        consistency_level = get_consistency_level(kwargs.get("consistency_level", consistency_level))
+
+        ts_utils.construct_guarantee_ts(consistency_level, collection_name, kwargs)
         request = Prepare.query_request(collection_name, expr, output_fields, partition_names, **kwargs)
 
         future = self._stub.Query.future(request, timeout=timeout)
         response = future.result()
         if response.status.error_code == Status.EMPTY_COLLECTION:
             return []
         if response.status.error_code != Status.SUCCESS:
@@ -994,21 +955,47 @@
 
         # check if all lists are of the same length
         it = iter(response.fields_data)
         num_entities = len_of(next(it))
         if not all(len_of(field_data) == num_entities for field_data in it):
             raise MilvusException(message="The length of fields data is inconsistent")
 
-        _, dynamic_fields = entity_helper.extract_dynamic_field_from_result(response)
-
+        # transpose
         results = []
         for index in range(0, num_entities):
-            entity_row_data = entity_helper.extract_row_data_from_fields_data(response.fields_data, index,
-                                                                              dynamic_fields)
-            results.append(entity_row_data)
+            result = {}
+            for field_data in response.fields_data:
+                if field_data.type == DataType.BOOL:
+                    result[field_data.field_name] = field_data.scalars.bool_data.data[index]
+                elif field_data.type in (DataType.INT8, DataType.INT16, DataType.INT32):
+                    result[field_data.field_name] = field_data.scalars.int_data.data[index]
+                elif field_data.type == DataType.INT64:
+                    result[field_data.field_name] = field_data.scalars.long_data.data[index]
+                elif field_data.type == DataType.FLOAT:
+                    result[field_data.field_name] = np.single(field_data.scalars.float_data.data[index])
+                elif field_data.type == DataType.DOUBLE:
+                    result[field_data.field_name] = field_data.scalars.double_data.data[index]
+                elif field_data.type == DataType.VARCHAR:
+                    result[field_data.field_name] = field_data.scalars.string_data.data[index]
+                elif field_data.type == DataType.STRING:
+                    raise MilvusException(message="Not support string yet")
+                    # result[field_data.field_name] = field_data.scalars.string_data.data[index]
+                elif field_data.type == DataType.FLOAT_VECTOR:
+                    dim = field_data.vectors.dim
+                    start_pos = index * dim
+                    end_pos = index * dim + dim
+                    result[field_data.field_name] = [np.single(x) for x in
+                                                     field_data.vectors.float_vector.data[start_pos:end_pos]]
+                elif field_data.type == DataType.BINARY_VECTOR:
+                    dim = field_data.vectors.dim
+                    start_pos = index * (int(dim / 8))
+                    end_pos = (index + 1) * (int(dim / 8))
+                    result[field_data.field_name] = field_data.vectors.binary_vector[start_pos:end_pos]
+            results.append(result)
+
         return results
 
     @retry_on_rpc_failure()
     def load_balance(self, collection_name: str, src_node_id, dst_node_ids, sealed_segment_ids, timeout=None, **kwargs):
         req = Prepare.load_balance_request(collection_name, src_node_id, dst_node_ids, sealed_segment_ids)
         future = self._stub.LoadBalance.future(req, timeout=timeout)
         status = future.result()
@@ -1217,41 +1204,41 @@
         req = Prepare.select_user_request(None, include_role_info)
         resp = self._stub.SelectUser(req, wait_for_ready=True, timeout=timeout)
         if resp.status.error_code != 0:
             raise MilvusException(resp.status.error_code, resp.status.reason)
         return UserInfo(resp.results)
 
     @retry_on_rpc_failure()
-    def grant_privilege(self, role_name, object, object_name, privilege, db_name, timeout=None, **kwargs):
-        req = Prepare.operate_privilege_request(role_name, object, object_name, privilege, db_name,
+    def grant_privilege(self, role_name, object, object_name, privilege, timeout=None, **kwargs):
+        req = Prepare.operate_privilege_request(role_name, object, object_name, privilege,
                                                 milvus_types.OperatePrivilegeType.Grant)
         resp = self._stub.OperatePrivilege(req, wait_for_ready=True, timeout=timeout)
         if resp.error_code != 0:
             raise MilvusException(resp.error_code, resp.reason)
 
     @retry_on_rpc_failure()
-    def revoke_privilege(self, role_name, object, object_name, privilege, db_name, timeout=None, **kwargs):
-        req = Prepare.operate_privilege_request(role_name, object, object_name, privilege, db_name,
+    def revoke_privilege(self, role_name, object, object_name, privilege, timeout=None, **kwargs):
+        req = Prepare.operate_privilege_request(role_name, object, object_name, privilege,
                                                 milvus_types.OperatePrivilegeType.Revoke)
         resp = self._stub.OperatePrivilege(req, wait_for_ready=True, timeout=timeout)
         if resp.error_code != 0:
             raise MilvusException(resp.error_code, resp.reason)
 
     @retry_on_rpc_failure()
-    def select_grant_for_one_role(self, role_name, db_name, timeout=None, **kwargs):
-        req = Prepare.select_grant_request(role_name, None, None, db_name)
+    def select_grant_for_one_role(self, role_name, timeout=None, **kwargs):
+        req = Prepare.select_grant_request(role_name, None, None)
         resp = self._stub.SelectGrant(req, wait_for_ready=True, timeout=timeout)
         if resp.status.error_code != 0:
             raise MilvusException(resp.status.error_code, resp.status.reason)
 
         return GrantInfo(resp.entities)
 
     @retry_on_rpc_failure()
-    def select_grant_for_role_and_object(self, role_name, object, object_name, db_name, timeout=None, **kwargs):
-        req = Prepare.select_grant_request(role_name, object, object_name, db_name)
+    def select_grant_for_role_and_object(self, role_name, object, object_name, timeout=None, **kwargs):
+        req = Prepare.select_grant_request(role_name, object, object_name)
         resp = self._stub.SelectGrant(req, wait_for_ready=True, timeout=timeout)
         if resp.status.error_code != 0:
             raise MilvusException(resp.status.error_code, resp.status.reason)
 
         return GrantInfo(resp.entities)
 
     @retry_on_rpc_failure()
@@ -1302,61 +1289,7 @@
 
     @retry_on_rpc_failure()
     def transfer_replica(self, source, target, collection_name, num_replica, timeout=None, **kwargs):
         req = Prepare.transfer_replica(source, target, collection_name, num_replica)
         resp = self._stub.TransferReplica(req, wait_for_ready=True, timeout=timeout)
         if resp.error_code != 0:
             raise MilvusException(resp.error_code, resp.reason)
-
-    @retry_on_rpc_failure()
-    def get_flush_all_state(self, flush_all_ts, timeout=None, **kwargs):
-        req = Prepare.get_flush_all_state_request(flush_all_ts)
-        response = self._stub.GetFlushAllState(req, timeout=timeout)
-        status = response.status
-        if status.error_code == 0:
-            return response.flushed
-        raise MilvusException(status.error_code, status.reason)
-
-    def _wait_for_flush_all(self, flush_all_ts, timeout=None, **kwargs):
-        flush_ret = False
-        start = time.time()
-        while not flush_ret:
-            flush_ret = self.get_flush_all_state(flush_all_ts, timeout, **kwargs)
-            end = time.time()
-            if timeout is not None:
-                if end - start > timeout:
-                    raise MilvusException(message=f"wait for flush all timeout, flush_all_ts: {flush_all_ts}")
-
-            if not flush_ret:
-                time.sleep(5)
-
-    @retry_on_rpc_failure()
-    def flush_all(self, timeout=None, **kwargs):
-        request = Prepare.flush_all_request()
-        future = self._stub.FlushAll.future(request, timeout=timeout)
-        response = future.result()
-        if response.status.error_code != 0:
-            raise MilvusException(response.status.error_code, response.status.reason)
-
-        def _check():
-            self._wait_for_flush_all(response.flush_all_ts, timeout, **kwargs)
-
-        if kwargs.get("_async", False):
-            flush_future = FlushFuture(future)
-            flush_future.add_callback(_check)
-
-            user_cb = kwargs.get("_callback", None)
-            if user_cb:
-                flush_future.add_callback(user_cb)
-
-            return flush_future
-
-        _check()
-
-    @retry_on_rpc_failure()
-    @upgrade_reminder
-    def __internal_register(self, user, host) -> int:
-        req = Prepare.register_request(user, host)
-        response = self._stub.Connect(request=req)
-        if response.status.error_code != common_pb2.Success:
-            raise MilvusException(response.status.error_code, response.status.reason)
-        return response.identifier
```

### Comparing `pymilvus-2.2.9/pymilvus/client/interceptor.py` & `pymilvus-2.3.0b1/pymilvus/client/interceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,21 +62,25 @@
 class _ClientCallDetails(
         collections.namedtuple(
             '_ClientCallDetails',
             ('method', 'timeout', 'metadata', 'credentials')),
         grpc.ClientCallDetails):
     pass
 
-def header_adder_interceptor(headers, values):
+
+def header_adder_interceptor(header, value):
+
     def intercept_call(client_call_details, request_iterator, request_streaming,
                        response_streaming):
         metadata = []
         if client_call_details.metadata is not None:
             metadata = list(client_call_details.metadata)
-        for item in zip(headers, values):
-            metadata.append(item)
+        metadata.append((
+            header,
+            value,
+        ))
         client_call_details = _ClientCallDetails(
             client_call_details.method, client_call_details.timeout, metadata,
             client_call_details.credentials)
         return client_call_details, request_iterator, None
 
     return create(intercept_call)
```

### Comparing `pymilvus-2.2.9/pymilvus/client/prepare.py` & `pymilvus-2.3.0b1/pymilvus/client/prepare.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,132 +1,99 @@
+import copy
 import base64
-import datetime
 from typing import Dict, Iterable, Union
 
 import ujson
 
 from . import blob
 from . import entity_helper
-from . import ts_utils
 from .check import check_pass_param, is_legal_collection_properties
 from .types import DataType, PlaceholderType, get_consistency_level
-from .utils import traverse_rows_info
+from .utils import traverse_info
 from .constants import DEFAULT_CONSISTENCY_LEVEL
 from ..exceptions import ParamError, DataNotMatchException, ExceptionsMessage
 from ..orm.schema import CollectionSchema
 
-from ..client import __version__
-
 from ..grpc_gen import common_pb2 as common_types
 from ..grpc_gen import schema_pb2 as schema_types
 from ..grpc_gen import milvus_pb2 as milvus_types
 
 
 class Prepare:
     @classmethod
     def create_collection_request(cls, collection_name: str, fields: Union[Dict[str, Iterable], CollectionSchema],
-                                  **kwargs) -> milvus_types.CreateCollectionRequest:
+                                  shards_num=2, **kwargs) -> milvus_types.CreateCollectionRequest:
         """
-        Args:
-            fields (Union(Dict[str, Iterable], CollectionSchema)).
+        :type fields: Union(Dict[str, Iterable], CollectionSchema)
+        :param fields: (Required)
 
-                {"fields": [
-                        {"name": "A", "type": DataType.INT32}
-                        {"name": "B", "type": DataType.INT64, "auto_id": True, "is_primary": True},
-                        {"name": "C", "type": DataType.FLOAT},
-                        {"name": "Vec", "type": DataType.FLOAT_VECTOR, "params": {"dim": 128}}]
-                }
+            `{"fields": [
+                    {"name": "A", "type": DataType.INT32}
+                    {"name": "B", "type": DataType.INT64, "auto_id": True, "is_primary": True},
+                    {"name": "C", "type": DataType.FLOAT},
+                    {"name": "Vec", "type": DataType.FLOAT_VECTOR, "params": {"dim": 128}}]
+            }`
 
-        Returns:
-            milvus_types.CreateCollectionRequest
+        :return: milvus_types.CreateCollectionRequest
         """
-
         if isinstance(fields, CollectionSchema):
-            schema = cls.get_schema_from_collection_schema(collection_name, fields, **kwargs)
+            schema = cls.get_schema_from_collection_schema(collection_name, fields, shards_num, **kwargs)
         else:
-            schema = cls.get_schema(collection_name, fields, **kwargs)
+            schema = cls.get_schema(collection_name, fields, shards_num, **kwargs)
 
         consistency_level = get_consistency_level(kwargs.get("consistency_level", DEFAULT_CONSISTENCY_LEVEL))
 
         req = milvus_types.CreateCollectionRequest(collection_name=collection_name,
-                                                   schema=bytes(schema.SerializeToString()),
-                                                   consistency_level=consistency_level)
+                                                    schema=bytes(schema.SerializeToString()),
+                                                    shards_num=shards_num,
+                                                    consistency_level=consistency_level)
 
         properties = kwargs.get("properties")
         if is_legal_collection_properties(properties):
             properties = [common_types.KeyValuePair(key=str(k), value=str(v)) for k, v in properties.items()]
             req.properties.extend(properties)
 
-        same_key = set(kwargs.keys()).intersection({"num_shards", "shards_num"})
-        if len(same_key) > 0:
-            if len(same_key) > 1:
-                raise ParamError(message="got both num_shards and shards_num in kwargs, expected only one of them")
-
-            num_shards = kwargs[list(same_key)[0]]
-            if not isinstance(num_shards, int):
-                raise ParamError(message=f"invalid num_shards type, got {type(num_shards)}, expected int")
-            req.shards_num = num_shards
-
-        num_partitions = kwargs.get("num_partitions", None)
-        if num_partitions is not None:
-            if not isinstance(num_partitions, int) or isinstance(num_partitions, bool):
-                raise ParamError(message=f"invalid num_partitions type, got {type(num_partitions)}, expected int")
-            if num_partitions < 1:
-                raise ParamError(
-                    message=f"The specified num_partitions should be greater than or equal to 1, got {num_partitions}")
-            req.num_partitions = num_partitions
-
         return req
 
     @classmethod
-    def get_schema_from_collection_schema(cls, collection_name: str, fields: CollectionSchema,
-                                          **kwargs) -> schema_types.CollectionSchema:
+    def get_schema_from_collection_schema(cls, collection_name: str, fields: CollectionSchema, shards_num=2, **kwargs) -> milvus_types.CreateCollectionRequest:
         coll_description = fields.description
         if not isinstance(coll_description, (str, bytes)):
-            raise ParamError(
-                message=f"description [{coll_description}] has type {type(coll_description).__name__},  but expected one of: bytes, str")
+            raise ParamError(message=f"description [{coll_description}] has type {type(coll_description).__name__},  but expected one of: bytes, str")
 
         schema = schema_types.CollectionSchema(name=collection_name,
                                                autoID=fields.auto_id,
-                                               description=coll_description,
-                                               enable_dynamic_field=fields.enable_dynamic_field)
+                                               description=coll_description)
         for f in fields.fields:
             field_schema = schema_types.FieldSchema(name=f.name,
                                                     data_type=f.dtype,
                                                     description=f.description,
                                                     is_primary_key=f.is_primary,
-                                                    autoID=f.auto_id,
-                                                    is_partition_key=f.is_partition_key,
-                                                    is_dynamic=f.is_dynamic)
+                                                    autoID=f.auto_id)
             for k, v in f.params.items():
                 kv_pair = common_types.KeyValuePair(key=str(k), value=str(v))
                 field_schema.type_params.append(kv_pair)
 
             schema.fields.append(field_schema)
         return schema
 
     @classmethod
-    def get_schema(cls, collection_name: str, fields: Dict[str, Iterable], **kwargs) -> schema_types.CollectionSchema:
+    def get_schema(cls, collection_name: str, fields: Dict[str, Iterable], shards_num=2, **kwargs) -> schema_types.CollectionSchema:
         if not isinstance(fields, dict):
             raise ParamError(message="Param fields must be a dict")
 
         all_fields = fields.get("fields")
         if all_fields is None:
             raise ParamError(message="Param fields must contain key 'fields'")
         if len(all_fields) == 0:
             raise ParamError(message="Param fields value cannot be empty")
 
-        enable_dynamic_field = kwargs.get("enable_dynamic_field", False)
-        if "enable_dynamic_field" in fields:
-            enable_dynamic_field = fields["enable_dynamic_field"]
-
         schema = schema_types.CollectionSchema(name=collection_name,
                                                autoID=False,
-                                               description=fields.get('description', ''),
-                                               enable_dynamic_field=enable_dynamic_field)
+                                               description=fields.get('description', ''))
 
         primary_field = None
         auto_id_field = None
         for field in all_fields:
             field_name = field.get('name')
             if field_name is None:
                 raise ParamError(message="You should specify the name of field!")
@@ -157,16 +124,15 @@
                     raise ParamError(message="int64 is the only supported type of automatic generated id")
                 auto_id_field = field_name
 
             field_schema = schema_types.FieldSchema(name=field_name,
                                                     data_type=data_type,
                                                     description=field.get('description', ''),
                                                     is_primary_key=is_primary,
-                                                    autoID=auto_id,
-                                                    is_partition_key=field.get("is_partition_key", False))
+                                                    autoID=auto_id)
 
             type_params = field.get('params', {})
             if not isinstance(type_params, dict):
                 raise ParamError(message="params should be dictionary type")
             kvs = [common_types.KeyValuePair(key=str(k), value=str(v)) for k, v in type_params.items()]
             field_schema.type_params.extend(kvs)
 
@@ -278,136 +244,30 @@
             raise ParamError(message="collection_name must be of str type")
         if not isinstance(partition_name, str):
             raise ParamError(message="partition_name must be of str type")
         return milvus_types.PartitionName(collection_name=collection_name,
                                           tag=partition_name)
 
     @classmethod
-    def row_insert_or_upsert_param(cls, collection_name, entities, partition_name, fields_info=None, is_insert=True,
-                                   enable_dynamic=False, **kwargs):
+    def batch_insert_or_upsert_param(cls, collection_name, entities, partition_name, fields_info=None, isInsert=True, **kwargs):
         # insert_request.hash_keys and upsert_request.hash_keys won't be filled in client. It will be filled in proxy.
 
-        tag = partition_name if isinstance(partition_name, str) else ""
+        tag = partition_name or "_default"  # should here?
         request = milvus_types.InsertRequest(collection_name=collection_name, partition_name=tag)
 
-        if not fields_info:
-            raise ParamError(message="Missing collection meta to validate entities")
-
-        _, _, auto_id_loc = traverse_rows_info(fields_info, entities)
-
-        meta_field = schema_types.FieldData()
-        fields_data, field_info_map = {}, {}
-        for field in fields_info:
-            if field.get("auto_id", False):
-                continue
-            field_name, field_type = field["name"], field["type"]
-            field_info_map[field_name] = field
-            field_data = schema_types.FieldData()
-            field_data.field_name = field_name
-            field_data.type = field_type
-            fields_data[field_name] = field_data
-
-        if enable_dynamic:
-            meta_field.is_dynamic, meta_field.type = True, DataType.JSON
-            field_info_map[meta_field.field_name] = meta_field
-            fields_data[meta_field.field_name] = meta_field
-
-        try:
-            for entity in entities:
-                json_dict = {}
-                for key in entity:
-                    if key in fields_data:
-                        field_info, field_data = field_info_map[key], fields_data[key]
-                        entity_helper.pack_field_value_to_field_data(entity[key], field_data, field_info)
-                    elif enable_dynamic:
-                        json_dict[key] = entity[key]
-
-                if enable_dynamic:
-                    json_value = entity_helper.convert_to_json(json_dict)
-                    meta_field.scalars.json_data.data.append(json_value)
-
-        except (TypeError, ValueError) as e:
-            raise DataNotMatchException(message=ExceptionsMessage.DataTypeInconsistent) from e
-
-        request.num_rows = len(entities)
-        for field in fields_info:
-            if not field.get("auto_id", False):
-                field_name = field["name"]
-                field_data = fields_data[field_name]
-                request.fields_data.append(field_data)
-
-        if enable_dynamic:
-            request.fields_data.append(meta_field)
-
-        if auto_id_loc is not None:
-            if enable_dynamic:
-                # len(fields_data) = len(fields_info) - 1(auto_ID) + 1 (dynamic_field)
-                if len(fields_data) != len(fields_info):
-                    raise ParamError(ExceptionsMessage.FieldsNumInconsistent)
-            # len(fields_data) = len(fields_info) - 1(auto_ID)
-            elif len(fields_data) + 1 != len(fields_info):
-                raise ParamError(ExceptionsMessage.FieldsNumInconsistent)
-        elif enable_dynamic:
-            if len(fields_data) != len(fields_info) + 1:
-                raise ParamError(ExceptionsMessage.FieldsNumInconsistent)
-        return request
-
-    @classmethod
-    def batch_insert_param(cls, collection_name, entities, partition_name, fields_info=None, **kwargs):
-        # insert_request.hash_keys won't be filled in client. It will be filled in proxy.
-
-        tag = partition_name if isinstance(partition_name, str) else ""
-        insert_request = milvus_types.InsertRequest(collection_name=collection_name, partition_name=tag)
+        if not isInsert:
+            request = milvus_types.UpsertRequest(collection_name=collection_name, partition_name=tag)
 
         for entity in entities:
             if not entity.get("name", None) or not entity.get("values", None) or not entity.get("type", None):
                 raise ParamError(message="Missing param in entities, a field must have type, name and values")
         if not fields_info:
             raise ParamError(message="Missing collection meta to validate entities")
 
-        location, primary_key_loc, auto_id_loc = {}, None, None
-        for i, field in enumerate(fields_info):
-            if field.get("is_primary", False):
-                primary_key_loc = i
-
-            if field.get("auto_id", False):
-                auto_id_loc = i
-                continue
-
-            match_flag = False
-            field_name = field["name"]
-            field_type = field["type"]
-
-            for entity in entities:
-                entity_name, entity_type = entity["name"], entity["type"]
-
-                if field_name == entity_name:
-                    if field_type != entity_type:
-                        raise ParamError(message=f"Collection field type is {field_type}"
-                                         f", but entities field type is {entity_type}")
-
-                    entity_dim, field_dim = 0, 0
-                    if entity_type in [DataType.FLOAT_VECTOR, DataType.BINARY_VECTOR]:
-                        field_dim = field["params"]["dim"]
-                        entity_dim = len(entity["values"][0])
-
-                    if entity_type in [DataType.FLOAT_VECTOR, ] and entity_dim != field_dim:
-                        raise ParamError(message=f"Collection field dim is {field_dim}"
-                                         f", but entities field dim is {entity_dim}")
-
-                    if entity_type in [DataType.BINARY_VECTOR, ] and entity_dim * 8 != field_dim:
-                        raise ParamError(message=f"Collection field dim is {field_dim}"
-                                         f", but entities field dim is {entity_dim * 8}")
-
-                    location[field["name"]] = i
-                    match_flag = True
-                    break
-
-            if not match_flag:
-                raise ParamError(message=f"Field {field['name']} don't match in entities")
+        location, primary_key_loc, auto_id_loc = traverse_info(fields_info, entities)
 
         # though impossible from sdk
         if primary_key_loc is None:
             raise ParamError(message="primary key not found")
 
         if auto_id_loc is None and len(entities) != len(fields_info):
             raise ParamError(message=f"number of fields: {len(fields_info)}, number of entities: {len(entities)}")
@@ -419,21 +279,21 @@
         try:
             for entity in entities:
                 current = len(entity.get("values"))
                 if row_num not in (0, current):
                     raise ParamError(message="row num misaligned current[{current}]!= previous[{row_num}]")
                 row_num = current
                 field_data = entity_helper.entity_to_field_data(entity, fields_info[location[entity.get("name")]])
-                insert_request.fields_data.append(field_data)
+                request.fields_data.append(field_data)
         except (TypeError, ValueError) as e:
             raise DataNotMatchException(message=ExceptionsMessage.DataTypeInconsistent) from e
 
-        insert_request.num_rows = row_num
+        request.num_rows = row_num
 
-        return insert_request
+        return request
 
     @classmethod
     def delete_request(cls, collection_name, partition_name, expr):
         def check_str(instr, prefix):
             if instr is None:
                 raise ParamError(message=f"{prefix} cannot be None")
             if not isinstance(instr, str):
@@ -446,76 +306,164 @@
             check_str(partition_name, "partition_name")
         check_str(expr, "expr")
 
         request = milvus_types.DeleteRequest(collection_name=collection_name, expr=expr, partition_name=partition_name)
         return request
 
     @classmethod
-    def _prepare_placeholders(cls, vectors, nq, tag, pl_type, is_binary):
+    def _prepare_placeholders(cls, vectors, nq, tag, pl_type, is_binary, dimension=0):
         pl = common_types.PlaceholderValue(tag=tag)
         pl.type = pl_type
         for i in range(0, nq):
             if is_binary:
+                if len(vectors[i]) * 8 != dimension:
+                    raise ParamError(message=f"The dimension of query entities[{vectors[i]*8}] is different from schema [{dimension}]")
                 pl.values.append(blob.vectorBinaryToBytes(vectors[i]))
             else:
+                if len(vectors[i]) != dimension:
+                    raise ParamError(message=f"The dimension of query entities[{vectors[i]*8}] is different from schema [{dimension}]")
                 pl.values.append(blob.vectorFloatToBytes(vectors[i]))
         return pl
 
     @classmethod
-    def search_requests_with_expr(cls, collection_name, data, anns_field, param, limit, expr=None,
+    def search_request(cls, collection_name, query_entities, partition_names=None, fields=None, round_decimal=-1, **kwargs):
+        schema = kwargs.get("schema", None)
+        fields_schema = schema.get("fields", None)  # list
+        fields_name_locs = {fields_schema[loc]["name"]: loc
+                            for loc in range(len(fields_schema))}
+
+        if not isinstance(query_entities, (dict,)):
+            raise ParamError(message="Invalid query format. 'query_entities' must be a dict")
+
+        if fields is not None and not isinstance(fields, (list,)):
+            raise ParamError(message="Invalid query format. 'fields' must be a list")
+
+        request = milvus_types.SearchRequest(
+            collection_name=collection_name,
+            partition_names=partition_names,
+            output_fields=fields,
+            guarantee_timestamp=kwargs.get("guarantee_timestamp", 0),
+        )
+
+        duplicated_entities = copy.deepcopy(query_entities)
+        vector_placeholders = {}
+        vector_names = {}
+
+        def extract_vectors_param(param, placeholders, names, round_decimal):
+            if not isinstance(param, (dict, list)):
+                return
+
+            if isinstance(param, dict):
+                if "vector" in param:
+                    # TODO: Here may not replace ph
+                    ph = "$" + str(len(placeholders))
+
+                    for pk, pv in param["vector"].items():
+                        if "query" not in pv:
+                            raise ParamError(message="param vector must contain 'query'")
+                        placeholders[ph] = pv["query"]
+                        names[ph] = pk
+                        param["vector"][pk]["query"] = ph
+                        param["vector"][pk]["round_decimal"] = round_decimal
+                    return
+
+                for _, v in param.items():
+                    extract_vectors_param(v, placeholders, names, round_decimal)
+
+            if isinstance(param, list):
+                for item in param:
+                    extract_vectors_param(item, placeholders, names, round_decimal)
+
+        extract_vectors_param(duplicated_entities, vector_placeholders, vector_names, round_decimal)
+        request.dsl = ujson.dumps(duplicated_entities)
+
+        plg = common_types.PlaceholderGroup()
+        for tag, vectors in vector_placeholders.items():
+            if len(vectors) <= 0:
+                continue
+            pl = common_types.PlaceholderValue(tag=tag)
+
+            fname = vector_names[tag]
+            if fname not in fields_name_locs:
+                raise ParamError(message=f"Field {fname} doesn't exist in schema")
+            dimension = int(fields_schema[fields_name_locs[fname]]["params"].get("dim", 0))
+
+            if isinstance(vectors[0], bytes):
+                pl.type = PlaceholderType.BinaryVector
+                for vector in vectors:
+                    if dimension != len(vector) * 8:
+                        raise ParamError(message="The dimension of query vector is different from schema")
+                    pl.values.append(blob.vectorBinaryToBytes(vector))
+            else:
+                pl.type = PlaceholderType.FloatVector
+                for vector in vectors:
+                    if dimension != len(vector):
+                        raise ParamError(message="The dimension of query vector is different from schema")
+                    pl.values.append(blob.vectorFloatToBytes(vector))
+            # vector_values_bytes = service_msg_types.VectorValues.SerializeToString(vector_values)
+
+            plg.placeholders.append(pl)
+        plg_str = common_types.PlaceholderGroup.SerializeToString(plg)
+        request.placeholder_group = plg_str
+
+        return request
+
+    @classmethod
+    def search_requests_with_expr(cls, collection_name, data, anns_field, param, limit, schema, expr=None,
                                   partition_names=None, output_fields=None, round_decimal=-1, **kwargs):
+        # TODO Move this impl into server side
+        fields_schema = schema.get("fields", None)  # list
+        fields_name_locs = {fields_schema[loc]["name"]: loc for loc in range(len(fields_schema))}
+
         requests = []
         if len(data) <= 0:
             return requests
 
         if isinstance(data[0], bytes):
             is_binary = True
             pl_type = PlaceholderType.BinaryVector
         else:
             is_binary = False
             pl_type = PlaceholderType.FloatVector
 
+        if anns_field not in fields_name_locs:
+            raise ParamError(message=f"Field {anns_field} doesn't exist in schema")
+        dimension = int(fields_schema[fields_name_locs[anns_field]]["params"].get("dim", 0))
 
-        use_default_consistency = ts_utils.construct_guarantee_ts(collection_name, kwargs)
-
-        ignore_growing = param.get("ignore_growing", False) or kwargs.get("ignore_growing", False)
+        ignore_growing = param.get("ignore_growing",False)
         params = param.get("params", {})
         if not isinstance(params, dict):
             raise ParamError(message=f"Search params must be a dict, got {type(params)}")
         search_params = {
+            "anns_field": anns_field,
             "topk": limit,
-            "metric_type": param.get("metric_type", ""),
+            "metric_type": param.get("metric_type", "L2"),
             "params": params,
             "round_decimal": round_decimal,
             "offset": param.get("offset", 0),
             "ignore_growing": ignore_growing,
         }
 
-        if anns_field:
-            search_params["anns_field"] = anns_field
-
         def dump(v):
             if isinstance(v, dict):
                 return ujson.dumps(v)
             return str(v)
 
         nq = len(data)
         tag = "$0"
-        pl = cls._prepare_placeholders(data, nq, tag, pl_type, is_binary)
+        pl = cls._prepare_placeholders(data, nq, tag, pl_type, is_binary, dimension)
         plg = common_types.PlaceholderGroup()
         plg.placeholders.append(pl)
         plg_str = common_types.PlaceholderGroup.SerializeToString(plg)
         request = milvus_types.SearchRequest(
             collection_name=collection_name,
             partition_names=partition_names,
             output_fields=output_fields,
             guarantee_timestamp=kwargs.get("guarantee_timestamp", 0),
             travel_timestamp=kwargs.get("travel_timestamp", 0),
-            use_default_consistency=use_default_consistency,
-            consistency_level=kwargs.get("consistency_level", 0),
             nq=nq,
         )
         request.placeholder_group = plg_str
 
         request.dsl_type = common_types.DslType.BoolExprV1
         if expr is not None:
             request.dsl = expr
@@ -543,15 +491,16 @@
                                                        index_name=kwargs.get("index_name", ""))
 
         # index_params.collection_name = collection_name
         # index_params.field_name = field_name
 
         def dump(tv):
             if isinstance(tv, dict):
-                return ujson.dumps(tv)
+                import json
+                return json.dumps(tv)
             return str(tv)
 
         if isinstance(params, dict):
             for tk, tv in params.items():
                 if tk == "dim":
                     if not tv or not isinstance(tv, int):
                         raise ParamError(message="dim must be of int!")
@@ -636,25 +585,21 @@
                                             collection_name=collection_name,
                                             ids=ids,
                                             output_fields=output_fields,
                                             partition_names=partition_names)
 
     @classmethod
     def query_request(cls, collection_name, expr, output_fields, partition_names, **kwargs):
-
-        use_default_consistency = ts_utils.construct_guarantee_ts(collection_name, kwargs)
         req = milvus_types.QueryRequest(db_name="",
                                         collection_name=collection_name,
                                         expr=expr,
                                         output_fields=output_fields,
                                         partition_names=partition_names,
                                         guarantee_timestamp=kwargs.get("guarantee_timestamp", 0),
                                         travel_timestamp=kwargs.get("travel_timestamp", 0),
-                                        use_default_consistency=use_default_consistency,
-                                        consistency_level=kwargs.get("consistency_level", 0)
                                         )
 
         limit = kwargs.get("limit", None)
         if limit is not None:
             req.query_params.append(common_types.KeyValuePair(key="limit", value=str(limit)))
 
         offset = kwargs.get("offset", None)
@@ -810,42 +755,39 @@
         if username:
             check_pass_param(user=username)
         check_pass_param(include_role_info=include_role_info)
         return milvus_types.SelectUserRequest(user=milvus_types.UserEntity(name=username) if username else None,
                                               include_role_info=include_role_info)
 
     @classmethod
-    def operate_privilege_request(cls, role_name, object, object_name, privilege, db_name, operate_privilege_type):
+    def operate_privilege_request(cls, role_name, object, object_name, privilege, operate_privilege_type):
         check_pass_param(role_name=role_name)
         check_pass_param(object=object)
         check_pass_param(object_name=object_name)
         check_pass_param(privilege=privilege)
         check_pass_param(operate_privilege_type=operate_privilege_type)
         return milvus_types.OperatePrivilegeRequest(
             entity=milvus_types.GrantEntity(role=milvus_types.RoleEntity(name=role_name),
                                             object=milvus_types.ObjectEntity(name=object),
                                             object_name=object_name,
-                                            db_name=db_name,
                                             grantor=milvus_types.GrantorEntity(
                                                 privilege=milvus_types.PrivilegeEntity(name=privilege))),
             type=operate_privilege_type)
 
     @classmethod
-    def select_grant_request(cls, role_name, object, object_name, db_name):
+    def select_grant_request(cls, role_name, object, object_name):
         check_pass_param(role_name=role_name)
         if object:
             check_pass_param(object=object)
         if object_name:
             check_pass_param(object_name=object_name)
         return milvus_types.SelectGrantRequest(
             entity=milvus_types.GrantEntity(role=milvus_types.RoleEntity(name=role_name),
                                             object=milvus_types.ObjectEntity(name=object) if object else None,
-                                            object_name=object_name if object_name else None,
-                                            db_name=db_name,
-                                            ))
+                                            object_name=object_name if object_name else None))
 
     @classmethod
     def get_server_version(cls):
         return milvus_types.GetVersionRequest()
 
     @classmethod
     def create_resource_group(cls, name):
@@ -878,52 +820,7 @@
     def transfer_replica(cls, source, target, collection_name, num_replica):
         check_pass_param(resource_group_name=source)
         check_pass_param(resource_group_name=target)
         return milvus_types.TransferReplicaRequest(source_resource_group=source,
                                                    target_resource_group=target,
                                                    collection_name=collection_name,
                                                    num_replica=num_replica)
-
-    @classmethod
-    def flush_all_request(cls):
-        return milvus_types.FlushAllRequest()
-
-    @classmethod
-    def get_flush_all_state_request(cls, flush_all_ts):
-        return milvus_types.GetFlushAllStateRequest(flush_all_ts=flush_all_ts)
-
-    @classmethod
-    def create_database_req(cls, db_name):
-        check_pass_param(db_name=db_name)
-        req = milvus_types.CreateDatabaseRequest(db_name=db_name)
-        return req
-
-    @classmethod
-    def drop_database_req(cls, db_name):
-        check_pass_param(db_name=db_name)
-        req = milvus_types.DropDatabaseRequest(db_name=db_name)
-        return req
-
-    @classmethod
-    def list_database_req(cls):
-        req = milvus_types.ListDatabasesRequest()
-        return req
-
-    @classmethod
-    def register_request(cls, user, host, **kwargs):
-        reserved = {}
-        for k, v in kwargs.items():
-            reserved[k] = v
-        now = datetime.datetime.now()
-        this = common_types.ClientInfo(
-            sdk_type="Python",
-            sdk_version=__version__,
-            local_time=now.__str__(),
-            reserved=reserved,
-        )
-        if user is not None:
-            this.user = user
-        if host is not None:
-            this.host = host
-        return milvus_types.ConnectRequest(
-            client_info=this,
-        )
```

### Comparing `pymilvus-2.2.9/pymilvus/client/stub.py` & `pymilvus-2.3.0b1/pymilvus/client/stub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from urllib import parse
 
 from .grpc_handler import GrpcHandler
 from ..exceptions import MilvusException, ParamError
 from .types import CompactionState, CompactionPlans, Replica, BulkInsertState, ResourceGroupInfo
-from ..settings import Config
+from ..settings import DefaultConfig as config
 from ..decorators import deprecated
 
 from .check import is_legal_host, is_legal_port
 
 
 class Milvus:
     @deprecated
-    def __init__(self, host=None, port=Config.GRPC_PORT, uri=Config.GRPC_URI, channel=None, **kwargs):
+    def __init__(self, host=None, port=config.GRPC_PORT, uri=config.GRPC_URI, channel=None, **kwargs):
         self.address = self.__get_address(host, port, uri)
         self._handler = GrpcHandler(address=self.address, channel=channel, **kwargs)
 
         if kwargs.get("pre_ping", False) is True:
             self._handler._wait_for_channel_ready()
 
-    def __get_address(self, host=None, port=Config.GRPC_PORT, uri=Config.GRPC_URI):
+    def __get_address(self, host=None, port=config.GRPC_PORT, uri=config.GRPC_URI):
         if host is None and uri is None:
             raise ParamError(message='Host and uri cannot both be None')
 
         if host is None:
             try:
                 parsed_uri = parse.urlparse(uri, "tcp")
             except (Exception) as e:
@@ -43,27 +43,24 @@
     def name(self):
         return self._name
 
     @property
     def handler(self):
         return self._handler
 
-    def get_server_type(self):
-        return self._handler.get_server_type()
-
     def reset_password(self, user, old_password, new_password):
         self._handler.reset_password(user, old_password, new_password)
 
     def close(self):
         if self._handler is None:
             raise MilvusException(message="Closing on closed handler")
         self.handler.close()
         self._handler = None
 
-    def create_collection(self, collection_name, fields, timeout=None, **kwargs):
+    def create_collection(self, collection_name, fields, shards_num=2, timeout=None, **kwargs):
         """ Creates a collection.
 
         :param collection_name: The name of the collection. A collection name can only include
         numbers, letters, and underscores, and must not begin with a number.
         :type  collection_name: str
 
         :param fields: Field parameters.
@@ -74,23 +71,23 @@
                     {"field": "B", "type": DataType.INT64},
                     {"field": "C", "type": DataType.FLOAT},
                     {"field": "Vec", "type": DataType.FLOAT_VECTOR,
                      "params": {"dim": 128}}
                 ],
             "auto_id": True}`
 
+        :param shards_num: How wide to scale collection. Corresponds to how many active datanodes
+                        can be used on insert.
+        :type shards_num: int
+
         :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
                         is set to None, client waits until server response or error occur.
         :type  timeout: float
 
         :param kwargs:
-            * *num_shards* (``int``) --
-            How wide to scale collection. Corresponds to how many active datanodes can be used on insert.
-            * *shards_num* (``int``, deprecated) --
-            How wide to scale collection. Corresponds to how many active datanodes can be used on insert.
             * *consistency_level* (``str/int``) --
             Which consistency level to use when searching in the collection. For details, see
             https://github.com/milvus-io/milvus/blob/master/docs/developer_guides/how-guarantee-ts-works.md.
             Note: this parameter can be overwritten by the same parameter specified in search.
             * *properties* (``dict``) --
 
 
@@ -98,15 +95,15 @@
         :rtype: NoneType
 
         :raises RpcError: If gRPC encounter an error
         :raises ParamError: If parameters are invalid
         :raises MilvusException: If the return result from server is not ok
         """
         with self._connection() as handler:
-            return handler.create_collection(collection_name, fields, timeout=timeout, **kwargs)
+            return handler.create_collection(collection_name, fields, shards_num=shards_num, timeout=timeout, **kwargs)
 
     def drop_collection(self, collection_name, timeout=None):
         """
         Delete a specified collection.
 
         :param collection_name: The name of the collection to delete.
         :type  collection_name: str
```

### Comparing `pymilvus-2.2.9/pymilvus/client/ts_utils.py` & `pymilvus-2.3.0b1/pymilvus/client/ts_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import threading
 import datetime
 
 from .singleton_utils import Singleton
 from .utils import hybridts_to_unixtime
-from .types import get_consistency_level
 from .constants import EVENTUALLY_TS, BOUNDED_TS
 
-from ..grpc_gen import common_pb2
+from ..grpc_gen.common_pb2 import ConsistencyLevel
 
-ConsistencyLevel = common_pb2.ConsistencyLevel
 
 class GTsDict(metaclass=Singleton):
     def __init__(self):
         # collection id -> last write ts
         self._last_write_ts_dict = {}
         self._last_write_ts_dict_lock = threading.Lock()
 
@@ -68,31 +66,24 @@
     return EVENTUALLY_TS
 
 
 def get_bounded_ts():
     return BOUNDED_TS
 
 
-def construct_guarantee_ts(collection_name, kwargs):
-    consistency_level = kwargs.get("consistency_level", None)
-    use_default = consistency_level is None
-    if use_default:
-        # in case of the default consistency is Customized or Session,
-        # we set guarantee_timestamp to the cached mutation ts or 1
-        kwargs["guarantee_timestamp"] = get_collection_ts(collection_name) or get_eventually_ts()
-        return True
-    consistency_level = get_consistency_level(consistency_level)
-    kwargs["consistency_level"] = consistency_level
+def construct_guarantee_ts(consistency_level, collection_name, kwargs):
     if consistency_level == ConsistencyLevel.Strong:
         # Milvus will assign a newest ts.
         kwargs["guarantee_timestamp"] = 0
     elif consistency_level == ConsistencyLevel.Session:
         # Using the last write ts of the collection.
         # TODO: get a timestamp from server?
         kwargs["guarantee_timestamp"] = get_collection_ts(collection_name) or get_eventually_ts()
     elif consistency_level == ConsistencyLevel.Bounded:
         # Milvus will assign ts according to the server timestamp and a configured time interval
         kwargs["guarantee_timestamp"] = get_bounded_ts()
+    elif consistency_level == ConsistencyLevel.Eventually:
+        # Using a very small timestamp.
+        kwargs["guarantee_timestamp"] = get_eventually_ts()
     else:
         # Users customize the consistency level, no modification on `guarantee_timestamp`.
-        kwargs.setdefault("guarantee_timestamp", get_eventually_ts())
-    return use_default
+        pass
```

### Comparing `pymilvus-2.2.9/pymilvus/client/types.py` & `pymilvus-2.3.0b1/pymilvus/client/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import time
 from enum import IntEnum
+from ..grpc_gen.common_pb2 import ConsistencyLevel
 from ..grpc_gen import common_pb2
 from ..exceptions import (
     AutoIDException,
     ExceptionsMessage,
     InvalidConsistencyLevel,
 )
 from ..grpc_gen import milvus_pb2 as milvus_types
 
 
-ConsistencyLevel = common_pb2.ConsistencyLevel
-
 class Status:
     """
     :attribute code: int (optional) default as ok
 
     :attribute message: str (optional) current status message
     """
 
@@ -77,15 +76,14 @@
     INT64 = 5
 
     FLOAT = 10
     DOUBLE = 11
 
     STRING = 20
     VARCHAR = 21
-    JSON = 23
 
     BINARY_VECTOR = 100
     FLOAT_VECTOR = 101
 
     UNKNOWN = 999
 
 
@@ -287,17 +285,17 @@
             return ConsistencyLevel.Value(consistency_level)
         except ValueError as e:
             raise InvalidConsistencyLevel(message=f"invalid consistency level: {consistency_level}") from e
     raise InvalidConsistencyLevel(message="invalid consistency level")
 
 
 class Shard:
-    def __init__(self, channel_name: str, shard_nodes: list, shard_leader: int):
+    def __init__(self, channel_name: str, shard_nodes, shard_leader: int):
         self._channel_name = channel_name
-        self._shard_nodes = set(shard_nodes)
+        self._shard_nodes = shard_nodes
         self._shard_leader = shard_leader
 
     def __repr__(self):
         return f"""Shard: <channel_name:{self.channel_name}>, <shard_leader:{self.shard_leader}>, <shard_nodes:{self.shard_nodes}>"""
 
     @property
     def channel_name(self) -> str:
@@ -533,39 +531,33 @@
         return int(percent)
 
 
 class GrantItem:
     def __init__(self, entity):
         self._object = entity.object.name
         self._object_name = entity.object_name
-        self._db_name = entity.db_name
         self._role_name = entity.role.name
         self._grantor_name = entity.grantor.user.name
         self._privilege = entity.grantor.privilege.name
 
     def __repr__(self) -> str:
         s = f"GrantItem: <object:{self.object}>, <object_name:{self.object_name}>, " \
-            f"<db_name:{self.db_name}>, " \
             f"<role_name:{self.role_name}>, <grantor_name:{self.grantor_name}>, " \
             f"<privilege:{self.privilege}>"
         return s
 
     @property
     def object(self):
         return self._object
 
     @property
     def object_name(self):
         return self._object_name
 
     @property
-    def db_name(self):
-        return self._db_name
-
-    @property
     def role_name(self):
         return self._role_name
 
     @property
     def grantor_name(self):
         return self._grantor_name
 
@@ -701,20 +693,20 @@
         self._num_available_node = resource_group.num_available_node
         self._num_loaded_replica = resource_group.num_loaded_replica
         self._num_outgoing_node = resource_group.num_outgoing_node
         self._num_incoming_node = resource_group.num_incoming_node
 
     def __repr__(self) -> str:
         s = f"""ResourceGroupInfo:
-<name:{self.name}>,
-<capacity:{self.capacity}>,
-<num_available_node:{self.num_available_node}>,
-<num_loaded_replica:{self.num_loaded_replica}>,
-<num_outgoing_node:{self.num_outgoing_node}>,
-<num_incoming_node:{self.num_incoming_node}>"""
+        <name:{self.name}>, 
+        <capacity:{self.capacity}>, 
+        <num_available_node:{self.num_available_node}>, 
+        <num_loaded_replica:{self.num_loaded_replica}>, 
+        <num_outgoing_node:{self.num_outgoing_node}>, 
+        <num_incoming_node:{self.num_incoming_node}>"""
         return s
 
 
     @property
     def name(self):
         return self._name
```

### Comparing `pymilvus-2.2.9/pymilvus/client/utils.py` & `pymilvus-2.3.0b1/pymilvus/client/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import datetime
 
-from .constants import LOGICAL_BITS, LOGICAL_BITS_MASK
 from .types import DataType
+from .constants import LOGICAL_BITS, LOGICAL_BITS_MASK
 from ..exceptions import ParamError, MilvusException
 
-MILVUS = "milvus"
-ZILLIZ = "zilliz"
-
 valid_index_types = [
+    "GPU_FLAT",
+    "GPU_IVF_FLAT",
+    "GPU_IVF_SQ8",
+    "GPU_IVF_PQ",
+    "RAFT_IVF_FLAT",
+    "RAFT_IVF_PQ",
     "FLAT",
     "IVF_FLAT",
     "IVF_SQ8",
-    # "IVF_SQ8_HYBRID",
     "IVF_PQ",
     "HNSW",
-    # "NSG",
     "ANNOY",
-    "RHNSW_FLAT",
-    "RHNSW_PQ",
-    "RHNSW_SQ",
     "BIN_FLAT",
     "BIN_IVF_FLAT",
     "DISKANN",
     "AUTOINDEX"
 ]
 
 valid_index_params_keys = [
@@ -134,17 +132,14 @@
 
         if field_data.scalars.HasField("string_data"):
             return len(field_data.scalars.string_data.data)
 
         if field_data.scalars.HasField("bytes_data"):
             return len(field_data.scalars.bytes_data.data)
 
-        if field_data.scalars.HasField("json_data"):
-            return len(field_data.scalars.json_data.data)
-
         raise MilvusException(message="Unsupported scalar type")
 
     if field_data.HasField("vectors"):
         dim = field_data.vectors.dim
         if field_data.vectors.HasField("float_vector"):
             total_len = len(field_data.vectors.float_vector.data)
             if total_len % dim != 0:
@@ -153,73 +148,51 @@
 
         total_len = len(field_data.vectors.binary_vector)
         return int(total_len / (dim / 8))
 
     raise MilvusException(message="Unknown data type")
 
 
-def traverse_rows_info(fields_info, entities):
+def traverse_info(fields_info, entities):
     location, primary_key_loc, auto_id_loc = {}, None, None
-
     for i, field in enumerate(fields_info):
-        is_auto_id = False
-        is_dynamic = False
+        if field.get("is_primary", False):
+            primary_key_loc = i
 
         if field.get("auto_id", False):
             auto_id_loc = i
-            is_auto_id = True
-
-        if field.get("is_primary", False):
-            primary_key_loc = i
+            continue
 
+        match_flag = False
         field_name = field["name"]
-        location[field_name] = i
         field_type = field["type"]
 
-        if field.get("is_dynamic", False):
-            is_dynamic = True
+        for entity in entities:
+            entity_name, entity_type = entity["name"], entity["type"]
 
-        for j, entity in enumerate(entities):
-            if is_auto_id:
-                if field_name in entity:
-                    raise ParamError(
-                        message=f"auto id enabled, {field_name} shouldn't in entities[{j}]")
-                continue
-
-            if is_dynamic:
-                if field_name in entity:
-                    raise ParamError(
-                        message=f"dynamic field enabled, {field_name} shouldn't in entities[{j}]")
-
-            value = entity.get(field_name, None)
-            if value is None:
-                raise ParamError(
-                    message=f"Field {field_name} don't match in entities[{j}]")
-
-            if field_type in [DataType.FLOAT_VECTOR, DataType.BINARY_VECTOR]:
-                field_dim = field["params"]["dim"]
-                if field_type == DataType.FLOAT_VECTOR:
-                    entity_dim = len(value)
-                else:
-                    entity_dim = len(value) * 8
+            if field_name == entity_name:
+                if field_type != entity_type:
+                    raise ParamError(message=f"Collection field type is {field_type}"
+                                     f", but entities field type is {entity_type}")
+
+                entity_dim, field_dim = 0, 0
+                if entity_type in [DataType.FLOAT_VECTOR, DataType.BINARY_VECTOR]:
+                    field_dim = field["params"]["dim"]
+                    entity_dim = len(entity["values"][0])
 
-                if entity_dim != field_dim:
+                if entity_type in [DataType.FLOAT_VECTOR, ] and entity_dim != field_dim:
                     raise ParamError(message=f"Collection field dim is {field_dim}"
-                                             f", but entities field dim is {entity_dim}")
+                                     f", but entities field dim is {entity_dim}")
 
-    # though impossible from sdk
-    if primary_key_loc is None:
-        raise ParamError(message="primary key not found")
+                if entity_type in [DataType.BINARY_VECTOR, ] and entity_dim * 8 != field_dim:
+                    raise ParamError(message=f"Collection field dim is {field_dim}"
+                                     f", but entities field dim is {entity_dim * 8}")
 
-    return location, primary_key_loc, auto_id_loc
+                location[field["name"]] = i
+                match_flag = True
+                break
+
+        if not match_flag:
+            raise ParamError(
+                message=f"Field {field['name']} don't match in entities")
 
-def get_server_type(host):
-    if host is None or not isinstance(host, str):
-        return MILVUS
-    splits = host.split('.')
-    len_of_splits = len(splits)
-    if len_of_splits >= 2 and \
-            (splits[len_of_splits - 2].lower() == "zilliz" or
-             splits[len_of_splits - 2].lower() == "zillizcloud") and \
-            splits[len_of_splits - 1].lower() == "com":
-        return ZILLIZ
-    return MILVUS
+    return location, primary_key_loc, auto_id_loc
```

### Comparing `pymilvus-2.2.9/pymilvus/decorators.py` & `pymilvus-2.3.0b1/pymilvus/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -133,40 +133,7 @@
                 self.set_onetime_loglevel(level)
             if req_id:
                 self.set_onetime_request_id(req_id)
             ret = func(self, *args, **kwargs)
             return ret
         return handler
     return wrapper
-
-
-def ignore_unimplemented(default_return_value):
-    def wrapper(func):
-        @functools.wraps(func)
-        def handler(*args, **kwargs):
-            try:
-                return func(*args, **kwargs)
-            except grpc.RpcError as e:
-                if e.code() == grpc.StatusCode.UNIMPLEMENTED:
-                    LOGGER.warning(f"{func.__name__} unimplemented, ignore it")
-                    return default_return_value
-                raise e
-            except Exception as e:
-                raise e
-        return handler
-    return wrapper
-
-
-def upgrade_reminder(func):
-    @functools.wraps(func)
-    def handler(*args, **kwargs):
-        try:
-            return func(*args, **kwargs)
-        except grpc.RpcError as e:
-            if e.code() == grpc.StatusCode.UNIMPLEMENTED:
-                msg = "this version of sdk is incompatible with server, please downgrade your sdk or upgrade your " \
-                      "server "
-                raise MilvusException(message=msg) from e
-            raise e
-        except Exception as e:
-            raise e
-    return handler
```

### Comparing `pymilvus-2.2.9/pymilvus/exceptions.py` & `pymilvus-2.3.0b1/pymilvus/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,18 +100,14 @@
     """ Raise when configs of connection are invalid """
 
 
 class PrimaryKeyException(MilvusException):
     """ Raise when primarykey are invalid """
 
 
-class PartitionKeyException(MilvusException):
-    """ Raise when partitionkey are invalid """
-
-
 class FieldsTypeException(MilvusException):
     """ Raise when fields is invalid """
 
 
 class FieldTypeException(MilvusException):
     """ Raise when one field is invalid """
 
@@ -120,14 +116,18 @@
     """ Raise when autoID is invalid """
 
 
 class InvalidConsistencyLevel(MilvusException):
     """ Raise when consistency level is invalid """
 
 
+class UpsertAutoIDTrueException(MilvusException):
+    """ Raise when upsert autoID is true """
+
+
 class ExceptionsMessage:
     NoHostPort = "connection configuration must contain 'host' and 'port'."
     HostType = "Type of 'host' must be str."
     PortType = "Type of 'port' must be str or int."
     ConnDiffConf = "Alias of %r already creating connections, but the configure is not the same as passed in."
     AliasType = "Alias should be string, but %r is given."
     ConnLackConf = "You need to pass in the configuration of the connection named %r ."
@@ -135,36 +135,28 @@
     CollectionNotExistNoSchema = "Collection %r not exist, or you can pass in schema to create one."
     NoSchema = "Should be passed into the schema."
     EmptySchema = "The field of the schema cannot be empty."
     SchemaType = "Schema type must be schema.CollectionSchema."
     SchemaInconsistent = "The collection already exist, but the schema is not the same as the schema passed in."
     AutoIDWithData = "Auto_id is True, primary field should not have data."
     AutoIDType = "Param auto_id must be bool type."
-    NumPartitionsType = "Param num_partitions must be int type."
     AutoIDInconsistent = "The auto_id of the collection is inconsistent with the auto_id of the primary key field."
     AutoIDIllegalRanges = "The auto-generated id ranges should be pairs."
     ConsistencyLevelInconsistent = "The parameter consistency_level is inconsistent with that of existed collection."
     AutoIDOnlyOnPK = "The auto_id can only be specified on the primary key field"
     AutoIDFieldType = "The auto_id can only be specified on field with DataType.INT64"
     FieldsNumInconsistent = "The data fields number is not match with schema."
     NoVector = "No vector field is found."
     NoneDataFrame = "Dataframe can not be None."
     DataFrameType = "Data type must be pandas.DataFrame."
     NoPrimaryKey = "Schema must have a primary key field."
     PrimaryKeyNotExist = "Primary field must in dataframe."
-    PrimaryKeyOnlyOne = "Expected only one primary key field, got [%s, %s, ...]."
-    PartitionKeyOnlyOne = "Expected only one partition key field, got [%s, %s, ...]."
+    PrimaryKeyOnlyOne = "Primary key field can only be one."
     PrimaryKeyType = "Primary key type must be DataType.INT64 or DataType.VARCHAR."
-    PartitionKeyType = "Partition key field type must be DataType.INT64 or DataType.VARCHAR."
-    PartitionKeyNotPrimary = "Primary key filed should not be primary field"
     IsPrimaryType = "Param is_primary must be bool type."
-    PrimaryFieldType = "Param primary_field must be str type."
-    PartitionKeyFieldType = "Param partition_key_field must be str type."
-    PartitionKeyFieldNotExist = "the specified partition key field {%s} not exist"
-    IsPartitionKeyType = "Param is_partition_key must be bool type."
     DataTypeInconsistent = "The data in the same column must be of the same type."
     DataTypeNotSupport = "Data type is not support."
     DataLengthsInconsistent = "Arrays must all be same length."
     DataFrameInvalid = "Cannot infer schema from empty dataframe."
     NdArrayNotSupport = "Data type not support numpy.ndarray."
     TypeOfDataAndSchemaInconsistent = "The types of schema and data do not match."
     PartitionAlreadyExist = "Partition already exist."
@@ -173,7 +165,8 @@
     CollectionType = "The type of collection must be pymilvus.Collection."
     FieldsType = "The fields of schema must be type list."
     FieldType = "The field of schema type must be FieldSchema."
     FieldDtype = "Field dtype must be of DataType"
     ExprType = "The type of expr must be string ,but %r is given."
     EnvConfigErr = "Environment variable %s has a wrong format, please check it: %s"
     AmbiguousIndexName = "There are multiple indexes, please specify the index_name."
+    UpsertAutoIDTrue = "Upsert don't support autoid == true"
```

### Comparing `pymilvus-2.2.9/pymilvus/grpc_gen/milvus_pb2_grpc.py` & `pymilvus-2.3.0b1/pymilvus/grpc_gen/milvus_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,19 +126,14 @@
                 response_deserializer=common__pb2.Status.FromString,
                 )
         self.DescribeIndex = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/DescribeIndex',
                 request_serializer=milvus__pb2.DescribeIndexRequest.SerializeToString,
                 response_deserializer=milvus__pb2.DescribeIndexResponse.FromString,
                 )
-        self.GetIndexStatistics = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/GetIndexStatistics',
-                request_serializer=milvus__pb2.GetIndexStatisticsRequest.SerializeToString,
-                response_deserializer=milvus__pb2.GetIndexStatisticsResponse.FromString,
-                )
         self.GetIndexState = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetIndexState',
                 request_serializer=milvus__pb2.GetIndexStateRequest.SerializeToString,
                 response_deserializer=milvus__pb2.GetIndexStateResponse.FromString,
                 )
         self.GetIndexBuildProgress = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetIndexBuildProgress',
@@ -156,14 +151,19 @@
                 response_deserializer=milvus__pb2.MutationResult.FromString,
                 )
         self.Delete = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/Delete',
                 request_serializer=milvus__pb2.DeleteRequest.SerializeToString,
                 response_deserializer=milvus__pb2.MutationResult.FromString,
                 )
+        self.Upsert = channel.unary_unary(
+                '/milvus.proto.milvus.MilvusService/Upsert',
+                request_serializer=milvus__pb2.UpsertRequest.SerializeToString,
+                response_deserializer=milvus__pb2.MutationResult.FromString,
+                )
         self.Search = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/Search',
                 request_serializer=milvus__pb2.SearchRequest.SerializeToString,
                 response_deserializer=milvus__pb2.SearchResults.FromString,
                 )
         self.Flush = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/Flush',
@@ -176,29 +176,19 @@
                 response_deserializer=milvus__pb2.QueryResults.FromString,
                 )
         self.CalcDistance = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/CalcDistance',
                 request_serializer=milvus__pb2.CalcDistanceRequest.SerializeToString,
                 response_deserializer=milvus__pb2.CalcDistanceResults.FromString,
                 )
-        self.FlushAll = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/FlushAll',
-                request_serializer=milvus__pb2.FlushAllRequest.SerializeToString,
-                response_deserializer=milvus__pb2.FlushAllResponse.FromString,
-                )
         self.GetFlushState = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetFlushState',
                 request_serializer=milvus__pb2.GetFlushStateRequest.SerializeToString,
                 response_deserializer=milvus__pb2.GetFlushStateResponse.FromString,
                 )
-        self.GetFlushAllState = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/GetFlushAllState',
-                request_serializer=milvus__pb2.GetFlushAllStateRequest.SerializeToString,
-                response_deserializer=milvus__pb2.GetFlushAllStateResponse.FromString,
-                )
         self.GetPersistentSegmentInfo = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetPersistentSegmentInfo',
                 request_serializer=milvus__pb2.GetPersistentSegmentInfoRequest.SerializeToString,
                 response_deserializer=milvus__pb2.GetPersistentSegmentInfoResponse.FromString,
                 )
         self.GetQuerySegmentInfo = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetQuerySegmentInfo',
@@ -361,34 +351,14 @@
                 response_deserializer=milvus__pb2.DescribeResourceGroupResponse.FromString,
                 )
         self.RenameCollection = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/RenameCollection',
                 request_serializer=milvus__pb2.RenameCollectionRequest.SerializeToString,
                 response_deserializer=common__pb2.Status.FromString,
                 )
-        self.CreateDatabase = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/CreateDatabase',
-                request_serializer=milvus__pb2.CreateDatabaseRequest.SerializeToString,
-                response_deserializer=common__pb2.Status.FromString,
-                )
-        self.DropDatabase = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/DropDatabase',
-                request_serializer=milvus__pb2.DropDatabaseRequest.SerializeToString,
-                response_deserializer=common__pb2.Status.FromString,
-                )
-        self.ListDatabases = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/ListDatabases',
-                request_serializer=milvus__pb2.ListDatabasesRequest.SerializeToString,
-                response_deserializer=milvus__pb2.ListDatabasesResponse.FromString,
-                )
-        self.Connect = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/Connect',
-                request_serializer=milvus__pb2.ConnectRequest.SerializeToString,
-                response_deserializer=milvus__pb2.ConnectResponse.FromString,
-                )
 
 
 class MilvusServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def CreateCollection(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -524,20 +494,14 @@
 
     def DescribeIndex(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetIndexStatistics(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def GetIndexState(self, request, context):
         """Deprecated: use DescribeIndex instead
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -562,56 +526,50 @@
 
     def Delete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Search(self, request, context):
+    def Upsert(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Flush(self, request, context):
+    def Search(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Query(self, request, context):
+    def Flush(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CalcDistance(self, request, context):
+    def Query(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FlushAll(self, request, context):
+    def CalcDistance(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFlushState(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetFlushAllState(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def GetPersistentSegmentInfo(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetQuerySegmentInfo(self, request, context):
@@ -813,38 +771,14 @@
 
     def RenameCollection(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateDatabase(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def DropDatabase(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ListDatabases(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Connect(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
 
 def add_MilvusServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateCollection': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateCollection,
                     request_deserializer=milvus__pb2.CreateCollectionRequest.FromString,
                     response_serializer=common__pb2.Status.SerializeToString,
@@ -955,19 +889,14 @@
                     response_serializer=common__pb2.Status.SerializeToString,
             ),
             'DescribeIndex': grpc.unary_unary_rpc_method_handler(
                     servicer.DescribeIndex,
                     request_deserializer=milvus__pb2.DescribeIndexRequest.FromString,
                     response_serializer=milvus__pb2.DescribeIndexResponse.SerializeToString,
             ),
-            'GetIndexStatistics': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetIndexStatistics,
-                    request_deserializer=milvus__pb2.GetIndexStatisticsRequest.FromString,
-                    response_serializer=milvus__pb2.GetIndexStatisticsResponse.SerializeToString,
-            ),
             'GetIndexState': grpc.unary_unary_rpc_method_handler(
                     servicer.GetIndexState,
                     request_deserializer=milvus__pb2.GetIndexStateRequest.FromString,
                     response_serializer=milvus__pb2.GetIndexStateResponse.SerializeToString,
             ),
             'GetIndexBuildProgress': grpc.unary_unary_rpc_method_handler(
                     servicer.GetIndexBuildProgress,
@@ -985,14 +914,19 @@
                     response_serializer=milvus__pb2.MutationResult.SerializeToString,
             ),
             'Delete': grpc.unary_unary_rpc_method_handler(
                     servicer.Delete,
                     request_deserializer=milvus__pb2.DeleteRequest.FromString,
                     response_serializer=milvus__pb2.MutationResult.SerializeToString,
             ),
+            'Upsert': grpc.unary_unary_rpc_method_handler(
+                    servicer.Upsert,
+                    request_deserializer=milvus__pb2.UpsertRequest.FromString,
+                    response_serializer=milvus__pb2.MutationResult.SerializeToString,
+            ),
             'Search': grpc.unary_unary_rpc_method_handler(
                     servicer.Search,
                     request_deserializer=milvus__pb2.SearchRequest.FromString,
                     response_serializer=milvus__pb2.SearchResults.SerializeToString,
             ),
             'Flush': grpc.unary_unary_rpc_method_handler(
                     servicer.Flush,
@@ -1005,29 +939,19 @@
                     response_serializer=milvus__pb2.QueryResults.SerializeToString,
             ),
             'CalcDistance': grpc.unary_unary_rpc_method_handler(
                     servicer.CalcDistance,
                     request_deserializer=milvus__pb2.CalcDistanceRequest.FromString,
                     response_serializer=milvus__pb2.CalcDistanceResults.SerializeToString,
             ),
-            'FlushAll': grpc.unary_unary_rpc_method_handler(
-                    servicer.FlushAll,
-                    request_deserializer=milvus__pb2.FlushAllRequest.FromString,
-                    response_serializer=milvus__pb2.FlushAllResponse.SerializeToString,
-            ),
             'GetFlushState': grpc.unary_unary_rpc_method_handler(
                     servicer.GetFlushState,
                     request_deserializer=milvus__pb2.GetFlushStateRequest.FromString,
                     response_serializer=milvus__pb2.GetFlushStateResponse.SerializeToString,
             ),
-            'GetFlushAllState': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetFlushAllState,
-                    request_deserializer=milvus__pb2.GetFlushAllStateRequest.FromString,
-                    response_serializer=milvus__pb2.GetFlushAllStateResponse.SerializeToString,
-            ),
             'GetPersistentSegmentInfo': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPersistentSegmentInfo,
                     request_deserializer=milvus__pb2.GetPersistentSegmentInfoRequest.FromString,
                     response_serializer=milvus__pb2.GetPersistentSegmentInfoResponse.SerializeToString,
             ),
             'GetQuerySegmentInfo': grpc.unary_unary_rpc_method_handler(
                     servicer.GetQuerySegmentInfo,
@@ -1190,34 +1114,14 @@
                     response_serializer=milvus__pb2.DescribeResourceGroupResponse.SerializeToString,
             ),
             'RenameCollection': grpc.unary_unary_rpc_method_handler(
                     servicer.RenameCollection,
                     request_deserializer=milvus__pb2.RenameCollectionRequest.FromString,
                     response_serializer=common__pb2.Status.SerializeToString,
             ),
-            'CreateDatabase': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateDatabase,
-                    request_deserializer=milvus__pb2.CreateDatabaseRequest.FromString,
-                    response_serializer=common__pb2.Status.SerializeToString,
-            ),
-            'DropDatabase': grpc.unary_unary_rpc_method_handler(
-                    servicer.DropDatabase,
-                    request_deserializer=milvus__pb2.DropDatabaseRequest.FromString,
-                    response_serializer=common__pb2.Status.SerializeToString,
-            ),
-            'ListDatabases': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListDatabases,
-                    request_deserializer=milvus__pb2.ListDatabasesRequest.FromString,
-                    response_serializer=milvus__pb2.ListDatabasesResponse.SerializeToString,
-            ),
-            'Connect': grpc.unary_unary_rpc_method_handler(
-                    servicer.Connect,
-                    request_deserializer=milvus__pb2.ConnectRequest.FromString,
-                    response_serializer=milvus__pb2.ConnectResponse.SerializeToString,
-            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'milvus.proto.milvus.MilvusService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -1612,31 +1516,14 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/DescribeIndex',
             milvus__pb2.DescribeIndexRequest.SerializeToString,
             milvus__pb2.DescribeIndexResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetIndexStatistics(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/GetIndexStatistics',
-            milvus__pb2.GetIndexStatisticsRequest.SerializeToString,
-            milvus__pb2.GetIndexStatisticsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetIndexState(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1714,14 +1601,31 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/Delete',
             milvus__pb2.DeleteRequest.SerializeToString,
             milvus__pb2.MutationResult.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def Upsert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/Upsert',
+            milvus__pb2.UpsertRequest.SerializeToString,
+            milvus__pb2.MutationResult.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def Search(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1782,31 +1686,14 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/CalcDistance',
             milvus__pb2.CalcDistanceRequest.SerializeToString,
             milvus__pb2.CalcDistanceResults.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FlushAll(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/FlushAll',
-            milvus__pb2.FlushAllRequest.SerializeToString,
-            milvus__pb2.FlushAllResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetFlushState(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1816,31 +1703,14 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/GetFlushState',
             milvus__pb2.GetFlushStateRequest.SerializeToString,
             milvus__pb2.GetFlushStateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetFlushAllState(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/GetFlushAllState',
-            milvus__pb2.GetFlushAllStateRequest.SerializeToString,
-            milvus__pb2.GetFlushAllStateResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetPersistentSegmentInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -2410,82 +2280,14 @@
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/RenameCollection',
             milvus__pb2.RenameCollectionRequest.SerializeToString,
             common__pb2.Status.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
-    @staticmethod
-    def CreateDatabase(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/CreateDatabase',
-            milvus__pb2.CreateDatabaseRequest.SerializeToString,
-            common__pb2.Status.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def DropDatabase(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/DropDatabase',
-            milvus__pb2.DropDatabaseRequest.SerializeToString,
-            common__pb2.Status.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ListDatabases(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/ListDatabases',
-            milvus__pb2.ListDatabasesRequest.SerializeToString,
-            milvus__pb2.ListDatabasesResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Connect(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/Connect',
-            milvus__pb2.ConnectRequest.SerializeToString,
-            milvus__pb2.ConnectResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
 
 class ProxyServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `pymilvus-2.2.9/pymilvus/milvus_client/milvus_client.py` & `pymilvus-2.3.0b1/pymilvus/orm/partition.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,879 +1,623 @@
-"""MilvusClient for dealing with simple workflows."""
-import logging
-import threading
-from typing import Dict, List, Union
-from uuid import uuid4
-
-from pymilvus.exceptions import MilvusException
-from pymilvus.milvus_client.defaults import DEFAULT_SEARCH_PARAMS
-from pymilvus.orm import utility
-from pymilvus.orm.collection import Collection, CollectionSchema, FieldSchema
-from pymilvus.orm.connections import connections
-from pymilvus.orm.types import DataType, infer_dtype_bydata
-
-logger = logging.getLogger()
-logger.setLevel(logging.DEBUG)
-
-
-class MilvusClient:
-    """The Milvus Client"""
-
-    # pylint: disable=logging-too-many-args, too-many-instance-attributes, import-outside-toplevel
-
-    def __init__(
-        self,
-        collection_name: str = "ClientCollection",
-        pk_field: str = None,
-        vector_field: str = None,
-        uri: str = "http://localhost:19530",
-        num_shards: int = None,
-        partitions: List[str] = None,
-        consistency_level: str = "Session",
-        replica_number: int = 1,
-        index_params: dict = None,
-        distance_metric: str = "L2",
-        timeout: int = None,
-        overwrite: bool = False,
-    ):
-        """A client for the common Milvus use case.
-
-        This client attempts to hide away the complexity of using Pymilvus. In a lot ofcases what
-        the user wants is a simple wrapper that supports adding data, deleting data, and searching.
-        This wrapper can autoinfer the schema from a previous collection or newly inserted data,
-        can update the paritions, can query, and can delete by pk.
+# Copyright (C) 2019-2021 Zilliz. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except
+# in compliance with the License. You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software distributed under the License
+# is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
+# or implied. See the License for the specific language governing permissions and limitations under
+# the License.
+
+import copy
+import json
+
+from ..exceptions import (
+    CollectionNotExistException,
+    PartitionNotExistException,
+    ExceptionsMessage,
+)
+
+from .prepare import Prepare
+from .search import SearchResult
+from .mutation import MutationResult
+from .future import SearchFuture, MutationFuture
+from ..client.types import Replica
+
+
+class Partition:
+    def __init__(self, collection, name, description="", **kwargs):
+        # TODO: Need a place to store the description
+        from .collection import Collection
+        if not isinstance(collection, Collection):
+            raise CollectionNotExistException(message=ExceptionsMessage.CollectionType)
+        self._collection = collection
+        self._name = name
+        self._description = description
+        self._schema = collection._schema
+        self._consistency_level = collection._consistency_level
+        self._kwargs = kwargs
 
-        Args:
-            pk_field (str, optional): Which entry in data is considered the primary key. If None,
-                an auto-id will be created. Will be overwritten if loading from a previous
-                collection. Defaults to None.
-            vector_field (str, optional): Which entry in the data is considered the vector field.
-                Will get overwritten if loading from previous collection. Required if not using
-                already made collection.
-            uri (str, optional): The connection address to use to connect to the
-                instance. Defaults to "http://localhost:19530". Another example:
-                "https://username:password@in01-12a.aws-us-west-2.vectordb.zillizcloud.com:19538
-            num_shards (int, optional): The amount of shards to use for the collection. Unless
-                dealing with huge scale, recommended to keep at default. Defaults to None and allows
-                server to set.
-            partitions (List[str], optional): Which paritions to create for the collection.
-                Defaults to None.
-            consistency_level (str, optional): Which consistency level to use for the Client.
-                The options are "Strong", "Bounded", "Eventually", "Session". Defaults to "Bounded".
-            replica_number (int, optional): The amount of in memomory replicas to use.
-                Defaults to 1.
-            distance_metric (str, optional): Which distance metric to use if not supplying
-                index params. Valid types are "IP" and "L2".
-            index_params (dict, optional): What index parameteres to use for the Collection.
-                If none, will use a default one. If collection already exists, will overwrite
-                using this index.
-            timeout (int, optional): What timeout to use for function calls. Defaults
-                to None.
-            overwrite (bool, optional): Whether to overwrite existing collection if exists.
-                Defaults to False
-        """
-        # Optionial TQDM import
-        try:
-            import tqdm
-            self.tqdm = tqdm.tqdm
-        except ImportError:
-            logger.debug("tqdm not found")
-            self.tqdm = (lambda x, disable: x)
-
-        self.uri = uri
-        self.collection_name = collection_name
-        self.num_shards = num_shards
-        self.partitions = partitions
-        self.consistency_level = consistency_level
-        self.replica_number = replica_number
-        self.distance_metric = distance_metric
-        self.index_params = index_params
-        self.timeout = timeout
-        self.pk_field = pk_field
-        self.vector_field = vector_field
-
-        # TODO: Figure out thread safety
-        # self.concurrent_counter = 0
-        self.concurrent_lock = threading.RLock()
-        self.default_search_params = None
-        self.collection = None
-        self.fields = None
-
-        self.alias = self._create_connection()
-        self.is_self_hosted = bool(
-            utility.get_server_type(using=self.alias) == "milvus"
-        )
-        if overwrite and utility.has_collection(self.collection_name, using=self.alias):
-            utility.drop_collection(self.collection_name, using=self.alias)
-
-        self._init(None)
+        conn = self._get_connection()
+        if kwargs.get("construct_only", False):
+            return
+        copy_kwargs = copy.deepcopy(kwargs)
+        if copy_kwargs.get("partition_name"):
+            copy_kwargs.pop("partition_name")
+        has = conn.has_partition(self._collection.name, self._name, **copy_kwargs)
+        if not has:
+            conn.create_partition(self._collection.name, self._name, **copy_kwargs)
+
+        self._schema_dict = self._schema.to_dict()
+        self._schema_dict["consistency_level"] = self._consistency_level
+
+    def __repr__(self):
+        return json.dumps({
+            'name': self.name,
+            'collection_name': self._collection.name,
+            'description': self.description,
+        })
+
+    def _get_connection(self):
+        return self._collection._get_connection()
+
+    @property
+    def description(self) -> str:
+        """ Return the description text.
+
+        :return:  Partition description
+        :rtype: str
+
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_description", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> partition.description
+            'comedy films'
+        """
+        return self._description
 
-    def __len__(self):
-        return self.num_entities()
+    @property
+    def name(self) -> str:
+        """
+        Return the partition name.
 
-    def num_entities(self):
-        """return the number of rows in the collection.
+        :return str: Partition name, return when operation is successful
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_name", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> partition.name
+            'comedy'
+        """
+        return self._name
 
-        Returns:
-            int: Number for rows.
+    @property
+    def is_empty(self) -> bool:
         """
-        if self.collection is None:
-            return 0
+        Returns whether the partition is empty
 
-        self.collection.flush()
-        return self.collection.num_entities
+        :return bool: Whether the partition is empty
+        * True: The partition is empty.
+        * False: The partition is not empty.
+
+        :example:
+
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_is_empty", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> partition.is_empty
+            True
+        """
+        return self.num_entities == 0
 
-    def insert_data(
-        self,
-        data: List[Dict[str, any]],
-        timeout: int = None,
-        batch_size: int = 100,
-        partition: str = None,
-        progress_bar: bool = False,
-    ) -> List[Union[str, int]]:
-        """Insert data into the collection.
+    @property
+    def num_entities(self, **kwargs) -> int:
+        """
+        Return the number of entities.
 
-        If the Milvus Client was initiated without an existing Collection, the first dict passed
-        in will be used to initiate the collection.
+        :return int: Number of entities in this partition.
 
-        Args:
-            data (List[Dict[str, any]]): A list of dicts to pass in. If list not provided, will
-                cast to list.
-            timeout (int, optional): The timeout to use, will override init timeout. Defaults
-                to None.
-            batch_size (int, optional): The batch size to perform inputs with. Defaults to 100.
-            partition (str, optional): Which partition to insert into. Defaults to None.
-            progress_bar (bool, optional): Whether to display a progress bar for the input.
-                Defaults to False.
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_num_entities", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> data = [
+            ...     [i for i in range(10)],
+            ...     [[float(i) for i in range(2)] for _ in range(10)],
+            ... ]
+            >>> partition.insert(data)
+            >>> partition.num_entities
+            10
+        """
+        conn = self._get_connection()
+        stats = conn.get_partition_stats(collection_name=self._collection.name, partition_name=self._name, **kwargs)
+        result = {stat.key: stat.value for stat in stats}
+        result["row_count"] = int(result["row_count"])
+        return result["row_count"]
+
+    def flush(self, timeout=None, **kwargs):
+        """ Flush """
+        conn = self._get_connection()
+        conn.flush([self._collection.name], timeout=timeout, **kwargs)
 
-        Raises:
-            DataNotMatchException: If the data has misssing fields an exception will be thrown.
-            MilvusException: General Milvus error on insert.
+    def drop(self, timeout=None, **kwargs):
+        """
+        Drop the partition, as well as its corresponding index files.
 
-        Returns:
-            List[Union[str, int]]: A list of primary keys that were inserted.
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :raises PartitionNotExistException:
+            When partitoin does not exist
+
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_drop", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> partition.drop()
         """
-        # If no data provided, we cannot input anything
-        if len(data) == 0:
-            return []
-
-        if batch_size < 1:
-            logger.error("Invalid batch size provided for insert.")
-
-            raise ValueError("Invalid batch size provided for insert.")
-
-        # If the collection hasnt been initialized, initialize it
-        with self.concurrent_lock:
-            if self.collection is None:
-                self._init(data[0])
-
-        # Dont include the primary key if auto_id is true and they included it in data
-        ignore_pk = self.pk_field if self.collection.schema.auto_id else None
-        insert_dict = {}
-        pks = []
-
-        for k in data:
-            for key, value in k.items():
-                if key in self.fields:
-                    insert_dict.setdefault(key, []).append(value)
-
-        for i in self.tqdm(range(0, len(data), batch_size), disable=not progress_bar):
-            # Convert dict to list of lists batch for insertion
-            try:
-                insert_batch = [
-                    insert_dict[key][i : i + batch_size]
-                    for key in self.fields
-                    if key != ignore_pk
-                ]
-            except KeyError as ex:
-                logger.error(
-                    "Malformed data, at least one of the inserts does not contain all"
-                    " the required fields."
-                )
-                raise KeyError(
-                    f"Malformed data, at least one of the inserts does not"
-                    f" the required fields: {ex}",
-                ) from ex
-            # Insert into the collection.
-            try:
-                res = self.collection.insert(
-                    insert_batch,
-                    timeout=timeout or self.timeout,
-                    partition_name=partition,
-                )
-                pks.extend(res.primary_keys)
-            except MilvusException as ex:
-                logger.error(
-                    "Failed to insert batch starting at entity: %s/%s",
-                    str(i),
-                    str(len(data)),
-                )
-                raise ex
-        return pks
-
-    def upsert_data(
-        self,
-        data: List[Dict[str, any]],
-        timeout: int = None,
-        batch_size: int = 100,
-        partition: str = None,
-        progress_bar: bool = False,
-    ) -> List[Union[str, int]]:
-        """WARNING: SLOW AND NOT ATOMIC. Will be updated for 2.3 release.
+        conn = self._get_connection()
+        if conn.has_partition(self._collection.name, self._name, timeout=timeout, **kwargs) is False:
+            raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
+        return conn.drop_partition(self._collection.name, self._name, timeout=timeout, **kwargs)
 
-        Upsert the data into the collection.
+    def load(self, replica_number=1, timeout=None, **kwargs):
+        """
+        Load the partition from disk to memory.
 
-        If the Milvus Client was initiated without an existing Collection, the first dict passed
-        in will be used to initiate the collection.
+        :param replica_number: The replication numbers to load.
+        :type  replica_number: int
 
-        Args:
-            data (List[Dict[str, any]]): A list of dicts to upsert.
-            timeout (int, optional): The timeout to use, will override init timeout. Defaults
-                to None.
-            batch_size (int, optional): The batch size to perform inputs with. Defaults to 100.
-            partition (str, optional): Which partition to insert into. Defaults to None.
-            progress_bar (bool, optional): Whether to display a progress bar for the input.
-                Defaults to False.
-        Returns:
-            List[Union[str, int]]: A list of primary keys that were inserted.
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :raises ParamError:
+            If params are invalid
+
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_load", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> partition.load()
         """
-        # If the collection exists we need to first delete the values
-        if self.collection is not None:
-            pks = [x[self.pk_field] for x in data]
-            self.delete_by_pk(pks, timeout)
-
-        ret = self.insert_data(
-            data=data,
-            timeout=timeout,
-            batch_size=batch_size,
-            partition=partition,
-            progress_bar=progress_bar,
-        )
-
-        return ret
-
-    def search_data(
-        self,
-        data: Union[List[list], list],
-        top_k: int = 10,
-        filter_expression: str = None,
-        return_fields: List[str] = None,
-        partitions: List[str] = None,
-        search_params: dict = None,
-        timeout: int = None,
-    ) -> List[dict]:
-        """Search for a query vector/vectors.
+        # TODO(yukun): If field_names is not None and not equal schema.field_names,
+        #  raise Exception Not Supported,
+        #  if index_names is not None, raise Exception Not Supported
+        conn = self._get_connection()
+        if conn.has_partition(self._collection.name, self._name, **kwargs):
+            return conn.load_partitions(self._collection.name, [self._name], replica_number, timeout=timeout, **kwargs)
+        raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
 
-        In order for the search to process, a collection needs to have been either provided
-        at init or data needs to have been inserted.
+    def release(self, timeout=None, **kwargs):
+        """
+        Release the partition from memory.
 
-        Args:
-            data (Union[List[list], list]): The vector/vectors to search.
-            top_k (int, optional): How many results to return per search. Defaults to 10.
-            filter_expression (str, optional): A filter to use for the search. Defaults to None.
-            return_fields (List[str], optional): List of which field values to return. If None
-                specified, all fields excluding vector field will be returned.
-            search_params (dict, optional): The search params to use for the search. Will default
-                to the default set for the client.
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :raises PartitionNotExistException:
+            When partitoin does not exist
+
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_release", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> partition.load()
+            >>> partition.release()
+        """
+        conn = self._get_connection()
+        if conn.has_partition(self._collection.name, self._name, **kwargs):
+            return conn.release_partitions(self._collection.name, [self._name], timeout=timeout, **kwargs)
+        raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
 
+    def insert(self, data, timeout=None, **kwargs):
+        """
+        Insert data into partition.
 
-            partitions (List[str], optional): Which partitions to search within. Defaults to
-                searching through all.
-            timeout (int, optional): Timeout to use, overides the client level assigned at init.
-                Defaults to None.
+        :param data: The specified data to insert, the dimension of data needs to align with column
+                     number
+        :type  data: list-like(list, tuple) object or pandas.DataFrame
+
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :param kwargs:
+            * *timeout* (``float``) --
+              An optional duration of time in seconds to allow for the RPC. When timeout
+              is set to None, client waits until server response or error occur.
+
+        :return: A MutationResult object contains a property named `insert_count` represents how many
+        entities have been inserted into milvus and a property named `primary_keys` is a list of primary
+        keys of the inserted entities.
+        :rtype: MutationResult
+
+        :raises PartitionNotExistException:
+            When partitoin does not exist
+
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_insert", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> data = [
+            ...     [i for i in range(10)],
+            ...     [[float(i) for i in range(2)] for _ in range(10)],
+            ... ]
+            >>> partition.insert(data)
+            >>> partition.num_entities
+            10
+        """
+        conn = self._get_connection()
+        if conn.has_partition(self._collection.name, self._name, **kwargs) is False:
+            raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
+        # TODO: check insert data schema here?
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._collection.schema)
+        res = conn.batch_insert(self._collection.name, entities=entities, partition_name=self._name,
+            timeout=timeout, orm=True, schema=self._schema_dict, **kwargs)
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
+        return MutationResult(res)
+
+    def delete(self, expr, timeout=None, **kwargs):
+        """ Delete entities with an expression condition.
+
+        :param expr: The expression to specify entities to be deleted
+        :type  expr: str
+
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :return: A MutationResult object contains a property named `delete_count` represents how many
+                 entities will be deleted.
+        :rtype: MutationResult
+
+        :raises RpcError: If gRPC encounter an error
+        :raises ParamError: If parameters are invalid
+        :raises BaseException: If the return result from server is not ok
+
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> test_collection = Collection("test_partition_delete", schema)
+            >>> test_partition = test_collection.create_partition("comedy", "comedy films")
+            >>> data = [
+            ...     [i for i in range(10)],
+            ...     [[float(i) for i in range(2)] for _ in range(10)],
+            ... ]
+            >>> test_partition.insert(data)
+            (insert count: 10, delete count: 0, upsert count: 0, timestamp: 431044482906718212)
+            >>> test_partition.num_entities
+            10
+            >>> test_partition.delete("film_id in [0, 1]")
+            (insert count: 0, delete count: 2, upsert count: 0, timestamp: 431044582560759811)
+        """
 
-        Raises:
-            ValueError: The collection being searched doesnt exist. Need to insert data first.
+        conn = self._get_connection()
+        res = conn.delete(self._collection.name, expr, self.name, timeout=timeout, **kwargs)
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
+        return MutationResult(res)
 
-        Returns:
-            List[dict]: A list of dicts containing the score and the result data. Embeddings are
-                not included in the result data.
+    def upsert(self, data, timeout=None, **kwargs):
         """
+        Upsert data into partition.
 
-        # TODO: Figure out thread safety
-        # with self.concurrent_lock:
-        #     self.concurrent_counter += 1
-
-        if self.collection is None:
-            logger.error("Collection does not exist: %s", self.collection_name)
-            raise ValueError(
-                "Missing collection. Make sure data inserted or intialized on existing collection."
-            )
-
-        if not isinstance(data[0], list):
-            data = [data]
-        if return_fields is None or len(return_fields) == 0:
-            return_fields = list(self.fields.keys())
-            return_fields.remove(self.vector_field)
-
-        try:
-            res = self.collection.search(
-                data,
-                anns_field=self.vector_field,
-                expr=filter_expression,
-                param=search_params or self.default_search_params,
-                limit=top_k,
-                partition_names=partitions,
-                output_fields=return_fields,
-                timeout=timeout or self.timeout,
-            )
-        except Exception as ex:
-            logger.error("Failed to search collection: %s", self.collection_name)
-            raise ex
-
-        ret = []
-        for hits in res:
-            query_result = []
-            for hit in hits:
-                ret_dict = {x: hit.entity.get(x) for x in return_fields}
-                query_result.append({"score": hit.score, "data": ret_dict})
-            ret.append(query_result)
-
-        # TODO: Figure out thread safety
-        # with self.concurrent_lock:
-        #     self.concurrent_counter -= 1
-        return ret
-
-    def query_data(
-        self,
-        filter_expression: str,
-        return_fields: List[str] = None,
-        partitions: List[str] = None,
-        timeout: int = None,
-    ) -> List[dict]:
-        """Query for entries in the Collection.
+        :param data: The specified data to upsert, the dimension of data needs to align with column
+                     number
+        :type  data: list-like(list, tuple) object or pandas.DataFrame
+
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :param kwargs:
+            * *timeout* (``float``) --
+              An optional duration of time in seconds to allow for the RPC. When timeout
+              is set to None, client waits until server response or error occur.
+
+        :return: A MutationResult object contains a property named `upsert_count` represents how many
+        entities have been upserted at milvus and a property named `primary_keys` is a list of primary
+        keys of the upserted entities.
+        :rtype: MutationResult
+
+        :raises PartitionNotExistException:
+            When partitoin does not exist
+
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_upsert", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> data = [
+            ...     [i for i in range(10)],
+            ...     [[float(i) for i in range(2)] for _ in range(10)],
+            ... ]
+            >>> partition.upsert(data)
+            >>> partition.num_entities
+            10
+        """
+        conn = self._get_connection()
+        if conn.has_partition(self._collection.name, self._name, **kwargs) is False:
+            raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
+        # TODO: check upsert data schema here?
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._collection.schema,False)
+        res = conn.upsert(self._collection.name, entities=entities, partition_name=self._name,
+            timeout=timeout, orm=True, schema=self._schema_dict, **kwargs)
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
+        return MutationResult(res)
+
+    def search(self, data, anns_field, param, limit,
+               expr=None, output_fields=None, timeout=None, round_decimal=-1, **kwargs):
+        """ Conducts a vector similarity search with an optional boolean expression as filter.
 
         Args:
-            filter_expression (str): The filter to use for the query.
-            return_fields (List[str], optional): List of which field values to return. If None
-                specified, all fields excluding vector field will be returned.
-            partitions (List[str], optional): Which partitions to perform query. Defaults to None.
-            timeout (int, optional): Timeout to use, overides the client level assigned at init.
-                Defaults to None.
+            data (``List[List[float]]``): The vectors of search data.
+                the length of data is number of query (nq), and the dim of every vector in data must be equal to
+                the vector field's of collection.
+            anns_field (``str``): The name of the vector field used to search of collection.
+            param (``dict[str, Any]``):
 
-        Raises:
-            ValueError: Missing collection.
+                The parameters of search. The followings are valid keys of param.
 
-        Returns:
-            List[dict]: A list of result dicts, vectors are not included.
-        """
+                * *nprobe*, *ef*, *search_k*, etc
+                    Corresponding search params for a certain index.
 
-        # TODO: Figure out thread safety
-        # with self.concurrent_lock:
-        #     self.concurrent_counter += 1
-
-        if self.collection is None:
-            logger.error("Collection does not exist: %s", self.collection_name)
-            raise ValueError(
-                "Missing collection. Make sure data inserted or intialized on existing collection."
-            )
-
-        if return_fields is None or len(return_fields) == 0:
-            return_fields = list(self.fields.keys())
-            return_fields.remove(self.vector_field)
-
-        res = self.collection.query(
-            expr=filter_expression,
-            partition_names=partitions,
-            output_fields=return_fields,
-            timeout=timeout or self.timeout,
-        )
-
-        # TODO: Figure out thread safety
-        # with self.concurrent_lock:
-        #     self.concurrent_counter -= 1
+                * *metric_type* (``str``)
+                    similar metricy types, the value must be of type str.
 
-        return res
+                * *offset* (``int``, optional)
+                    offset for pagination.
 
-    def get_vectors_by_pk(
-        self,
-        pks: Union[list, str, int],
-        timeout: int = None,
-    ) -> List[List[float]]:
-        """Grab the inserted vectors using the primary key from the Collection.
+                * *limit* (``int``, optional)
+                    limit for the search results and pagination.
 
-        Due to current implementations, grabbing a large amount of vectors is slow.
+                example for param::
 
-        Args:
-            pks (str): The pk's to get vectors for. Depending on pk_field type it can be int or str
-            or a list of either.
-            timeout (int, optional): Timeout to use, overides the client level assigned at
-                init. Defaults to None.
+                    {
+                        "nprobe": 128,
+                        "metric_type": "L2",
+                        "offset": 10,
+                        "limit": 10,
+                    }
 
-        Raises:
-            ValueError: Missing collection.
+            limit (``int``): The max number of returned record, also known as `topk`.
+            expr (``str``): The boolean expression used to filter attribute. Default to None.
 
-        Returns:
-            List[dict]: A list of result dicts with keys {pk_field, vector_field}
-        """
+                example for expr::
 
-        # TODO: Figure out thread safety
-        # with self.concurrent_lock:
-        #     self.concurrent_counter += 1
-
-        if self.collection is None:
-            logger.error("Collection does not exist: %s", self.collection_name)
-            raise ValueError(
-                "Missing collection. Make sure data inserted or intialized on existing collection."
-            )
-
-        if not isinstance(pks, list):
-            pks = [pks]
-
-        if len(pks) == 0:
-            return []
-
-        # Varchar pks need double quotes around the values
-        if self.fields[self.pk_field] == DataType.VARCHAR:
-            ids = ['"' + str(entry) + '"' for entry in pks]
-            expr = f"""{self.pk_field} in [{','.join(ids)}]"""
-        else:
-            ids = [str(entry) for entry in pks]
-            expr = f"{self.pk_field} in [{','.join(ids)}]"
-
-        res = self.collection.query(
-            expr=expr,
-            output_fields=[self.vector_field],
-            timeout=timeout or self.timeout,
-        )
-
-        # TODO: Figure out thread safety
-        # with self.concurrent_lock:
-        #     self.concurrent_counter -= 1
+                    "id_field >= 0", "id_field in [1, 2, 3, 4]"
 
-        return res
+            output_fields (``List[str]``, optional):
+                The name of fields to return in the search result.  Can only get scalar fields.
+            round_decimal (``int``, optional): The specified number of decimal places of returned distance
+                Defaults to -1 means no round to returned distance.
+            **kwargs (``dict``): Optional search params
 
-    def delete_by_pk(
-        self,
-        pks: Union[list, str, int],
-        timeout: int = None,
-    ) -> None:
-        """Delete entries in the collection by their pk.
+                *  *_async* (``bool``, optional)
+                    Indicate if invoke asynchronously.
+                    Returns a SearchFuture if True, else returns results from server directly.
 
-        Delete all the entries based on the pk. If unsure of pk you can first query the collection
-        to grab the corresponding data. Then you can delete using the pk_field.
+                * *_callback* (``function``, optional)
+                    The callback function which is invoked after server response successfully.
+                    It functions only if _async is set to True.
 
-        Args:
-            pks (list, str, int): The pk's to delete. Depending on pk_field type it can be int
-                or str or alist of either.
-            timeout (int, optional): Timeout to use, overides the client level assigned at init.
-                Defaults to None.
-        """
+                * *consistency_level* (``str/int``, optional)
+                    Which consistency level to use when searching in the collection.
 
-        # TODO: Figure out thread safety
-        # with self.concurrent_lock:
-        #     self.concurrent_counter += 1
+                    Options of consistency level: Strong, Bounded, Eventually, Session, Customized.
 
-        if self.collection is None:
-            logger.error("Collection does not exist: %s", self.collection_name)
-            return
+                    Note: this parameter will overwrite the same parameter specified when user created the collection,
+                    if no consistency level was specified, search will use the consistency level when you create the
+                    collection.
 
-        if not isinstance(pks, list):
-            pks = [pks]
+                * *guarantee_timestamp* (``int``, optional)
+                    Instructs Milvus to see all operations performed before this timestamp.
+                    By default Milvus will search all operations performed to date.
 
-        if len(pks) == 0:
-            return
+                    Note: only valid in Customized consistency level.
 
-        if self.fields[self.pk_field] == DataType.VARCHAR:
-            ids = ['"' + str(entry) + '"' for entry in pks]
-            expr = f"""{self.pk_field} in [{','.join(ids)}]"""
-        else:
-            ids = [str(entry) for entry in pks]
-            expr = f"{self.pk_field} in [{','.join(ids)}]"
-
-        self.collection.delete(expr=expr, timout=timeout or self.timeout)
-
-        # TODO: Figure out thread safety
-        # with self.concurrent_lock:
-        #     self.concurrent_counter -= 1
+                * *graceful_time* (``int``, optional)
+                    Search will use the (current_timestamp - the graceful_time) as the
+                    `guarantee_timestamp`. By default with 5s.
 
-    def add_partitions(self, input_partitions: List[str]):
-        """Add partitions to the collection.
+                    Note: only valid in Bounded consistency level
 
-        Add a list of partition names to the collection. If the collection is loaded
-        it will first be unloaded, then the partitions will be added, and then reloaded.
+                * *travel_timestamp* (``int``, optional)
+                    A specific timestamp to get results based on a data view at.
 
-        Args:
-            input_partitions (List[str]): The list of partition names to be added.
+        Returns:
+            SearchResult:
+                Returns ``SearchResult`` if `_async` is False , otherwise ``SearchFuture``
+
+        .. _Metric type documentations:
+            https://milvus.io/docs/v2.2.x/metric.md
+        .. _Index documentations:
+            https://milvus.io/docs/v2.2.x/index.md
+        .. _How guarantee ts works:
+            https://github.com/milvus-io/milvus/blob/master/docs/developer_guides/how-guarantee-ts-works.md
 
         Raises:
-            MilvusException: Unable to add the partition.
+            MilvusException: If anything goes wrong
+
+        :example:
+            >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType
+            >>> import random
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_collection_search", schema)
+            >>> collection.create_index("films", {"index_type": "FLAT", "metric_type": "L2", "params": {}})
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> # insert
+            >>> data = [
+            ...     [i for i in range(10)],
+            ...     [[random.random() for _ in range(2)] for _ in range(10)],
+            ... ]
+            >>> partition.insert(data)
+            >>> partition.load()
+            >>> # search
+            >>> search_param = {
+            ...     "data": [[1.0, 1.0]],
+            ...     "anns_field": "films",
+            ...     "param": {"metric_type": "L2"},
+            ...     "limit": 2,
+            ...     "expr": "film_id > 0",
+            ... }
+            >>> res = partition.search(**search_param)
+            >>> assert len(res) == 1
+            >>> hits = res[0]
+            >>> assert len(hits) == 2
+            >>> print(f"- Total hits: {len(hits)}, hits ids: {hits.ids} ")
+            - Total hits: 2, hits ids: [8, 5]
+            >>> print(f"- Top1 hit id: {hits[0].id}, distance: {hits[0].distance}, score: {hits[0].score} ")
+            - Top1 hit id: 8, distance: 0.10143111646175385, score: 0.10143111646175385
         """
-        if self.collection is not None and self.is_self_hosted:
-            # Calculate which partitions need to be added
-            input_partitions = set(input_partitions)
-            current_partitions = {
-                partition.name for partition in self.collection.partitions
-            }
-            new_partitions = input_partitions.difference(current_partitions)
-            # If partitions need to be added, add them
-            if len(new_partitions) != 0:
-                # TODO: Remove with Milvus 2.3
-                # Try to unload the collection
-                self.collection.release()
-                try:
-                    for part in new_partitions:
-                        self.collection.create_partition(part)
-                    logger.debug(
-                        "Successfully added partitions to collection: %s partitions: %s",
-                        self.collection_name,
-                        ",".join(part for part in list(new_partitions)),
-                    )
-                    # TODO: Remove with Milvus 2.3
-                    self._load()
-                except MilvusException as ex:
-                    logger.debug(
-                        "Failed to add partitions to: %s", self.collection_name
-                    )
-                    # TODO: Remove with Milvus 2.3
-                    # Even if failed, attempt to reload collection
-                    self._load()
-                    raise ex
-            else:
-                logger.debug(
-                    "No parititons to add for collection: %s", self.collection_name
-                )
-        else:
-            logger.debug(
-                "Collection either on Zilliz or non existant for collection: %s",
-                self.collection_name,
-            )
+        conn = self._get_connection()
+        res = conn.search(self._collection.name, data, anns_field, param, limit, expr, [self._name], output_fields,
+                          round_decimal=round_decimal, timeout=timeout, schema=self._schema_dict, **kwargs)
+        if kwargs.get("_async", False):
+            return SearchFuture(res)
+        return SearchResult(res)
 
-    def delete_partitions(self, remove_partitions: List[str]):
-        """Remove partitions from the collection.
+    def query(self, expr, output_fields=None, timeout=None, **kwargs):
+        """
+        Query with a set of criteria, and results in a list of records that match the query exactly.
 
-        Remove a list of partition names from the collection. If the collection is loaded
-        it will first be unloaded, then the partitions will be removed, and then reloaded.
+        :param expr: The query expression
+        :type  expr: str
 
-        Args:
-            remove_partitions (List[str]): The list of partition names to be removed.
+        :param output_fields: A list of fields to return
+        :type  output_fields: list[str]
 
-        Raises:
-            MilvusException: Unable to remove the partition.
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :param kwargs:
+            * *consistency_level* (``str/int``) --
+              Which consistency level to use during a query on the collection. For details, see
+              https://github.com/milvus-io/milvus/blob/master/docs/developer_guides/how-guarantee-ts-works.md.
+              Note: this parameter will overwrite the same parameter specified when user created the collection,
+              if no consistency level was specified, query will use the collection consistency level.
+            * *guarantee_timestamp* (``int``) --
+              This function instructs Milvus to see all operations performed before a provided timestamp. If no
+              such timestamp is specified, Milvus will query all operations performed to date.
+              Note: only used in Customized consistency level.
+            * *graceful_time* (``int``) --
+              Only used in bounded consistency level. If graceful_time is set, PyMilvus will use current timestamp minus
+              the graceful_time as the `guarantee_timestamp`. This option is 5s by default if not set.
+            * *travel_timestamp* (``int``) --
+              Users can specify a timestamp in a search to get results based on a data view
+              at a specified point in time.
+
+        :return: A list that contains all results
+        :rtype: list
+
+        :raises RpcError: If gRPC encounter an error
+        :raises ParamError: If parameters are invalid
+        :raises BaseException: If the return result from server is not ok
+
+        :example:
+            >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType
+            >>> import random
+            >>> connections.connect()
+            <pymilvus.client.stub.Milvus object at 0x7f8579002dc0>
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("film_date", DataType.INT64),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_collection_query", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> # insert
+            >>> data = [
+            ...     [i for i in range(10)],
+            ...     [i + 2000 for i in range(10)],
+            ...     [[random.random() for _ in range(2)] for _ in range(10)],
+            ... ]
+            >>> partition.insert(data)
+            >>> partition.num_entities
+            10
+            >>> partition.load()
+            >>> # query
+            >>> expr = "film_id in [ 0, 1 ]"
+            >>> res = partition.query(expr, output_fields=["film_date"])
+            >>> assert len(res) == 2
+            >>> print(f"- Query results: {res}")
+            - Query results: [{'film_id': 0, 'film_date': 2000}, {'film_id': 1, 'film_date': 2001}]
         """
-        if self.collection is not None and self.is_self_hosted:
-            # Calculate which partitions need to be removed
-            remove_partitions = set(remove_partitions)
-            current_partitions = {
-                partition.name for partition in self.collection.partitions
-            }
-            removal_partitions = remove_partitions.intersection(current_partitions)
-            # If partitions need to be added, add them
-            if len(removal_partitions) != 0:
-                # TODO: Remove with Milvus 2.3
-                # Try to unload the collection
-                self.collection.release()
-                try:
-                    for part in removal_partitions:
-                        self.collection.drop_partition(part)
-                    logger.debug(
-                        "Successfully deleted partitions from collection: %s partitions: %s",
-                        self.collection_name,
-                        ",".join(part for part in list(removal_partitions)),
-                    )
-                    # TODO: Remove with Milvus 2.3
-                    self._load()
-                except MilvusException as ex:
-                    logger.debug(
-                        "Failed to delete partitions from: %s", self.collection_name
-                    )
-                    # TODO: Remove with Milvus 2.3
-                    # Even if failed, attempt to reload collection
-                    self._load()
-                    raise ex
-            else:
-                logger.debug(
-                    "No parititons to delete for collection: %s",
-                    self.collection_name,
-                )
-
-    def delete_collection(self):
-        """Delete the collection stored in this object"""
-        with self.concurrent_lock:
-            if self.collection is None:
-                return
-            self.collection.drop()
-            self.collection = None
-
-    def close(self, delete_collection=False):
-        if delete_collection:
-            self.delete_collection()
-        connections.disconnect(self.alias)
-
-    def _create_connection(self) -> str:
-        """Create the connection to the Milvus server."""
-        # TODO: Implement reuse with new uri style
-        alias = uuid4().hex
-        try:
-            connections.connect(alias=alias, uri=self.uri)
-            logger.debug("Created new connection using: %s", alias)
-            return alias
-        except MilvusException as ex:
-            logger.error("Failed to create new connection using: %s", alias)
-            raise ex
-
-    def _init(self, input_data: dict):
-        """Create/connect to the colletion"""
-        # If no input data and collection exists, use that
-        if input_data is None and utility.has_collection(
-            self.collection_name, using=self.alias
-        ):
-            self.collection = Collection(self.collection_name, using=self.alias)
-            # Grab the field information from the existing collection
-            self._extract_fields()
-        # If data is supplied we can create a new collection
-        elif input_data is not None:
-            self._create_collection(input_data)
-        # Nothin to init from
-        else:
-            logger.debug(
-                "No information to perform init from for collection %s",
-                self.collection_name,
-            )
-            return
+        conn = self._get_connection()
+        res = conn.query(self._collection.name, expr, output_fields, [self._name],
+                         timeout=timeout, schema=self._schema_dict, **kwargs)
+        return res
+
+    def get_replicas(self, timeout=None, **kwargs) -> Replica:
+        """get_replicas returns the current collection's replica information
 
-        # TODO: Make sure this drops the correct index
-        if self.index_params is not None:
-            self.collection.drop_index()
-
-        self._create_index()
-        # Partitions only allowed on Milvus at the moment
-        if self.is_self_hosted and self.partitions is not None:
-            self.add_partitions(self.partitions)
-        self._create_default_search_params()
-        self._load()
-
-    def _create_collection(self, data: dict) -> None:
-        """Create the collection by autoinferring the schema."""
-
-        fields = self._infer_fields(data)
-
-        if self.vector_field is None:
-            logger.error(
-                "vector_field not supplied at init(), cannot infer schema from data collection: %s",
-                self.collection_name,
-            )
-            raise ValueError(
-                "vector_field not supplied at init(), cannot infer schema."
-            )
-
-        if self.vector_field not in fields:
-            logger.error(
-                "Missing vector_field: %s in data for collection: %s",
-                self.vector_field,
-                self.collection_name,
-            )
-            raise ValueError(
-                "vector_field missing in inserted data, cannot infer schema."
-            )
-
-        if fields[self.vector_field]["dtype"] not in (
-            DataType.BINARY_VECTOR,
-            DataType.FLOAT_VECTOR,
-        ):
-            logger.error(
-                "vector_field: %s does not correspond with vector dtype in data for collection: %s",
-                self.vector_field,
-                self.collection_name,
-            )
-            raise ValueError("vector_field does not correspond to vector dtype.")
-
-        if fields[self.vector_field]["dtype"] == DataType.BINARY_VECTOR:
-            dim = 8 * len(data[self.vector_field])
-        elif fields[self.vector_field]["dtype"] == DataType.FLOAT_VECTOR:
-            dim = len(data[self.vector_field])
-        # Attach dim kwarg to vector field
-        fields[self.vector_field]["dim"] = dim
-
-        # If pk not provided, created autoid pk
-        if self.pk_field is None:
-            # Generate a unique auto-id field
-            self.pk_field = "internal_pk_" + uuid4().hex[:4]
-            # Create a new field for pk
-            fields[self.pk_field] = {}
-            fields[self.pk_field]["name"] = self.pk_field
-            fields[self.pk_field]["dtype"] = DataType.INT64
-            fields[self.pk_field]["auto_id"] = True
-            fields[self.pk_field]["is_primary"] = True
-            logger.debug(
-                "Missing pk_field, creating auto-id pk for collection: %s",
-                self.collection_name,
-            )
-        # If pk_field given, we assume it will be provided for all inputs
-        else:
-            try:
-                fields[self.pk_field]["auto_id"] = False
-                fields[self.pk_field]["is_primary"] = True
-            except KeyError as ex:
-                logger.error(
-                    "Missing pk_field: %s in data for collection: %s",
-                    self.pk_field,
-                    self.collection_name,
-                )
-                raise ex
-        try:
-            # Create the fieldschemas
-            fieldschemas = []
-            # TODO: Assuming ordered dicts for 3.7
-            self.fields = {}
-            for field_dict in fields.values():
-                fieldschemas.append(FieldSchema(**field_dict))
-                self.fields[field_dict["name"]] = field_dict["dtype"]
-            # Create the schema for the collection
-            schema = CollectionSchema(fieldschemas)
-            # Create the collection
-            self.collection = Collection(
-                name=self.collection_name,
-                schema=schema,
-                consistency_level=self.consistency_level,
-                num_shards=self.num_shards,
-                num_partitions=self.num_partitions,
-                using=self.alias,
-            )
-            logger.debug("Successfully created collection: %s", self.collection_name)
-        except MilvusException as ex:
-            logger.error("Failed to create collection: %s", self.collection_name)
-            raise ex
-
-    def _infer_fields(self, data):
-        """Infer all the fields based on the input data."""
-        # TODO: Assuming ordered dict for 3.7
-        fields = {}
-        # Figure out each datatype of the input.
-        for key, value in data.items():
-            # Infer the corresponding datatype of the metadata
-            dtype = infer_dtype_bydata(value)
-            # Datatype isnt compatible
-            if dtype in (DataType.UNKNOWN, DataType.NONE):
-                logger.error(
-                    "Failed to parse schema for collection %s, unrecognized dtype for key: %s",
-                    self.collection_name,
-                    key,
-                )
-                raise ValueError(f"Unrecognized datatype for {key}.")
-
-            # Create an entry under the field name
-            fields[key] = {}
-            fields[key]["name"] = key
-            fields[key]["dtype"] = dtype
-
-            # Area for attaching kwargs for certain datatypes
-            if dtype == DataType.VARCHAR:
-                fields[key]["max_length"] = 65_535
-
-        return fields
-
-    def _extract_fields(self) -> None:
-        """Grab the existing fields from the Collection"""
-        self.fields = {}
-        schema = self.collection.schema
-        for field in schema.fields:
-            field_dict = field.to_dict()
-            if field_dict.get("is_primary", None) is not None:
-                logger.debug("Updating pk_field with one from collection.")
-                self.pk_field = field_dict["name"]
-            if field_dict["type"] in (DataType.FLOAT_VECTOR, DataType.BINARY_VECTOR):
-                logger.debug("Updating vector_field  with one from collection.")
-                self.vector_field = field_dict["name"]
-            self.fields[field_dict["name"]] = field_dict["type"]
-
-        logger.debug(
-            "Successfully extracted fields from for collection: %s, total fields: %s, "
-            "pk_field: %s, vector_field: %s",
-            self.collection_name,
-            len(self.fields),
-            self.pk_field,
-            self.vector_field,
-        )
-
-    def _create_index(self) -> None:
-        """Create a index on the collection"""
-        if self._get_index() is None:
-            # If no index params, use a default HNSW based one
-            if self.index_params is None:
-                # TODO: Once segment normalization we can default to IP
-                metric_type = (
-                    self.distance_metric
-                    if self.fields[self.vector_field] == DataType.FLOAT_VECTOR
-                    else "JACCARD"
-                )
-                # TODO: Once AUTOINDEX type is supported by Milvus we can default to HNSW always
-                index_type = "HNSW" if self.is_self_hosted else "AUTOINDEX"
-                params = {"M": 8, "efConstruction": 64} if self.is_self_hosted else {}
-                self.index_params = {
-                    "metric_type": metric_type,
-                    "index_type": index_type,
-                    "params": params,
-                }
-            try:
-                self.collection.create_index(
-                    self.vector_field,
-                    index_params=self.index_params,
-                    using=self.alias,
-                    timeout=self.timeout,
-                )
-                logger.debug(
-                    "Successfully created an index on collection: %s",
-                    self.collection_name,
-                )
-            except MilvusException as ex:
-                logger.error(
-                    "Failed to create an index on collection: %s", self.collection_name
-                )
-                raise ex
-        else:
-            logger.debug(
-                "Index exists already for collection: %s", self.collection_name
-            )
-
-    def _get_index(self):
-        """Return the index dict if index exists."""
-        for index in self.collection.indexes:
-            if index.field_name == self.vector_field:
-                return index
-        return None
-
-    def _create_default_search_params(self) -> None:
-        """Generate search params based on the current index type"""
-        index = self._get_index().to_dict()
-        if index is not None:
-            index_type = index["index_param"]["index_type"]
-            metric_type = index["index_param"]["metric_type"]
-            self.default_search_params = DEFAULT_SEARCH_PARAMS[index_type]
-            self.default_search_params["metric_type"] = metric_type
-
-    def _load(self):
-        """Loads the collection."""
-        if self._get_index() is not None:
-            if self.is_self_hosted:
-                try:
-                    self.collection.load(replica_number=self.replica_number)
-                    logger.debug(
-                        "Collection loaded: %s",
-                        self.collection_name,
-                    )
-                # If the replica count is incorrect, release the collection
-                except MilvusException:
-                    try:
-                        self.collection.release(timeout=self.timeout)
-                        self.collection.load(replica_number=self.replica_number)
-                        logger.debug(
-                            "Successfully reloaded collection: %s",
-                            self.collection_name,
-                        )
-                    except MilvusException as ex:
-                        logger.error(
-                            "Failed to load collection: %s",
-                            self.collection_name,
-                        )
-                        raise ex
-            else:
-                try:
-                    self.collection.load(replica_number=1)
-                    logger.debug(
-                        "Collection loaded: %s",
-                        self.collection_name,
-                    )
-                # If both loads fail, raise exception
-                except MilvusException as ex:
-                    logger.error("Failed to load collection: %s", self.collection_name)
-                    raise ex
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :raises BaseException: If the collection does not exist.
+
+        :example:
+        """
+        conn = self._get_connection()
+        return conn.get_replicas(self._collection.name, timeout=timeout, **kwargs)
```

### Comparing `pymilvus-2.2.9/pymilvus/orm/__init__.py` & `pymilvus-2.3.0b1/pymilvus/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/pymilvus/orm/collection.py` & `pymilvus-2.3.0b1/pymilvus/orm/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import copy
 import json
-from typing import List, Union, Dict
+from typing import List, Union
 import pandas
 
 from .connections import connections
 from .schema import (
     CollectionSchema,
     FieldSchema,
-    construct_fields_from_dataframe,
-    check_insert_data_schema,
-    check_insert_or_upsert_is_row_based,
+    parse_fields_from_data,
+    check_insert_or_upsert_data_schema,
     check_schema,
 )
 from .prepare import Prepare
 from .partition import Partition
 from .index import Index
 from .search import SearchResult
 from .mutation import MutationResult
@@ -37,46 +36,45 @@
     PartitionNotExistException,
     IndexNotExistException,
     AutoIDException,
     ExceptionsMessage,
 )
 from .future import SearchFuture, MutationFuture
 from .utility import _get_connection
-from ..settings import Config
+from .default_config import DefaultConfig
 from ..client.types import CompactionState, CompactionPlans, Replica, get_consistency_level, cmp_consistency_level
 from ..client.constants import DEFAULT_CONSISTENCY_LEVEL
+from ..client.configs import DefaultConfigs
 
 
 
 class Collection:
-    def __init__(self, name: str, schema: CollectionSchema=None, using: str="default",  **kwargs):
+    def __init__(self, name: str, schema: CollectionSchema=None, using: str="default", shards_num: int=2, **kwargs):
         """ Constructs a collection by name, schema and other parameters.
 
         Args:
             name (``str``): the name of collection
             schema (``CollectionSchema``, optional): the schema of collection, defaults to None.
             using (``str``, optional): Milvus connection alias name, defaults to 'default'.
+            shards_num (``int``, optional): how many shards will the insert data be divided, defaults to 2.
             **kwargs (``dict``):
 
-                * *num_shards (``int``, optional): how many shards will the insert data be divided.
-                * *shards_num (``int``, optional, deprecated): how many shards will the insert data be divided.
                 * *consistency_level* (``int/ str``)
                     Which consistency level to use when searching in the collection.
                     Options of consistency level: Strong, Bounded, Eventually, Session, Customized.
 
                     Note: this parameter can be overwritten by the same parameter specified in search.
 
                 * *properties* (``dict``, optional)
                     Collection properties.
 
                 * *timeout* (``float``)
                     An optional duration of time in seconds to allow for the RPCs.
                     If timeout is not set, the client keeps waiting until the server responds or an error occurs.
 
-
         Raises:
             SchemaNotReadyException: if the schema is wrong.
 
         Examples:
             >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
             >>> fields = [
@@ -87,16 +85,16 @@
             >>> properties = {"collection.ttl.seconds": 1800}
             >>> collection = Collection(name="test_collection_init", schema=schema, properties=properties)
             >>> collection.name
             'test_collection_init'
         """
         self._name = name
         self._using = using
+        self._shards_num = shards_num
         self._kwargs = kwargs
-        self._num_shards = None
         conn = self._get_connection()
 
         has = conn.has_collection(self._name, **kwargs)
         if has:
             resp = conn.describe_collection(self._name, **kwargs)
             s_consistency_level = resp.get("consistency_level", DEFAULT_CONSISTENCY_LEVEL)
             arg_consistency_level = kwargs.get("consistency_level", s_consistency_level)
@@ -115,27 +113,27 @@
 
         else:
             if schema is None:
                 raise SchemaNotReadyException(message=ExceptionsMessage.CollectionNotExistNoSchema % name)
             if isinstance(schema, CollectionSchema):
                 check_schema(schema)
                 consistency_level = get_consistency_level(kwargs.get("consistency_level", DEFAULT_CONSISTENCY_LEVEL))
-
-                conn.create_collection(self._name, schema, **kwargs)
+                conn.create_collection(self._name, schema, shards_num=self._shards_num, **kwargs)
                 self._schema = schema
                 self._consistency_level = consistency_level
             else:
                 raise SchemaNotReadyException(message=ExceptionsMessage.SchemaType)
 
         self._schema_dict = self._schema.to_dict()
         self._schema_dict["consistency_level"] = self._consistency_level
 
     def __repr__(self):
         _dict = {
             'name': self.name,
+            'partitions': self.partitions,
             'description': self.description,
             'schema': self._schema,
         }
         r = ["<Collection>:\n-------------\n"]
         s = "<{}>: {}\n"
         for k, v in _dict.items():
             r.append(s.format(k, v))
@@ -165,34 +163,34 @@
         auto_id = kwargs.pop("auto_id", False)
         if auto_id:
             if dataframe[primary_field].isnull().all():
                 dataframe = dataframe.drop(primary_field, axis=1)
             else:
                 raise SchemaNotReadyException(message=ExceptionsMessage.AutoIDWithData)
 
-        using = kwargs.get("using", Config.MILVUS_CONN_ALIAS)
+        using = kwargs.get("using", DefaultConfig.DEFAULT_USING)
         conn = _get_connection(using)
         if conn.has_collection(name, **kwargs):
             resp = conn.describe_collection(name, **kwargs)
             server_schema = CollectionSchema.construct_from_dict(resp)
             schema = server_schema
         else:
-            fields_schema = construct_fields_from_dataframe(dataframe)
+            fields_schema = parse_fields_from_data(dataframe)
             if auto_id:
                 fields_schema.insert(pk_index,
                                      FieldSchema(name=primary_field, dtype=DataType.INT64, is_primary=True,
                                                  auto_id=True,
                                                  **kwargs))
 
             for field in fields_schema:
                 if auto_id is False and field.name == primary_field:
                     field.is_primary = True
                     field.auto_id = False
                 if field.dtype == DataType.VARCHAR:
-                    field.params[Config.MaxVarCharLengthKey] = int(Config.MaxVarCharLength)
+                    field.params[DefaultConfigs.MaxVarCharLengthKey] = int(DefaultConfigs.MaxVarCharLength)
             schema = CollectionSchema(fields=fields_schema)
 
         check_schema(schema)
         collection = cls(name, schema, **kwargs)
         res = collection.insert(data=dataframe)
         return collection, res
 
@@ -221,21 +219,14 @@
 
     @property
     def is_empty(self) -> bool:
         """bool: whether the collection is empty or not."""
         return self.num_entities == 0
 
     @property
-    def num_shards(self, **kwargs) -> int:
-        """int: number of shards used by the collection."""
-        if self._num_shards is None:
-            self._num_shards = self.describe().get("num_shards")
-        return self._num_shards
-
-    @property
     def num_entities(self, **kwargs) -> int:
         """int: The number of entities in the collection, not real time.
 
         Examples:
             >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
             >>> schema = CollectionSchema([
@@ -393,16 +384,15 @@
             >>> collection.create_index("films", {"index_type": "FLAT", "metric_type": "L2", "params": {}})
             >>> collection.load()
             >>> collection.release()
         """
         conn = self._get_connection()
         conn.release_collection(self._name, timeout=timeout, **kwargs)
 
-    def insert(self, data: Union[List, pandas.DataFrame, Dict], partition_name: str = None, timeout=None,
-               **kwargs) -> MutationResult:
+    def insert(self, data: Union[List, pandas.DataFrame], partition_name: str=None, timeout=None, **kwargs) -> MutationResult:
         """ Insert data into the collection.
 
         Args:
             data (``list/tuple/pandas.DataFrame``): The specified data to insert
             partition_name (``str``): The partition name which the data will be inserted to,
                 if partition name is not passed, then the data will be inserted to "_default" partition
             timeout (``float``, optional): A duration of time in seconds to allow for the RPC. Defaults to None.
@@ -429,27 +419,23 @@
             ... ]
             >>> res = collection.insert(data)
             >>> res.insert_count
             10
         """
         if data is None:
             return MutationResult(data)
+        check_insert_or_upsert_data_schema(self._schema, data)
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._schema)
 
-        row_based = check_insert_or_upsert_is_row_based(data)
         conn = self._get_connection()
-        if not row_based:
-            check_insert_data_schema(self._schema, data)
-            entities = Prepare.prepare_insert_data(data, self._schema)
-            res = conn.batch_insert(self._name, entities, partition_name,
-                                    timeout=timeout, schema=self._schema_dict, **kwargs)
-            if kwargs.get("_async", False):
-                return MutationFuture(res)
-        else:
-            res = conn.insert_rows(self._name, data, partition_name,
-                                   timeout=timeout, schema=self._schema_dict, **kwargs)
+        res = conn.batch_insert(self._name, entities, partition_name,
+                                timeout=timeout, schema=self._schema_dict, **kwargs)
+
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
         return MutationResult(res)
 
     def delete(self, expr, partition_name=None, timeout=None, **kwargs):
         """ Delete entities with an expression condition.
 
         Args:
             expr (``str``): The specified data to insert.
@@ -487,14 +473,60 @@
 
         conn = self._get_connection()
         res = conn.delete(self._name, expr, partition_name, timeout=timeout, **kwargs)
         if kwargs.get("_async", False):
             return MutationFuture(res)
         return MutationResult(res)
 
+    def upsert(self, data: Union[List, pandas.DataFrame], partition_name: str=None, timeout=None, **kwargs) -> MutationResult:
+        """ Upsert data into the collection.
+
+        Args:
+            data (``list/tuple/pandas.DataFrame``): The specified data to upsert
+            partition_name (``str``): The partition name which the data will be upserted at,
+                if partition name is not passed, then the data will be upserted in "_default" partition
+            timeout (``float``, optional): A duration of time in seconds to allow for the RPC. Defaults to None.
+                If timeout is set to None, the client keeps waiting until the server responds or an error occurs.
+        Returns:
+            MutationResult: contains 2 properties `upsert_count`, and, `primary_keys`
+                `upsert_count`: how may entites have been upserted at Milvus,
+                `primary_keys`: list of primary keys of the upserted entities
+        Raises:
+            MilvusException: If anything goes wrong.
+
+        Examples:
+            >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType
+            >>> import random
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_collection_upsert", schema)
+            >>> data = [
+            ...     [random.randint(1, 100) for _ in range(10)],
+            ...     [[random.random() for _ in range(2)] for _ in range(10)],
+            ... ]
+            >>> res = collection.upsert(data)
+            >>> res.upsert_count
+            10
+        """
+        if data is None:
+            return MutationResult(data)
+        check_insert_or_upsert_data_schema(self._schema, data, False)
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._schema, False)
+
+        conn = self._get_connection()
+        res = conn.upsert(self._name, entities, partition_name,
+                                timeout=timeout, schema=self._schema_dict, **kwargs)
+
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
+        return MutationResult(res)
+
     def search(self, data, anns_field, param, limit, expr=None, partition_names=None,
                output_fields=None, timeout=None, round_decimal=-1, **kwargs):
         """ Conducts a vector similarity search with an optional boolean expression as filter.
 
         Args:
             data (``List[List[float]]``): The vectors of search data.
                 the length of data is number of query (nq), and the dim of every vector in data must be equal to
@@ -915,15 +947,15 @@
             Status(code=0, message='')
             >>> collection.indexes
             [<pymilvus.index.Index object at 0x7f4435587e20>]
             >>> collection.index()
             <pymilvus.index.Index object at 0x7f44355a1460>
         """
         copy_kwargs = copy.deepcopy(kwargs)
-        index_name = copy_kwargs.pop("index_name", Config.IndexName)
+        index_name = copy_kwargs.pop("index_name", DefaultConfigs.IndexName)
         conn = self._get_connection()
         tmp_index = conn.describe_index(self._name, index_name, **copy_kwargs)
         if tmp_index is not None:
             field_name = tmp_index.pop("field_name", None)
             index_name = tmp_index.pop("index_name", index_name)
             return Index(self, field_name, tmp_index, construct_only=True, index_name=index_name)
         raise IndexNotExistException(message=ExceptionsMessage.IndexNotExist)
@@ -991,15 +1023,15 @@
             >>> index = {"index_type": "IVF_FLAT", "params": {"nlist": 128}, "metric_type": "L2"}
             >>> collection.create_index("films", index)
             >>> collection.has_index()
             True
         """
         conn = self._get_connection()
         copy_kwargs = copy.deepcopy(kwargs)
-        index_name = copy_kwargs.pop("index_name", Config.IndexName)
+        index_name = copy_kwargs.pop("index_name", DefaultConfigs.IndexName)
         if conn.describe_index(self._name, index_name, timeout=timeout, **copy_kwargs) is None:
             return False
         return True
 
     def drop_index(self, timeout=None, **kwargs):
         """ Drop index and its corresponding index files.
         Args:
@@ -1026,15 +1058,15 @@
             >>> collection.has_index()
             True
             >>> collection.drop_index()
             >>> collection.has_index()
             False
         """
         copy_kwargs = copy.deepcopy(kwargs)
-        index_name = copy_kwargs.pop("index_name", Config.IndexName)
+        index_name = copy_kwargs.pop("index_name", DefaultConfigs.IndexName)
         conn = self._get_connection()
         tmp_index = conn.describe_index(self._name, index_name, timeout=timeout, **copy_kwargs)
         if tmp_index is not None:
             index = Index(self, tmp_index['field_name'], tmp_index, construct_only=True, index_name=index_name)
             index.drop(timeout=timeout, **kwargs)
 
     def compact(self, timeout=None, **kwargs):
```

### Comparing `pymilvus-2.2.9/pymilvus/orm/connections.py` & `pymilvus-2.3.0b1/pymilvus/orm/connections.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
+import os
 import copy
+import re
 import threading
 from urllib import parse
 from typing import Tuple
 
 from ..client.check import is_legal_host, is_legal_port, is_legal_address
 from ..client.grpc_handler import GrpcHandler
-from ..client.utils import get_server_type, ZILLIZ
 
-from ..settings import Config
+from .default_config import DefaultConfig, ENV_CONNECTION_CONF
 from ..exceptions import ExceptionsMessage, ConnectionConfigException, ConnectionNotExistException
 
-VIRTUAL_PORT = 443
 
 def synchronized(func):
     """
     Decorator in order to achieve thread-safe singleton class.
     """
     func.__lock__ = threading.Lock()
 
@@ -57,80 +57,57 @@
 
 class Connections(metaclass=SingleInstanceMetaClass):
     """ Class for managing all connections of milvus.  Used as a singleton in this module.  """
 
     def __init__(self):
         """ Constructs a default milvus alias config
 
-            default config will be read from env: MILVUS_URI and MILVUS_CONN_ALIAS
-            with default value: default="localhost:19530"
+            default config will be read from env: MILVUS_DEFAULT_CONNECTION，
+            or "localhost:19530"
 
-         Read default connection config from environment variable: MILVUS_URI.
-            Format is:
-                [scheme://][<user>@<password>]host[:<port>]
+        """
+        self._alias = {}
+        self._connected_alias = {}
 
-                scheme is one of: http, https, or <empty>
+        self.add_connection(default=self._read_default_config_from_os_env())
 
-        Examples:
+    def _read_default_config_from_os_env(self):
+        """ Read default connection config from environment variable: MILVUS_DEFAULT_CONNECTION.
+        Format is:
+            [<user>@]host[:<port>]
+
+            protocol is one of: http, https, tcp, or <empty>
+        Examples::
             localhost
             localhost:19530
             test_user@localhost:19530
-            http://test_userlocalhost:19530
-            https://test_user:password@localhost:19530
-
         """
-        self._alias = {}
-        self._connected_alias = {}
-        self._env_uri = None
-
-        if Config.MILVUS_URI != "":
-            address, parsed_uri = self.__parse_address_from_uri(Config.MILVUS_URI)
-            self._env_uri = (address, parsed_uri)
-
-            default_conn_config = {
-                "user": parsed_uri.username if parsed_uri.username is not None else "",
-                "address": address,
-            }
-        else:
-            default_conn_config = {
-                "user": "",
-                "address": f"{Config.DEFAULT_HOST}:{Config.DEFAULT_PORT}",
-            }
 
-        self.add_connection(**{Config.MILVUS_CONN_ALIAS: default_conn_config})
+        # no need to adjust http://xxx, https://xxx, tcp://xxxx,
+        # because protocol is ignored
+        # @see __generate_address
 
-    def __verify_host_port(self, host, port):
-        if not is_legal_host(host):
-            raise ConnectionConfigException(message=ExceptionsMessage.HostType)
-        if not is_legal_port(port):
-            raise ConnectionConfigException(message=ExceptionsMessage.PortType)
-        if not 0 <= int(port) < 65535:
-            raise ConnectionConfigException(message=f"port number {port} out of range, valid range [0, 65535)")
+        conf = os.getenv(ENV_CONNECTION_CONF, "").strip()
+        if not conf:
+            conf = DefaultConfig.DEFAULT_HOST
 
-    def __parse_address_from_uri(self, uri: str) -> (str, parse.ParseResult):
-        illegal_uri_msg = "Illegal uri: [{}], expected form 'https://user:pwd@example.com:12345'"
-        try:
-            parsed_uri = parse.urlparse(uri)
-        except (Exception) as e:
-            raise ConnectionConfigException(
-                message=f"{illegal_uri_msg.format(uri)}: <{type(e).__name__}, {e}>") from None
-
-        if len(parsed_uri.netloc) == 0:
-            raise ConnectionConfigException(message=f"{illegal_uri_msg.format(uri)}") from None
-
-        host = parsed_uri.hostname if parsed_uri.hostname is not None else Config.DEFAULT_HOST
-        port = parsed_uri.port if parsed_uri.port is not None else Config.DEFAULT_PORT
-        addr = f"{host}:{port}"
+        rex = re.compile(r"^(?:([^\s/\\:]+)@)?([^\s/\\:]+)(?::(\d{1,5}))?$")
+        matched = rex.search(conf)
 
-        self.__verify_host_port(host, port)
+        if not matched:
+            raise ConnectionConfigException(message=ExceptionsMessage.EnvConfigErr % (ENV_CONNECTION_CONF, conf))
 
-        if not is_legal_address(addr):
-            raise ConnectionConfigException(message=illegal_uri_msg.format(uri))
+        user, host, port = matched.groups()
+        user = user or ""
+        port = port or DefaultConfig.DEFAULT_PORT
 
-        return addr, parsed_uri
+        return {
+            "user": user,
+            "address": f"{host}:{port}"
+        }
 
     def add_connection(self, **kwargs):
         """ Configures a milvus connection.
 
         Addresses priority in kwargs: address, uri, host and port
 
         :param kwargs:
@@ -155,15 +132,15 @@
                 dev3={"uri": "http://localhost:19530"},
                 dev4={"uri": "tcp://localhost:19530"},
                 dev5={"address": "localhost:19530"},
                 prod={"uri": "http://random.random.random.com:19530"},
             )
         """
         for alias, config in kwargs.items():
-            addr, _ = self.__get_full_address(
+            addr = self.__get_full_address(
                 config.get("address", ""),
                 config.get("uri", ""),
                 config.get("host", ""),
                 config.get("port", ""))
 
             if alias in self._connected_alias:
                 if self._alias[alias].get("address") != addr:
@@ -172,31 +149,50 @@
             alias_config = {
                 "address": addr,
                 "user": config.get("user", ""),
             }
 
             self._alias[alias] = alias_config
 
-    def __get_full_address(self, address: str = "", uri: str = "", host: str = "", port: str = "") -> (
-    str, parse.ParseResult):
+    def __get_full_address(self, address: str = "", uri: str = "", host: str = "", port: str = "") -> str:
         if address != "":
             if not is_legal_address(address):
-                raise ConnectionConfigException(
-                    message=f"Illegal address: {address}, should be in form 'localhost:19530'")
-            return address, None
+                raise ConnectionConfigException(message=f"Illegal address: {address}, should be in form 'localhost:19530'")
+        else:
+            address = self.__generate_address(uri, host, port)
+
+        return address
 
+    def __generate_address(self, uri: str, host: str, port: str) -> str:
+        illegal_uri_msg = "Illegal uri: [{}], should be in form 'http://example.com' or 'tcp://6.6.6.6:12345'"
         if uri != "":
-            address, parsed = self.__parse_address_from_uri(uri)
-            return address, parsed
+            try:
+                parsed_uri = parse.urlparse(uri)
+            except (Exception) as e:
+                raise ConnectionConfigException(message=f"{illegal_uri_msg.format(uri)}: <{type(e).__name__}, {e}>") from None
+
+            if len(parsed_uri.netloc) == 0:
+                raise ConnectionConfigException(message=illegal_uri_msg.format(uri))
+
+            addr = parsed_uri.netloc if ":" in parsed_uri.netloc else f"{parsed_uri.netloc}:{DefaultConfig.DEFAULT_PORT}"
+            if not is_legal_address(addr):
+                raise ConnectionConfigException(message=illegal_uri_msg.format(uri))
+            return addr
+
+        host = host if host != "" else DefaultConfig.DEFAULT_HOST
+        port = port if port != "" else DefaultConfig.DEFAULT_PORT
 
-        host = host if host != "" else Config.DEFAULT_HOST
-        port = port if port != "" else Config.DEFAULT_PORT
-        self.__verify_host_port(host, port)
+        if not is_legal_host(host):
+            raise ConnectionConfigException(message=ExceptionsMessage.HostType)
+        if not is_legal_port(port):
+            raise ConnectionConfigException(message=ExceptionsMessage.PortType)
+        if not 0 <= int(port) < 65535:
+            raise ConnectionConfigException(message=f"port number {port} out of range, valid range [0, 65535)")
 
-        return f"{host}:{port}", None
+        return f"{host}:{port}"
 
     def disconnect(self, alias: str):
         """ Disconnects connection from the registry.
 
         :param alias: The name of milvus connection
         :type alias: str
         """
@@ -214,16 +210,15 @@
         """
         if not isinstance(alias, str):
             raise ConnectionConfigException(message=ExceptionsMessage.AliasType % type(alias))
 
         self.disconnect(alias)
         self._alias.pop(alias, None)
 
-    # pylint: disable=too-many-statements
-    def connect(self, alias=Config.MILVUS_CONN_ALIAS, user="", password="", db_name="", token="", **kwargs):
+    def connect(self, alias=DefaultConfig.DEFAULT_USING, user="", password="", **kwargs):
         """
         Constructs a milvus connection and register it under given alias.
 
         :param alias: The name of milvus connection
         :type  alias: str
 
         :param kwargs:
@@ -235,27 +230,22 @@
 
             * *host* (``str``) -- Optional. The host of Milvus instance.
                 Default at "localhost", PyMilvus will fill in the default host if only port is provided.
 
             * *port* (``str/int``) -- Optional. The port of Milvus instance.
                 Default at 19530, PyMilvus will fill in the default port if only host is provided.
 
-            * *secure* (``bool``) --
-                Optional. Default is false. If set to true, tls will be enabled.
             * *user* (``str``) --
                 Optional. Use which user to connect to Milvus instance. If user and password
                 are provided, we will add related header in every RPC call.
             * *password* (``str``) --
                 Optional and required when user is provided. The password corresponding to
                 the user.
-            * *token* (``str``) --
-                Optional. Serving as the key for identification and authentication purposes.
-                Whenever a token is furnished, we shall supplement the corresponding header to each RPC call.
-            * *db_name* (``str``) --
-                Optional. default database name of this connection
+            * *secure* (``bool``) --
+                Optional. Default is false. If set to true, tls will be enabled.
             * *client_key_path* (``str``) --
                 Optional. If use tls two-way authentication, need to write the client.key path.
             * *client_pem_path* (``str``) --
                 Optional. If use tls two-way authentication, need to write the client.pem path.
             * *ca_pem_path* (``str``) --
                 Optional. If use tls two-way authentication, need to write the ca.pem path.
             * *server_pem_path* (``str``) --
@@ -268,115 +258,61 @@
         :raises Exception: If server specified in parameters is not ready, we cannot connect to
                            server.
 
         :example:
             >>> from pymilvus import connections
             >>> connections.connect("test", host="localhost", port="19530")
         """
+        if not isinstance(alias, str):
+            raise ConnectionConfigException(message=ExceptionsMessage.AliasType % type(alias))
 
         def connect_milvus(**kwargs):
             gh = GrpcHandler(**kwargs)
 
             t = kwargs.get("timeout")
-            timeout = t if isinstance(t, (int, float)) else Config.MILVUS_CONN_TIMEOUT
+            timeout = t if isinstance(t, (int, float)) else DefaultConfig.DEFAULT_CONNECT_TIMEOUT
 
             gh._wait_for_channel_ready(timeout=timeout)
             kwargs.pop('password')
-            kwargs.pop("token", None)
-            #  kwargs.pop('db_name', None)
             kwargs.pop('secure', None)
-            kwargs.pop("db_name", "")
 
             self._connected_alias[alias] = gh
             self._alias[alias] = copy.deepcopy(kwargs)
 
         def with_config(config: Tuple) -> bool:
             for c in config:
                 if c != "":
                     return True
 
             return False
 
-        if not isinstance(alias, str):
-            raise ConnectionConfigException(message=ExceptionsMessage.AliasType % type(alias))
-
-        # Set port if server type is zilliz cloud serverless
-        uri = kwargs.get("uri")
-        if uri is not None:
-            server_type = get_server_type(uri)
-            if server_type == ZILLIZ and ":" not in token:
-                kwargs["uri"] = uri+":"+str(VIRTUAL_PORT)
-
         config = (
             kwargs.pop("address", ""),
             kwargs.pop("uri", ""),
             kwargs.pop("host", ""),
             kwargs.pop("port", "")
         )
 
-        # Make sure passed in None doesnt break
-        user = user or ""
-        password = password or ""
-        token = token or ""
-        # Make sure passed in are Strings
-        user = str(user)
-        password = str(password)
-        token = str(token)
-
-        # 1st Priority: connection from params
         if with_config(config):
-            in_addr, parsed_uri = self.__get_full_address(*config)
+            in_addr = self.__get_full_address(*config)
             kwargs["address"] = in_addr
 
             if self.has_connection(alias):
                 if self._alias[alias].get("address") != in_addr:
                     raise ConnectionConfigException(message=ExceptionsMessage.ConnDiffConf % alias)
 
-            # uri might take extra info
-            if parsed_uri is not None:
-                user = parsed_uri.username if parsed_uri.username is not None else user
-                password = parsed_uri.password if parsed_uri.password is not None else password
-
-                group = parsed_uri.path.split("/")
-                db_name = "default"
-                if len(group) > 1:
-                    db_name = group[1]
-
-                # Set secure=True if https scheme
-                if parsed_uri.scheme == "https":
-                    kwargs["secure"] = True
-
+            connect_milvus(**kwargs, user=user, password=password)
 
-            connect_milvus(**kwargs, user=user, password=password, token=token, db_name=db_name)
-            return
-
-        # 2nd Priority, connection configs from env
-        if self._env_uri is not None:
-            addr, parsed_uri = self._env_uri
-            kwargs["address"] = addr
-
-            user = parsed_uri.username if parsed_uri.username is not None else ""
-            password = parsed_uri.password if parsed_uri.password is not None else ""
-
-            # Set secure=True if https scheme
-            if parsed_uri.scheme == "https":
-                kwargs["secure"] = True
-
-            connect_milvus(**kwargs, user=user, password=password, db_name=db_name)
-            return
+        else:
+            if alias not in self._alias:
+                raise ConnectionConfigException(message=ExceptionsMessage.ConnLackConf % alias)
 
-        # 3rd Priority, connect to cached configs with provided user and password
-        if alias in self._alias:
             connect_alias = dict(self._alias[alias].items())
             connect_alias["user"] = user
-            connect_milvus(**connect_alias, password=password, db_name=db_name, **kwargs)
-            return
-
-        # No params, env, and cached configs for the alias
-        raise ConnectionConfigException(message=ExceptionsMessage.ConnLackConf % alias)
+            connect_milvus(**connect_alias, password=password, **kwargs)
 
     def list_connections(self) -> list:
         """ List names of all connections.
 
         :return list:
             Names of all connections.
 
@@ -429,15 +365,15 @@
             >>> connections.get_connection_addr('test')
             {'host': 'localhost', 'port': '19530'}
         """
         if not isinstance(alias, str):
             raise ConnectionConfigException(message=ExceptionsMessage.AliasType % type(alias))
         return alias in self._connected_alias
 
-    def _fetch_handler(self, alias=Config.MILVUS_CONN_ALIAS) -> GrpcHandler:
+    def _fetch_handler(self, alias=DefaultConfig.DEFAULT_USING) -> GrpcHandler:
         """ Retrieves a GrpcHandler by alias. """
         if not isinstance(alias, str):
             raise ConnectionConfigException(message=ExceptionsMessage.AliasType % type(alias))
 
         conn = self._connected_alias.get(alias, None)
         if conn is None:
             raise ConnectionNotExistException(message=ExceptionsMessage.ConnectFirst)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymilvus-2.2.9/pymilvus/orm/constants.py` & `pymilvus-2.3.0b1/pymilvus/orm/constants.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/pymilvus/orm/future.py` & `pymilvus-2.3.0b1/pymilvus/orm/future.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/pymilvus/orm/index.py` & `pymilvus-2.3.0b1/pymilvus/orm/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import copy
 
 from ..exceptions import CollectionNotExistException, ExceptionsMessage
-from ..settings import Config
+from ..client.configs import DefaultConfigs
 
 
 class Index:
     def __init__(self, collection, field_name, index_params, **kwargs):
         """
         Creates index on a specified field according to the index parameters.
 
@@ -60,15 +60,15 @@
         """
         from .collection import Collection
         if not isinstance(collection, Collection):
             raise CollectionNotExistException(message=ExceptionsMessage.CollectionType)
         self._collection = collection
         self._field_name = field_name
         self._index_params = index_params
-        index_name = kwargs.get("index_name", Config.IndexName)
+        index_name = kwargs.get("index_name", DefaultConfigs.IndexName)
         self._index_name = index_name
         self._kwargs = kwargs
         if self._kwargs.pop("construct_only", False):
             return
 
         conn = self._get_connection()
         conn.create_index(self._collection.name, self._field_name, self._index_params, **kwargs)
@@ -151,10 +151,10 @@
 
         :param kwargs:
             * *index_name* (``str``) --
               The name of index. If no index is specified, the default index name is used.
 
         """
         copy_kwargs = copy.deepcopy(kwargs)
-        index_name = copy_kwargs.pop("index_name", Config.IndexName)
+        index_name = copy_kwargs.pop("index_name", DefaultConfigs.IndexName)
         conn = self._get_connection()
         conn.drop_index(self._collection.name, self.field_name, index_name, timeout=timeout, **copy_kwargs)
```

### Comparing `pymilvus-2.2.9/pymilvus/orm/mutation.py` & `pymilvus-2.3.0b1/pymilvus/orm/mutation.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/pymilvus/orm/prepare.py` & `pymilvus-2.3.0b1/pymilvus/orm/prepare.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,29 +10,36 @@
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 import copy
 
 import numpy
 import pandas
 
-from ..exceptions import DataNotMatchException, DataTypeNotSupportException, ExceptionsMessage
+from ..exceptions import (
+    DataNotMatchException,
+    DataTypeNotSupportException,
+    ExceptionsMessage,
+    UpsertAutoIDTrueException,
+)
 
 
 class Prepare:
     @classmethod
-    def prepare_insert_data(cls, data, schema):
+    def prepare_insert_or_upsert_data(cls, data, schema, isInsert = True):
         if not isinstance(data, (list, tuple, pandas.DataFrame)):
             raise DataTypeNotSupportException(message=ExceptionsMessage.DataTypeNotSupport)
 
         fields = schema.fields
         entities = []  # Entities
         raw_lengths = []  # Check if each row has the same numbers.
 
         if isinstance(data, pandas.DataFrame):
             if schema.auto_id:
+                if isInsert is False:
+                    raise UpsertAutoIDTrueException(message=ExceptionsMessage.UpsertAutoIDTrue)
                 if schema.primary_field.name in data:
                     if len(fields) != len(data.columns):
                         raise DataNotMatchException(message=ExceptionsMessage.FieldsNumInconsistent)
                     if not data[schema.primary_field.name].isnull().all():
                         raise DataNotMatchException(message=ExceptionsMessage.AutoIDWithData)
                 else:
                     if len(fields) != len(data.columns) + 1:
```

### Comparing `pymilvus-2.2.9/pymilvus/orm/role.py` & `pymilvus-2.3.0b1/pymilvus/orm/role.py`

 * *Files 16% similar despite different names*

```diff
@@ -127,88 +127,80 @@
             >>> role = Role(name=role_name)
             >>> is_exist = role.is_exist()
             >>> print(f"the role: {is_exist}")
         """
         roles = self._get_connection().select_one_role(self._name, False)
         return len(roles.groups) != 0
 
-    def grant(self, object: str, object_name: str, privilege: str, db_name: str = "default"):
+    def grant(self, object: str, object_name: str, privilege: str):
         """ Grant a privilege for the role
             :param object: object type.
             :type  object: str
             :param object_name: identifies a specific object name.
             :type  object_name: str
             :param privilege: privilege name.
             :type  privilege: str
-            :param db_name: db name.
-            :type  db_name: str
 
         :example:
             >>> from pymilvus import connections
             >>> from pymilvus.orm.role import Role
             >>> connections.connect()
             >>> role = Role(role_name)
             >>> role.grant("Collection", collection_name, "Insert")
         """
-        return self._get_connection().grant_privilege(self._name, object, object_name, privilege, db_name)
+        return self._get_connection().grant_privilege(self._name, object, object_name, privilege)
 
-    def revoke(self, object: str, object_name: str, privilege: str, db_name: str = "default"):
+    def revoke(self, object: str, object_name: str, privilege: str):
         """ Revoke a privilege for the role
             :param object: object type.
             :type  object: str
             :param object_name: identifies a specific object name.
             :type  object_name: str
             :param privilege: privilege name.
             :type  privilege: str
-            :param db_name: db name.
-            :type  db_name: str
 
         :example:
             >>> from pymilvus import connections
             >>> from pymilvus.orm.role import Role
             >>> connections.connect()
             >>> role = Role(role_name)
             >>> role.revoke("Collection", collection_name, "Insert")
         """
-        return self._get_connection().revoke_privilege(self._name, object, object_name, privilege, db_name)
+        return self._get_connection().revoke_privilege(self._name, object, object_name, privilege)
 
-    def list_grant(self, object: str, object_name: str, db_name: str = "default"):
+    def list_grant(self, object: str, object_name: str):
         """ List a grant info for the role and the specific object
             :param object: object type.
             :type  object: str
             :param object_name: identifies a specific object name.
             :type  object_name: str
-            :param db_name: db name.
-            :type  db_name: str
             :return a GrantInfo object
             :rtype GrantInfo
 
             GrantInfo groups:
             - GrantItem: <object:Collection>, <object_name:foo>, <role_name:x>, <grantor_name:root>, <privilege:Load>
 
         :example:
             >>> from pymilvus import connections
             >>> from pymilvus.orm.role import Role
             >>> connections.connect()
             >>> role = Role(role_name)
             >>> role.list_grant("Collection", collection_name)
         """
-        return self._get_connection().select_grant_for_role_and_object(self._name, object, object_name, db_name)
+        return self._get_connection().select_grant_for_role_and_object(self._name, object, object_name)
 
-    def list_grants(self, db_name: str = "default"):
+    def list_grants(self):
         """ List a grant info for the role
-            :param db_name: db name.
-            :type  db_name: str
             :return a GrantInfo object
             :rtype GrantInfo
 
             GrantInfo groups:
             - GrantItem: <object:Collection>, <object_name:foo>, <role_name:x>, <grantor_name:root>, <privilege:Load>
 
         :example:
             >>> from pymilvus import connections
             >>> from pymilvus.orm.role import Role
             >>> connections.connect()
             >>> role = Role(role_name)
             >>> role.list_grants()
         """
-        return self._get_connection().select_grant_for_one_role(self._name, db_name)
+        return self._get_connection().select_grant_for_one_role(self._name)
```

### Comparing `pymilvus-2.2.9/pymilvus/orm/schema.py` & `pymilvus-2.3.0b1/pymilvus/orm/schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,132 +7,109 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import copy
-from typing import List, Union, Dict
+from typing import List, Union
 import pandas
 from pandas.api.types import is_list_like
 
 from .constants import COMMON_TYPE_PARAMS
 from .types import DataType, map_numpy_dtype_to_datatype, infer_dtype_bydata
 from ..exceptions import (
     CannotInferSchemaException,
     DataTypeNotSupportException,
     PrimaryKeyException,
-    PartitionKeyException,
     FieldsTypeException,
     FieldTypeException,
     AutoIDException,
     ExceptionsMessage,
     DataNotMatchException,
     SchemaNotReadyException,
+    UpsertAutoIDTrueException
 )
 
 
-def validate_primary_key(primary_field):
-    if primary_field is None:
-        raise PrimaryKeyException(message=ExceptionsMessage.PrimaryKeyNotExist)
-
-    if primary_field.dtype not in [DataType.INT64, DataType.VARCHAR]:
-        raise PrimaryKeyException(message=ExceptionsMessage.PrimaryKeyType)
-
-
-def validate_partition_key(partition_key_field_name, partition_key_field, primary_field_name):
-    # not allow partition_key field is primary key field
-    if partition_key_field is not None:
-        if partition_key_field.name == primary_field_name:
-            PartitionKeyException(
-                message=ExceptionsMessage.PartitionKeyNotPrimary)
-
-        if partition_key_field.dtype not in [DataType.INT64, DataType.VARCHAR]:
-            raise PartitionKeyException(
-                message=ExceptionsMessage.PartitionKeyType)
-    else:
-        if partition_key_field_name is not None:
-            raise PartitionKeyException(
-                message=ExceptionsMessage.PartitionKeyFieldNotExist % partition_key_field_name)
-
-
 class CollectionSchema:
     def __init__(self, fields, description="", **kwargs):
         if not isinstance(fields, list):
             raise FieldsTypeException(message=ExceptionsMessage.FieldsType)
         self._fields = [copy.deepcopy(field) for field in fields]
-        primary_field_name = kwargs.get("primary_field", None)
-        if primary_field_name is not None and not isinstance(primary_field_name, str):
-            raise PrimaryKeyException(
-                message=ExceptionsMessage.PrimaryFieldType)
-        partition_key_field_name = kwargs.get("partition_key_field", None)
-        if partition_key_field_name is not None and not isinstance(partition_key_field_name, str):
-            raise PartitionKeyException(
-                message=ExceptionsMessage.PartitionKeyFieldType)
+        primary_field = kwargs.get("primary_field", None)
         for field in self._fields:
             if not isinstance(field, FieldSchema):
                 raise FieldTypeException(message=ExceptionsMessage.FieldType)
-            if primary_field_name == field.name:
+            if primary_field == field.name:
                 field.is_primary = True
-            if partition_key_field_name == field.name:
-                field.is_partition_key = True
         self._primary_field = None
-        self._partition_key_field = None
-        self._enable_dynamic_field = kwargs.get("enable_dynamic_field", False)
         for field in self._fields:
             if field.is_primary:
-                if primary_field_name is not None and primary_field_name != field.name:
-                    raise PrimaryKeyException(
-                        message=ExceptionsMessage.PrimaryKeyOnlyOne % (primary_field_name, field.name))
+                if primary_field is not None and primary_field != field.name:
+                    raise PrimaryKeyException(message=ExceptionsMessage.PrimaryKeyOnlyOne)
                 self._primary_field = field
-                primary_field_name = field.name
-            if field.is_partition_key:
-                if partition_key_field_name is not None and partition_key_field_name != field.name:
-                    raise PartitionKeyException(
-                        message=ExceptionsMessage.PartitionKeyOnlyOne % (partition_key_field_name, field.name))
-                self._partition_key_field = field
-                partition_key_field_name = field.name
-
-        validate_primary_key(self._primary_field)
-        validate_partition_key(partition_key_field_name,
-                               self._partition_key_field, self._primary_field)
-
-        auto_id = kwargs.get("auto_id", False)
-        if auto_id:
-            self._primary_field.auto_id = auto_id
+                primary_field = field.name
+
+        if self._primary_field is None:
+            raise PrimaryKeyException(message=ExceptionsMessage.PrimaryKeyNotExist)
+
+        if self._primary_field.dtype not in [DataType.INT64, DataType.VARCHAR]:
+            raise PrimaryKeyException(message=ExceptionsMessage.PrimaryKeyType)
+
+        self._auto_id = kwargs.get("auto_id", None)
+        if "auto_id" in kwargs:
+            if not isinstance(self._auto_id, bool):
+                raise AutoIDException(message=ExceptionsMessage.AutoIDType)
+            if self._primary_field.auto_id is not None and self._primary_field.auto_id != self._auto_id:
+                raise AutoIDException(message=ExceptionsMessage.AutoIDInconsistent)
+            self._primary_field.auto_id = self._auto_id
+            if self._primary_field.auto_id and self._primary_field.dtype == DataType.VARCHAR:
+                raise AutoIDException(message=ExceptionsMessage.AutoIDFieldType)
+        else:
+            if self._primary_field.auto_id is None:
+                self._primary_field.auto_id = False
+            self._auto_id = self._primary_field.auto_id
 
         self._description = description
         self._kwargs = copy.deepcopy(kwargs)
 
     def __repr__(self):
-        return str(self.to_dict())
+        _dict = {
+            "auto_id": self.auto_id,
+            "description": self._description,
+            "fields": self._fields,
+        }
+        r = ["{\n"]
+        s = "  {}: {}\n"
+        for k, v in _dict.items():
+            r.append(s.format(k, v))
+        r.append("}")
+        return "".join(r)
 
     def __len__(self):
         return len(self.fields)
 
     def __eq__(self, other):
-        """ The order of the fields of schema must be consistent."""
+        """
+        The order of the fields of schema must be consistent.
+        """
         return self.to_dict() == other.to_dict()
 
     @classmethod
     def construct_from_dict(cls, raw):
-        fields = [FieldSchema.construct_from_dict(
-            field_raw) for field_raw in raw['fields']]
-        enable_dynamic_field = raw.get("enable_dynamic_field", False)
-        return CollectionSchema(fields, raw.get('description', ""), enable_dynamic_field=enable_dynamic_field)
+        fields = [FieldSchema.construct_from_dict(field_raw) for field_raw in raw['fields']]
+        return CollectionSchema(fields, raw.get('description', ""))
 
     @property
+    # TODO:
     def primary_field(self):
         return self._primary_field
 
     @property
-    def partition_key_field(self):
-        return self._partition_key_field
-
-    @property
     def fields(self):
         """
         Returns the fields about the CollectionSchema.
 
         :return list:
             List of FieldSchema, return when operation is successful.
 
@@ -174,67 +151,57 @@
         :example:
             >>> from pymilvus import FieldSchema, CollectionSchema, DataType
             >>> field = FieldSchema("int64", DataType.INT64, description="int64", is_primary=True)
             >>> schema = CollectionSchema(fields=[field])
             >>> schema.auto_id
             False
         """
-        return self.primary_field.auto_id
-
-    @property
-    def enable_dynamic_field(self):
-        return self._enable_dynamic_field
+        return self._auto_id
 
     def to_dict(self):
         _dict = {
             "auto_id": self.auto_id,
             "description": self._description,
             "fields": [s.to_dict() for s in self._fields],
         }
-        if self._enable_dynamic_field:
-            _dict["enable_dynamic_field"] = self._enable_dynamic_field
         return _dict
 
 
 class FieldSchema:
-    def __init__(self, name: str, dtype: DataType, description="", **kwargs):
+    def __init__(self, name, dtype, description="", **kwargs):
         self.name = name
         try:
-            dtype = DataType(dtype)
+            DataType(dtype)
         except ValueError:
-            raise DataTypeNotSupportException(
-                message=ExceptionsMessage.FieldDtype) from None
+            raise DataTypeNotSupportException(message=ExceptionsMessage.FieldDtype) from None
         if dtype == DataType.UNKNOWN:
-            raise DataTypeNotSupportException(
-                message=ExceptionsMessage.FieldDtype)
+            raise DataTypeNotSupportException(message=ExceptionsMessage.FieldDtype)
         self._dtype = dtype
         self._description = description
         self._type_params = {}
         self._kwargs = copy.deepcopy(kwargs)
         if not isinstance(kwargs.get("is_primary", False), bool):
             raise PrimaryKeyException(message=ExceptionsMessage.IsPrimaryType)
         self.is_primary = kwargs.get("is_primary", False)
-        self.is_dynamic = kwargs.get("is_dynamic", False)
-        self.auto_id = kwargs.get("auto_id", False)
+        self.auto_id = kwargs.get("auto_id", None)
         if "auto_id" in kwargs:
             if not isinstance(self.auto_id, bool):
                 raise AutoIDException(message=ExceptionsMessage.AutoIDType)
             if not self.is_primary and self.auto_id:
-                raise PrimaryKeyException(
-                    message=ExceptionsMessage.AutoIDOnlyOnPK)
-
-        if not isinstance(kwargs.get("is_partition_key", False), bool):
-            raise PartitionKeyException(
-                message=ExceptionsMessage.IsPartitionKeyType)
-        self.is_partition_key = kwargs.get("is_partition_key", False)
+                raise PrimaryKeyException(message=ExceptionsMessage.AutoIDOnlyOnPK)
 
         self._parse_type_params()
 
     def __repr__(self):
-        return str(self.to_dict())
+        r = ["{\n"]
+        s = "    {}: {}\n"
+        for k, v in self.to_dict().items():
+            r.append(s.format(k, v))
+        r.append("  }")
+        return "".join(r)
 
     def __deepcopy__(self, memodict=None):
         if memodict is None:
             memodict = {}
         return self.construct_from_dict(self.to_dict())
 
     def _parse_type_params(self):
@@ -254,33 +221,27 @@
     @classmethod
     def construct_from_dict(cls, raw):
         kwargs = {}
         kwargs.update(raw.get("params", {}))
         kwargs['is_primary'] = raw.get("is_primary", False)
         if raw.get("auto_id", None) is not None:
             kwargs['auto_id'] = raw.get("auto_id", None)
-        kwargs['is_partition_key'] = raw.get("is_partition_key", False)
-        kwargs['is_dynamic'] = raw.get("is_dynamic", False)
         return FieldSchema(raw['name'], raw['type'], raw.get("description", ""), **kwargs)
 
     def to_dict(self):
         _dict = {
             "name": self.name,
             "description": self._description,
             "type": self.dtype,
         }
         if self._type_params:
             _dict["params"] = copy.deepcopy(self.params)
         if self.is_primary:
             _dict["is_primary"] = True
             _dict["auto_id"] = self.auto_id
-        if self.is_partition_key:
-            _dict["is_partition_key"] = True
-        if self.is_dynamic:
-            _dict["is_dynamic"] = self.is_dynamic
         return _dict
 
     def __getattr__(self, item):
         if self._type_params and item in self._type_params:
             return self._type_params[item]
         return None
 
@@ -321,138 +282,109 @@
         >>> fvec_field = FieldSchema("fvec", DataType.FLOAT_VECTOR, is_primary=False, dim=128)
         >>> fvec_field.params
         {'dim': 128}
         """
         return self._type_params
 
     @property
-    def dtype(self) -> DataType:
+    def dtype(self):
         return self._dtype
 
 
-def check_insert_or_upsert_is_row_based(data: Union[List[List], List[Dict], Dict, pandas.DataFrame]) -> bool:
-    if not isinstance(data, (pandas.DataFrame, list, dict)):
-        raise DataTypeNotSupportException(message="The type of data should be list or pandas.DataFrame or dict")
-
-    if isinstance(data, pandas.DataFrame):
-        return False
-
-    if isinstance(data, dict):
-        return True
-
-    if isinstance(data, list):
-        if len(data) == 0:
-            return False
-        if isinstance(data[0], Dict):
-            return True
-
-    return False
-
-
-def check_insert_data_schema(schema: CollectionSchema, data: [List[List], pandas.DataFrame]) -> None:
-    """ check if the insert data is consist with the collection schema
+def check_insert_or_upsert_data_schema(schema: CollectionSchema, data: Union[List[List], pandas.DataFrame], isInsert=True) -> None:
+    """ check if the insert or upsert data is consist with the collection schema
 
     Args:
         schema (CollectionSchema): the schema of the collection
-        data (List[List], pandas.DataFrame): the data to be inserted
+        data (List[List], pandas.DataFrame): the data to be inserted or upserted
 
     Raise:
         SchemaNotReadyException: if the schema is None
+        UpsertAutoIDTrueException: if autoid option is true
         DataNotMatchException: if the data is in consist with the schema
     """
     if schema is None:
         raise SchemaNotReadyException(message="Schema shouldn't be None")
     if schema.auto_id:
-        if isinstance(data, pandas.DataFrame):
-            if schema.primary_field.name in data:
-                if not data[schema.primary_field.name].isnull().all():
-                    raise DataNotMatchException(
-                        message=f"Please don't provide data for auto_id primary field: {schema.primary_field.name}")
-                data = data.drop(schema.primary_field.name, axis=1)
-
+        if isInsert:
+            if isinstance(data, pandas.DataFrame):
+                if schema.primary_field.name in data:
+                    if not data[schema.primary_field.name].isnull().all():
+                        raise DataNotMatchException(message=f"Please don't provide data for auto_id primary field: {schema.primary_field.name}")
+                    data = data.drop(schema.primary_field.name, axis=1)
+        else:
+            raise UpsertAutoIDTrueException(message=ExceptionsMessage.UpsertAutoIDTrue)
     infer_fields = parse_fields_from_data(data)
     tmp_fields = copy.deepcopy(schema.fields)
 
     for i, field in enumerate(schema.fields):
         if field.is_primary and field.auto_id:
             tmp_fields.pop(i)
 
-    check_infer_fields_valid(infer_fields, tmp_fields, isinstance(data, pandas.DataFrame))
+    if len(infer_fields) != len(tmp_fields):
+
+        i_name = [f.name for f in infer_fields]
+        t_name = [f.name for f in tmp_fields]
+        raise DataNotMatchException(message=f"The fields don't match with schema fields, expected: {t_name}, got {i_name}")
+
+    for x, y in zip(infer_fields, tmp_fields):
+        if x.dtype != y.dtype:
+            raise DataNotMatchException(message=f"The data type of field {y.name} doesn't match, expected: {y.dtype.name}, got {x.dtype.name}")
+        if isinstance(data, pandas.DataFrame) and x.name != y.name:
+            raise DataNotMatchException(message=f"The name of field don't match, expected: {y.name}, got {x.name}")
+
 
-def parse_fields_from_data(data: [List[List], pandas.DataFrame]) -> List[FieldSchema]:
+def parse_fields_from_data(data: Union[List[List], pandas.DataFrame]) -> List[FieldSchema]:
     if not isinstance(data, (pandas.DataFrame, list)):
         raise DataTypeNotSupportException(message="The type of data should be list or pandas.DataFrame")
 
     if isinstance(data, pandas.DataFrame):
-        return construct_fields_from_dataframe(data)
+        return parse_fields_from_dataframe(data)
 
     for d in data:
         if not is_list_like(d):
             raise DataTypeNotSupportException(message="data should be a list of list")
 
     fields = [FieldSchema("", infer_dtype_bydata(d[0])) for d in data]
     return fields
 
-def construct_fields_from_dataframe(df: pandas.DataFrame) -> List[FieldSchema]:
-    col_names, data_types, column_params_map = prepare_fields_from_dataframe(
-        df)
-    fields = []
-    for name, dtype in zip(col_names, data_types):
-        type_params = column_params_map.get(name, {})
-        field_schema = FieldSchema(name, dtype, **type_params)
-        fields.append(field_schema)
-
-    return fields
-
 
-def prepare_fields_from_dataframe(df: pandas.DataFrame):
+def parse_fields_from_dataframe(df: pandas.DataFrame) -> List[FieldSchema]:
     d_types = list(df.dtypes)
     data_types = list(map(map_numpy_dtype_to_datatype, d_types))
     col_names = list(df.columns)
 
     column_params_map = {}
 
     if DataType.UNKNOWN in data_types:
         if len(df) == 0:
-            raise CannotInferSchemaException(
-                message=ExceptionsMessage.DataFrameInvalid)
+            raise CannotInferSchemaException(message=ExceptionsMessage.DataFrameInvalid)
         values = df.head(1).values[0]
         for i, dtype in enumerate(data_types):
             if dtype == DataType.UNKNOWN:
                 new_dtype = infer_dtype_bydata(values[i])
                 if new_dtype in (DataType.BINARY_VECTOR, DataType.FLOAT_VECTOR):
                     vector_type_params = {}
                     if new_dtype == DataType.BINARY_VECTOR:
                         vector_type_params['dim'] = len(values[i]) * 8
                     else:
                         vector_type_params['dim'] = len(values[i])
                     column_params_map[col_names[i]] = vector_type_params
                 data_types[i] = new_dtype
 
     if DataType.UNKNOWN in data_types:
-        raise CannotInferSchemaException(
-            message=ExceptionsMessage.DataFrameInvalid)
-
-    return col_names, data_types, column_params_map
+        raise CannotInferSchemaException(message=ExceptionsMessage.DataFrameInvalid)
 
+    fields = []
+    for name, dtype in zip(col_names, data_types):
+        type_params = column_params_map.get(name, {})
+        field_schema = FieldSchema(name, dtype, **type_params)
+        fields.append(field_schema)
 
-def check_infer_fields_valid(infer_fields: List[FieldSchema], tmp_fields: list, is_data_frame: bool):
-    if len(infer_fields) != len(tmp_fields):
-        i_name = [f.name for f in infer_fields]
-        t_name = [f.name for f in tmp_fields]
-        raise DataNotMatchException(
-            message=f"The fields don't match with schema fields, expected: {t_name}, got {i_name}")
-
-    for x, y in zip(infer_fields, tmp_fields):
-        if x.dtype != y.dtype:
-            raise DataNotMatchException(
-                message=f"The data type of field {y.name} doesn't match, expected: {y.dtype.name}, got {x.dtype.name}")
-        if is_data_frame and x.name != y.name:
-            raise DataNotMatchException(
-                message=f"The name of field don't match, expected: {y.name}, got {x.name}")
+    return fields
 
 
 def check_schema(schema):
     if schema is None:
         raise SchemaNotReadyException(message=ExceptionsMessage.NoSchema)
     if len(schema.fields) < 1:
         raise SchemaNotReadyException(message=ExceptionsMessage.EmptySchema)
```

### Comparing `pymilvus-2.2.9/pymilvus/orm/search.py` & `pymilvus-2.3.0b1/pymilvus/orm/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     def __str__(self):
         """
         Return the information of hit record.
 
         :return str:
             The information of hit record.
         """
-        return str(self._hit)
+        return f"(distance: {self._hit.distance}, id: {self._hit.id})"
 
     __repr__ = __str__
 
 
 class Hits:
     def __init__(self, hits):
         """
```

### Comparing `pymilvus-2.2.9/pymilvus/orm/types.py` & `pymilvus-2.3.0b1/pymilvus/orm/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,14 @@
 
 def infer_dtype_bydata(data):
     d_type = DataType.UNKNOWN
     if is_scalar(data):
         d_type = infer_dtype_by_scaladata(data)
         return d_type
 
-    if isinstance(data, dict):
-        return DataType.JSON
-
     if is_list_like(data) or is_array_like(data):
         failed = False
         try:
             type_str = infer_dtype(data)
         except TypeError:
             failed = True
         if not failed:
```

### Comparing `pymilvus-2.2.9/pymilvus/orm/utility.py` & `pymilvus-2.3.0b1/pymilvus/orm/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,15 +472,14 @@
         >>> True
         >>> utility.drop_collection("new_collection")
         >>> utility.has_collection("new_collection")
         >>> False
     """
     return _get_connection(using).rename_collections(old_collection_name, new_collection_name, timeout=timeout)
 
-
 def list_collections(timeout=None, using="default") -> list:
     """
     Returns a list of all collection names.
 
     :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
                     is set to None, client waits until server response or error occur.
     :type  timeout: float
@@ -1033,85 +1032,7 @@
 
     :example:
         >>> from pymilvus import connections, utility
         >>> connections.connect()
         >>> rgs = utility.transfer_replica(source, target, collection_name, num_replica)
     """
     return _get_connection(using).transfer_replica(source_group, target_group, collection_name, num_replicas, timeout)
-
-
-def flush_all(using="default", timeout=None, **kwargs):
-    """ Flush all collections. All insertions, deletions, and upserts before `flush_all` will be synced.
-
-    Args:
-        timeout (float): an optional duration of time in seconds to allow for the RPCs.
-            If timeout is not set, the client keeps waiting until the server responds or an error occurs.
-            **kwargs (``dict``, optional):
-
-        * *_async*(``bool``)
-            Indicate if invoke asynchronously. Default `False`.
-
-    Examples:
-        >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType, utility
-        >>> connections.connect()
-        >>> fields = [
-        ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
-        ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=128)
-        ... ]
-        >>> schema = CollectionSchema(fields=fields)
-        >>> collection = Collection(name="test_collection_flush", schema=schema)
-        >>> collection.insert([[1, 2], [[1.0, 2.0], [3.0, 4.0]]])
-        >>> utility.flush_all(_async=False) # synchronized flush_all
-        >>> # or use `future` to flush_all asynchronously
-        >>> future = utility.flush_all(_async=True)
-        >>> future.done() # flush_all finished
-    """
-    return _get_connection(using).flush_all(timeout=timeout, **kwargs)
-
-
-def get_server_type(using="default"):
-    """ Get the server type. Now, it will return "zilliz" if the connection related to an instance on the zilliz cloud,
-        otherwise "milvus" will be returned.
-
-    :param using: Alias to the connection. Default connection is used if this is not specified.
-    :type  using: str
-
-    :return: The server type.
-    :rtype: str
-    """
-    return _get_connection(using).get_server_type()
-
-
-def list_indexes(collection_name, using="default", timeout=None, **kwargs):
-    """ List all indexes of collection. If `field_name` is not specified, return all the indexes of this collection,
-        otherwise this interface will return all indexes on this field of the collection.
-
-    :param collection_name: The name of collection.
-    :type  collection_name: str
-
-    :param using: Alias to the connection. Default connection is used if this is not specified.
-    :type  using: str
-
-    :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
-                    is set to None, client waits until server response or error occur
-    :type  timeout: float/int
-
-    :param kwargs:
-            * *field_name* (``str``)
-                The name of field. If no field name is specified, all indexes of this collection will be returned.
-    :type  kwargs: dict
-
-    :return: The name list of all indexes.
-    :rtype: str list
-    """
-    indexes = _get_connection(using).list_indexes(collection_name, timeout, **kwargs)
-    field_name = kwargs.get("field_name", None)
-    index_name_list = []
-    for index in indexes:
-        if index is not None:
-            if field_name is None:
-                # list all indexes anyway.
-                index_name_list.append(index.index_name)
-            if field_name is not None and index.field_name == field_name:
-                # list all indexes of this field.
-                index_name_list.append(index.index_name)
-    return index_name_list
```

### Comparing `pymilvus-2.2.9/pymilvus.egg-info/PKG-INFO` & `pymilvus-2.3.0b1/pymilvus.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.2.9
+Version: 2.3.0b1
 Summary: Python Sdk for Milvus
 Home-page: https://github.com/milvus-io/pymilvus
 Author: Milvus Team
 Author-email: milvus-team@zilliz.com
 License: Apache-2.0
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
```

### Comparing `pymilvus-2.2.9/pymilvus.egg-info/SOURCES.txt` & `pymilvus-2.3.0b1/pymilvus.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-.env.example
 .gitignore
 .gitmodules
 CONTRIBUTING.md
 CONTRIBUTING_CN.md
 Dockerfile
 LICENSE
 Makefile
 OWNERS
 README.md
 check_proto_product.sh
 pylint.conf
 pyproject.toml
 requirements.txt
 setup.py
-test_requirements.txt
 .github/mergify.yml
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.yaml
 .github/ISSUE_TEMPLATE/general-question.yaml
 .github/workflows/check_milvus_proto.yml
 .github/workflows/code_checker.yml
@@ -50,18 +48,15 @@
 docs/source/api/milvus_index.rst
 docs/source/api/partition.rst
 docs/source/api/schema.rst
 docs/source/api/search.rst
 docs/source/api/utility.rst
 docs/source/res/Intro_to_Indexes.md
 docs/source/res/about_documentation.md
-examples/binary_example.py
 examples/collection.py
-examples/database.py
-examples/dynamic_field.py
 examples/example.py
 examples/example_bulkinsert.py
 examples/example_index.py
 examples/example_str.py
 examples/example_tls1.py
 examples/example_tls2.py
 examples/films.csv
@@ -90,41 +85,36 @@
 pymilvus.egg-info/requires.txt
 pymilvus.egg-info/top_level.txt
 pymilvus/client/__init__.py
 pymilvus/client/abstract.py
 pymilvus/client/asynch.py
 pymilvus/client/blob.py
 pymilvus/client/check.py
+pymilvus/client/configs.py
 pymilvus/client/constants.py
 pymilvus/client/entity_helper.py
 pymilvus/client/grpc_handler.py
 pymilvus/client/interceptor.py
 pymilvus/client/prepare.py
 pymilvus/client/singleton_utils.py
 pymilvus/client/stub.py
 pymilvus/client/ts_utils.py
 pymilvus/client/types.py
 pymilvus/client/utils.py
+pymilvus/grpc_gen/__init__.py
 pymilvus/grpc_gen/common_pb2.py
-pymilvus/grpc_gen/common_pb2.pyi
 pymilvus/grpc_gen/milvus_pb2.py
-pymilvus/grpc_gen/milvus_pb2.pyi
 pymilvus/grpc_gen/milvus_pb2_grpc.py
 pymilvus/grpc_gen/python_gen.sh
 pymilvus/grpc_gen/schema_pb2.py
-pymilvus/grpc_gen/schema_pb2.pyi
-pymilvus/milvus_client/__init__.py
-pymilvus/milvus_client/defaults.py
-pymilvus/milvus_client/milvus_client.py
-pymilvus/milvus_client/milvus_client_tests.py
 pymilvus/orm/__init__.py
 pymilvus/orm/collection.py
 pymilvus/orm/connections.py
 pymilvus/orm/constants.py
-pymilvus/orm/db.py
+pymilvus/orm/default_config.py
 pymilvus/orm/future.py
 pymilvus/orm/index.py
 pymilvus/orm/mutation.py
 pymilvus/orm/partition.py
 pymilvus/orm/prepare.py
 pymilvus/orm/role.py
 pymilvus/orm/schema.py
@@ -143,9 +133,8 @@
 tests/test_grpc_handler.py
 tests/test_index.py
 tests/test_partition.py
 tests/test_prepare.py
 tests/test_schema.py
 tests/test_ts_utils.py
 tests/test_types.py
-tests/test_utils.py
 tests/utils.py
```

### Comparing `pymilvus-2.2.9/setup.py` & `pymilvus-2.3.0b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,24 +15,22 @@
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/milvus-io/pymilvus',
     license="Apache-2.0",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
-        "grpcio>=1.49.1,<=1.53.0",
-        "protobuf>=3.20.0",
-        "environs<=9.5.0",
-        "ujson>=2.0.0",
-        "pandas>=1.2.4",
-        "numpy!=1.25.0rc1",
+        "grpcio>=1.47.0,<=1.48.0",
+        "grpcio-tools>=1.47.0, <=1.48.0",
+        "ujson>=2.0.0,<=5.4.0",
+        "mmh3>=2.0,<=3.0.0",
+        "pandas==1.1.5; python_version<'3.7'",
+        "pandas>=1.2.4; python_version>'3.6'",
     ],
     classifiers=[
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
 
-    python_requires='>=3.7'
+    python_requires='>=3.6'
 )
```

### Comparing `pymilvus-2.2.9/tests/conftest.py` & `pymilvus-2.3.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/tests/mock_milvus.py` & `pymilvus-2.3.0b1/tests/mock_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/tests/mock_result.py` & `pymilvus-2.3.0b1/tests/mock_result.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/tests/test_check.py` & `pymilvus-2.3.0b1/tests/test_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # For tests
 from pymilvus import *
 
 from pymilvus import MilvusException
 from pymilvus.client.check import (
     check_pass_param,
+    check_index_params
 )
 from pymilvus.client.utils import (
     mkts_from_unixtime,
     mkts_from_datetime,
     mkts_from_hybridts,
     hybridts_to_unixtime
 )
@@ -157,7 +158,27 @@
         for v in versions:
             rv = p.match(v)
             if rv is not None:
                 assert rv.group() == v
 
                 print(f"group {rv.group()}")
                 print(f"group {rv.groups()}")
+
+
+class TestCheckIndexParams:
+    @pytest.mark.parametrize("invalid_params", [
+        ["params type wrong", None],
+        ["params missing index_type", {}],
+        ["params missing params", {"index_type": "IVF_FLAT"}],
+        ["params missing metric_type", {"index_type": "IVF_FLAT", "params": {}}],
+        ["params.params not a dict", {"index_type": "IVF_FLAT", "metric_type": "L2", "params": None}],
+        ["index_type invalid", {"index_type": "INVALID", "metric_type": "L2", "params": {}}],
+        ["params index key invalid", {"index_type": "IVF_FLAT", "metric_type": "L2", "params": {"INVALID": 1}}],
+        ["params index value invalid", {"index_type": "IVF_FLAT", "metric_type": "L2", "params": {"nlist": "INVALID"}}],
+        ["float metric_type invalid", {"index_type": "IVF_FLAT", "metric_type": "INVALIE", "params": {"nlist": 1}}],
+        ["binary metric_type invalid", {"index_type": "BIN_FLAT", "metric_type": "INVALIE", "params": {"nlist": 1}}],
+        ["binary metric_type None", {"index_type": "BIN_FLAT", "metric_type": None, "params": {"nlist": 1}}],
+    ])
+    def test_check_params_invalid(self, invalid_params):
+        with pytest.raises(MilvusException):
+            print(f"sub test: {invalid_params[0]}")
+            check_index_params(invalid_params[1])
```

### Comparing `pymilvus-2.2.9/tests/test_collection.py` & `pymilvus-2.3.0b1/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/tests/test_connections.py` & `pymilvus-2.3.0b1/tests/test_connections.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 import pytest
 import pymilvus
 from unittest import mock
 
 from pymilvus import connections
-from pymilvus import DefaultConfig, MilvusException
+from pymilvus import DefaultConfig, MilvusException, ENV_CONNECTION_CONF
 from pymilvus.exceptions import ErrorCode
 
 LOGGER = logging.getLogger(__name__)
 
 mock_prefix = "pymilvus.client.grpc_handler.GrpcHandler"
 
 
@@ -21,15 +21,15 @@
         - raise ConnectionConfigException if inconsistent configs are given
 
         Connect to an existing and not connected alias will:
         - connect with the existing alias config if no configs are given
         - connect with the providing configs if valid, and replace the old ones.
 
         Connect to a new alias will:
-        - connect with the providing configs if valid, store the new alias with these configs
+        - connect with the provieding configs if valid, store the new alias with these configs
 
     """
     @pytest.fixture(scope="function", params=[
         {},
         {"random": "not useful"},
     ])
     def no_host_port(self, request):
@@ -43,16 +43,14 @@
         return request.param
 
     @pytest.fixture(scope="function", params=[
         {"uri": "https://127.0.0.1:19530"},
         {"uri": "tcp://127.0.0.1:19530"},
         {"uri": "http://127.0.0.1:19530"},
         {"uri": "http://example.com:80"},
-        {"uri": "http://example.com:80/database1"},
-        {"uri": "https://127.0.0.1:19530/databse2"},
     ])
     def uri(self, request):
         return request.param
 
     def test_connect_with_default_config(self):
         alias = "default"
         default_addr = {"address": "localhost:19530", "user": ""}
@@ -70,46 +68,30 @@
 
         addr = connections.get_connection_addr(alias)
         assert addr == default_addr
 
         with mock.patch(f"{mock_prefix}.close", return_value=None):
             connections.disconnect(alias)
 
-    @pytest.fixture(scope="function", params=[
-        ("", {"address": "localhost:19530", "user": ""}),
-        ("localhost", {"address": "localhost:19530", "user": ""}),
-        ("localhost:19530", {"address": "localhost:19530", "user": ""}),
-        ("abc@localhost", {"address": "localhost:19530", "user": "abc"}),
-        ("milvus_host", {"address": "milvus_host:19530", "user": ""}),
-        ("milvus_host:12012", {"address": "milvus_host:12012", "user": ""}),
-        ("abc@milvus_host:12012", {"address": "milvus_host:12012", "user": "abc"}),
-        ("abc@milvus_host", {"address": "milvus_host:19530", "user": "abc"}),
-    ])
-    def test_connect_with_default_config_from_environment(self, env_result):
-        os.environ[DefaultConfig.MILVUS_URI] = env_result[0]
-        assert env_result[1] == connections._read_default_config_from_os_env()
-
-        with mock.patch(f"{mock_prefix}.__init__", return_value=None):
-            with mock.patch(f"{mock_prefix}._wait_for_channel_ready", return_value=None):
-                # use env
-                connections.connect()
+    def test_connect_with_default_config_from_environment(self):
+        test_list = [
+            ["", {"address": "localhost:19530", "user": ""}],
+            ["localhost", {"address": "localhost:19530", "user": ""}],
+            ["localhost:19530", {"address": "localhost:19530", "user": ""}],
+            ["abc@localhost", {"address": "localhost:19530", "user": "abc"}],
+            ["milvus_host", {"address": "milvus_host:19530", "user": ""}],
+            ["milvus_host:12012", {"address": "milvus_host:12012", "user": ""}],
+            ["abc@milvus_host:12012", {"address": "milvus_host:12012", "user": "abc"}],
+            ["abc@milvus_host", {"address": "milvus_host:19530", "user": "abc"}],
+        ]
 
-        assert env_result[1] == connections.get_connection_addr(DefaultConfig.MILVUS_CONN_ALIAS)
+        for env_str, assert_config in test_list:
+            os.environ[ENV_CONNECTION_CONF] = env_str
 
-        with mock.patch(f"{mock_prefix}.__init__", return_value=None):
-            with mock.patch(f"{mock_prefix}._wait_for_channel_ready", return_value=None):
-                # use param
-                connections.connect(DefaultConfig.MILVUS_CONN_ALIAS, host="test_host", port="19999")
-
-        curr_addr = connections.get_connection_addr(DefaultConfig.MILVUS_CONN_ALIAS)
-        assert env_result[1] != curr_addr
-        assert {"address":"test_host:19999", "user": ""} == curr_addr
-
-        with mock.patch(f"{mock_prefix}.close", return_value=None):
-            connections.remove_connection(DefaultConfig.MILVUS_CONN_ALIAS)
+            assert assert_config == connections._read_default_config_from_os_env()
 
     def test_connect_new_alias_with_configs(self):
         alias = "exist"
         addr = {"address": "localhost:19530"}
 
         assert connections.has_connection(alias) is False
         a = connections.get_connection_addr(alias)
@@ -310,21 +292,22 @@
 
         addr = connections.get_connection_addr(alias)
         LOGGER.info(f"addr: {addr}")
 
         host, port = addr["address"].split(':')
         assert host in valid_uri['uri'] or host in DefaultConfig.DEFAULT_HOST
         assert port in valid_uri['uri'] or port in DefaultConfig.DEFAULT_PORT
-        print(addr)
 
         with mock.patch(f"{mock_prefix}.close", return_value=None):
             connections.remove_connection(alias)
 
     @pytest.mark.parametrize("invalid_uri", [
-        {"uri": "http://"},
+        {"uri": "http://:19530"},
+        {"uri": "localhost:19530"},
+        {"uri": ":80"},
         {"uri": None},
         {"uri": -1},
     ])
     def test_add_connection_uri_invalid(self, invalid_uri):
         alias = self.test_add_connection_uri_invalid.__name__
         config = {alias: invalid_uri}
```

### Comparing `pymilvus-2.2.9/tests/test_create_collection.py` & `pymilvus-2.3.0b1/tests/test_create_collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,26 +79,25 @@
         }
         vector_field = {
             "name": "embedding",
             "type": DataType.FLOAT_VECTOR,
             "metric_type": "L2",
             "params": {"dim": "4"},
         }
-        fields = {"fields": [id_field, vector_field], "enable_dynamic_field": True}
+        fields = {"fields": [id_field, vector_field]}
         future = self._milvus.create_collection(collection_name=collection_name, fields=fields, _async=True)
 
         invocation_metadata, request, rpc = self._real_time_channel.take_unary_unary(
             self._servicer.methods_by_name['CreateCollection']
         )
         rpc.send_initial_metadata(())
         rpc.terminate(common_pb2.Status(error_code=common_pb2.Success, reason="success"), (), grpc.StatusCode.OK, '')
 
         request_schema = schema_pb2.CollectionSchema()
         request_schema.ParseFromString(request.schema)
 
         assert request.collection_name == collection_name
         assert Fields.equal(request_schema.fields, fields["fields"])
-        assert request_schema.enable_dynamic_field == fields["enable_dynamic_field"]
 
         return_value = future.result()
         assert return_value.error_code == common_pb2.Success
         assert return_value.reason == "success"
```

### Comparing `pymilvus-2.2.9/tests/test_decorators.py` & `pymilvus-2.3.0b1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/tests/test_grpc_handler.py` & `pymilvus-2.3.0b1/tests/test_grpc_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 reason="unexpected error"),
         )
         rpc.terminate(expected_result, (), grpc.StatusCode.OK, '')
 
         with pytest.raises(MilvusException):
             get_version_future.result()
 
-    def test_get_server_version(self, channel, client_thread):
+    def test_get_server_version_error(self, channel, client_thread):
         version = "2.2.0"
         handler = GrpcHandler(channel=channel)
 
         get_version_future = client_thread.submit(
             handler.get_server_version)
 
         (invocation_metadata, request, rpc) = (
@@ -106,44 +106,7 @@
             status=common_pb2.Status(error_code=common_pb2.Success),
             version=version,
         )
         rpc.terminate(expected_result, (), grpc.StatusCode.OK, '')
 
         got_result = get_version_future.result()
         assert got_result == version
-
-    @pytest.mark.parametrize("_async", [True])
-    def test_flush_all(self, channel, client_thread, _async):
-        handler = GrpcHandler(channel=channel)
-
-        flush_all_future = client_thread.submit(
-            handler.flush_all, _async=_async, timeout=10)
-
-        (invocation_metadata, request, rpc) = (
-            channel.take_unary_unary(descriptor.methods_by_name['FlushAll']))
-        rpc.send_initial_metadata(())
-
-        expected_result = milvus_pb2.FlushAllResponse(
-            status=common_pb2.Status(error_code=common_pb2.Success),
-            flush_all_ts=100,
-        )
-
-        rpc.terminate(expected_result, (), grpc.StatusCode.OK, '')
-        assert flush_all_future is not None
-
-    def test_get_flush_all_state(self, channel, client_thread):
-        handler = GrpcHandler(channel=channel)
-
-        flushed = client_thread.submit(
-            handler.get_flush_all_state, flush_all_ts=100)
-
-        (invocation_metadata, request, rpc) = (
-            channel.take_unary_unary(descriptor.methods_by_name['GetFlushAllState']))
-        rpc.send_initial_metadata(())
-
-        expected_result = milvus_pb2.GetFlushStateResponse(
-            status=common_pb2.Status(error_code=common_pb2.Success),
-            flushed=True,
-        )
-
-        rpc.terminate(expected_result, (), grpc.StatusCode.OK, '')
-        assert flushed.result() is True
```

### Comparing `pymilvus-2.2.9/tests/test_index.py` & `pymilvus-2.3.0b1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/tests/test_partition.py` & `pymilvus-2.3.0b1/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/tests/test_schema.py` & `pymilvus-2.3.0b1/tests/test_schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy
 import pytest
 
-from pymilvus import CollectionSchema, FieldSchema, DataType, MilvusException
+from pymilvus import CollectionSchema, FieldSchema, DataType
 from utils import *
-from pymilvus.orm import schema as s
 
 
 class TestCollectionSchema:
     @pytest.fixture(scope="function")
     def raw_dict(self):
         _dict = {}
         _dict["description"] = "TestCollectionSchema_description"
@@ -30,21 +29,19 @@
                 "description": "ID",
                 "type": DataType.INT64,
                 "is_primary": True,
                 "auto_id": False
             },
         ]
         _dict["fields"] = fields
-        _dict["enable_dynamic_field"] = True
 
         return _dict
 
     def test_constructor_from_dict(self, raw_dict):
         schema = CollectionSchema.construct_from_dict(raw_dict)
-        assert schema.enable_dynamic_field == raw_dict.get("enable_dynamic_field", False)
         assert schema.description, raw_dict['description']
         assert len(schema.fields) == len(raw_dict['fields'])
         f = schema.primary_field
         assert isinstance(f, FieldSchema)
         assert f.name == raw_dict['fields'][2]['name']
 
     def test_to_dict(self, raw_dict):
@@ -142,28 +139,7 @@
 
     #  def test_parse_fields_from_dataframe(self, dataframe1):
     #      fields = parse_fields_from_dataframe(dataframe1)
     #      assert len(fields) == len(dataframe1.columns)
     #      for f in fields:
     #          if f.dtype == DataType.FLOAT_VECTOR:
     #              assert f.dim == len(dataframe1['float_vec'].values[0])
-
-
-class TestCheckInsertDataSchema:
-    def test_check_insert_data_schema_issue1324(self):
-        schema = CollectionSchema([
-            FieldSchema(name="id", dtype=DataType.INT64, descrition="int64", is_primary=True, auto_id=True),
-            FieldSchema(name="embedding", dtype=DataType.FLOAT_VECTOR, descrition="float vector", dim=2),
-            FieldSchema(name="work_id2", dtype=5, descrition="work id"),
-            FieldSchema(name='path', dtype=DataType.VARCHAR, description='path to image', max_length=200),
-            FieldSchema(name="uid", dtype=DataType.INT64, descrition="user id"),
-        ])
-
-        data = [
-            [[0.003984056, 0.05035976]],
-            ['15755403'],
-            ['https://xxx.com/app/works/105149/2023-01-11/w_63be653c4643b/963be653c8aa8c.jpg'],
-            ['105149'],
-        ]
-
-        with pytest.raises(MilvusException):
-            s.check_insert_data_schema(schema, data)
```

### Comparing `pymilvus-2.2.9/tests/test_ts_utils.py` & `pymilvus-2.3.0b1/tests/test_ts_utils.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.9/tests/test_types.py` & `pymilvus-2.3.0b1/tests/test_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under the License.
 
 from pymilvus import DataType, DEFAULT_RESOURCE_GROUP
 from pymilvus.exceptions import InvalidConsistencyLevel
 from pymilvus.client.types import (
-    get_consistency_level, Shard, Group, Replica, ConsistencyLevel
+    get_consistency_level, ConsistencyLevel,
+    Shard, Group, Replica
 )
 
-from pymilvus.grpc_gen import common_pb2
-
 import pytest
 import pandas as pd
 import numpy as np
 
 
 @pytest.mark.xfail
 class TestTypes:
@@ -121,28 +120,21 @@
             get_consistency_level(invalid)
 
 
 class TestReplica:
     def test_shard(self):
         s = Shard("channel-1", (1, 2, 3), 1)
         assert s.channel_name == "channel-1"
-        assert s.shard_nodes == {1, 2, 3}
+        assert s.shard_nodes == (1, 2, 3)
         assert s.shard_leader == 1
         print(s)
 
         g = Group(2, [s], [1, 2, 3], DEFAULT_RESOURCE_GROUP, {})
         assert g.id == 2
         assert g.shards == [s]
         assert g.group_nodes == (1, 2, 3)
 
         print(g)
 
         replica = Replica([g, g])
         assert replica.groups == [g, g]
         print(replica)
-
-    def test_shard_dup_nodeIDs(self):
-        s = Shard("channel-1", (1, 1, 1), 1)
-        assert s.channel_name == "channel-1"
-        assert s.shard_nodes == {1,}
-        assert s.shard_leader == 1
-        print(s)
```

### Comparing `pymilvus-2.2.9/tests/utils.py` & `pymilvus-2.3.0b1/tests/utils.py`

 * *Files identical despite different names*

