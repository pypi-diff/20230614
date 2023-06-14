# Comparing `tmp/service-identity-21.1.0.tar.gz` & `tmp/service_identity-23.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service-identity-21.1.0.tar", last modified: Sun May  9 12:22:16 2021, max compression
+gzip compressed data, last modified: Wed Jun 14 07:54:35 2023, max compression
```

## Comparing `service-identity-21.1.0.tar` & `service_identity-23.1.0.tar`

### file list

```diff
@@ -1,54 +1,44 @@
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-05-09 12:22:16.931798 service-identity-21.1.0/
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-05-09 12:22:16.923117 service-identity-21.1.0/.github/
--rw-r--r--   0 hynek      (501) staff       (20)     3250 2018-02-11 07:20:39.000000 service-identity-21.1.0/.github/CODE_OF_CONDUCT.rst
--rw-r--r--   0 hynek      (501) staff       (20)     6852 2021-05-09 11:53:58.000000 service-identity-21.1.0/.github/CONTRIBUTING.rst
--rw-r--r--   0 hynek      (501) staff       (20)       36 2020-07-01 07:04:22.000000 service-identity-21.1.0/.github/FUNDING.yml
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-05-09 12:22:16.923384 service-identity-21.1.0/.github/workflows/
--rw-r--r--   0 hynek      (501) staff       (20)     2438 2021-05-09 12:20:46.000000 service-identity-21.1.0/.github/workflows/main.yml
--rw-r--r--   0 hynek      (501) staff       (20)      637 2021-04-17 14:15:37.000000 service-identity-21.1.0/.pre-commit-config.yaml
--rw-r--r--   0 hynek      (501) staff       (20)      185 2020-07-01 07:39:30.000000 service-identity-21.1.0/.readthedocs.yml
--rw-r--r--   0 hynek      (501) staff       (20)      315 2019-06-08 13:52:32.000000 service-identity-21.1.0/AUTHORS.rst
--rw-r--r--   0 hynek      (501) staff       (20)     5166 2021-05-09 12:20:46.000000 service-identity-21.1.0/CHANGELOG.rst
--rw-r--r--   0 hynek      (501) staff       (20)     1059 2014-02-20 12:08:05.000000 service-identity-21.1.0/LICENSE
--rw-r--r--   0 hynek      (501) staff       (20)      243 2020-07-01 06:40:40.000000 service-identity-21.1.0/MANIFEST.in
--rw-r--r--   0 hynek      (501) staff       (20)     5773 2021-05-09 12:22:16.931535 service-identity-21.1.0/PKG-INFO
--rw-r--r--   0 hynek      (501) staff       (20)     1965 2021-05-09 11:53:58.000000 service-identity-21.1.0/README.rst
--rw-r--r--   0 hynek      (501) staff       (20)      511 2021-05-09 09:16:46.000000 service-identity-21.1.0/SECURITY.md
--rw-r--r--   0 hynek      (501) staff       (20)      175 2019-05-27 14:46:18.000000 service-identity-21.1.0/codecov.yml
--rw-r--r--   0 hynek      (501) staff       (20)      738 2018-12-05 11:13:48.000000 service-identity-21.1.0/conftest.py
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-05-09 12:22:16.926280 service-identity-21.1.0/docs/
--rw-r--r--   0 hynek      (501) staff       (20)     6802 2019-06-05 12:51:43.000000 service-identity-21.1.0/docs/Makefile
--rw-r--r--   0 hynek      (501) staff       (20)     1949 2021-05-09 11:53:58.000000 service-identity-21.1.0/docs/api.rst
--rw-r--r--   0 hynek      (501) staff       (20)      411 2019-06-08 13:52:32.000000 service-identity-21.1.0/docs/backward-compatibility.rst
--rw-r--r--   0 hynek      (501) staff       (20)       30 2018-12-05 09:48:07.000000 service-identity-21.1.0/docs/changelog.rst
--rw-r--r--   0 hynek      (501) staff       (20)     9383 2021-05-09 12:20:46.000000 service-identity-21.1.0/docs/conf.py
--rw-r--r--   0 hynek      (501) staff       (20)      105 2018-12-05 10:26:34.000000 service-identity-21.1.0/docs/contributing.rst
--rw-r--r--   0 hynek      (501) staff       (20)      599 2018-12-05 09:46:16.000000 service-identity-21.1.0/docs/implemented-standards.rst
--rw-r--r--   0 hynek      (501) staff       (20)      605 2018-02-11 07:21:36.000000 service-identity-21.1.0/docs/index.rst
--rw-r--r--   0 hynek      (501) staff       (20)     1391 2021-05-09 05:11:13.000000 service-identity-21.1.0/docs/installation.rst
--rw-r--r--   0 hynek      (501) staff       (20)      283 2021-05-09 11:53:58.000000 service-identity-21.1.0/docs/license.rst
--rw-r--r--   0 hynek      (501) staff       (20)      353 2021-05-09 09:16:46.000000 service-identity-21.1.0/pyproject.toml
--rw-r--r--   0 hynek      (501) staff       (20)       38 2021-05-09 12:22:16.931890 service-identity-21.1.0/setup.cfg
--rw-r--r--   0 hynek      (501) staff       (20)     4111 2021-05-09 12:20:46.000000 service-identity-21.1.0/setup.py
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-05-09 12:22:16.917529 service-identity-21.1.0/src/
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-05-09 12:22:16.928137 service-identity-21.1.0/src/service_identity/
--rw-r--r--   0 hynek      (501) staff       (20)      708 2021-05-09 12:20:46.000000 service-identity-21.1.0/src/service_identity/__init__.py
--rw-r--r--   0 hynek      (501) staff       (20)    11796 2019-06-05 12:44:08.000000 service-identity-21.1.0/src/service_identity/_common.py
--rw-r--r--   0 hynek      (501) staff       (20)      308 2018-12-05 09:48:06.000000 service-identity-21.1.0/src/service_identity/_compat.py
--rw-r--r--   0 hynek      (501) staff       (20)     4977 2021-05-09 05:11:13.000000 service-identity-21.1.0/src/service_identity/cryptography.py
--rw-r--r--   0 hynek      (501) staff       (20)     1279 2021-04-17 14:15:37.000000 service-identity-21.1.0/src/service_identity/exceptions.py
--rw-r--r--   0 hynek      (501) staff       (20)     5154 2021-05-09 05:11:13.000000 service-identity-21.1.0/src/service_identity/pyopenssl.py
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-05-09 12:22:16.929781 service-identity-21.1.0/src/service_identity.egg-info/
--rw-r--r--   0 hynek      (501) staff       (20)     5773 2021-05-09 12:22:16.000000 service-identity-21.1.0/src/service_identity.egg-info/PKG-INFO
--rw-r--r--   0 hynek      (501) staff       (20)     1032 2021-05-09 12:22:16.000000 service-identity-21.1.0/src/service_identity.egg-info/SOURCES.txt
--rw-r--r--   0 hynek      (501) staff       (20)        1 2021-05-09 12:22:16.000000 service-identity-21.1.0/src/service_identity.egg-info/dependency_links.txt
--rw-r--r--   0 hynek      (501) staff       (20)        1 2019-06-05 12:44:45.000000 service-identity-21.1.0/src/service_identity.egg-info/not-zip-safe
--rw-r--r--   0 hynek      (501) staff       (20)      224 2021-05-09 12:22:16.000000 service-identity-21.1.0/src/service_identity.egg-info/requires.txt
--rw-r--r--   0 hynek      (501) staff       (20)       17 2021-05-09 12:22:16.000000 service-identity-21.1.0/src/service_identity.egg-info/top_level.txt
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-05-09 12:22:16.931108 service-identity-21.1.0/tests/
--rw-r--r--   0 hynek      (501) staff       (20)        0 2014-04-06 01:00:13.000000 service-identity-21.1.0/tests/__init__.py
--rw-r--r--   0 hynek      (501) staff       (20)    20689 2021-04-17 14:15:37.000000 service-identity-21.1.0/tests/test_common.py
--rw-r--r--   0 hynek      (501) staff       (20)     4109 2019-06-05 12:44:09.000000 service-identity-21.1.0/tests/test_cryptography.py
--rw-r--r--   0 hynek      (501) staff       (20)     4635 2019-06-08 13:52:32.000000 service-identity-21.1.0/tests/test_pyopenssl.py
--rw-r--r--   0 hynek      (501) staff       (20)     8782 2019-06-05 12:44:09.000000 service-identity-21.1.0/tests/util.py
--rw-r--r--   0 hynek      (501) staff       (20)     1861 2021-05-09 12:20:46.000000 service-identity-21.1.0/tox.ini
+-rw-r--r--   0        0        0      125 2023-06-14 07:54:35.000000 service_identity-23.1.0/.git_archival.txt
+-rw-r--r--   0        0        0      143 2023-06-14 07:54:35.000000 service_identity-23.1.0/.gitattributes
+-rw-r--r--   0        0        0      664 2023-06-14 07:54:35.000000 service_identity-23.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-06-14 07:54:35.000000 service_identity-23.1.0/.python-version-default
+-rw-r--r--   0        0        0      216 2023-06-14 07:54:35.000000 service_identity-23.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     6929 2023-06-14 07:54:35.000000 service_identity-23.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3031 2023-06-14 07:54:35.000000 service_identity-23.1.0/README.md
+-rw-r--r--   0        0        0     1362 2023-06-14 07:54:35.000000 service_identity-23.1.0/tox.ini
+-rw-r--r--   0        0        0     3167 2023-06-14 07:54:35.000000 service_identity-23.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     8788 2023-06-14 07:54:35.000000 service_identity-23.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       52 2023-06-14 07:54:35.000000 service_identity-23.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      762 2023-06-14 07:54:35.000000 service_identity-23.1.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      123 2023-06-14 07:54:35.000000 service_identity-23.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     4353 2023-06-14 07:54:35.000000 service_identity-23.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      757 2023-06-14 07:54:35.000000 service_identity-23.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1647 2023-06-14 07:54:35.000000 service_identity-23.1.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0     6802 2023-06-14 07:54:35.000000 service_identity-23.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1854 2023-06-14 07:54:35.000000 service_identity-23.1.0/docs/api.rst
+-rw-r--r--   0        0        0       33 2023-06-14 07:54:35.000000 service_identity-23.1.0/docs/changelog.md
+-rw-r--r--   0        0        0     8546 2023-06-14 07:54:35.000000 service_identity-23.1.0/docs/conf.py
+-rw-r--r--   0        0        0      181 2023-06-14 07:54:35.000000 service_identity-23.1.0/docs/implemented-standards.md
+-rw-r--r--   0        0        0      565 2023-06-14 07:54:35.000000 service_identity-23.1.0/docs/index.md
+-rw-r--r--   0        0        0     1353 2023-06-14 07:54:35.000000 service_identity-23.1.0/docs/installation.md
+-rw-r--r--   0        0        0     1184 2023-06-14 07:54:35.000000 service_identity-23.1.0/docs/pyopenssl_example.py
+-rw-r--r--   0        0        0     1396 2023-06-14 07:54:35.000000 service_identity-23.1.0/src/service_identity/__init__.py
+-rw-r--r--   0        0        0     4592 2023-06-14 07:54:35.000000 service_identity-23.1.0/src/service_identity/cryptography.py
+-rw-r--r--   0        0        0     1427 2023-06-14 07:54:35.000000 service_identity-23.1.0/src/service_identity/exceptions.py
+-rw-r--r--   0        0        0    12365 2023-06-14 07:54:35.000000 service_identity-23.1.0/src/service_identity/hazmat.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:54:35.000000 service_identity-23.1.0/src/service_identity/py.typed
+-rw-r--r--   0        0        0     5031 2023-06-14 07:54:35.000000 service_identity-23.1.0/src/service_identity/pyopenssl.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:54:35.000000 service_identity-23.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      641 2023-06-14 07:54:35.000000 service_identity-23.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     4402 2023-06-14 07:54:35.000000 service_identity-23.1.0/tests/test_cryptography.py
+-rw-r--r--   0        0        0    21002 2023-06-14 07:54:35.000000 service_identity-23.1.0/tests/test_hazmat.py
+-rw-r--r--   0        0        0     1701 2023-06-14 07:54:35.000000 service_identity-23.1.0/tests/test_packaging.py
+-rw-r--r--   0        0        0     4659 2023-06-14 07:54:35.000000 service_identity-23.1.0/tests/test_pyopenssl.py
+-rw-r--r--   0        0        0     7735 2023-06-14 07:54:35.000000 service_identity-23.1.0/tests/util.py
+-rw-r--r--   0        0        0       29 2023-06-14 07:54:35.000000 service_identity-23.1.0/tests/constraints/oldest-cryptography.txt
+-rw-r--r--   0        0        0       48 2023-06-14 07:54:35.000000 service_identity-23.1.0/tests/constraints/oldest-pyopenssl.txt
+-rw-r--r--   0        0        0     1166 2023-06-14 07:54:35.000000 service_identity-23.1.0/tests/typing/api.py
+-rw-r--r--   0        0        0       98 2023-06-14 07:54:35.000000 service_identity-23.1.0/.gitignore
+-rw-r--r--   0        0        0     1119 2023-06-14 07:54:35.000000 service_identity-23.1.0/LICENSE
+-rw-r--r--   0        0        0     4969 2023-06-14 07:54:35.000000 service_identity-23.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5534 2023-06-14 07:54:35.000000 service_identity-23.1.0/PKG-INFO
```

### Comparing `service-identity-21.1.0/.github/CODE_OF_CONDUCT.rst` & `service_identity-23.1.0/.github/CODE_OF_CONDUCT.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,48 @@
-Contributor Covenant Code of Conduct
-====================================
+# Contributor Covenant Code of Conduct
 
-Our Pledge
-----------
+## Our Pledge
 
 In the interest of fostering an open and welcoming environment, we as contributors and maintainers pledge to make participation in our project and our community a harassment-free experience for everyone, regardless of age, body size, disability, ethnicity, gender identity and expression, level of experience, nationality, personal appearance, race, religion, or sexual identity and orientation.
 
-Our Standards
--------------
+## Our Standards
 
 Examples of behavior that contributes to creating a positive environment include:
 
-* Using welcoming and inclusive language
-* Being respectful of differing viewpoints and experiences
-* Gracefully accepting constructive criticism
-* Focusing on what is best for the community
-* Showing empathy towards other community members
+- Using welcoming and inclusive language
+- Being respectful of differing viewpoints and experiences
+- Gracefully accepting constructive criticism
+- Focusing on what is best for the community
+- Showing empathy towards other community members
 
 Examples of unacceptable behavior by participants include:
 
-* The use of sexualized language or imagery and unwelcome sexual attention or advances
-* Trolling, insulting/derogatory comments, and personal or political attacks
-* Public or private harassment
-* Publishing others' private information, such as a physical or electronic address, without explicit permission
-* Other conduct which could reasonably be considered inappropriate in a professional setting
+- The use of sexualized language or imagery and unwelcome sexual attention or advances
+- Trolling, insulting/derogatory comments, and personal or political attacks
+- Public or private harassment
+- Publishing others' private information, such as a physical or electronic address, without explicit permission
+- Other conduct which could reasonably be considered inappropriate in a professional setting
 
-Our Responsibilities
---------------------
+## Our Responsibilities
 
 Project maintainers are responsible for clarifying the standards of acceptable behavior and are expected to take appropriate and fair corrective action in response to any instances of unacceptable behavior.
 
 Project maintainers have the right and responsibility to remove, edit, or reject comments, commits, code, wiki edits, issues, and other contributions that are not aligned to this Code of Conduct, or to ban temporarily or permanently any contributor for other behaviors that they deem inappropriate, threatening, offensive, or harmful.
 
-Scope
------
+## Scope
 
 This Code of Conduct applies both within project spaces and in public spaces when an individual is representing the project or its community.
 Examples of representing a project or community include using an official project e-mail address, posting via an official social media account, or acting as an appointed representative at an online or offline event.
 Representation of a project may be further defined and clarified by project maintainers.
 
-Enforcement
------------
+## Enforcement
 
-Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting the project team at hs@ox.cx.
+Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting the project team at <mailto:hs@ox.cx>.
 All complaints will be reviewed and investigated and will result in a response that is deemed necessary and appropriate to the circumstances.
 The project team is obligated to maintain confidentiality with regard to the reporter of an incident.
 Further details of specific enforcement policies may be posted separately.
 
 Project maintainers who do not follow or enforce the Code of Conduct in good faith may face temporary or permanent repercussions as determined by other members of the project's leadership.
 
-Attribution
------------
+## Attribution
 
-This Code of Conduct is adapted from the `Contributor Covenant <https://www.contributor-covenant.org>`_, version 1.4, available at <https://www.contributor-covenant.org/version/1/4/code-of-conduct.html>.
+This Code of Conduct is adapted from the [Contributor Covenant](https://www.contributor-covenant.org), version 1.4, available at \<<https://www.contributor-covenant.org/version/1/4/code-of-conduct.html>>.
```

### Comparing `service-identity-21.1.0/LICENSE` & `service_identity-23.1.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2014 Hynek Schlawack
+The MIT License (MIT)
+
+Copyright (c) 2014 Hynek Schlawack and the service-identity contibutors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `service-identity-21.1.0/README.rst` & `service_identity-23.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,123 +1,190 @@
-00000000: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 5365  =============.Se
-00000020: 7276 6963 6520 4964 656e 7469 7479 2056  rvice Identity V
-00000030: 6572 6966 6963 6174 696f 6e0a 3d3d 3d3d  erification.====
-00000040: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000050: 3d3d 3d3d 3d3d 3d3d 3d0a 0a2e 2e20 696d  =========.... im
-00000060: 6167 653a 3a20 6874 7470 733a 2f2f 7265  age:: https://re
-00000070: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
-00000080: 6f6a 6563 7473 2f73 6572 7669 6365 2d69  ojects/service-i
-00000090: 6465 6e74 6974 792f 6261 6467 652f 3f76  dentity/badge/?v
-000000a0: 6572 7369 6f6e 3d73 7461 626c 650a 2020  ersion=stable.  
-000000b0: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-000000c0: 2f2f 7365 7276 6963 652d 6964 656e 7469  //service-identi
-000000d0: 7479 2e72 6561 6474 6865 646f 6373 2e69  ty.readthedocs.i
-000000e0: 6f2f 656e 2f73 7461 626c 652f 3f62 6164  o/en/stable/?bad
-000000f0: 6765 3d73 7461 626c 650a 2020 203a 616c  ge=stable.   :al
-00000100: 743a 2044 6f63 756d 656e 7461 7469 6f6e  t: Documentation
-00000110: 2053 7461 7475 730a 0a2e 2e20 696d 6167   Status.... imag
-00000120: 653a 3a20 6874 7470 733a 2f2f 6769 7468  e:: https://gith
-00000130: 7562 2e63 6f6d 2f70 7963 612f 7365 7276  ub.com/pyca/serv
-00000140: 6963 652d 6964 656e 7469 7479 2f77 6f72  ice-identity/wor
-00000150: 6b66 6c6f 7773 2f43 492f 6261 6467 652e  kflows/CI/badge.
-00000160: 7376 673f 6272 616e 6368 3d6d 6169 6e0a  svg?branch=main.
-00000170: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
-00000180: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000190: 7963 612f 7365 7276 6963 652d 6964 656e  yca/service-iden
-000001a0: 7469 7479 2f61 6374 696f 6e73 3f77 6f72  tity/actions?wor
-000001b0: 6b66 6c6f 773d 4349 0a20 2020 3a61 6c74  kflow=CI.   :alt
-000001c0: 3a20 4349 2053 7461 7475 730a 0a2e 2e20  : CI Status.... 
-000001d0: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-000001e0: 636f 6465 636f 762e 696f 2f67 6974 6875  codecov.io/githu
-000001f0: 622f 7079 6361 2f73 6572 7669 6365 2d69  b/pyca/service-i
-00000200: 6465 6e74 6974 792f 6272 616e 6368 2f6d  dentity/branch/m
-00000210: 6169 6e2f 6772 6170 682f 6261 6467 652e  ain/graph/badge.
-00000220: 7376 670a 2020 203a 7461 7267 6574 3a20  svg.   :target: 
-00000230: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
-00000240: 696f 2f67 6974 6875 622f 7079 6361 2f73  io/github/pyca/s
-00000250: 6572 7669 6365 2d69 6465 6e74 6974 790a  ervice-identity.
-00000260: 2020 203a 616c 743a 2054 6573 7420 436f     :alt: Test Co
-00000270: 7665 7261 6765 0a0a 2e2e 2069 6d61 6765  verage.... image
-00000280: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
-00000290: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000002a0: 636f 6465 2532 3073 7479 6c65 2d62 6c61  code%20style-bla
-000002b0: 636b 2d30 3030 3030 302e 7376 670a 2020  ck-000000.svg.  
-000002c0: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-000002d0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6d62  //github.com/amb
-000002e0: 762f 626c 6163 6b0a 2020 203a 616c 743a  v/black.   :alt:
-000002f0: 2043 6f64 6520 7374 796c 653a 2062 6c61   Code style: bla
-00000300: 636b 0a0a 2e2e 2069 6d61 6765 3a3a 2068  ck.... image:: h
-00000310: 7474 7073 3a2f 2f77 7777 2e69 7263 636c  ttps://www.irccl
-00000320: 6f75 642e 636f 6d2f 696e 7669 7465 2d73  oud.com/invite-s
-00000330: 7667 3f63 6861 6e6e 656c 3d25 3233 6372  vg?channel=%23cr
-00000340: 7970 746f 6772 6170 6879 2d64 6576 2661  yptography-dev&a
-00000350: 6d70 3b68 6f73 746e 616d 653d 6972 632e  mp;hostname=irc.
-00000360: 6672 6565 6e6f 6465 2e6e 6574 2661 6d70  freenode.net&amp
-00000370: 3b70 6f72 743d 3636 3937 2661 6d70 3b73  ;port=6697&amp;s
-00000380: 736c 3d31 0a20 2020 203a 7461 7267 6574  sl=1.    :target
-00000390: 3a20 6874 7470 733a 2f2f 7777 772e 6972  : https://www.ir
-000003a0: 6363 6c6f 7564 2e63 6f6d 2f69 6e76 6974  ccloud.com/invit
-000003b0: 653f 6368 616e 6e65 6c3d 2532 3363 7279  e?channel=%23cry
-000003c0: 7074 6f67 7261 7068 792d 6465 7626 616d  ptography-dev&am
-000003d0: 703b 686f 7374 6e61 6d65 3d69 7263 2e66  p;hostname=irc.f
-000003e0: 7265 656e 6f64 652e 6e65 7426 616d 703b  reenode.net&amp;
-000003f0: 706f 7274 3d36 3639 3726 616d 703b 7373  port=6697&amp;ss
-00000400: 6c3d 310a 0a2e 2e20 6265 6769 6e0a 0a55  l=1.... begin..U
-00000410: 7365 2074 6869 7320 7061 636b 6167 6520  se this package 
-00000420: 6966 3a0a 0a2d 2079 6f75 2075 7365 2070  if:..- you use p
-00000430: 794f 7065 6e53 534c 5f20 616e 6420 646f  yOpenSSL_ and do
-00000440: 6ee2 8099 7420 7761 6e74 2074 6f20 6265  n...t want to be
-00000450: 204d 4954 4d5f 5c20 6564 206f 720a 2d20   MITM_\ ed or.- 
-00000460: 6966 2079 6f75 2077 616e 7420 746f 2076  if you want to v
-00000470: 6572 6966 7920 7468 6174 2061 2060 5079  erify that a `Py
-00000480: 4341 2063 7279 7074 6f67 7261 7068 7960  CA cryptography`
-00000490: 5f20 6365 7274 6966 6963 6174 6520 6973  _ certificate is
-000004a0: 2076 616c 6964 2066 6f72 2061 2063 6572   valid for a cer
-000004b0: 7461 696e 2068 6f73 746e 616d 6520 6f72  tain hostname or
-000004c0: 2049 5020 6164 6472 6573 732e 0a0a 6060   IP address...``
-000004d0: 7365 7276 6963 652d 6964 656e 7469 7479  service-identity
-000004e0: 6060 2061 7370 6972 6573 2074 6f20 6769  `` aspires to gi
-000004f0: 7665 2079 6f75 2061 6c6c 2074 6865 2074  ve you all the t
-00000500: 6f6f 6c73 2079 6f75 206e 6565 6420 666f  ools you need fo
-00000510: 7220 7665 7269 6679 696e 6720 7768 6574  r verifying whet
-00000520: 6865 7220 6120 6365 7274 6966 6963 6174  her a certificat
-00000530: 6520 6973 2076 616c 6964 2066 6f72 2074  e is valid for t
-00000540: 6865 2069 6e74 656e 6465 6420 7075 7270  he intended purp
-00000550: 6f73 6573 2e0a 0a49 6e20 7468 6520 7369  oses...In the si
-00000560: 6d70 6c65 7374 2063 6173 652c 2074 6869  mplest case, thi
-00000570: 7320 6d65 616e 7320 2a68 6f73 7420 6e61  s means *host na
-00000580: 6d65 2076 6572 6966 6963 6174 696f 6e2a  me verification*
-00000590: 2e0a 486f 7765 7665 722c 2060 6073 6572  ..However, ``ser
-000005a0: 7669 6365 2d69 6465 6e74 6974 7960 6020  vice-identity`` 
-000005b0: 696d 706c 656d 656e 7473 2060 5246 4320  implements `RFC 
-000005c0: 3631 3235 605f 2066 756c 6c79 2061 6e64  6125`_ fully and
-000005d0: 2070 6c61 6e73 2074 6f20 6164 6420 6f74   plans to add ot
-000005e0: 6865 7220 7265 6c65 7661 6e74 2052 4643  her relevant RFC
-000005f0: 7320 746f 6f2e 0a0a 6060 7365 7276 6963  s too...``servic
-00000600: 652d 6964 656e 7469 7479 6060 5c20 e280  e-identity``\ ..
-00000610: 9973 2064 6f63 756d 656e 7461 7469 6f6e  .s documentation
-00000620: 206c 6976 6573 2061 7420 6052 6561 6420   lives at `Read 
-00000630: 7468 6520 446f 6373 203c 6874 7470 733a  the Docs <https:
-00000640: 2f2f 7365 7276 6963 652d 6964 656e 7469  //service-identi
-00000650: 7479 2e72 6561 6474 6865 646f 6373 2e69  ty.readthedocs.i
-00000660: 6f2f 3e60 5f2c 2074 6865 2063 6f64 6520  o/>`_, the code 
-00000670: 6f6e 2060 4769 7448 7562 203c 6874 7470  on `GitHub <http
-00000680: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000690: 7963 612f 7365 7276 6963 652d 6964 656e  yca/service-iden
-000006a0: 7469 7479 3e60 5f2e 0a0a 0a2e 2e20 5f54  tity>`_...... _T
-000006b0: 7769 7374 6564 3a20 6874 7470 733a 2f2f  wisted: https://
-000006c0: 7477 6973 7465 646d 6174 7269 782e 636f  twistedmatrix.co
-000006d0: 6d2f 0a2e 2e20 5f70 794f 7065 6e53 534c  m/... _pyOpenSSL
-000006e0: 3a20 6874 7470 733a 2f2f 7079 7069 2e6f  : https://pypi.o
-000006f0: 7267 2f70 726f 6a65 6374 2f70 794f 7065  rg/project/pyOpe
-00000700: 6e53 534c 2f0a 2e2e 205f 4d49 544d 3a20  nSSL/... _MITM: 
-00000710: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00000720: 6564 6961 2e6f 7267 2f77 696b 692f 4d61  edia.org/wiki/Ma
-00000730: 6e2d 696e 2d74 6865 2d6d 6964 646c 655f  n-in-the-middle_
-00000740: 6174 7461 636b 0a2e 2e20 5f52 4643 2036  attack... _RFC 6
-00000750: 3132 353a 2068 7474 7073 3a2f 2f77 7777  125: https://www
-00000760: 2e72 6663 2d65 6469 746f 722e 6f72 672f  .rfc-editor.org/
-00000770: 696e 666f 2f72 6663 3631 3235 0a2e 2e20  info/rfc6125... 
-00000780: 5f50 7943 4120 6372 7970 746f 6772 6170  _PyCA cryptograp
-00000790: 6879 3a20 6874 7470 733a 2f2f 6372 7970  hy: https://cryp
-000007a0: 746f 6772 6170 6879 2e69 6f2f 0a         tography.io/.
+00000000: 2320 5365 7276 6963 6520 4964 656e 7469  # Service Identi
+00000010: 7479 2056 6572 6966 6963 6174 696f 6e0a  ty Verification.
+00000020: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000030: 2f2f 7365 7276 6963 652d 6964 656e 7469  //service-identi
+00000040: 7479 2e72 6561 6474 6865 646f 6373 2e69  ty.readthedocs.i
+00000050: 6f2f 223e 0a20 2020 203c 696d 6720 7372  o/">.    <img sr
+00000060: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000070: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000080: 446f 6373 2d52 6561 6425 3230 5468 6525  Docs-Read%20The%
+00000090: 3230 446f 6373 2d62 6c61 636b 2220 616c  20Docs-black" al
+000000a0: 743d 2244 6f63 756d 656e 7461 7469 6f6e  t="Documentation
+000000b0: 2220 2f3e 0a3c 2f61 3e0a 3c61 2068 7265  " />.</a>.<a hre
+000000c0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+000000d0: 622e 636f 6d2f 7079 6361 2f73 6572 7669  b.com/pyca/servi
+000000e0: 6365 2d69 6465 6e74 6974 792f 626c 6f62  ce-identity/blob
+000000f0: 2f6d 6169 6e2f 4c49 4345 4e53 4522 3e0a  /main/LICENSE">.
+00000100: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000110: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000120: 732e 696f 2f62 6164 6765 2f6c 6963 656e  s.io/badge/licen
+00000130: 7365 2d4d 4954 2d43 3036 3532 3422 2061  se-MIT-C06524" a
+00000140: 6c74 3d22 4c69 6365 6e73 653a 204d 4954  lt="License: MIT
+00000150: 2220 2f3e 0a3c 2f61 3e0a 3c61 2068 7265  " />.</a>.<a hre
+00000160: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+00000170: 6f72 672f 7072 6f6a 6563 742f 7365 7276  org/project/serv
+00000180: 6963 652d 6964 656e 7469 7479 2f22 3e0a  ice-identity/">.
+00000190: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000001a0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000001b0: 732e 696f 2f70 7970 692f 762f 7365 7276  s.io/pypi/v/serv
+000001c0: 6963 652d 6964 656e 7469 7479 2220 616c  ice-identity" al
+000001d0: 743d 2250 7950 4920 7265 6c65 6173 6522  t="PyPI release"
+000001e0: 202f 3e0a 3c2f 613e 0a3c 6120 6872 6566   />.</a>.<a href
+000001f0: 3d22 6874 7470 733a 2f2f 7065 7079 2e74  ="https://pepy.t
+00000200: 6563 682f 7072 6f6a 6563 742f 7365 7276  ech/project/serv
+00000210: 6963 652d 6964 656e 7469 7479 223e 0a20  ice-identity">. 
+00000220: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000230: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
+00000240: 2e74 6563 682f 6261 6467 652f 7365 7276  .tech/badge/serv
+00000250: 6963 652d 6964 656e 7469 7479 2f6d 6f6e  ice-identity/mon
+00000260: 7468 2220 616c 743d 2244 6f77 6e6c 6f61  th" alt="Downloa
+00000270: 6473 2070 6572 206d 6f6e 7468 2220 2f3e  ds per month" />
+00000280: 0a3c 2f61 3e0a 3c61 2068 7265 663d 2268  .</a>.<a href="h
+00000290: 7474 7073 3a2f 2f62 6573 7470 7261 6374  ttps://bestpract
+000002a0: 6963 6573 2e63 6f72 6569 6e66 7261 7374  ices.coreinfrast
+000002b0: 7275 6374 7572 652e 6f72 672f 7072 6f6a  ructure.org/proj
+000002c0: 6563 7473 2f37 3436 3222 3e0a 2020 2020  ects/7462">.    
+000002d0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000002e0: 2f2f 6265 7374 7072 6163 7469 6365 732e  //bestpractices.
+000002f0: 636f 7265 696e 6672 6173 7472 7563 7475  coreinfrastructu
+00000300: 7265 2e6f 7267 2f70 726f 6a65 6374 732f  re.org/projects/
+00000310: 3734 3632 2f62 6164 6765 2220 2f3e 0a3c  7462/badge" />.<
+00000320: 2f61 3e0a 3c61 2068 7265 663d 2268 7474  /a>.<a href="htt
+00000330: 7073 3a2f 2f77 7777 2e69 7263 636c 6f75  ps://www.ircclou
+00000340: 642e 636f 6d2f 696e 7669 7465 3f63 6861  d.com/invite?cha
+00000350: 6e6e 656c 3d25 3233 7079 6361 2661 6d70  nnel=%23pyca&amp
+00000360: 3b68 6f73 746e 616d 653d 6972 632e 6c69  ;hostname=irc.li
+00000370: 6265 7261 2e63 6861 7426 616d 703b 706f  bera.chat&amp;po
+00000380: 7274 3d36 3639 3726 616d 703b 7373 6c3d  rt=6697&amp;ssl=
+00000390: 3122 3e0a 2020 2020 3c69 6d67 2073 7263  1">.    <img src
+000003a0: 3d22 6874 7470 733a 2f2f 7777 772e 6972  ="https://www.ir
+000003b0: 6363 6c6f 7564 2e63 6f6d 2f69 6e76 6974  ccloud.com/invit
+000003c0: 652d 7376 673f 6368 616e 6e65 6c3d 2532  e-svg?channel=%2
+000003d0: 3370 7963 6126 616d 703b 686f 7374 6e61  3pyca&amp;hostna
+000003e0: 6d65 3d69 7263 2e6c 6962 6572 612e 6368  me=irc.libera.ch
+000003f0: 6174 2661 6d70 3b70 6f72 743d 3636 3937  at&amp;port=6697
+00000400: 2661 6d70 3b73 736c 3d31 2220 616c 743d  &amp;ssl=1" alt=
+00000410: 2250 7943 4120 6f6e 2049 5243 2220 2f3e  "PyCA on IRC" />
+00000420: 0a3c 2f61 3e0a 0a3c 212d 2d20 7370 6965  .</a>..<!-- spie
+00000430: 6c2d 6265 6769 6e20 2d2d 3e0a 0a55 7365  l-begin -->..Use
+00000440: 2074 6869 7320 7061 636b 6167 6520 6966   this package if
+00000450: 3a0a 0a2d 2079 6f75 2077 616e 7420 746f  :..- you want to
+00000460: 202a 2a76 6572 6966 792a 2a20 7468 6174   **verify** that
+00000470: 2061 205b 5079 4341 202a 6372 7970 746f   a [PyCA *crypto
+00000480: 6772 6170 6879 2a5d 2868 7474 7073 3a2f  graphy*](https:/
+00000490: 2f63 7279 7074 6f67 7261 7068 792e 696f  /cryptography.io
+000004a0: 2f29 2063 6572 7469 6669 6361 7465 2069  /) certificate i
+000004b0: 7320 7661 6c69 6420 666f 7220 6120 6365  s valid for a ce
+000004c0: 7274 6169 6e20 686f 7374 6e61 6d65 206f  rtain hostname o
+000004d0: 7220 4950 2061 6464 7265 7373 2c0a 2d20  r IP address,.- 
+000004e0: 6f72 2069 6620 796f 7520 7573 6520 5b70  or if you use [p
+000004f0: 794f 7065 6e53 534c 5d28 6874 7470 733a  yOpenSSL](https:
+00000500: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000510: 6374 2f70 794f 7065 6e53 534c 2f29 2061  ct/pyOpenSSL/) a
+00000520: 6e64 2064 6f6e e280 9974 2077 616e 7420  nd don...t want 
+00000530: 746f 2062 6520 5b2a 2a4d 4954 4d2a 2a5d  to be [**MITM**]
+00000540: 2868 7474 7073 3a2f 2f65 6e2e 7769 6b69  (https://en.wiki
+00000550: 7065 6469 612e 6f72 672f 7769 6b69 2f4d  pedia.org/wiki/M
+00000560: 616e 2d69 6e2d 7468 652d 6d69 6464 6c65  an-in-the-middle
+00000570: 5f61 7474 6163 6b29 6564 2c0a 2d20 6f72  _attack)ed,.- or
+00000580: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
+00000590: 2a2a 696e 7370 6563 742a 2a20 6365 7274  **inspect** cert
+000005a0: 6966 6963 6174 6573 2066 726f 6d20 6569  ificates from ei
+000005b0: 7468 6572 2066 6f72 2073 6572 7669 6365  ther for service
+000005c0: 2049 4473 2e0a 0a2a 7365 7276 6963 652d   IDs...*service-
+000005d0: 6964 656e 7469 7479 2a20 6173 7069 7265  identity* aspire
+000005e0: 7320 746f 2067 6976 6520 796f 7520 616c  s to give you al
+000005f0: 6c20 7468 6520 746f 6f6c 7320 796f 7520  l the tools you 
+00000600: 6e65 6564 2066 6f72 2076 6572 6966 7969  need for verifyi
+00000610: 6e67 2077 6865 7468 6572 2061 2063 6572  ng whether a cer
+00000620: 7469 6669 6361 7465 2069 7320 7661 6c69  tificate is vali
+00000630: 6420 666f 7220 7468 6520 696e 7465 6e64  d for the intend
+00000640: 6564 2070 7572 706f 7365 732e 0a49 6e20  ed purposes..In 
+00000650: 7468 6520 7369 6d70 6c65 7374 2063 6173  the simplest cas
+00000660: 652c 2074 6869 7320 6d65 616e 7320 2a68  e, this means *h
+00000670: 6f73 7420 6e61 6d65 2076 6572 6966 6963  ost name verific
+00000680: 6174 696f 6e2a 2e0a 486f 7765 7665 722c  ation*..However,
+00000690: 202a 7365 7276 6963 652d 6964 656e 7469   *service-identi
+000006a0: 7479 2a20 696d 706c 656d 656e 7473 205b  ty* implements [
+000006b0: 5246 4320 3631 3235 5d28 6874 7470 733a  RFC 6125](https:
+000006c0: 2f2f 6461 7461 7472 6163 6b65 722e 6965  //datatracker.ie
+000006d0: 7466 2e6f 7267 2f64 6f63 2f68 746d 6c2f  tf.org/doc/html/
+000006e0: 7266 6336 3132 352e 6874 6d6c 2920 6675  rfc6125.html) fu
+000006f0: 6c6c 792e 0a0a 0a23 2320 5072 6f6a 6563  lly....## Projec
+00000700: 7420 496e 666f 726d 6174 696f 6e0a 0a2a  t Information..*
+00000710: 7365 7276 6963 652d 6964 656e 7469 7479  service-identity
+00000720: 2a20 6973 2072 656c 6561 7365 6420 756e  * is released un
+00000730: 6465 7220 7468 6520 5b4d 4954 5d28 6874  der the [MIT](ht
+00000740: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000750: 2f70 7963 612f 7365 7276 6963 652d 6964  /pyca/service-id
+00000760: 656e 7469 7479 2f62 6c6f 622f 6d61 696e  entity/blob/main
+00000770: 2f4c 4943 454e 5345 2920 6c69 6365 6e73  /LICENSE) licens
+00000780: 652c 2069 7473 2064 6f63 756d 656e 7461  e, its documenta
+00000790: 7469 6f6e 206c 6976 6573 2061 7420 5b52  tion lives at [R
+000007a0: 6561 6420 7468 6520 446f 6373 5d28 6874  ead the Docs](ht
+000007b0: 7470 733a 2f2f 7365 7276 6963 652d 6964  tps://service-id
+000007c0: 656e 7469 7479 2e72 6561 6474 6865 646f  entity.readthedo
+000007d0: 6373 2e69 6f2f 292c 2074 6865 2063 6f64  cs.io/), the cod
+000007e0: 6520 6f6e 205b 4769 7448 7562 5d28 6874  e on [GitHub](ht
+000007f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000800: 2f70 7963 612f 7365 7276 6963 652d 6964  /pyca/service-id
+00000810: 656e 7469 7479 292c 2061 6e64 2074 6865  entity), and the
+00000820: 206c 6174 6573 7420 7265 6c65 6173 6520   latest release 
+00000830: 6f6e 205b 5079 5049 5d28 6874 7470 733a  on [PyPI](https:
+00000840: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000850: 6374 2f73 6572 7669 6365 2d69 6465 6e74  ct/service-ident
+00000860: 6974 792f 292e 0a0a 0a23 2323 2043 7265  ity/)....### Cre
+00000870: 6469 7473 0a0a 2a73 6572 7669 6365 2d69  dits..*service-i
+00000880: 6465 6e74 6974 792a 2069 7320 7772 6974  dentity* is writ
+00000890: 7465 6e20 616e 6420 6d61 696e 7461 696e  ten and maintain
+000008a0: 6564 2062 7920 5b48 796e 656b 2053 6368  ed by [Hynek Sch
+000008b0: 6c61 7761 636b 5d28 6874 7470 733a 2f2f  lawack](https://
+000008c0: 6879 6e65 6b2e 6d65 2f29 2e0a 0a54 6865  hynek.me/)...The
+000008d0: 2064 6576 656c 6f70 6d65 6e74 2069 7320   development is 
+000008e0: 6b69 6e64 6c79 2073 7570 706f 7274 6564  kindly supported
+000008f0: 2062 7920 6d79 2065 6d70 6c6f 7965 7220   by my employer 
+00000900: 5b56 6172 696f 6d65 6469 6120 4147 5d28  [Variomedia AG](
+00000910: 6874 7470 733a 2f2f 7777 772e 7661 7269  https://www.vari
+00000920: 6f6d 6564 6961 2e64 652f 292c 202a 7365  omedia.de/), *se
+00000930: 7276 6963 652d 6964 656e 7469 7479 2a27  rvice-identity*'
+00000940: 7320 5b54 6964 656c 6966 7420 7375 6273  s [Tidelift subs
+00000950: 6372 6962 6572 735d 5b54 6964 656c 6966  cribers][Tidelif
+00000960: 745d 2c20 616e 6420 616c 6c20 6d79 2061  t], and all my a
+00000970: 6d61 7a69 6e67 205b 4769 7448 7562 2053  mazing [GitHub S
+00000980: 706f 6e73 6f72 735d 2868 7474 7073 3a2f  ponsors](https:/
+00000990: 2f67 6974 6875 622e 636f 6d2f 7370 6f6e  /github.com/spon
+000009a0: 736f 7273 2f68 796e 656b 292e 0a0a 0a23  sors/hynek)....#
+000009b0: 2323 202a 7365 7276 6963 652d 6964 656e  ## *service-iden
+000009c0: 7469 7479 2a20 666f 7220 456e 7465 7270  tity* for Enterp
+000009d0: 7269 7365 0a0a 4176 6169 6c61 626c 6520  rise..Available 
+000009e0: 6173 2070 6172 7420 6f66 2074 6865 2054  as part of the T
+000009f0: 6964 656c 6966 7420 5375 6273 6372 6970  idelift Subscrip
+00000a00: 7469 6f6e 2e0a 0a54 6865 206d 6169 6e74  tion...The maint
+00000a10: 6169 6e65 7273 206f 6620 2a73 6572 7669  ainers of *servi
+00000a20: 6365 2d69 6465 6e74 6974 792a 2061 6e64  ce-identity* and
+00000a30: 2074 686f 7573 616e 6473 206f 6620 6f74   thousands of ot
+00000a40: 6865 7220 7061 636b 6167 6573 2061 7265  her packages are
+00000a50: 2077 6f72 6b69 6e67 2077 6974 6820 5469   working with Ti
+00000a60: 6465 6c69 6674 2074 6f20 6465 6c69 7665  delift to delive
+00000a70: 7220 636f 6d6d 6572 6369 616c 2073 7570  r commercial sup
+00000a80: 706f 7274 2061 6e64 206d 6169 6e74 656e  port and mainten
+00000a90: 616e 6365 2066 6f72 2074 6865 206f 7065  ance for the ope
+00000aa0: 6e2d 736f 7572 6365 2070 6163 6b61 6765  n-source package
+00000ab0: 7320 796f 7520 7573 6520 746f 2062 7569  s you use to bui
+00000ac0: 6c64 2079 6f75 7220 6170 706c 6963 6174  ld your applicat
+00000ad0: 696f 6e73 2e0a 5361 7665 2074 696d 652c  ions..Save time,
+00000ae0: 2072 6564 7563 6520 7269 736b 2c20 616e   reduce risk, an
+00000af0: 6420 696d 7072 6f76 6520 636f 6465 2068  d improve code h
+00000b00: 6561 6c74 682c 2077 6869 6c65 2070 6179  ealth, while pay
+00000b10: 696e 6720 7468 6520 6d61 696e 7461 696e  ing the maintain
+00000b20: 6572 7320 6f66 2074 6865 2065 7861 6374  ers of the exact
+00000b30: 2070 6163 6b61 6765 7320 796f 7520 7573   packages you us
+00000b40: 652e 0a5b 4c65 6172 6e20 6d6f 7265 2e5d  e..[Learn more.]
+00000b50: 5b54 6964 656c 6966 745d 0a0a 5b54 6964  [Tidelift]..[Tid
+00000b60: 656c 6966 745d 3a20 6874 7470 733a 2f2f  elift]: https://
+00000b70: 7469 6465 6c69 6674 2e63 6f6d 2f73 7562  tidelift.com/sub
+00000b80: 7363 7269 7074 696f 6e2f 706b 672f 7079  scription/pkg/py
+00000b90: 7069 2d73 6572 7669 6365 2d69 6465 6e74  pi-service-ident
+00000ba0: 6974 793f 7574 6d5f 736f 7572 6365 3d70  ity?utm_source=p
+00000bb0: 7970 692d 7365 7276 6963 652d 6964 656e  ypi-service-iden
+00000bc0: 7469 7479 2675 746d 5f6d 6564 6975 6d3d  tity&utm_medium=
+00000bd0: 7265 6164 6d65 0a                        readme.
```

### Comparing `service-identity-21.1.0/conftest.py` & `service_identity-23.1.0/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,12 +22,7 @@
 OpenSSL: {openssl}
 pyOpenSSL: {pyOpenSSL}
 cryptography: {cryptography}""".format(
         openssl=openssl_version,
         pyOpenSSL=pyopenssl_version,
         cryptography=cryptography.__version__,
     )
-
-
-collect_ignore = []
-if OpenSSL is None:
-    collect_ignore.extend(["tests/test_pyopenssl.py"])
```

### Comparing `service-identity-21.1.0/docs/Makefile` & `service_identity-23.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `service-identity-21.1.0/docs/api.rst` & `service_identity-23.1.0/docs/api.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,75 @@
 ===
 API
 ===
 
 .. note::
 
-   So far, public APIs are only available for hostnames (RFC 6125) and IP addresses (RFC 2818).
-   All IDs specified by RFC 6125 are already implemented though.
-   If you'd like to play with them and provide feedback have a look at the ``verify_service_identity`` function in the `_common module <https://github.com/pyca/service-identity/blob/main/src/service_identity/_common.py>`_.
+   So far, public high-level APIs are only available for host names (:rfc:`6125`) and IP addresses (:rfc:`2818`).
+   All IDs specified by :rfc:`6125` are already implemented though.
+   If you'd like to play with them and provide feedback have a look at the ``verify_service_identity`` function in the `hazmat module <https://github.com/pyca/service-identity/blob/main/src/service_identity/hazmat.py>`_.
+
+
+PyCA cryptography
+=================
+
+.. currentmodule:: service_identity.cryptography
+
+.. autofunction:: verify_certificate_hostname
+.. autofunction:: verify_certificate_ip_address
+.. autofunction:: extract_patterns
 
 
 pyOpenSSL
 =========
 
 .. currentmodule:: service_identity.pyopenssl
 
 .. autofunction:: verify_hostname
 
-   In practice, this may look like the following::
+   In practice, this may look like the following:
 
-      from __future__ import absolute_import, division, print_function
+   .. include:: pyopenssl_example.py
+      :literal:
 
-      import socket
+.. autofunction:: verify_ip_address
+.. autofunction:: extract_patterns
 
-      from OpenSSL import SSL
-      from service_identity import VerificationError
-      from service_identity.pyopenssl import verify_hostname
-
-
-      ctx = SSL.Context(SSL.SSLv23_METHOD)
-      ctx.set_verify(SSL.VERIFY_PEER, lambda conn, cert, errno, depth, ok: ok)
-      ctx.set_default_verify_paths()
-
-      hostname = u"twistedmatrix.com"
-      conn = SSL.Connection(ctx, socket.socket(socket.AF_INET, socket.SOCK_STREAM))
-      conn.connect((hostname, 443))
-
-      try:
-         conn.do_handshake()
-         verify_hostname(conn, hostname)
-         # Do your super-secure stuff here.
-      except SSL.Error as e:
-         print("TLS Handshake failed: {0!r}.".format(e.args[0]))
-      except VerificationError:
-         print("Presented certificate is not valid for {0}.".format(hostname))
-      finally:
-         conn.shutdown()
-         conn.close()
 
-.. autofunction:: verify_ip_address
+Hazardous Materials
+===================
 
+.. currentmodule:: service_identity.hazmat
 
-PyCA cryptography
-=================
 
-.. currentmodule:: service_identity.cryptography
+.. danger::
 
-.. autofunction:: verify_certificate_hostname
-.. autofunction:: verify_certificate_ip_address
+   The following APIs require reader's discretion.
+   They are stable and they've been using internally by *service-identity* for years, but you need to know what you're doing.
+
+
+Pattern Objects
+---------------
+
+The following are the objects return by the ``extract_patterns`` functions.
+They each carry the attributes that are necessary to match an ID of their type.
+
+
+.. autoclass:: CertificatePattern
+
+   It includes all of those that follow now.
+
+.. autoclass:: DNSPattern
+   :members:
+.. autoclass:: IPAddressPattern
+   :members:
+.. autoclass:: URIPattern
+   :members:
+.. autoclass:: SRVPattern
+   :members:
 
 
 Universal Errors and Warnings
 =============================
 
 .. currentmodule:: service_identity
```

### Comparing `service-identity-21.1.0/docs/conf.py` & `service_identity-23.1.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,8 @@
-# -*- coding: utf-8 -*-
-#
-# service-identity documentation build configuration file, created by
-# sphinx-quickstart on Mon Jun  2 16:32:11 2014.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-import codecs
-import datetime
-import os
-import re
-
-
-def read(*parts):
-    """
-    Build an absolute path from *parts* and and return the contents of the
-    resulting file.  Assume UTF-8 encoding.
-    """
-    here = os.path.abspath(os.path.dirname(__file__))
-    with codecs.open(os.path.join(here, *parts), "rb", "utf-8") as f:
-        return f.read()
-
-
-def find_version(*file_paths):
-    """
-    Build a path from *file_paths* and search for a ``__version__``
-    string inside.
-    """
-    version_file = read(*file_paths)
-    version_match = re.search(
-        r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M
-    )
-    if version_match:
-        return version_match.group(1)
-    raise RuntimeError("Unable to find version string.")
+from importlib import metadata
 
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.insert(0, os.path.abspath('.'))
 
@@ -55,16 +14,32 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.doctest",
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
-    "sphinx.ext.todo",
-    "sphinx.ext.coverage",
+    "myst_parser",
+    "notfound.extension",
+]
+
+myst_enable_extensions = [
+    "colon_fence",
+    "smartquotes",
+    "deflist",
+]
+
+# Move type hints into the description block, instead of the func definition.
+autodoc_typehints = "description"
+autodoc_typehints_description_target = "documented"
+
+# GitHub has rate limits
+linkcheck_ignore = [
+    r"https://github.com/.*/(issues|pull|compare)/\d+",
+    r"https://twitter.com/.*",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
 source_suffix = ".rst"
@@ -72,24 +47,25 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"service-identity"
-year = datetime.date.today().year
-copyright = u"2014, Hynek Schlawack"
+project = "service-identity"
+year = 2014
+copyright = "2014, Hynek Schlawack"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
-#
-release = find_version("..", "src", "service_identity", "__init__.py")
-version = release.rsplit(u".", 1)[0]
+
+release = metadata.version("service-identity")
+# The short X.Y version.
+version = release.rsplit(".", 1)[0]
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -219,16 +195,16 @@
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
     (
         "index",
         "service-identity.tex",
-        u"service\\_identity Documentation",
-        u"Hynek Schlawack",
+        "service\\_identity Documentation",
+        "Hynek Schlawack",
         "manual",
     )
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
@@ -254,16 +230,16 @@
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     (
         "index",
         "service-identity",
-        u"service-identity Documentation",
-        [u"Hynek Schlawack"],
+        "service-identity Documentation",
+        ["Hynek Schlawack"],
         1,
     )
 ]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
@@ -273,16 +249,16 @@
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         "index",
         "service-identity",
-        u"service-identity Documentation",
-        u"Hynek Schlawack",
+        "service-identity Documentation",
+        "Hynek Schlawack",
         "service-identity",
         "Service Identity Verification for pyOpenSSL",
         "Miscellaneous",
     )
 ]
 
 # Documents to append as an appendix to all manuals.
@@ -294,13 +270,12 @@
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 # texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 
-# Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    "https://docs.python.org/3/": None,
-    "https://pyopenssl.readthedocs.io/en/stable": None,
-    "https://cryptography.io/en/stable/": None,
+    "python": ("https://docs.python.org/3", None),
+    "pyopenssl": ("https://www.pyopenssl.org/en/stable/", None),
+    "cryptography": ("https://cryptography.io/en/stable/", None),
 }
```

### Comparing `service-identity-21.1.0/docs/installation.rst` & `service_identity-23.1.0/docs/installation.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-=============================
-Installation and Requirements
-=============================
+# Installation and Requirements
 
+## Installation
 
-Installation
-============
+```console
+$ python -Im pip install service-identity
+```
 
-``$ pip install service-identity``
 
+## Requirements
 
-Requirements
-============
+*service-identity* depends on the [cryptography] package.
+In addition to the latest release, we're also testing against the following oldest version constraint:
 
-Python 2.7, 3.5 and later, as well as PyPy are supported.
+```{include} ../tests/constraints/oldest-cryptography.txt
+:literal: true
+```
 
-Additionally, the following PyPI packages are required:
+If you want to use the [pyOpenSSL] functionality, you have to install it yourself.
+In addition to the latest release, we are also testing against the following oldest version constraints
+(you have to add the *cryptography* pin yourself, if you want to use an old version of pyOpenSSL):
 
-- attrs_
-- pyOpenSSL_ ``>= 0.14`` (``0.12`` and ``0.13`` may work but are not part of CI anymore)
-- pyasn1_
-- pyasn1-modules_
-- ipaddress_ on Python 2.7
+```{include} ../tests/constraints/oldest-pyopenssl.txt
+:literal: true
+```
 
-Optionally, idna_ ``>= 0.6`` can be used for `internationalized domain names`_ (IDN), i.e. non-ASCII domains.
-Unfortunately it’s required because Python’s IDN support in the standard library is outdated_ even in the latest releases.
 
-If you need Python 3.2 support, you will have to use the latest 0.2.x release.
-If you need Python 2.6 or 3.3 support, you will have to use the latest 14.0.x release.
-They will receive bug fix releases if necessary but other than that no further development is planned.
+### International Domain Names
 
-.. _attrs: https://www.attrs.org/
-.. _pyOpenSSL: https://pypi.org/project/pyOpenSSL/
-.. _pyasn1-modules: https://pypi.org/project/pyasn1-modules/
-.. _pyasn1: https://pypi.org/project/pyasn1/
-.. _`internationalized domain names`: https://en.wikipedia.org/wiki/Internationalized_domain_name
-.. _idna: https://pypi.org/project/idna/
-.. _outdated: https://bugs.python.org/issue17305
-.. _ipaddress: https://pypi.org/project/ipaddress/
+Optionally, the `idna` extra dependency can be used for [internationalized domain names] (IDN), i.e. non-ASCII domains:
+
+```console
+$ python -Im pip install service-identity[idna]
+```
+
+Unfortunately it's required because Python's IDN support in the standard library is [outdated] even in the latest releases.
+
+[cryptography]: https://cryptography.io/
+[idna]: https://pypi.org/project/idna/
+[internationalized domain names]: https://en.wikipedia.org/wiki/Internationalized_domain_name
+[outdated]: https://github.com/python/cpython/issues/61507
+[pyopenssl]: https://pypi.org/project/pyOpenSSL/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `service-identity-21.1.0/src/service_identity/_common.py` & `service_identity-23.1.0/src/service_identity/hazmat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 """
 Common verification code.
 """
 
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import ipaddress
 import re
 
+from typing import Protocol, Sequence, Union, runtime_checkable
+
 import attr
 
-from ._compat import maketrans, text_type
 from .exceptions import (
     CertificateError,
     DNSMismatch,
     IPAddressMismatch,
+    Mismatch,
     SRVMismatch,
     URIMismatch,
     VerificationError,
 )
 
 
 try:
     import idna
-except ImportError:  # pragma: nocover
-    idna = None
+except ImportError:
+    idna = None  # type: ignore[assignment]
 
 
 @attr.s(slots=True)
-class ServiceMatch(object):
+class ServiceMatch:
     """
     A match of a service id and a certificate pattern.
     """
 
-    service_id = attr.ib()
-    cert_pattern = attr.ib()
+    service_id: ServiceID = attr.ib()
+    cert_pattern: CertificatePattern = attr.ib()
 
 
-def verify_service_identity(cert_patterns, obligatory_ids, optional_ids):
+def verify_service_identity(
+    cert_patterns: Sequence[CertificatePattern],
+    obligatory_ids: Sequence[ServiceID],
+    optional_ids: Sequence[ServiceID],
+) -> list[ServiceMatch]:
     """
     Verify whether *cert_patterns* are valid for *obligatory_ids* and
     *optional_ids*.
 
     *obligatory_ids* must be both present and match.  *optional_ids* must match
     if a pattern of the respective type is present.
     """
@@ -66,56 +72,43 @@
 
     if errors:
         raise VerificationError(errors=errors)
 
     return matches
 
 
-def _find_matches(cert_patterns, service_ids):
+def _find_matches(
+    cert_patterns: Sequence[CertificatePattern],
+    service_ids: Sequence[ServiceID],
+) -> list[ServiceMatch]:
     """
     Search for matching certificate patterns and service_ids.
 
-    :param cert_ids: List certificate IDs like DNSPattern.
-    :type cert_ids: `list`
-
     :param service_ids: List of service IDs like DNS_ID.
     :type service_ids: `list`
-
-    :rtype: `list` of `ServiceMatch`
     """
     matches = []
     for sid in service_ids:
         for cid in cert_patterns:
             if sid.verify(cid):
                 matches.append(ServiceMatch(cert_pattern=cid, service_id=sid))
     return matches
 
 
-def _contains_instance_of(seq, cl):
-    """
-    :type seq: iterable
-    :type cl: type
+def _contains_instance_of(seq: Sequence[object], cl: type) -> bool:
+    return any(isinstance(e, cl) for e in seq)
 
-    :rtype: bool
-    """
-    for e in seq:
-        if isinstance(e, cl):
-            return True
-    return False
 
-
-def _is_ip_address(pattern):
+def _is_ip_address(pattern: str | bytes) -> bool:
     """
     Check whether *pattern* could be/match an IP address.
 
     :param pattern: A pattern for a host name.
-    :type pattern: `bytes` or `unicode`
 
     :return: `True` if *pattern* could be an IP address, else `False`.
-    :rtype: bool
     """
     if isinstance(pattern, bytes):
         try:
             pattern = pattern.decode("ascii")
         except UnicodeError:
             return False
 
@@ -129,141 +122,164 @@
         ipaddress.ip_address(pattern.replace("*", "1"))
     except ValueError:
         return False
 
     return True
 
 
-@attr.s(init=False, slots=True)
-class DNSPattern(object):
+@attr.s(slots=True)
+class DNSPattern:
     """
     A DNS pattern as extracted from certificates.
     """
 
-    pattern = attr.ib()
+    #: The pattern.
+    pattern: bytes = attr.ib()
 
-    _RE_LEGAL_CHARS = re.compile(br"^[a-z0-9\-_.]+$")
+    _RE_LEGAL_CHARS = re.compile(rb"^[a-z0-9\-_.]+$")
 
-    def __init__(self, pattern):
-        """
-        :type pattern: `bytes`
-        """
+    @classmethod
+    def from_bytes(cls, pattern: bytes) -> DNSPattern:
         if not isinstance(pattern, bytes):
             raise TypeError("The DNS pattern must be a bytes string.")
 
         pattern = pattern.strip()
 
         if pattern == b"" or _is_ip_address(pattern) or b"\0" in pattern:
-            raise CertificateError(
-                "Invalid DNS pattern {0!r}.".format(pattern)
-            )
+            raise CertificateError(f"Invalid DNS pattern {pattern!r}.")
 
-        self.pattern = pattern.translate(_TRANS_TO_LOWER)
-        if b"*" in self.pattern:
-            _validate_pattern(self.pattern)
+        pattern = pattern.translate(_TRANS_TO_LOWER)
+        if b"*" in pattern:
+            _validate_pattern(pattern)
+
+        return cls(pattern=pattern)
 
 
 @attr.s(slots=True)
-class IPAddressPattern(object):
+class IPAddressPattern:
     """
     An IP address pattern as extracted from certificates.
     """
 
-    pattern = attr.ib()
+    #: The pattern.
+    pattern: ipaddress.IPv4Address | ipaddress.IPv6Address = attr.ib()
 
     @classmethod
-    def from_bytes(cls, bs):
+    def from_bytes(cls, bs: bytes) -> IPAddressPattern:
         try:
             return cls(pattern=ipaddress.ip_address(bs))
         except ValueError:
             raise CertificateError(
-                "Invalid IP address pattern {!r}.".format(bs)
-            )
+                f"Invalid IP address pattern {bs!r}."
+            ) from None
 
 
-@attr.s(init=False, slots=True)
-class URIPattern(object):
+@attr.s(slots=True)
+class URIPattern:
     """
     An URI pattern as extracted from certificates.
     """
 
-    protocol_pattern = attr.ib()
-    dns_pattern = attr.ib()
+    #: The pattern for the protocol part.
+    protocol_pattern: bytes = attr.ib()
+    #: The pattern for the DNS part.
+    dns_pattern: DNSPattern = attr.ib()
 
-    def __init__(self, pattern):
-        """
-        :type pattern: `bytes`
-        """
+    @classmethod
+    def from_bytes(cls, pattern: bytes) -> URIPattern:
         if not isinstance(pattern, bytes):
             raise TypeError("The URI pattern must be a bytes string.")
 
         pattern = pattern.strip().translate(_TRANS_TO_LOWER)
 
         if b":" not in pattern or b"*" in pattern or _is_ip_address(pattern):
-            raise CertificateError(
-                "Invalid URI pattern {0!r}.".format(pattern)
-            )
-        self.protocol_pattern, hostname = pattern.split(b":")
-        self.dns_pattern = DNSPattern(hostname)
+            raise CertificateError(f"Invalid URI pattern {pattern!r}.")
 
+        protocol_pattern, hostname = pattern.split(b":")
 
-@attr.s(init=False, slots=True)
-class SRVPattern(object):
+        return cls(
+            protocol_pattern=protocol_pattern,
+            dns_pattern=DNSPattern.from_bytes(hostname),
+        )
+
+
+@attr.s(slots=True)
+class SRVPattern:
     """
     An SRV pattern as extracted from certificates.
     """
 
-    name_pattern = attr.ib()
-    dns_pattern = attr.ib()
+    #: The pattern for the name part.
+    name_pattern: bytes = attr.ib()
+    #: The pattern for the DNS part.
+    dns_pattern: DNSPattern = attr.ib()
 
-    def __init__(self, pattern):
-        """
-        :type pattern: `bytes`
-        """
+    @classmethod
+    def from_bytes(cls, pattern: bytes) -> SRVPattern:
         if not isinstance(pattern, bytes):
             raise TypeError("The SRV pattern must be a bytes string.")
 
         pattern = pattern.strip().translate(_TRANS_TO_LOWER)
 
         if (
             pattern[0] != b"_"[0]
             or b"." not in pattern
             or b"*" in pattern
             or _is_ip_address(pattern)
         ):
-            raise CertificateError(
-                "Invalid SRV pattern {0!r}.".format(pattern)
-            )
+            raise CertificateError(f"Invalid SRV pattern {pattern!r}.")
+
         name, hostname = pattern.split(b".", 1)
-        self.name_pattern = name[1:]
-        self.dns_pattern = DNSPattern(hostname)
+        return cls(
+            name_pattern=name[1:], dns_pattern=DNSPattern.from_bytes(hostname)
+        )
+
+
+CertificatePattern = Union[
+    SRVPattern, URIPattern, DNSPattern, IPAddressPattern
+]
+"""
+A :class:`Union` of all possible patterns that can be extracted from a
+certificate.
+"""
+
+
+@runtime_checkable
+class ServiceID(Protocol):
+    @property
+    def pattern_class(self) -> type[CertificatePattern]:
+        ...
+
+    @property
+    def error_on_mismatch(self) -> type[Mismatch]:
+        ...
+
+    def verify(self, pattern: CertificatePattern) -> bool:
+        ...
 
 
 @attr.s(init=False, slots=True)
-class DNS_ID(object):
+class DNS_ID:
     """
     A DNS service ID, aka hostname.
     """
 
-    hostname = attr.ib()
+    hostname: bytes = attr.ib()
 
     # characters that are legal in a normalized hostname
-    _RE_LEGAL_CHARS = re.compile(br"^[a-z0-9\-_.]+$")
+    _RE_LEGAL_CHARS = re.compile(rb"^[a-z0-9\-_.]+$")
     pattern_class = DNSPattern
     error_on_mismatch = DNSMismatch
 
-    def __init__(self, hostname):
-        """
-        :type hostname: `unicode`
-        """
-        if not isinstance(hostname, text_type):
-            raise TypeError("DNS-ID must be a unicode string.")
+    def __init__(self, hostname: str):
+        if not isinstance(hostname, str):
+            raise TypeError("DNS-ID must be a text string.")
 
         hostname = hostname.strip()
-        if hostname == u"" or _is_ip_address(hostname):
+        if not hostname or _is_ip_address(hostname):
             raise ValueError("Invalid DNS-ID.")
 
         if any(ord(c) > 127 for c in hostname):
             if idna:
                 ascii_id = idna.encode(hostname)
             else:
                 raise ImportError(
@@ -272,178 +288,169 @@
         else:
             ascii_id = hostname.encode("ascii")
 
         self.hostname = ascii_id.translate(_TRANS_TO_LOWER)
         if self._RE_LEGAL_CHARS.match(self.hostname) is None:
             raise ValueError("Invalid DNS-ID.")
 
-    def verify(self, pattern):
+    def verify(self, pattern: CertificatePattern) -> bool:
         """
         https://tools.ietf.org/search/rfc6125#section-6.4
         """
         if isinstance(pattern, self.pattern_class):
             return _hostname_matches(pattern.pattern, self.hostname)
-        else:
-            return False
+
+        return False
 
 
 @attr.s(slots=True)
-class IPAddress_ID(object):
+class IPAddress_ID:
     """
     An IP address service ID.
     """
 
-    ip = attr.ib(converter=ipaddress.ip_address)
+    ip: ipaddress.IPv4Address | ipaddress.IPv6Address = attr.ib(
+        converter=ipaddress.ip_address
+    )
 
     pattern_class = IPAddressPattern
     error_on_mismatch = IPAddressMismatch
 
-    def verify(self, pattern):
+    def verify(self, pattern: CertificatePattern) -> bool:
         """
         https://tools.ietf.org/search/rfc2818#section-3.1
         """
-        return self.ip == pattern.pattern
+        if isinstance(pattern, self.pattern_class):
+            return self.ip == pattern.pattern
+
+        return False
 
 
 @attr.s(init=False, slots=True)
-class URI_ID(object):
+class URI_ID:
     """
     An URI service ID.
     """
 
-    protocol = attr.ib()
-    dns_id = attr.ib()
+    protocol: bytes = attr.ib()
+    dns_id: DNS_ID = attr.ib()
 
     pattern_class = URIPattern
     error_on_mismatch = URIMismatch
 
-    def __init__(self, uri):
-        """
-        :type uri: `unicode`
-        """
-        if not isinstance(uri, text_type):
-            raise TypeError("URI-ID must be a unicode string.")
+    def __init__(self, uri: str):
+        if not isinstance(uri, str):
+            raise TypeError("URI-ID must be a text string.")
 
         uri = uri.strip()
-        if u":" not in uri or _is_ip_address(uri):
+        if ":" not in uri or _is_ip_address(uri):
             raise ValueError("Invalid URI-ID.")
 
-        prot, hostname = uri.split(u":")
+        prot, hostname = uri.split(":")
 
         self.protocol = prot.encode("ascii").translate(_TRANS_TO_LOWER)
-        self.dns_id = DNS_ID(hostname.strip(u"/"))
+        self.dns_id = DNS_ID(hostname.strip("/"))
 
-    def verify(self, pattern):
+    def verify(self, pattern: CertificatePattern) -> bool:
         """
         https://tools.ietf.org/search/rfc6125#section-6.5.2
         """
         if isinstance(pattern, self.pattern_class):
             return (
                 pattern.protocol_pattern == self.protocol
                 and self.dns_id.verify(pattern.dns_pattern)
             )
-        else:
-            return False
+
+        return False
 
 
 @attr.s(init=False, slots=True)
-class SRV_ID(object):
+class SRV_ID:
     """
     An SRV service ID.
     """
 
-    name = attr.ib()
-    dns_id = attr.ib()
+    name: bytes = attr.ib()
+    dns_id: DNS_ID = attr.ib()
 
     pattern_class = SRVPattern
     error_on_mismatch = SRVMismatch
 
-    def __init__(self, srv):
-        """
-        :type srv: `unicode`
-        """
-        if not isinstance(srv, text_type):
-            raise TypeError("SRV-ID must be a unicode string.")
+    def __init__(self, srv: str):
+        if not isinstance(srv, str):
+            raise TypeError("SRV-ID must be a text string.")
 
         srv = srv.strip()
-        if u"." not in srv or _is_ip_address(srv) or srv[0] != u"_":
+        if "." not in srv or _is_ip_address(srv) or srv[0] != "_":
             raise ValueError("Invalid SRV-ID.")
 
-        name, hostname = srv.split(u".", 1)
+        name, hostname = srv.split(".", 1)
 
         self.name = name[1:].encode("ascii").translate(_TRANS_TO_LOWER)
         self.dns_id = DNS_ID(hostname)
 
-    def verify(self, pattern):
+    def verify(self, pattern: CertificatePattern) -> bool:
         """
         https://tools.ietf.org/search/rfc6125#section-6.5.1
         """
         if isinstance(pattern, self.pattern_class):
             return self.name == pattern.name_pattern and self.dns_id.verify(
                 pattern.dns_pattern
             )
-        else:
-            return False
 
+        return False
 
-def _hostname_matches(cert_pattern, actual_hostname):
-    """
-    :type cert_pattern: `bytes`
-    :type actual_hostname: `bytes`
 
+def _hostname_matches(cert_pattern: bytes, actual_hostname: bytes) -> bool:
+    """
     :return: `True` if *cert_pattern* matches *actual_hostname*, else `False`.
-    :rtype: `bool`
     """
     if b"*" in cert_pattern:
         cert_head, cert_tail = cert_pattern.split(b".", 1)
         actual_head, actual_tail = actual_hostname.split(b".", 1)
         if cert_tail != actual_tail:
             return False
         # No patterns for IDNA
         if actual_head.startswith(b"xn--"):
             return False
 
         return cert_head == b"*" or cert_head == actual_head
-    else:
-        return cert_pattern == actual_hostname
+
+    return cert_pattern == actual_hostname
 
 
-def _validate_pattern(cert_pattern):
+def _validate_pattern(cert_pattern: bytes) -> None:
     """
     Check whether the usage of wildcards within *cert_pattern* conforms with
     our expectations.
-
-    :type hostname: `bytes`
-
-    :return: None
     """
     cnt = cert_pattern.count(b"*")
     if cnt > 1:
         raise CertificateError(
-            "Certificate's DNS-ID {0!r} contains too many wildcards.".format(
+            "Certificate's DNS-ID {!r} contains too many wildcards.".format(
                 cert_pattern
             )
         )
     parts = cert_pattern.split(b".")
     if len(parts) < 3:
         raise CertificateError(
-            "Certificate's DNS-ID {0!r} has too few host components for "
+            "Certificate's DNS-ID {!r} has too few host components for "
             "wildcard usage.".format(cert_pattern)
         )
     # We assume there will always be only one wildcard allowed.
     if b"*" not in parts[0]:
         raise CertificateError(
-            "Certificate's DNS-ID {0!r} has a wildcard outside the left-most "
+            "Certificate's DNS-ID {!r} has a wildcard outside the left-most "
             "part.".format(cert_pattern)
         )
     if any(not len(p) for p in parts):
         raise CertificateError(
-            "Certificate's DNS-ID {0!r} contains empty parts.".format(
+            "Certificate's DNS-ID {!r} contains empty parts.".format(
                 cert_pattern
             )
         )
 
 
 # Ensure no locale magic interferes.
-_TRANS_TO_LOWER = maketrans(
+_TRANS_TO_LOWER = bytes.maketrans(
     b"ABCDEFGHIJKLMNOPQRSTUVWXYZ", b"abcdefghijklmnopqrstuvwxyz"
 )
```

### Comparing `service-identity-21.1.0/src/service_identity/cryptography.py` & `service_identity-23.1.0/src/service_identity/cryptography.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,131 +1,134 @@
 """
 `cryptography.x509 <https://github.com/pyca/cryptography>`_-specific code.
 """
 
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import warnings
 
+from typing import Sequence
+
 from cryptography.x509 import (
+    Certificate,
     DNSName,
     ExtensionOID,
     IPAddress,
-    NameOID,
     ObjectIdentifier,
     OtherName,
     UniformResourceIdentifier,
 )
 from cryptography.x509.extensions import ExtensionNotFound
 from pyasn1.codec.der.decoder import decode
 from pyasn1.type.char import IA5String
 
-from ._common import (
+from .exceptions import CertificateError
+from .hazmat import (
     DNS_ID,
-    CertificateError,
+    CertificatePattern,
     DNSPattern,
     IPAddress_ID,
     IPAddressPattern,
     SRVPattern,
     URIPattern,
     verify_service_identity,
 )
-from .exceptions import SubjectAltNameWarning
 
 
 __all__ = ["verify_certificate_hostname"]
 
 
-def verify_certificate_hostname(certificate, hostname):
+def verify_certificate_hostname(
+    certificate: Certificate, hostname: str
+) -> None:
     """
     Verify whether *certificate* is valid for *hostname*.
 
     .. note:: Nothing is verified about the *authority* of the certificate;
        the caller must verify that the certificate chains to an appropriate
        trust root themselves.
 
-    :param cryptography.x509.Certificate certificate: A cryptography X509
-        certificate object.
-    :param unicode hostname: The hostname that *certificate* should be valid
-        for.
+    :param certificate: A *cryptography* X509 certificate object.
+    :param hostname: The hostname that *certificate* should be valid for.
 
     :raises service_identity.VerificationError: If *certificate* is not valid
         for *hostname*.
     :raises service_identity.CertificateError: If *certificate* contains
-        invalid/unexpected data.
+        invalid / unexpected data.
 
     :returns: ``None``
     """
     verify_service_identity(
-        cert_patterns=extract_ids(certificate),
+        cert_patterns=extract_patterns(certificate),
         obligatory_ids=[DNS_ID(hostname)],
         optional_ids=[],
     )
 
 
-def verify_certificate_ip_address(certificate, ip_address):
+def verify_certificate_ip_address(
+    certificate: Certificate, ip_address: str
+) -> None:
     """
     Verify whether *certificate* is valid for *ip_address*.
 
     .. note:: Nothing is verified about the *authority* of the certificate;
        the caller must verify that the certificate chains to an appropriate
        trust root themselves.
 
-    :param cryptography.x509.Certificate certificate: A cryptography X509
-        certificate object.
-    :param unicode ip_address: The IP address that *connection* should be valid
+    :param certificate: A *cryptography* X509 certificate object.
+    :param ip_address: The IP address that *connection* should be valid
         for.  Can be an IPv4 or IPv6 address.
 
     :raises service_identity.VerificationError: If *certificate* is not valid
         for *ip_address*.
     :raises service_identity.CertificateError: If *certificate* contains
-        invalid/unexpected data.
+        invalid / unexpected data.
 
     :returns: ``None``
 
     .. versionadded:: 18.1.0
     """
     verify_service_identity(
-        cert_patterns=extract_ids(certificate),
+        cert_patterns=extract_patterns(certificate),
         obligatory_ids=[IPAddress_ID(ip_address)],
         optional_ids=[],
     )
 
 
 ID_ON_DNS_SRV = ObjectIdentifier("1.3.6.1.5.5.7.8.7")  # id_on_dnsSRV
 
 
-def extract_ids(cert):
+def extract_patterns(cert: Certificate) -> Sequence[CertificatePattern]:
     """
-    Extract all valid IDs from a certificate for service verification.
-
-    If *cert* doesn't contain any identifiers, the ``CN``s are used as DNS-IDs
-    as fallback.
+    Extract all valid ID patterns from a certificate for service verification.
 
-    :param cryptography.x509.Certificate cert: The certificate to be dissected.
+    :param cert: The certificate to be dissected.
 
     :return: List of IDs.
+
+    .. versionchanged:: 23.1.0
+       ``commonName`` is not used as a fallback anymore.
     """
-    ids = []
+    ids: list[CertificatePattern] = []
     try:
         ext = cert.extensions.get_extension_for_oid(
             ExtensionOID.SUBJECT_ALTERNATIVE_NAME
         )
     except ExtensionNotFound:
         pass
     else:
         ids.extend(
             [
-                DNSPattern(name.encode("utf-8"))
+                DNSPattern.from_bytes(name.encode("utf-8"))
                 for name in ext.value.get_values_for_type(DNSName)
             ]
         )
         ids.extend(
             [
-                URIPattern(uri.encode("utf-8"))
+                URIPattern.from_bytes(uri.encode("utf-8"))
                 for uri in ext.value.get_values_for_type(
                     UniformResourceIdentifier
                 )
             ]
         )
         ids.extend(
             [
@@ -133,29 +136,26 @@
                 for ip in ext.value.get_values_for_type(IPAddress)
             ]
         )
         for other in ext.value.get_values_for_type(OtherName):
             if other.type_id == ID_ON_DNS_SRV:
                 srv, _ = decode(other.value)
                 if isinstance(srv, IA5String):
-                    ids.append(SRVPattern(srv.asOctets()))
-                else:  # pragma: nocover
+                    ids.append(SRVPattern.from_bytes(srv.asOctets()))
+                else:  # pragma: no cover
                     raise CertificateError("Unexpected certificate content.")
 
-    if not ids:
-        # https://tools.ietf.org/search/rfc6125#section-6.4.4
-        # A client MUST NOT seek a match for a reference identifier of CN-ID if
-        # the presented identifiers include a DNS-ID, SRV-ID, URI-ID, or any
-        # application-specific identifier types supported by the client.
-        cns = [
-            n.value
-            for n in cert.subject.get_attributes_for_oid(NameOID.COMMON_NAME)
-        ]
-        cn = next(iter(cns), b"<not given>")
-        ids = [DNSPattern(n.encode("utf-8")) for n in cns]
-        warnings.warn(
-            "Certificate with CN {!r} has no `subjectAltName`, falling back "
-            "to check for a `commonName` for now.  This feature is being "
-            "removed by major browsers and deprecated by RFC 2818.".format(cn),
-            SubjectAltNameWarning,
-        )
     return ids
+
+
+def extract_ids(cert: Certificate) -> Sequence[CertificatePattern]:
+    """
+    Deprecated and never public API.  Use :func:`extract_patterns` instead.
+
+    .. deprecated:: 23.1.0
+    """
+    warnings.warn(
+        category=DeprecationWarning,
+        message="`extract_ids()` is deprecated, please use `extract_patterns()`.",
+        stacklevel=2,
+    )
+    return extract_patterns(cert)
```

### Comparing `service-identity-21.1.0/src/service_identity/pyopenssl.py` & `service_identity-23.1.0/src/service_identity/pyopenssl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,146 +1,155 @@
 """
 `pyOpenSSL <https://github.com/pyca/pyopenssl>`_-specific code.
 """
 
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
+import contextlib
 import warnings
 
-import six
+from typing import Sequence
 
 from pyasn1.codec.der.decoder import decode
 from pyasn1.type.char import IA5String
 from pyasn1.type.univ import ObjectIdentifier
 from pyasn1_modules.rfc2459 import GeneralNames
 
-from ._common import (
+from .exceptions import CertificateError
+from .hazmat import (
     DNS_ID,
-    CertificateError,
+    CertificatePattern,
     DNSPattern,
     IPAddress_ID,
     IPAddressPattern,
     SRVPattern,
     URIPattern,
     verify_service_identity,
 )
-from .exceptions import SubjectAltNameWarning
+
+
+with contextlib.suppress(ImportError):
+    # We only use it for docstrings -- `if TYPE_CHECKING`` does not work.
+    from OpenSSL.crypto import X509
+    from OpenSSL.SSL import Connection
 
 
 __all__ = ["verify_hostname"]
 
 
-def verify_hostname(connection, hostname):
+def verify_hostname(connection: Connection, hostname: str) -> None:
     """
     Verify whether the certificate of *connection* is valid for *hostname*.
 
-    :param OpenSSL.SSL.Connection connection: A pyOpenSSL connection object.
-    :param unicode hostname: The hostname that *connection* should be connected
-        to.
+    :param connection: A pyOpenSSL connection object.
+    :param hostname: The hostname that *connection* should be connected to.
 
     :raises service_identity.VerificationError: If *connection* does not
         provide a certificate that is valid for *hostname*.
     :raises service_identity.CertificateError: If the certificate chain of
         *connection* contains a certificate that contains invalid/unexpected
         data.
 
     :returns: ``None``
     """
     verify_service_identity(
-        cert_patterns=extract_ids(connection.get_peer_certificate()),
+        cert_patterns=extract_patterns(
+            connection.get_peer_certificate()  # type:ignore[arg-type]
+        ),
         obligatory_ids=[DNS_ID(hostname)],
         optional_ids=[],
     )
 
 
-def verify_ip_address(connection, ip_address):
+def verify_ip_address(connection: Connection, ip_address: str) -> None:
     """
     Verify whether the certificate of *connection* is valid for *ip_address*.
 
-    :param OpenSSL.SSL.Connection connection: A pyOpenSSL connection object.
-    :param unicode ip_address: The IP address that *connection* should be
-        connected to.  Can be an IPv4 or IPv6 address.
+    :param connection: A pyOpenSSL connection object.
+    :param ip_address: The IP address that *connection* should be connected to.
+        Can be an IPv4 or IPv6 address.
 
     :raises service_identity.VerificationError: If *connection* does not
         provide a certificate that is valid for *ip_address*.
     :raises service_identity.CertificateError: If the certificate chain of
         *connection* contains a certificate that contains invalid/unexpected
         data.
 
     :returns: ``None``
 
     .. versionadded:: 18.1.0
     """
     verify_service_identity(
-        cert_patterns=extract_ids(connection.get_peer_certificate()),
+        cert_patterns=extract_patterns(
+            connection.get_peer_certificate()  # type:ignore[arg-type]
+        ),
         obligatory_ids=[IPAddress_ID(ip_address)],
         optional_ids=[],
     )
 
 
 ID_ON_DNS_SRV = ObjectIdentifier("1.3.6.1.5.5.7.8.7")  # id_on_dnsSRV
 
 
-def extract_ids(cert):
+def extract_patterns(cert: X509) -> Sequence[CertificatePattern]:
     """
-    Extract all valid IDs from a certificate for service verification.
+    Extract all valid ID patterns from a certificate for service verification.
 
-    If *cert* doesn't contain any identifiers, the ``CN``s are used as DNS-IDs
-    as fallback.
-
-    :param OpenSSL.SSL.X509 cert: The certificate to be dissected.
+    :param cert: The certificate to be dissected.
 
     :return: List of IDs.
+
+    .. versionchanged:: 23.1.0
+       ``commonName`` is not used as a fallback anymore.
     """
-    ids = []
-    for i in six.moves.range(cert.get_extension_count()):
+    ids: list[CertificatePattern] = []
+    for i in range(cert.get_extension_count()):
         ext = cert.get_extension(i)
         if ext.get_short_name() == b"subjectAltName":
             names, _ = decode(ext.get_data(), asn1Spec=GeneralNames())
             for n in names:
                 name_string = n.getName()
                 if name_string == "dNSName":
-                    ids.append(DNSPattern(n.getComponent().asOctets()))
+                    ids.append(
+                        DNSPattern.from_bytes(n.getComponent().asOctets())
+                    )
                 elif name_string == "iPAddress":
                     ids.append(
                         IPAddressPattern.from_bytes(
                             n.getComponent().asOctets()
                         )
                     )
                 elif name_string == "uniformResourceIdentifier":
-                    ids.append(URIPattern(n.getComponent().asOctets()))
+                    ids.append(
+                        URIPattern.from_bytes(n.getComponent().asOctets())
+                    )
                 elif name_string == "otherName":
                     comp = n.getComponent()
                     oid = comp.getComponentByPosition(0)
                     if oid == ID_ON_DNS_SRV:
                         srv, _ = decode(comp.getComponentByPosition(1))
                         if isinstance(srv, IA5String):
-                            ids.append(SRVPattern(srv.asOctets()))
-                        else:  # pragma: nocover
+                            ids.append(SRVPattern.from_bytes(srv.asOctets()))
+                        else:  # pragma: no cover
                             raise CertificateError(
                                 "Unexpected certificate content."
                             )
-                    else:  # pragma: nocover
+                    else:  # pragma: no cover
                         pass
-                else:  # pragma: nocover
+                else:  # pragma: no cover
                     pass
 
-    if not ids:
-        # https://tools.ietf.org/search/rfc6125#section-6.4.4
-        # A client MUST NOT seek a match for a reference identifier of CN-ID if
-        # the presented identifiers include a DNS-ID, SRV-ID, URI-ID, or any
-        # application-specific identifier types supported by the client.
-        components = [
-            c[1] for c in cert.get_subject().get_components() if c[0] == b"CN"
-        ]
-        cn = next(iter(components), b"<not given>")
-        ids = [DNSPattern(c) for c in components]
-        warnings.warn(
-            "Certificate with CN '%s' has no `subjectAltName`, falling back "
-            "to check for a `commonName` for now.  This feature is being "
-            "removed by major browsers and deprecated by RFC 2818.  "
-            "service-identity will remove the support for it in mid-2018."
-            % (cn.decode("utf-8"),),
-            SubjectAltNameWarning,
-            stacklevel=2,
-        )
     return ids
+
+
+def extract_ids(cert: X509) -> Sequence[CertificatePattern]:
+    """
+    Deprecated and never public API.  Use :func:`extract_patterns` instead.
+
+    .. deprecated:: 23.1.0
+    """
+    warnings.warn(
+        category=DeprecationWarning,
+        message="`extract_ids()` is deprecated, please use `extract_patterns()`.",
+        stacklevel=2,
+    )
+    return extract_patterns(cert)
```

### Comparing `service-identity-21.1.0/tests/test_common.py` & `service_identity-23.1.0/tests/test_hazmat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from __future__ import absolute_import, division, print_function
-
 import ipaddress
 import pickle
 
 import pytest
-import six
 
-import service_identity._common
+import service_identity.hazmat
 
-from service_identity._common import (
+from service_identity.cryptography import extract_patterns
+from service_identity.exceptions import (
+    CertificateError,
+    DNSMismatch,
+    SRVMismatch,
+    VerificationError,
+)
+from service_identity.hazmat import (
     DNS_ID,
     SRV_ID,
     URI_ID,
     DNSPattern,
     IPAddress_ID,
     IPAddressPattern,
     ServiceMatch,
@@ -21,236 +25,235 @@
     _contains_instance_of,
     _find_matches,
     _hostname_matches,
     _is_ip_address,
     _validate_pattern,
     verify_service_identity,
 )
-from service_identity.cryptography import extract_ids
-from service_identity.exceptions import (
-    CertificateError,
-    DNSMismatch,
-    SRVMismatch,
-    VerificationError,
-)
 
 from .test_cryptography import CERT_EVERYTHING
 from .util import DNS_IDS
 
 
 try:
     import idna
 except ImportError:
     idna = None
 
 
-class TestVerifyServiceIdentity(object):
+class TestVerifyServiceIdentity:
     """
     Simple integration tests for verify_service_identity.
     """
 
     def test_dns_id_success(self):
         """
         Return pairs of certificate ids and service ids on matches.
         """
         rv = verify_service_identity(
-            DNS_IDS, [DNS_ID(u"twistedmatrix.com")], []
+            DNS_IDS, [DNS_ID("twistedmatrix.com")], []
         )
         assert [
             ServiceMatch(
-                cert_pattern=DNSPattern(b"twistedmatrix.com"),
-                service_id=DNS_ID(u"twistedmatrix.com"),
+                cert_pattern=DNSPattern.from_bytes(b"twistedmatrix.com"),
+                service_id=DNS_ID("twistedmatrix.com"),
             )
         ] == rv
 
     def test_integration_dns_id_fail(self):
         """
         Raise VerificationError if no certificate id matches the supplied
         service ids.
         """
-        i = DNS_ID(u"wrong.host")
+        i = DNS_ID("wrong.host")
         with pytest.raises(VerificationError) as e:
             verify_service_identity(
                 DNS_IDS, obligatory_ids=[i], optional_ids=[]
             )
         assert [DNSMismatch(mismatched_id=i)] == e.value.errors
 
     def test_ip_address_success(self):
         """
         IP addresses patterns are matched against IP address IDs.
         """
-        ip4 = ipaddress.ip_address(u"2.2.2.2")
-        ip6 = ipaddress.ip_address(u"2a00:1c38::53")
-        id4 = IPAddress_ID(six.text_type(ip4))
-        id6 = IPAddress_ID(six.text_type(ip6))
+        ip4 = ipaddress.ip_address("2.2.2.2")
+        ip6 = ipaddress.ip_address("2a00:1c38::53")
+        id4 = IPAddress_ID(str(ip4))
+        id6 = IPAddress_ID(str(ip6))
         rv = verify_service_identity(
-            extract_ids(CERT_EVERYTHING), [id4, id6], []
+            extract_patterns(CERT_EVERYTHING), [id4, id6], []
         )
 
         assert [
             ServiceMatch(id4, IPAddressPattern(ip4)),
             ServiceMatch(id6, IPAddressPattern(ip6)),
         ] == rv
 
     def test_obligatory_missing(self):
         """
         Raise if everything matches but one of the obligatory IDs is missing.
         """
-        i = DNS_ID(u"example.net")
+        i = DNS_ID("example.net")
         with pytest.raises(VerificationError) as e:
             verify_service_identity(
-                [SRVPattern(b"_mail.example.net")],
-                obligatory_ids=[SRV_ID(u"_mail.example.net"), i],
+                [SRVPattern.from_bytes(b"_mail.example.net")],
+                obligatory_ids=[SRV_ID("_mail.example.net"), i],
                 optional_ids=[],
             )
         assert [DNSMismatch(mismatched_id=i)] == e.value.errors
 
     def test_obligatory_mismatch(self):
         """
         Raise if one of the obligatory IDs doesn't match.
         """
-        i = DNS_ID(u"example.net")
+        i = DNS_ID("example.net")
         with pytest.raises(VerificationError) as e:
             verify_service_identity(
-                [SRVPattern(b"_mail.example.net"), DNSPattern(b"example.com")],
-                obligatory_ids=[SRV_ID(u"_mail.example.net"), i],
+                [
+                    SRVPattern.from_bytes(b"_mail.example.net"),
+                    DNSPattern.from_bytes(b"example.com"),
+                ],
+                obligatory_ids=[SRV_ID("_mail.example.net"), i],
                 optional_ids=[],
             )
         assert [DNSMismatch(mismatched_id=i)] == e.value.errors
 
     def test_optional_missing(self):
         """
         Optional IDs may miss as long as they don't conflict with an existing
         pattern.
         """
-        p = DNSPattern(b"mail.foo.com")
-        i = DNS_ID(u"mail.foo.com")
+        p = DNSPattern.from_bytes(b"mail.foo.com")
+        i = DNS_ID("mail.foo.com")
         rv = verify_service_identity(
-            [p], obligatory_ids=[i], optional_ids=[SRV_ID(u"_mail.foo.com")]
+            [p], obligatory_ids=[i], optional_ids=[SRV_ID("_mail.foo.com")]
         )
         assert [ServiceMatch(cert_pattern=p, service_id=i)] == rv
 
     def test_optional_mismatch(self):
         """
         Raise VerificationError if an ID from optional_ids does not match
         a pattern of respective type even if obligatory IDs match.
         """
-        i = SRV_ID(u"_xmpp.example.com")
+        i = SRV_ID("_xmpp.example.com")
         with pytest.raises(VerificationError) as e:
             verify_service_identity(
-                [DNSPattern(b"example.net"), SRVPattern(b"_mail.example.com")],
-                obligatory_ids=[DNS_ID(u"example.net")],
+                [
+                    DNSPattern.from_bytes(b"example.net"),
+                    SRVPattern.from_bytes(b"_mail.example.com"),
+                ],
+                obligatory_ids=[DNS_ID("example.net")],
                 optional_ids=[i],
             )
         assert [SRVMismatch(mismatched_id=i)] == e.value.errors
 
     def test_contains_optional_and_matches(self):
         """
         If an optional ID is found, return the match within the returned
         list and don't raise an error.
         """
-        p = SRVPattern(b"_mail.example.net")
-        i = SRV_ID(u"_mail.example.net")
+        p = SRVPattern.from_bytes(b"_mail.example.net")
+        i = SRV_ID("_mail.example.net")
         rv = verify_service_identity(
-            [DNSPattern(b"example.net"), p],
-            obligatory_ids=[DNS_ID(u"example.net")],
+            [DNSPattern.from_bytes(b"example.net"), p],
+            obligatory_ids=[DNS_ID("example.net")],
             optional_ids=[i],
         )
         assert ServiceMatch(cert_pattern=p, service_id=i) == rv[1]
 
 
-class TestContainsInstance(object):
+class TestContainsInstance:
     def test_positive(self):
         """
         If the list contains an object of the type, return True.
         """
-        assert _contains_instance_of([object(), tuple(), object()], tuple)
+        assert _contains_instance_of([object(), (), object()], tuple)
 
     def test_negative(self):
         """
         If the list does not contain an object of the type, return False.
         """
-        assert not _contains_instance_of([object(), list(), {}], tuple)
+        assert not _contains_instance_of([object(), [], {}], tuple)
 
 
-class TestDNS_ID(object):
+class TestDNS_ID:
     def test_enforces_unicode(self):
         """
         Raise TypeError if pass DNS-ID is not unicode.
         """
         with pytest.raises(TypeError):
             DNS_ID(b"foo.com")
 
     def test_handles_missing_idna(self, monkeypatch):
         """
         Raise ImportError if idna is missing and a non-ASCII DNS-ID is passed.
         """
-        monkeypatch.setattr(service_identity._common, "idna", None)
+        monkeypatch.setattr(service_identity.hazmat, "idna", None)
         with pytest.raises(ImportError):
-            DNS_ID(u"f\xf8\xf8.com")
+            DNS_ID("f\xf8\xf8.com")
 
     def test_ascii_works_without_idna(self, monkeypatch):
         """
         7bit-ASCII DNS-IDs work no matter whether idna is present or not.
         """
-        monkeypatch.setattr(service_identity._common, "idna", None)
-        dns = DNS_ID(u"foo.com")
+        monkeypatch.setattr(service_identity.hazmat, "idna", None)
+        dns = DNS_ID("foo.com")
         assert b"foo.com" == dns.hostname
 
     @pytest.mark.skipif(idna is None, reason="idna not installed")
     def test_idna_used_if_available_on_non_ascii(self):
         """
         If idna is installed and a non-ASCII DNS-ID is passed, encode it to
         ASCII.
         """
-        dns = DNS_ID(u"f\xf8\xf8.com")
+        dns = DNS_ID("f\xf8\xf8.com")
         assert b"xn--f-5gaa.com" == dns.hostname
 
     @pytest.mark.parametrize(
         "invalid_id",
         [
-            u" ",
-            u"",  # empty strings
-            u"host,name",  # invalid chars
-            u"192.168.0.0",
-            u"::1",
-            u"1234",  # IP addresses
+            " ",
+            "",  # empty strings
+            "host,name",  # invalid chars
+            "192.168.0.0",
+            "::1",
+            "1234",  # IP addresses
         ],
     )
     def test_catches_invalid_dns_ids(self, invalid_id):
         """
         Raise ValueError on invalid DNS-IDs.
         """
         with pytest.raises(ValueError):
             DNS_ID(invalid_id)
 
     def test_lowercases(self):
         """
         The hostname is lowercased so it can be compared case-insensitively.
         """
-        dns_id = DNS_ID(u"hOsTnAmE")
+        dns_id = DNS_ID("hOsTnAmE")
         assert b"hostname" == dns_id.hostname
 
     def test_verifies_only_dns(self):
         """
         If anything else than DNSPattern is passed to verify, return False.
         """
-        assert not DNS_ID(u"foo.com").verify(object())
+        assert not DNS_ID("foo.com").verify(object())
 
     def test_simple_match(self):
         """
         Simple integration test with _hostname_matches with a match.
         """
-        assert DNS_ID(u"foo.com").verify(DNSPattern(b"foo.com"))
+        assert DNS_ID("foo.com").verify(DNSPattern.from_bytes(b"foo.com"))
 
     def test_simple_mismatch(self):
         """
         Simple integration test with _hostname_matches with a mismatch.
         """
-        assert not DNS_ID(u"foo.com").verify(DNSPattern(b"bar.com"))
+        assert not DNS_ID("foo.com").verify(DNSPattern.from_bytes(b"bar.com"))
 
     def test_matches(self):
         """
         Valid matches return `True`.
         """
         for cert, actual in [
             (b"www.example.com", b"www.example.com"),
@@ -273,230 +276,242 @@
             (b"f*.example.com", b"foo.example.com"),
             (b"*oo.bar.com", b"foo.bar.com"),
             (b"fo*oo.bar.com", b"fooooo.bar.com"),
         ]:
             assert not _hostname_matches(cert, actual)
 
 
-class TestURI_ID(object):
+class TestURI_ID:
     def test_enforces_unicode(self):
         """
         Raise TypeError if pass URI-ID is not unicode.
         """
         with pytest.raises(TypeError):
             URI_ID(b"sip:foo.com")
 
     def test_create_DNS_ID(self):
         """
         The hostname is converted into a DNS_ID object.
         """
-        uri_id = URI_ID(u"sip:foo.com")
-        assert DNS_ID(u"foo.com") == uri_id.dns_id
+        uri_id = URI_ID("sip:foo.com")
+        assert DNS_ID("foo.com") == uri_id.dns_id
         assert b"sip" == uri_id.protocol
 
     def test_lowercases(self):
         """
         The protocol is lowercased so it can be compared case-insensitively.
         """
-        uri_id = URI_ID(u"sIp:foo.com")
+        uri_id = URI_ID("sIp:foo.com")
         assert b"sip" == uri_id.protocol
 
     def test_catches_missing_colon(self):
         """
         Raise ValueError if there's no colon within a URI-ID.
         """
         with pytest.raises(ValueError):
-            URI_ID(u"sip;foo.com")
+            URI_ID("sip;foo.com")
 
     def test_is_only_valid_for_uri(self):
         """
         If anything else than an URIPattern is passed to verify, return
         False.
         """
-        assert not URI_ID(u"sip:foo.com").verify(object())
+        assert not URI_ID("sip:foo.com").verify(object())
 
     def test_protocol_mismatch(self):
         """
         If protocol doesn't match, verify returns False.
         """
-        assert not URI_ID(u"sip:foo.com").verify(URIPattern(b"xmpp:foo.com"))
+        assert not URI_ID("sip:foo.com").verify(
+            URIPattern.from_bytes(b"xmpp:foo.com")
+        )
 
     def test_dns_mismatch(self):
         """
         If the hostname doesn't match, verify returns False.
         """
-        assert not URI_ID(u"sip:bar.com").verify(URIPattern(b"sip:foo.com"))
+        assert not URI_ID("sip:bar.com").verify(
+            URIPattern.from_bytes(b"sip:foo.com")
+        )
 
     def test_match(self):
         """
         Accept legal matches.
         """
-        assert URI_ID(u"sip:foo.com").verify(URIPattern(b"sip:foo.com"))
+        assert URI_ID("sip:foo.com").verify(
+            URIPattern.from_bytes(b"sip:foo.com")
+        )
 
 
-class TestSRV_ID(object):
+class TestSRV_ID:
     def test_enforces_unicode(self):
         """
         Raise TypeError if pass srv-ID is not unicode.
         """
         with pytest.raises(TypeError):
             SRV_ID(b"_mail.example.com")
 
     def test_create_DNS_ID(self):
         """
         The hostname is converted into a DNS_ID object.
         """
-        srv_id = SRV_ID(u"_mail.example.com")
-        assert DNS_ID(u"example.com") == srv_id.dns_id
+        srv_id = SRV_ID("_mail.example.com")
+        assert DNS_ID("example.com") == srv_id.dns_id
 
     def test_lowercases(self):
         """
         The service name is lowercased so it can be compared
         case-insensitively.
         """
-        srv_id = SRV_ID(u"_MaIl.foo.com")
+        srv_id = SRV_ID("_MaIl.foo.com")
         assert b"mail" == srv_id.name
 
     def test_catches_missing_dot(self):
         """
         Raise ValueError if there's no dot within a SRV-ID.
         """
         with pytest.raises(ValueError):
-            SRV_ID(u"_imapsfoocom")
+            SRV_ID("_imapsfoocom")
 
     def test_catches_missing_underscore(self):
         """
         Raise ValueError if the service is doesn't start with an underscore.
         """
         with pytest.raises(ValueError):
-            SRV_ID(u"imaps.foo.com")
+            SRV_ID("imaps.foo.com")
 
     def test_is_only_valid_for_SRV(self):
         """
         If anything else than an SRVPattern is passed to verify, return False.
         """
-        assert not SRV_ID(u"_mail.foo.com").verify(object())
+        assert not SRV_ID("_mail.foo.com").verify(object())
 
     def test_match(self):
         """
         Accept legal matches.
         """
-        assert SRV_ID(u"_mail.foo.com").verify(SRVPattern(b"_mail.foo.com"))
+        assert SRV_ID("_mail.foo.com").verify(
+            SRVPattern.from_bytes(b"_mail.foo.com")
+        )
 
     @pytest.mark.skipif(idna is None, reason="idna not installed")
     def test_match_idna(self):
         """
         IDNAs are handled properly.
         """
-        assert SRV_ID(u"_mail.f\xf8\xf8.com").verify(
-            SRVPattern(b"_mail.xn--f-5gaa.com")
+        assert SRV_ID("_mail.f\xf8\xf8.com").verify(
+            SRVPattern.from_bytes(b"_mail.xn--f-5gaa.com")
         )
 
     def test_mismatch_service_name(self):
         """
         If the service name doesn't match, verify returns False.
         """
         assert not (
-            SRV_ID(u"_mail.foo.com").verify(SRVPattern(b"_xmpp.foo.com"))
+            SRV_ID("_mail.foo.com").verify(
+                SRVPattern.from_bytes(b"_xmpp.foo.com")
+            )
         )
 
     def test_mismatch_dns(self):
         """
         If the dns_id doesn't match, verify returns False.
         """
         assert not (
-            SRV_ID(u"_mail.foo.com").verify(SRVPattern(b"_mail.bar.com"))
+            SRV_ID("_mail.foo.com").verify(
+                SRVPattern.from_bytes(b"_mail.bar.com")
+            )
         )
 
 
-class TestDNSPattern(object):
+class TestDNSPattern:
     def test_enforces_bytes(self):
         """
         Raise TypeError if unicode is passed.
         """
         with pytest.raises(TypeError):
-            DNSPattern(u"foo.com")
+            DNSPattern.from_bytes("foo.com")
 
     def test_catches_empty(self):
         """
         Empty DNS-IDs raise a :class:`CertificateError`.
         """
         with pytest.raises(CertificateError):
-            DNSPattern(b" ")
+            DNSPattern.from_bytes(b" ")
 
     def test_catches_NULL_bytes(self):
         """
         Raise :class:`CertificateError` if a NULL byte is in the hostname.
         """
         with pytest.raises(CertificateError):
-            DNSPattern(b"www.google.com\0nasty.h4x0r.com")
+            DNSPattern.from_bytes(b"www.google.com\0nasty.h4x0r.com")
 
     def test_catches_ip_address(self):
         """
         IP addresses are invalid and raise a :class:`CertificateError`.
         """
         with pytest.raises(CertificateError):
-            DNSPattern(b"192.168.0.0")
+            DNSPattern.from_bytes(b"192.168.0.0")
 
     def test_invalid_wildcard(self):
         """
         Integration test with _validate_pattern: catches double wildcards thus
         is used if an wildward is present.
         """
         with pytest.raises(CertificateError):
-            DNSPattern(b"*.foo.*")
+            DNSPattern.from_bytes(b"*.foo.*")
 
 
-class TestURIPattern(object):
+class TestURIPattern:
     def test_enforces_bytes(self):
         """
         Raise TypeError if unicode is passed.
         """
         with pytest.raises(TypeError):
-            URIPattern(u"sip:foo.com")
+            URIPattern.from_bytes("sip:foo.com")
 
     def test_catches_missing_colon(self):
         """
         Raise CertificateError if URI doesn't contain a `:`.
         """
         with pytest.raises(CertificateError):
-            URIPattern(b"sip;foo.com")
+            URIPattern.from_bytes(b"sip;foo.com")
 
     def test_catches_wildcards(self):
         """
         Raise CertificateError if URI contains a *.
         """
         with pytest.raises(CertificateError):
-            URIPattern(b"sip:*.foo.com")
+            URIPattern.from_bytes(b"sip:*.foo.com")
 
 
-class TestSRVPattern(object):
+class TestSRVPattern:
     def test_enforces_bytes(self):
         """
         Raise TypeError if unicode is passed.
         """
         with pytest.raises(TypeError):
-            SRVPattern(u"_mail.example.com")
+            SRVPattern.from_bytes("_mail.example.com")
 
     def test_catches_missing_underscore(self):
         """
         Raise CertificateError if SRV doesn't start with a `_`.
         """
         with pytest.raises(CertificateError):
-            SRVPattern(b"foo.com")
+            SRVPattern.from_bytes(b"foo.com")
 
     def test_catches_wildcards(self):
         """
         Raise CertificateError if SRV contains a *.
         """
         with pytest.raises(CertificateError):
-            SRVPattern(b"sip:*.foo.com")
+            SRVPattern.from_bytes(b"sip:*.foo.com")
 
 
-class TestValidateDNSWildcardPattern(object):
+class TestValidateDNSWildcardPattern:
     def test_allows_only_one_wildcard(self):
         """
         Raise CertificateError on multiple wildcards.
         """
         with pytest.raises(CertificateError):
             _validate_pattern(b"*.*.com")
 
@@ -533,52 +548,52 @@
             b"*oo.bar.com",
             b"f*.bar.com",
             b"f*o.bar.com",
         ]:
             _validate_pattern(pattern)
 
 
-class TestIPAddressPattern(object):
+class TestIPAddressPattern:
     def test_invalid_ip(self):
         """
         Raises CertificateError on invalid IP addresses.
         """
         with pytest.raises(CertificateError):
             IPAddressPattern.from_bytes(b"127.o.o.1")
 
-    @pytest.mark.parametrize("ip_s", [u"1.1.1.1", u"::1"])
+    @pytest.mark.parametrize("ip_s", ["1.1.1.1", "::1"])
     def test_verify_equal(self, ip_s):
         """
         Return True if IP addresses are identical.
         """
         ip = ipaddress.ip_address(ip_s)
 
         assert IPAddress_ID(ip).verify(IPAddressPattern(ip)) is True
 
 
-class FakeCertID(object):
+class FakeCertID:
     pass
 
 
-class Fake_ID(object):
+class Fake_ID:
     """
     An ID that accepts exactly on object as pattern.
     """
 
     def __init__(self, pattern):
         self._pattern = pattern
 
     def verify(self, other):
         """
         True iff other is the same object as pattern.
         """
         return other is self._pattern
 
 
-class TestFindMatches(object):
+class TestFindMatches:
     def test_one_match(self):
         """
         If there's a match, return a tuple of the certificate id and the
         service id.
         """
         valid_cert_id = FakeCertID()
         valid_id = Fake_ID(valid_cert_id)
@@ -625,20 +640,20 @@
         assert [
             ServiceMatch(cert_pattern=valid_cert_id_1, service_id=valid_id_1),
             ServiceMatch(cert_pattern=valid_cert_id_2, service_id=valid_id_2),
             ServiceMatch(cert_pattern=valid_cert_id_3, service_id=valid_id_3),
         ] == rv
 
 
-class TestIsIPAddress(object):
+class TestIsIPAddress:
     @pytest.mark.parametrize(
         "ip",
         [
             b"127.0.0.1",
-            u"127.0.0.1",
+            "127.0.0.1",
             "172.16.254.12",
             "*.0.0.1",
             "::1",
             "*::1",
             "2001:0db8:0000:0000:0000:ff00:0042:8329",
             "2001:0db8::ff00:0042:8329",
         ],
@@ -663,15 +678,15 @@
     def test_not_ips(self, not_ip):
         """
         Return False for patterns and hosts that aren't IP addresses.
         """
         assert _is_ip_address(not_ip) is False
 
 
-class TestVerificationError(object):
+class TestVerificationError:
     def test_repr_str(self):
         """
         The __str__ and __repr__ methods return something helpful.
         """
         try:
             raise VerificationError(errors=["foo"])
         except VerificationError as e:
```

### Comparing `service-identity-21.1.0/tests/test_cryptography.py` & `service_identity-23.1.0/tests/test_cryptography.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,124 +1,136 @@
-from __future__ import absolute_import, division, print_function
-
 import ipaddress
 
 import pytest
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.x509 import load_pem_x509_certificate
 
-from service_identity import SubjectAltNameWarning
-from service_identity._common import (
-    DNS_ID,
-    DNSPattern,
-    IPAddress_ID,
-    IPAddressPattern,
-    URIPattern,
-)
 from service_identity.cryptography import (
     extract_ids,
+    extract_patterns,
     verify_certificate_hostname,
     verify_certificate_ip_address,
 )
 from service_identity.exceptions import (
     DNSMismatch,
     IPAddressMismatch,
     VerificationError,
 )
+from service_identity.hazmat import (
+    DNS_ID,
+    DNSPattern,
+    IPAddress_ID,
+    IPAddressPattern,
+    URIPattern,
+)
 
 from .util import PEM_CN_ONLY, PEM_DNS_ONLY, PEM_EVERYTHING, PEM_OTHER_NAME
 
 
 backend = default_backend()
 X509_DNS_ONLY = load_pem_x509_certificate(PEM_DNS_ONLY, backend)
 X509_CN_ONLY = load_pem_x509_certificate(PEM_CN_ONLY, backend)
 X509_OTHER_NAME = load_pem_x509_certificate(PEM_OTHER_NAME, backend)
 CERT_EVERYTHING = load_pem_x509_certificate(PEM_EVERYTHING, backend)
 
 
-class TestPublicAPI(object):
+class TestPublicAPI:
     def test_certificate_verify_hostname_ok(self):
         """
         verify_certificate_hostname succeeds if the hostnames match.
         """
-        verify_certificate_hostname(X509_DNS_ONLY, u"twistedmatrix.com")
+        verify_certificate_hostname(X509_DNS_ONLY, "twistedmatrix.com")
 
     def test_certificate_verify_hostname_fail(self):
         """
         verify_certificate_hostname fails if the hostnames don't match and
         provides the user with helpful information.
         """
         with pytest.raises(VerificationError) as ei:
-            verify_certificate_hostname(X509_DNS_ONLY, u"google.com")
+            verify_certificate_hostname(X509_DNS_ONLY, "google.com")
 
         assert [
-            DNSMismatch(mismatched_id=DNS_ID(u"google.com"))
+            DNSMismatch(mismatched_id=DNS_ID("google.com"))
         ] == ei.value.errors
 
-    @pytest.mark.parametrize("ip", [u"1.1.1.1", u"::1"])
+    @pytest.mark.parametrize("ip", ["1.1.1.1", "::1"])
     def test_verify_certificate_ip_address_ok(self, ip):
         """
         verify_certificate_ip_address succeeds if the addresses match. Works
         both with IPv4 and IPv6.
         """
         verify_certificate_ip_address(CERT_EVERYTHING, ip)
 
-    @pytest.mark.parametrize("ip", [u"1.1.1.2", u"::2"])
+    @pytest.mark.parametrize("ip", ["1.1.1.2", "::2"])
     def test_verify_ip_address_fail(self, ip):
         """
         verify_ip_address fails if the addresses don't match and provides the
         user with helpful information.  Works both with IPv4 and IPv6.
         """
         with pytest.raises(VerificationError) as ei:
             verify_certificate_ip_address(CERT_EVERYTHING, ip)
 
         assert [
             IPAddressMismatch(mismatched_id=IPAddress_ID(ip))
         ] == ei.value.errors
 
 
-class TestExtractIDs(object):
+class TestExtractPatterns:
     def test_dns(self):
         """
         Returns the correct DNSPattern from a certificate.
         """
-        rv = extract_ids(X509_DNS_ONLY)
+        rv = extract_patterns(X509_DNS_ONLY)
         assert [
-            DNSPattern(b"www.twistedmatrix.com"),
-            DNSPattern(b"twistedmatrix.com"),
+            DNSPattern.from_bytes(b"www.twistedmatrix.com"),
+            DNSPattern.from_bytes(b"twistedmatrix.com"),
         ] == rv
 
-    def test_cn_ids_are_used_as_fallback(self):
+    def test_cn_ids_are_ignored(self):
         """
-        CNs are returned as DNSPattern if no other IDs are present
-        and a warning is raised.
+        commonName is not supported anymore and therefore ignored.
         """
-        with pytest.warns(SubjectAltNameWarning):
-            rv = extract_ids(X509_CN_ONLY)
-        assert [DNSPattern(b"www.microsoft.com")] == rv
+        assert [] == extract_patterns(X509_CN_ONLY)
 
     def test_uri(self):
         """
         Returns the correct URIPattern from a certificate.
         """
-        rv = extract_ids(X509_OTHER_NAME)
-        assert [URIPattern(b"http://example.com/")] == [
+        rv = extract_patterns(X509_OTHER_NAME)
+        assert [URIPattern.from_bytes(b"http://example.com/")] == [
             id for id in rv if isinstance(id, URIPattern)
         ]
 
     def test_ip(self):
         """
         Returns IP patterns.
         """
-        rv = extract_ids(CERT_EVERYTHING)
+        rv = extract_patterns(CERT_EVERYTHING)
 
         assert [
-            DNSPattern(pattern=b"service.identity.invalid"),
-            DNSPattern(pattern=b"*.wildcard.service.identity.invalid"),
-            DNSPattern(pattern=b"service.identity.invalid"),
-            DNSPattern(pattern=b"single.service.identity.invalid"),
-            IPAddressPattern(pattern=ipaddress.IPv4Address(u"1.1.1.1")),
-            IPAddressPattern(pattern=ipaddress.IPv6Address(u"::1")),
-            IPAddressPattern(pattern=ipaddress.IPv4Address(u"2.2.2.2")),
-            IPAddressPattern(pattern=ipaddress.IPv6Address(u"2a00:1c38::53")),
+            DNSPattern.from_bytes(pattern=b"service.identity.invalid"),
+            DNSPattern.from_bytes(
+                pattern=b"*.wildcard.service.identity.invalid"
+            ),
+            DNSPattern.from_bytes(pattern=b"service.identity.invalid"),
+            DNSPattern.from_bytes(pattern=b"single.service.identity.invalid"),
+            IPAddressPattern(pattern=ipaddress.IPv4Address("1.1.1.1")),
+            IPAddressPattern(pattern=ipaddress.IPv6Address("::1")),
+            IPAddressPattern(pattern=ipaddress.IPv4Address("2.2.2.2")),
+            IPAddressPattern(pattern=ipaddress.IPv6Address("2a00:1c38::53")),
         ] == rv
+
+    def test_extract_ids_deprecated(self):
+        """
+        `extract_ids` raises a DeprecationWarning with correct stacklevel.
+        """
+        with pytest.deprecated_call() as wr:
+            extract_ids(CERT_EVERYTHING)
+
+        w = wr.pop()
+
+        assert (
+            "`extract_ids()` is deprecated, please use `extract_patterns()`."
+            == w.message.args[0]
+        )
+        assert __file__ == w.filename
```

### Comparing `service-identity-21.1.0/tests/test_pyopenssl.py` & `service_identity-23.1.0/tests/test_pyopenssl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,151 +1,156 @@
-from __future__ import absolute_import, division, print_function
-
 import ipaddress
 
 import pytest
 
-from OpenSSL.crypto import FILETYPE_PEM, load_certificate
-
-from service_identity import SubjectAltNameWarning
-from service_identity._common import (
+from service_identity.exceptions import (
+    DNSMismatch,
+    IPAddressMismatch,
+    VerificationError,
+)
+from service_identity.hazmat import (
     DNS_ID,
     DNSPattern,
     IPAddress_ID,
     IPAddressPattern,
     URIPattern,
 )
-from service_identity.exceptions import (
-    DNSMismatch,
-    IPAddressMismatch,
-    VerificationError,
-)
 from service_identity.pyopenssl import (
     extract_ids,
+    extract_patterns,
     verify_hostname,
     verify_ip_address,
 )
 
 from .util import PEM_CN_ONLY, PEM_DNS_ONLY, PEM_EVERYTHING, PEM_OTHER_NAME
 
 
+if pytest.importorskip("OpenSSL"):
+    from OpenSSL.crypto import FILETYPE_PEM, load_certificate
+
+
 CERT_DNS_ONLY = load_certificate(FILETYPE_PEM, PEM_DNS_ONLY)
 CERT_CN_ONLY = load_certificate(FILETYPE_PEM, PEM_CN_ONLY)
 CERT_OTHER_NAME = load_certificate(FILETYPE_PEM, PEM_OTHER_NAME)
 CERT_EVERYTHING = load_certificate(FILETYPE_PEM, PEM_EVERYTHING)
 
 
-class TestPublicAPI(object):
+class TestPublicAPI:
     def test_verify_hostname_ok(self):
         """
         verify_hostname succeeds if the hostnames match.
         """
 
-        class FakeConnection(object):
+        class FakeConnection:
             def get_peer_certificate(self):
                 return CERT_DNS_ONLY
 
-        verify_hostname(FakeConnection(), u"twistedmatrix.com")
+        verify_hostname(FakeConnection(), "twistedmatrix.com")
 
     def test_verify_hostname_fail(self):
         """
         verify_hostname fails if the hostnames don't match and provides the
         user with helpful information.
         """
 
-        class FakeConnection(object):
+        class FakeConnection:
             def get_peer_certificate(self):
                 return CERT_DNS_ONLY
 
         with pytest.raises(VerificationError) as ei:
-            verify_hostname(FakeConnection(), u"google.com")
+            verify_hostname(FakeConnection(), "google.com")
 
         assert [
-            DNSMismatch(mismatched_id=DNS_ID(u"google.com"))
+            DNSMismatch(mismatched_id=DNS_ID("google.com"))
         ] == ei.value.errors
 
-    @pytest.mark.parametrize("ip", [u"1.1.1.1", u"::1"])
+    @pytest.mark.parametrize("ip", ["1.1.1.1", "::1"])
     def test_verify_ip_address_ok(self, ip):
         """
         verify_ip_address succeeds if the addresses match. Works both with IPv4
         and IPv6.
         """
 
-        class FakeConnection(object):
+        class FakeConnection:
             def get_peer_certificate(self):
                 return CERT_EVERYTHING
 
         verify_ip_address(FakeConnection(), ip)
 
-    @pytest.mark.parametrize("ip", [u"1.1.1.2", u"::2"])
+    @pytest.mark.parametrize("ip", ["1.1.1.2", "::2"])
     def test_verify_ip_address_fail(self, ip):
         """
         verify_ip_address fails if the addresses don't match and provides the
         user with helpful information. Works both with IPv4 and IPv6.
         """
 
-        class FakeConnection(object):
+        class FakeConnection:
             def get_peer_certificate(self):
                 return CERT_EVERYTHING
 
         with pytest.raises(VerificationError) as ei:
             verify_ip_address(FakeConnection(), ip)
 
         assert [
             IPAddressMismatch(mismatched_id=IPAddress_ID(ip))
         ] == ei.value.errors
 
 
-class TestExtractIDs(object):
+class TestExtractPatterns:
     def test_dns(self):
         """
         Returns the correct DNSPattern from a certificate.
         """
-        rv = extract_ids(CERT_DNS_ONLY)
+        rv = extract_patterns(CERT_DNS_ONLY)
         assert [
-            DNSPattern(b"www.twistedmatrix.com"),
-            DNSPattern(b"twistedmatrix.com"),
+            DNSPattern.from_bytes(b"www.twistedmatrix.com"),
+            DNSPattern.from_bytes(b"twistedmatrix.com"),
         ] == rv
 
-    def test_cn_ids_are_used_as_fallback(self):
+    def test_cn_ids_are_ignored(self):
         """
-        CNs are returned as DNSPattern if no other IDs are present
-        and a warning is raised.
+        commonName is not supported anymore and therefore ignored.
         """
-        with pytest.warns(SubjectAltNameWarning) as ws:
-            rv = extract_ids(CERT_CN_ONLY)
-
-        msg = ws[0].message.args[0]
-
-        assert [DNSPattern(b"www.microsoft.com")] == rv
-        assert msg.startswith(
-            "Certificate with CN 'www.microsoft.com' has no `subjectAltName`"
-        )
-        assert msg.endswith(
-            "service-identity will remove the support for it in mid-2018."
-        )
+        assert [] == extract_patterns(CERT_CN_ONLY)
 
     def test_uri(self):
         """
         Returns the correct URIPattern from a certificate.
         """
-        rv = extract_ids(CERT_OTHER_NAME)
-        assert [URIPattern(b"http://example.com/")] == [
+        rv = extract_patterns(CERT_OTHER_NAME)
+        assert [URIPattern.from_bytes(b"http://example.com/")] == [
             id for id in rv if isinstance(id, URIPattern)
         ]
 
     def test_ip(self):
         """
         Returns IP patterns.
         """
-        rv = extract_ids(CERT_EVERYTHING)
+        rv = extract_patterns(CERT_EVERYTHING)
 
         assert [
-            DNSPattern(pattern=b"service.identity.invalid"),
-            DNSPattern(pattern=b"*.wildcard.service.identity.invalid"),
-            DNSPattern(pattern=b"service.identity.invalid"),
-            DNSPattern(pattern=b"single.service.identity.invalid"),
-            IPAddressPattern(pattern=ipaddress.IPv4Address(u"1.1.1.1")),
-            IPAddressPattern(pattern=ipaddress.IPv6Address(u"::1")),
-            IPAddressPattern(pattern=ipaddress.IPv4Address(u"2.2.2.2")),
-            IPAddressPattern(pattern=ipaddress.IPv6Address(u"2a00:1c38::53")),
+            DNSPattern.from_bytes(pattern=b"service.identity.invalid"),
+            DNSPattern.from_bytes(
+                pattern=b"*.wildcard.service.identity.invalid"
+            ),
+            DNSPattern.from_bytes(pattern=b"service.identity.invalid"),
+            DNSPattern.from_bytes(pattern=b"single.service.identity.invalid"),
+            IPAddressPattern(pattern=ipaddress.IPv4Address("1.1.1.1")),
+            IPAddressPattern(pattern=ipaddress.IPv6Address("::1")),
+            IPAddressPattern(pattern=ipaddress.IPv4Address("2.2.2.2")),
+            IPAddressPattern(pattern=ipaddress.IPv6Address("2a00:1c38::53")),
         ] == rv
+
+    def test_extract_ids_deprecated(self):
+        """
+        `extract_ids` raises a DeprecationWarning with correct stacklevel.
+        """
+        with pytest.deprecated_call() as wr:
+            extract_ids(CERT_EVERYTHING)
+
+        w = wr.pop()
+
+        assert (
+            "`extract_ids()` is deprecated, please use `extract_patterns()`."
+            == w.message.args[0]
+        )
+        assert __file__ == w.filename
```

### Comparing `service-identity-21.1.0/tests/util.py` & `service_identity-23.1.0/tests/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from __future__ import absolute_import, division, print_function
-
 from cryptography.hazmat.backends import default_backend
 from cryptography.x509 import load_pem_x509_certificate
 
-from service_identity.cryptography import extract_ids
+from service_identity.cryptography import extract_patterns
 
 
 # Test certificates
 
 PEM_DNS_ONLY = b"""\
 -----BEGIN CERTIFICATE-----
 MIIGbjCCBVagAwIBAgIDCesrMA0GCSqGSIb3DQEBBQUAMIGMMQswCQYDVQQGEwJJ
@@ -43,55 +41,40 @@
 wtbPJQSm0LyGtfdrR6iKFPf28Vm/VkYXPiOV08GD9B7yl1SjktXOsGMPlOHU8YQZ
 DEsHOrRvaZBSA1VtBQjYnoO0pDVu9QwDLAPLFvFice2PN803HuMFIwcuQSIrh4nq
 PqwitBZ6nPPHz7aSiAut/+txK3EZll0d+hl0H3Phd+ICeITYhNkLe90k7l1IFpET
 fJiBDvG/iDAJISgkrR1heuX/e+yWfx7RvqGlMLIE35d+0MhWy92Jzejbl8fJdr4C
 Kulh/pV07MWAUZxscUPtWmPo
 -----END CERTIFICATE-----"""
 
-DNS_IDS = extract_ids(
+DNS_IDS = extract_patterns(
     load_pem_x509_certificate(PEM_DNS_ONLY, default_backend())
 )
 
 PEM_CN_ONLY = b"""\
 -----BEGIN CERTIFICATE-----
-MIIGdDCCBVygAwIBAgIKGOC4tAABAAAx0TANBgkqhkiG9w0BAQUFADCBgDETMBEG
-CgmSJomT8ixkARkWA2NvbTEZMBcGCgmSJomT8ixkARkWCW1pY3Jvc29mdDEUMBIG
-CgmSJomT8ixkARkWBGNvcnAxFzAVBgoJkiaJk/IsZAEZFgdyZWRtb25kMR8wHQYD
-VQQDExZNU0lUIE1hY2hpbmUgQXV0aCBDQSAyMB4XDTEzMDExMjAwMDc0MVoXDTE1
-MDExMjAwMDc0MVoweDELMAkGA1UEBhMCVVMxCzAJBgNVBAgTAldBMRAwDgYDVQQH
-EwdSZWRtb25kMR4wHAYDVQQKExVNaWNyb3NvZnQgQ29ycG9yYXRpb24xDjAMBgNV
-BAsTBU1TQ09NMRowGAYDVQQDExF3d3cubWljcm9zb2Z0LmNvbTCCASIwDQYJKoZI
-hvcNAQEBBQADggEPADCCAQoCggEBAJ+h4bQ7OlcO0M9UvM0Y2LISEzGkTDc9CT7v
-c91kI2GOlR/kbI1AUmJu3g6Cv0wqz4b9QT6BdXSE+WAxUM/yk4mf1HhkJtbSwucb
-AQAtgq0iC1u6mDDXH2sl/NUB4VKSGryIYYdRVHduZlFkAHmxwcmxyQt6BQykXl7G
-NkftiJZtVci/ZRPaBrFnkZjZCbJH+capx0v9hmBTLPVAGyIF5TwF1aldXT367S76
-QGGn6UnI0O5Cua7GU1JDVmbPus0kgRTazvyW4g17jGFtNJTy43UqlX7TZ8B76OZC
-sqoVxJblVh7I0WDcDFwIrSWiUEFc9i05g1g49xK8Y7tph8tbwv8CAwEAAaOCAvUw
-ggLxMAsGA1UdDwQEAwIEsDAdBgNVHSUEFjAUBggrBgEFBQcDAgYIKwYBBQUHAwEw
-eAYJKoZIhvcNAQkPBGswaTAOBggqhkiG9w0DAgICAIAwDgYIKoZIhvcNAwQCAgCA
-MAsGCWCGSAFlAwQBKjALBglghkgBZQMEAS0wCwYJYIZIAWUDBAECMAsGCWCGSAFl
-AwQBBTAHBgUrDgMCBzAKBggqhkiG9w0DBzAdBgNVHQ4EFgQUK9tKP5ACSJ4PiSHi
-60pzHuAPhWswHwYDVR0jBBgwFoAU69sRXvgJntjWYpz9Yp3jhEoo4Scwge4GA1Ud
-HwSB5jCB4zCB4KCB3aCB2oZPaHR0cDovL21zY3JsLm1pY3Jvc29mdC5jb20vcGtp
-L21zY29ycC9jcmwvTVNJVCUyME1hY2hpbmUlMjBBdXRoJTIwQ0ElMjAyKDEpLmNy
-bIZNaHR0cDovL2NybC5taWNyb3NvZnQuY29tL3BraS9tc2NvcnAvY3JsL01TSVQl
-MjBNYWNoaW5lJTIwQXV0aCUyMENBJTIwMigxKS5jcmyGOGh0dHA6Ly9jb3JwcGtp
-L2NybC9NU0lUJTIwTWFjaGluZSUyMEF1dGglMjBDQSUyMDIoMSkuY3JsMIGtBggr
-BgEFBQcBAQSBoDCBnTBVBggrBgEFBQcwAoZJaHR0cDovL3d3dy5taWNyb3NvZnQu
-Y29tL3BraS9tc2NvcnAvTVNJVCUyME1hY2hpbmUlMjBBdXRoJTIwQ0ElMjAyKDEp
-LmNydDBEBggrBgEFBQcwAoY4aHR0cDovL2NvcnBwa2kvYWlhL01TSVQlMjBNYWNo
-aW5lJTIwQXV0aCUyMENBJTIwMigxKS5jcnQwPwYJKwYBBAGCNxUHBDIwMAYoKwYB
-BAGCNxUIg8+JTa3yAoWhnwyC+sp9geH7dIFPg8LthQiOqdKFYwIBZAIBCjAnBgkr
-BgEEAYI3FQoEGjAYMAoGCCsGAQUFBwMCMAoGCCsGAQUFBwMBMA0GCSqGSIb3DQEB
-BQUAA4IBAQBgwMY9qix/FoBY3QBHTNFVf+d6siaBWoQjwBXDQlPXLmowbt97j62Z
-N6OogRP2V+ivnBcybucJTJE6zTxrGZ7hNeC9T3v34Q1OMezWiZf+jktNZvqiXctm
-Dh774lt5S9X2C+k1e9K8YrnNb8PNeKkX/vVX9MZzn2aQqU34dOg6vVnrq0pBrq/Y
-TJcPG4yq3kFR3ONTZb5JgE8EV1G43vW/LNQbEbQUgVtiKRapEs7rSSws6Jj47MUc
-on6HgPTtfuJGMNWFTiw7nZTM8mLXsXBMePSgq8PkKPmPkB3KET/OitmePmhk4l+S
-eMkNCM6YlrLcDF4fCLSjWYhoktmSJZnW
+MIIDlzCCAn+gAwIBAgIUNS9qfJRgoLrr68mAfmhzBior0JAwDQYJKoZIhvcNAQEL
+BQAwWzELMAkGA1UEBhMCQVUxEzARBgNVBAgMClNvbWUtU3RhdGUxITAfBgNVBAoM
+GEludGVybmV0IFdpZGdpdHMgUHR5IEx0ZDEUMBIGA1UEAwwLZXhhbXBsZS5jb20w
+HhcNMjMwNjA4MDkwNDAxWhcNNDkwMTI3MDkwNDAxWjBbMQswCQYDVQQGEwJBVTET
+MBEGA1UECAwKU29tZS1TdGF0ZTEhMB8GA1UECgwYSW50ZXJuZXQgV2lkZ2l0cyBQ
+dHkgTHRkMRQwEgYDVQQDDAtleGFtcGxlLmNvbTCCASIwDQYJKoZIhvcNAQEBBQAD
+ggEPADCCAQoCggEBALltBNRAyeFczK2kdKTkW6E3/+rptXBcaw3SyltY/Ft8DPe3
+lW/GWbbgAU7ceYC0LkYxOEnyQTlXhTyLHSk+PCQLi2ESgwWGnGY5Eusk1DRJ162q
+hLUkmz25KdTILnh402fgoziF2RU6PnA7iIwAVntT5uh4S1yPW7TWkdPsE0tc1yBx
+3SAHTXDkoahjKSot35Q87Jw92fxUd7WqVmDrgcLMvp8rXNjdg+HG4fQGoMcSQq2Z
+nVPIoWSTOGdL6SzSs6Wvllz3n7YWShTqp9CmGctCGubt02fHF+8G/dMTTukntG4q
+EjBtVfeDFx8yXUdOgN4egFxZGYATAUsLcyzNhQcCAwEAAaNTMFEwHQYDVR0OBBYE
+FDkuqwU8KxIvwAwMqVpNFYlgd6WbMB8GA1UdIwQYMBaAFDkuqwU8KxIvwAwMqVpN
+FYlgd6WbMA8GA1UdEwEB/wQFMAMBAf8wDQYJKoZIhvcNAQELBQADggEBAJ9Nb/C0
+2gkxhWm3S2/9onPMhFOxDLsYxBvZtJMeOvRRrJaxN2m0aXkm0Ww8Bq0qEegZE51m
+0T57IOS256rQlxEnZNeAWT2tf8FEqQGjbI1c/prj420e6afn18x8CSQgiOG4PJ+S
+YfufRjSHAYwiiNi+tiKBQ8jOuayFhih9/GsDJvAMW0HjaYZyG6jlA9p4bL1rSqD3
+gE+upYhkpVN1lFRZAhxRZOVIqJV/ppHp9RAuawsUdSNKm+rnlaExJKoVys+tZL9+
+djWWQVqnttYocQQ0umX4ydCTr1RM+7ziwWTR5kpOESA/gZePZQqeH9k+XrPEQtLn
+6QBxk+Ft53ZPVso=
 -----END CERTIFICATE-----
 """
 
 
 PEM_OTHER_NAME = b"""\
 -----BEGIN CERTIFICATE-----
 MIID/DCCAuSgAwIBAgIJAIS0TSddIw6cMA0GCSqGSIb3DQEBBQUAMGwxFDASBgNV
```

