# Comparing `tmp/mp-api-0.9.0.tar.gz` & `tmp/mp-api-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mp-api-0.9.0.tar", last modified: Thu Sep 23 19:14:15 2021, max compression
+gzip compressed data, was "dist/mp-api-0.9.1.tar", last modified: Wed Sep 29 00:04:08 2021, max compression
```

## Comparing `mp-api-0.9.0.tar` & `mp-api-0.9.1.tar`

### file list

```diff
@@ -1,337 +1,337 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-09-23 19:14:11.000000 mp-api-0.9.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-09-23 19:14:11.000000 mp-api-0.9.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)      432 2021-09-23 19:14:11.000000 mp-api-0.9.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      697 2021-09-23 19:14:11.000000 mp-api-0.9.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2176 2021-09-23 19:14:11.000000 mp-api-0.9.0/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2021-09-23 19:14:11.000000 mp-api-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      498 2021-09-23 19:14:11.000000 mp-api-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-09-23 19:14:11.000000 mp-api-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-09-23 19:14:11.000000 mp-api-0.9.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2021-09-23 19:14:11.000000 mp-api-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-09-23 19:14:15.000000 mp-api-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      641 2021-09-23 19:14:11.000000 mp-api-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    15621 2021-09-23 19:14:11.000000 mp-api-0.9.0/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2021-09-23 19:14:11.000000 mp-api-0.9.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-09-23 19:14:11.000000 mp-api-0.9.0/requirements-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      240 2021-09-23 19:14:11.000000 mp-api-0.9.0/requirements-testing.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-09-23 19:14:11.000000 mp-api-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      468 2021-09-23 19:14:15.000000 mp-api-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2021-09-23 19:14:11.000000 mp-api-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (121)     7922 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    11087 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (121)    18750 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/core/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    16211 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/core/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (121)      812 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    32920 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/matproj.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/_consumer/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/charge_density/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/charge_density/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/charge_density/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/dielectric/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dielectric/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dielectric/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      831 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dielectric/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      721 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dois/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dois/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dois/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/elasticity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/elasticity/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/elasticity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/elasticity/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5307 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/electrodes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4791 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electrodes/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electrodes/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8403 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electrodes/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14062 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electronic_structure/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electronic_structure/client.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/electronic_structure/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electronic_structure/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electronic_structure/models/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electronic_structure/models/doc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8577 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3326 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/eos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/eos/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/eos/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      731 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/eos/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/fermi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/fermi/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/fermi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/fermi/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/grain_boundary/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/grain_boundary/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/grain_boundary/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/magnetism/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4994 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/magnetism/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/magnetism/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/magnetism/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3840 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6222 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/materials/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/materials/client.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/materials/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/materials/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/materials/models/doc.py
--rw-r--r--   0 runner    (1001) docker     (121)    10119 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2043 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/molecules/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/molecules/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/molecules/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4031 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/mpcomplete/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/oxidation_states/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/oxidation_states/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      923 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/phonon/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/phonon/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/phonon/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/phonon/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/piezo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/piezo/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/piezo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/piezo/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/provenance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/provenance/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/provenance/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      539 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/robocrys/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/robocrys/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/robocrys/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/robocrys/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2599 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      720 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/similarity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/similarity/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/similarity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/similarity/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      579 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/substrates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3924 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/substrates/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/substrates/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/substrates/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/summary/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12929 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/summary/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/summary/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10075 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/summary/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     8467 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4069 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/surface_properties/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/surface_properties/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/surface_properties/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3893 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6007 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/data_adaptor_synpro.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/models/
--rw-r--r--   0 runner    (1001) docker     (121)      440 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/models/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/models/materials.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/models/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)      953 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/models/reaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     8130 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/tasks/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/tasks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7856 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/tasks/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/thermo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4693 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/thermo/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/thermo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      946 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api/routes/xas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/xas/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/xas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-09-23 19:14:11.000000 mp-api-0.9.0/src/mp_api/routes/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9960 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-09-23 19:14:15.000000 mp-api-0.9.0/src/mp_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/test_files/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-09-23 19:14:11.000000 mp-api-0.9.0/test_files/Si_mp_149.cif
--rw-r--r--   0 runner    (1001) docker     (121)    65661 2021-09-23 19:14:11.000000 mp-api-0.9.0/test_files/calcs_reversed_mp_1031016.json
--rw-r--r--   0 runner    (1001) docker     (121)  1340258 2021-09-23 19:14:11.000000 mp-api-0.9.0/test_files/materials_Li_Fe_V.json
--rw-r--r--   0 runner    (1001) docker     (121)     9125 2021-09-23 19:14:11.000000 mp-api-0.9.0/test_files/synth_doc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5420 2021-09-23 19:14:11.000000 mp-api-0.9.0/test_files/synth_doc_adaptor.json
--rw-r--r--   0 runner    (1001) docker     (121)    10805 2021-09-23 19:14:11.000000 mp-api-0.9.0/test_files/synth_doc_adaptor_synpro.json
--rw-r--r--   0 runner    (1001) docker     (121)  4920115 2021-09-23 19:14:11.000000 mp-api-0.9.0/test_files/tasks_Li_Fe_V.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/charge_density/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/core/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/dielectric/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/dielectric/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/elasticity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2822 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/elasticity/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/electrodes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2790 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/electrodes/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3850 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/electrodes/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5868 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/electronic_structure/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5044 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/eos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/eos/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3038 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/grain_boundary/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/magnetism/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2796 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/magnetism/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1928 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/materials/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/materials/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5829 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2867 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/molecules/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/piezo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/piezo/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/robocrys/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/robocrys/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/substrates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3028 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/substrates/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/summary/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3442 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/surface_properties/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/synthesis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (121)     5925 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/synthesis/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7514 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3332 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/tasks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2183 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/tasks/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    10501 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/test_mprester.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/thermo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/thermo/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:15.000000 mp-api-0.9.0/tests/xas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3579 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/xas/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2021-09-23 19:14:11.000000 mp-api-0.9.0/tests/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-09-29 00:03:59.000000 mp-api-0.9.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2021-09-29 00:03:59.000000 mp-api-0.9.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2021-09-29 00:03:59.000000 mp-api-0.9.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2021-09-29 00:03:59.000000 mp-api-0.9.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2176 2021-09-29 00:03:59.000000 mp-api-0.9.1/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1283 2021-09-29 00:03:59.000000 mp-api-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2021-09-29 00:03:59.000000 mp-api-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-09-29 00:03:59.000000 mp-api-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-09-29 00:03:59.000000 mp-api-0.9.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)     2417 2021-09-29 00:03:59.000000 mp-api-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-09-29 00:04:08.000000 mp-api-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2021-09-29 00:03:59.000000 mp-api-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    15625 2021-09-29 00:03:59.000000 mp-api-0.9.1/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2021-09-29 00:03:59.000000 mp-api-0.9.1/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-09-29 00:03:59.000000 mp-api-0.9.1/requirements-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2021-09-29 00:03:59.000000 mp-api-0.9.1/requirements-testing.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-09-29 00:03:59.000000 mp-api-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2021-09-29 00:04:08.000000 mp-api-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2021-09-29 00:03:59.000000 mp-api-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2155 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)     7922 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    11087 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (121)    18750 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16211 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/core/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33298 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/matproj.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1526 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/_consumer/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1026 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3424 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/charge_density/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/charge_density/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3091 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dielectric/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dielectric/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dielectric/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dois/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dois/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dois/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4623 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/elasticity/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/elasticity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1918 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/elasticity/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5307 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4791 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electrodes/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electrodes/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8403 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electrodes/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14062 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electronic_structure/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electronic_structure/client.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/electronic_structure/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electronic_structure/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electronic_structure/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electronic_structure/models/doc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8577 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3326 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/eos/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2475 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/eos/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/eos/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/eos/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/fermi/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/fermi/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/fermi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/fermi/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      530 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4581 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/grain_boundary/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/grain_boundary/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2022 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/grain_boundary/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2702 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4994 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/magnetism/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/magnetism/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2121 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/magnetism/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3840 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6222 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/materials/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/materials/client.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/materials/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/materials/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/materials/models/doc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10119 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2043 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2050 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/molecules/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/molecules/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/molecules/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4031 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/mpcomplete/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1696 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/oxidation_states/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/oxidation_states/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/phonon/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/phonon/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/phonon/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/phonon/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/piezo/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2420 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/piezo/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/piezo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/piezo/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/provenance/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/provenance/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/provenance/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/robocrys/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/robocrys/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1797 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/robocrys/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2599 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/similarity/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/similarity/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/similarity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/similarity/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/substrates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3924 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/substrates/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/substrates/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/substrates/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/summary/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13384 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/summary/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/summary/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    10075 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/summary/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8467 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1865 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4069 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/surface_properties/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/surface_properties/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2313 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/surface_properties/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      822 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3893 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2504 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6007 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/data_adaptor_synpro.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2282 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2114 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/models/materials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1758 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/models/operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/models/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8130 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2114 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/tasks/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/tasks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7856 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/tasks/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3079 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/thermo/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4689 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/thermo/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/thermo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      946 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api/routes/xas/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/xas/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/xas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1724 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-09-29 00:03:59.000000 mp-api-0.9.1/src/mp_api/routes/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9960 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-09-29 00:04:08.000000 mp-api-0.9.1/src/mp_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/test_files/
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-09-29 00:03:59.000000 mp-api-0.9.1/test_files/Si_mp_149.cif
+-rw-r--r--   0 runner    (1001) docker     (121)    65661 2021-09-29 00:03:59.000000 mp-api-0.9.1/test_files/calcs_reversed_mp_1031016.json
+-rw-r--r--   0 runner    (1001) docker     (121)  1340258 2021-09-29 00:04:00.000000 mp-api-0.9.1/test_files/materials_Li_Fe_V.json
+-rw-r--r--   0 runner    (1001) docker     (121)     9125 2021-09-29 00:04:00.000000 mp-api-0.9.1/test_files/synth_doc.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5420 2021-09-29 00:04:00.000000 mp-api-0.9.1/test_files/synth_doc_adaptor.json
+-rw-r--r--   0 runner    (1001) docker     (121)    10805 2021-09-29 00:04:00.000000 mp-api-0.9.1/test_files/synth_doc_adaptor_synpro.json
+-rw-r--r--   0 runner    (1001) docker     (121)  4920115 2021-09-29 00:04:00.000000 mp-api-0.9.1/test_files/tasks_Li_Fe_V.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1263 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1617 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/core/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1894 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2742 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/dielectric/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2822 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/elasticity/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2763 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2790 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/electrodes/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3850 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/electrodes/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5785 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/electronic_structure/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5044 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/eos/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2695 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/eos/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3038 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/grain_boundary/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1759 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2796 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/magnetism/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1928 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/materials/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3069 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/materials/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5829 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2867 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/molecules/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1965 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/piezo/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/piezo/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/robocrys/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1895 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/substrates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3028 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/substrates/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/summary/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3442 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2787 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/surface_properties/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2886 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5925 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/synthesis/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7514 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3332 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/tasks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2183 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/tasks/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10481 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/test_mprester.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/thermo/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3684 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/thermo/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:08.000000 mp-api-0.9.1/tests/xas/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3579 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/xas/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2021-09-29 00:04:00.000000 mp-api-0.9.1/tests/xas/test_query_operators.py
```

### Comparing `mp-api-0.9.0/.github/workflows/release.yaml` & `mp-api-0.9.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/.github/workflows/testing.yml` & `mp-api-0.9.1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/.gitignore` & `mp-api-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/CODE_OF_CONDUCT.md` & `mp-api-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/Dockerfile` & `mp-api-0.9.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/LICENSE` & `mp-api-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/PKG-INFO` & `mp-api-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mp-api
-Version: 0.9.0
+Version: 0.9.1
 Summary: API Server for the Materials Project
 Home-page: https://github.com/materialsproject/api
 Author: The Materials Project
 Author-email: feedback@materialsproject.org
 License: modified BSD
 Description: # The Materials Project API
```

### Comparing `mp-api-0.9.0/README.md` & `mp-api-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/app.py` & `mp-api-0.9.1/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         key="task_id",
         collection_name="surface_properties",
     )
 
     robo_store = MongoURIStore(
         uri=f"mongodb+srv://{db_uri}",
         database="mp_core",
-        key="task_id",
+        key="material_id",
         collection_name="robocrys",
     )
 
     synth_store = MongoURIStore(
         uri=f"mongodb+srv://{db_uri}",
         database="mp_core",
         key="_id",
```

### Comparing `mp-api-0.9.0/setup.py` & `mp-api-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/__init__.py` & `mp-api-0.9.1/src/mp_api/__init__.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/core/api.py` & `mp-api-0.9.1/src/mp_api/core/api.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/core/assets/mp_logo.svg` & `mp-api-0.9.1/src/mp_api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/core/assets/mp_logo_small.png` & `mp-api-0.9.1/src/mp_api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/core/client.py` & `mp-api-0.9.1/src/mp_api/core/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/core/documentation.py` & `mp-api-0.9.1/src/mp_api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/core/settings.py` & `mp-api-0.9.1/src/mp_api/core/settings.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/matproj.py` & `mp-api-0.9.1/src/mp_api/matproj.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,25 +467,26 @@
         return self.charge_density.get_charge_density_from_material_id(material_id)  # type: ignore
 
     def query(
         self,
         material_ids: Optional[List[MPID]] = None,
         chemsys_formula: Optional[str] = None,
         exclude_elements: Optional[List[str]] = None,
+        possible_species: Optional[List[str]] = None,
         nsites: Optional[Tuple[int, int]] = None,
         volume: Optional[Tuple[float, float]] = None,
         density: Optional[Tuple[float, float]] = None,
         crystal_system: Optional[CrystalSystem] = None,
         spacegroup_number: Optional[int] = None,
         spacegroup_symbol: Optional[str] = None,
         deprecated: Optional[bool] = None,
         total_energy: Optional[Tuple[float, float]] = None,
         formation_energy: Optional[Tuple[float, float]] = None,
         energy_above_hull: Optional[Tuple[float, float]] = None,
-        equillibrium_reaction_energy: Optional[Tuple[float, float]] = None,
+        equilibrium_reaction_energy: Optional[Tuple[float, float]] = None,
         uncorrected_energy: Optional[Tuple[float, float]] = None,
         is_stable: Optional[bool] = None,
         band_gap: Optional[Tuple[float, float]] = None,
         efermi: Optional[Tuple[float, float]] = None,
         is_gap_direct: Optional[bool] = None,
         is_metal: Optional[bool] = None,
         magnetic_ordering: Optional[Ordering] = None,
@@ -528,22 +529,26 @@
 
         Arguments:
             material_ids (List[MPID]): List of Materials Project IDs to return data for.
             chemsys_formula (str): A chemical system (e.g., Li-Fe-O),
                 or formula including anonomyzed formula
                 or wild cards (e.g., Fe2O3, ABO3, Si*).
             exclude_elements (List(str)): List of elements to exclude.
+            possible_species (List(str)): List of element symbols appended with oxidation states.
+                (e.g. Cr2+,O2-)
             crystal_system (CrystalSystem): Crystal system of material.
             spacegroup_number (int): Space group number of material.
             spacegroup_symbol (str): Space group symbol of the material in international short symbol notation.
             nsites (Tuple[int,int]): Minimum and maximum number of sites to consider.
             volume (Tuple[float,float]): Minimum and maximum volume to consider.
             density (Tuple[float,float]): Minimum and maximum density to consider.
             deprecated (bool): Whether the material is tagged as deprecated.
             total_energy (Tuple[int,int]): Minimum and maximum corrected total energy in eV/atom to consider.
+            equilibrium_reaction_energy (Tuple[float,float]): Minimum and maximum equilibrium reaction energy
+                in eV/atom to consider.
             formation_energy (Tuple[int,int]): Minimum and maximum formation energy in eV/atom to consider.
             energy_above_hull (Tuple[int,int]): Minimum and maximum energy above the hull in eV/atom to consider.
             uncorrected_energy (Tuple[int,int]): Minimum and maximum uncorrected total energy in eV/atom to consider.
             band_gap (Tuple[float,float]): Minimum and maximum band gap in eV to consider.
             efermi (Tuple[float,float]): Minimum and maximum fermi energy in eV to consider.
             is_gap_direct (bool): Whether the material has a direct band gap.
             is_metal (bool): Whether the material is considered a metal.
@@ -598,25 +603,26 @@
             ([SummaryDoc]) List of SummaryDoc documents
         """
 
         return self.summary.search_summary_docs(  # type: ignore
             material_ids=material_ids,
             chemsys_formula=chemsys_formula,
             exclude_elements=exclude_elements,
+            possible_species=possible_species,
             nsites=nsites,
             volume=volume,
             density=density,
             crystal_system=crystal_system,
             spacegroup_number=spacegroup_number,
             spacegroup_symbol=spacegroup_symbol,
             deprecated=deprecated,
             total_energy=total_energy,
             formation_energy=formation_energy,
             energy_above_hull=energy_above_hull,
-            equillibrium_reaction_energy=equillibrium_reaction_energy,
+            equilibrium_reaction_energy=equilibrium_reaction_energy,
             uncorrected_energy=uncorrected_energy,
             is_stable=is_stable,
             band_gap=band_gap,
             efermi=efermi,
             is_gap_direct=is_gap_direct,
             is_metal=is_metal,
             magnetic_ordering=magnetic_ordering,
```

### Comparing `mp-api-0.9.0/src/mp_api/routes/__init__.py` & `mp-api-0.9.1/src/mp_api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/_consumer/client.py` & `mp-api-0.9.1/src/mp_api/routes/_consumer/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/_consumer/query_operator.py` & `mp-api-0.9.1/src/mp_api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/_consumer/resources.py` & `mp-api-0.9.1/src/mp_api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/charge_density/client.py` & `mp-api-0.9.1/src/mp_api/routes/charge_density/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/charge_density/models.py` & `mp-api-0.9.1/src/mp_api/routes/charge_density/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/charge_density/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/charge_density/resources.py` & `mp-api-0.9.1/src/mp_api/routes/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/dielectric/client.py` & `mp-api-0.9.1/src/mp_api/routes/dielectric/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/dielectric/models.py` & `mp-api-0.9.1/src/mp_api/routes/dielectric/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/dielectric/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/dielectric/resources.py` & `mp-api-0.9.1/src/mp_api/routes/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/dois/resources.py` & `mp-api-0.9.1/src/mp_api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/elasticity/client.py` & `mp-api-0.9.1/src/mp_api/routes/elasticity/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/elasticity/models.py` & `mp-api-0.9.1/src/mp_api/routes/elasticity/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/elasticity/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/elasticity/resources.py` & `mp-api-0.9.1/src/mp_api/routes/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/electrodes/client.py` & `mp-api-0.9.1/src/mp_api/routes/electrodes/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/electrodes/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/electrodes/resources.py` & `mp-api-0.9.1/src/mp_api/routes/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/electronic_structure/client.py` & `mp-api-0.9.1/src/mp_api/routes/electronic_structure/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/electronic_structure/client.pyi` & `mp-api-0.9.1/src/mp_api/routes/electronic_structure/client.pyi`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/electronic_structure/models/doc.py` & `mp-api-0.9.1/src/mp_api/routes/electronic_structure/models/doc.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/electronic_structure/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/electronic_structure/resources.py` & `mp-api-0.9.1/src/mp_api/routes/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/eos/client.py` & `mp-api-0.9.1/src/mp_api/routes/eos/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/eos/models.py` & `mp-api-0.9.1/src/mp_api/routes/eos/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/eos/resources.py` & `mp-api-0.9.1/src/mp_api/routes/eos/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/fermi/models.py` & `mp-api-0.9.1/src/mp_api/routes/fermi/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/fermi/resources.py` & `mp-api-0.9.1/src/mp_api/routes/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/grain_boundary/client.py` & `mp-api-0.9.1/src/mp_api/routes/grain_boundary/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/grain_boundary/models.py` & `mp-api-0.9.1/src/mp_api/routes/grain_boundary/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/grain_boundary/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/grain_boundary/resources.py` & `mp-api-0.9.1/src/mp_api/routes/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/magnetism/client.py` & `mp-api-0.9.1/src/mp_api/routes/magnetism/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/magnetism/models.py` & `mp-api-0.9.1/src/mp_api/routes/magnetism/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/magnetism/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/magnetism/resources.py` & `mp-api-0.9.1/src/mp_api/routes/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/materials/client.py` & `mp-api-0.9.1/src/mp_api/routes/materials/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/materials/models/doc.py` & `mp-api-0.9.1/src/mp_api/routes/materials/models/doc.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/materials/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/materials/resources.py` & `mp-api-0.9.1/src/mp_api/routes/materials/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/materials/utils.py` & `mp-api-0.9.1/src/mp_api/routes/materials/utils.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/molecules/client.py` & `mp-api-0.9.1/src/mp_api/routes/molecules/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/molecules/models.py` & `mp-api-0.9.1/src/mp_api/routes/molecules/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/molecules/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/molecules/resources.py` & `mp-api-0.9.1/src/mp_api/routes/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/mpcomplete/models.py` & `mp-api-0.9.1/src/mp_api/routes/mpcomplete/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/mpcomplete/query_operator.py` & `mp-api-0.9.1/src/mp_api/routes/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/mpcomplete/resources.py` & `mp-api-0.9.1/src/mp_api/routes/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/oxidation_states/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/oxidation_states/resources.py` & `mp-api-0.9.1/src/mp_api/routes/oxidation_states/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.oxidation_states import OxidationStateDoc
 
 from maggma.api.query_operator import (
     PaginationQuery,
     SortQuery,
     SparseFieldsQuery,
-    NumericQuery,
 )
 
 from mp_api.routes.materials.query_operators import FormulaQuery
 from mp_api.routes.oxidation_states.query_operators import PossibleOxiStateQuery
 
 
 def oxi_states_resource(oxi_states_store):
```

### Comparing `mp-api-0.9.0/src/mp_api/routes/phonon/models.py` & `mp-api-0.9.1/src/mp_api/routes/phonon/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/phonon/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/phonon/resources.py` & `mp-api-0.9.1/src/mp_api/routes/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/piezo/client.py` & `mp-api-0.9.1/src/mp_api/routes/piezo/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/piezo/models.py` & `mp-api-0.9.1/src/mp_api/routes/piezo/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/piezo/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/piezo/resources.py` & `mp-api-0.9.1/src/mp_api/routes/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/provenance/resources.py` & `mp-api-0.9.1/src/mp_api/routes/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/robocrys/client.py` & `mp-api-0.9.1/src/mp_api/routes/robocrys/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from mp_api.routes.robocrys.models import RobocrysDoc
 
 
 class RobocrysRester(BaseRester):
 
     suffix = "robocrys"
     document_model = RobocrysDoc  # type: ignore
-    primary_key = "task_id"
+    primary_key = "material_id"
 
     def search_robocrys_text(self, keywords: List[str]):
         """
         Search text generated from Robocrystallographer.
 
         Arguments:
             keywords (List[str]): List of search keywords
```

### Comparing `mp-api-0.9.0/src/mp_api/routes/robocrys/models.py` & `mp-api-0.9.1/src/mp_api/routes/robocrys/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,72 +6,63 @@
 
 class MineralData(BaseModel):
     """
     Model for mineral data in the condensed structure robocrystallographer field
     """
 
     type: str = Field(
-        None,
-        description="Mineral type.",
+        None, description="Mineral type.",
     )
 
 
 class CondensedStructureData(BaseModel):
     """
     Model for data in the condensed structure robocrystallographer field
     """
 
     formula: str = Field(
-        None,
-        description="Formula for the material.",
+        None, description="Formula for the material.",
     )
 
     spg_symbol: str = Field(
-        None,
-        description="Space group symbol of the material.",
+        None, description="Space group symbol of the material.",
     )
 
     crystal_system: str = Field(
-        None,
-        description="Crystal system of the material.",
+        None, description="Crystal system of the material.",
     )
 
     mineral: MineralData = Field(
-        None,
-        description="Matched mineral data for the material.",
+        None, description="Matched mineral data for the material.",
     )
 
     dimensionality: int = Field(
-        None,
-        description="Dimensionality of the material.",
+        None, description="Dimensionality of the material.",
     )
 
 
 class RobocrysDoc(BaseModel):
     """
     Structural features, mineral prototypes, dimensionality, ...
     """
 
     description: str = Field(
-        None,
-        description="Decription text from robocrytallographer.",
+        None, description="Decription text from robocrytallographer.",
     )
 
     condensed_structure: CondensedStructureData = Field(
-        None,
-        description="Condensed structure data from robocrytallographer.",
+        None, description="Condensed structure data from robocrytallographer.",
     )
 
-    task_id: str = Field(
+    material_id: str = Field(
         None,
         description="The Materials Project ID of the material. This comes in the form: mp-******",
     )
 
     last_updated: datetime = Field(
-        None,
-        description="Timestamp for the most recent calculation for this document",
+        None, description="Timestamp for the most recent calculation for this document",
     )
 
     # Make sure that the datetime field is properly formatted
     @validator("last_updated", pre=True)
     def last_updated_dict_ok(cls, v):
         return MontyDecoder().process_decoded(v)
```

### Comparing `mp-api-0.9.0/src/mp_api/routes/robocrys/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/robocrys/resources.py` & `mp-api-0.9.1/src/mp_api/routes/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/similarity/models.py` & `mp-api-0.9.1/src/mp_api/routes/similarity/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/similarity/resources.py` & `mp-api-0.9.1/src/mp_api/routes/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/substrates/client.py` & `mp-api-0.9.1/src/mp_api/routes/substrates/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/substrates/models.py` & `mp-api-0.9.1/src/mp_api/routes/substrates/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/substrates/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/substrates/resources.py` & `mp-api-0.9.1/src/mp_api/routes/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/summary/client.py` & `mp-api-0.9.1/src/mp_api/routes/summary/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,26 @@
     primary_key = "material_id"
 
     def search_summary_docs(
         self,
         material_ids: Optional[List[MPID]] = None,
         chemsys_formula: Optional[str] = None,
         exclude_elements: Optional[List[str]] = None,
+        possible_species: Optional[List[str]] = None,
         nsites: Optional[Tuple[int, int]] = None,
         volume: Optional[Tuple[float, float]] = None,
         density: Optional[Tuple[float, float]] = None,
         crystal_system: Optional[CrystalSystem] = None,
         spacegroup_number: Optional[int] = None,
         spacegroup_symbol: Optional[str] = None,
         deprecated: Optional[bool] = None,
         total_energy: Optional[Tuple[float, float]] = None,
         formation_energy: Optional[Tuple[float, float]] = None,
         energy_above_hull: Optional[Tuple[float, float]] = None,
-        equillibrium_reaction_energy: Optional[Tuple[float, float]] = None,
+        equilibrium_reaction_energy: Optional[Tuple[float, float]] = None,
         uncorrected_energy: Optional[Tuple[float, float]] = None,
         is_stable: Optional[bool] = None,
         band_gap: Optional[Tuple[float, float]] = None,
         efermi: Optional[Tuple[float, float]] = None,
         is_gap_direct: Optional[bool] = None,
         is_metal: Optional[bool] = None,
         magnetic_ordering: Optional[Ordering] = None,
@@ -76,22 +77,26 @@
 
         Arguments:
             material_ids (List[MPID]): List of Materials Project IDs to return data for.
             chemsys_formula (str): A chemical system (e.g., Li-Fe-O),
                 or formula including anonomyzed formula
                 or wild cards (e.g., Fe2O3, ABO3, Si*).
             exclude_elements (List(str)): List of elements to exclude.
+            possible_species (List(str)): List of element symbols appended with oxidation states.
+                (e.g. Cr2+,O2-)
             crystal_system (CrystalSystem): Crystal system of material.
             spacegroup_number (int): Space group number of material.
             spacegroup_symbol (str): Space group symbol of the material in international short symbol notation.
             nsites (Tuple[int,int]): Minimum and maximum number of sites to consider.
             volume (Tuple[float,float]): Minimum and maximum volume to consider.
             density (Tuple[float,float]): Minimum and maximum density to consider.
             deprecated (bool): Whether the material is tagged as deprecated.
             total_energy (Tuple[int,int]): Minimum and maximum corrected total energy in eV/atom to consider.
+            equilibrium_reaction_energy (Tuple[float,float]): Minimum and maximum equilibrium reaction energy
+                in eV/atom to consider.
             formation_energy (Tuple[int,int]): Minimum and maximum formation energy in eV/atom to consider.
             energy_above_hull (Tuple[int,int]): Minimum and maximum energy above the hull in eV/atom to consider.
             uncorrected_energy (Tuple[int,int]): Minimum and maximum uncorrected total energy in eV/atom to consider.
             band_gap (Tuple[float,float]): Minimum and maximum band gap in eV to consider.
             efermi (Tuple[float,float]): Minimum and maximum fermi energy in eV to consider.
             is_gap_direct (bool): Whether the material has a direct band gap.
             is_metal (bool): Whether the material is considered a metal.
@@ -149,15 +154,15 @@
         query_params = defaultdict(dict)  # type: dict
 
         min_max_name_dict = {
             "total_energy": "energy_per_atom",
             "formation_energy": "formation_energy_per_atom",
             "energy_above_hull": "energy_above_hull",
             "uncorrected_energy": "uncorrected_energy_per_atom",
-            "equillibrium_reaction_energy": "equillibrium_reaction_energy_per_atom",
+            "equilibrium_reaction_energy": "equilibrium_reaction_energy_per_atom",
             "nsites": "nsites",
             "volume": "volume",
             "density": "density",
             "band_gap": "band_gap",
             "efermi": "efermi",
             "total_magnetization": "total_magnetization",
             "total_magnetization_normalized_vol": "total_magnetization_normalized_vol",
@@ -200,14 +205,17 @@
 
         if chemsys_formula:
             query_params.update({"formula": chemsys_formula})
 
         if exclude_elements is not None:
             query_params.update({"exclude_elements": ",".join(exclude_elements)})
 
+        if possible_species is not None:
+            query_params.update({"possible_species": ",".join(possible_species)})
+
         query_params.update(
             {
                 "crystal_system": crystal_system,
                 "spacegroup_number": spacegroup_number,
                 "spacegroup_symbol": spacegroup_symbol,
             }
         )
```

### Comparing `mp-api-0.9.0/src/mp_api/routes/summary/models.py` & `mp-api-0.9.1/src/mp_api/routes/summary/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/summary/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/summary/resources.py` & `mp-api-0.9.1/src/mp_api/routes/summary/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from maggma.api.resource import ReadOnlyResource, AggregationResource
 from mp_api.routes.materials.query_operators import (
     DeprecationQuery,
     ElementsQuery,
     FormulaQuery,
     SymmetryQuery,
 )
+from mp_api.routes.oxidation_states.query_operators import PossibleOxiStateQuery
 from emmet.core.summary import SummaryStats
 from mp_api.routes.summary.query_operators import (
     HasPropsQuery,
     MaterialIDsSearchQuery,
     SearchIsStableQuery,
     SearchIsTheoreticalQuery,
     SearchMagneticQuery,
@@ -30,14 +31,15 @@
     resource = ReadOnlyResource(
         summary_store,
         SummaryDoc,
         query_operators=[
             MaterialIDsSearchQuery(),
             FormulaQuery(),
             ElementsQuery(),
+            PossibleOxiStateQuery(),
             SymmetryQuery(),
             SearchIsStableQuery(),
             SearchIsTheoreticalQuery(),
             SearchMagneticQuery(),
             SearchESQuery(),
             NumericQuery(model=SummaryDoc, excluded_fields=["composition"]),
             SearchHasReconstructedQuery(),
```

### Comparing `mp-api-0.9.0/src/mp_api/routes/surface_properties/client.py` & `mp-api-0.9.1/src/mp_api/routes/surface_properties/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/surface_properties/models.py` & `mp-api-0.9.1/src/mp_api/routes/surface_properties/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/surface_properties/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/surface_properties/resources.py` & `mp-api-0.9.1/src/mp_api/routes/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/client.py` & `mp-api-0.9.1/src/mp_api/routes/synthesis/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/client.pyi` & `mp-api-0.9.1/src/mp_api/routes/synthesis/client.pyi`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/data_adaptor.py` & `mp-api-0.9.1/src/mp_api/routes/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/data_adaptor_synpro.py` & `mp-api-0.9.1/src/mp_api/routes/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/models/core.py` & `mp-api-0.9.1/src/mp_api/routes/synthesis/models/core.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/models/materials.py` & `mp-api-0.9.1/src/mp_api/routes/synthesis/models/materials.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/models/operations.py` & `mp-api-0.9.1/src/mp_api/routes/synthesis/models/operations.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/models/reaction.py` & `mp-api-0.9.1/src/mp_api/routes/synthesis/models/reaction.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/resources.py` & `mp-api-0.9.1/src/mp_api/routes/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/synthesis/utils.py` & `mp-api-0.9.1/src/mp_api/routes/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/tasks/client.py` & `mp-api-0.9.1/src/mp_api/routes/tasks/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/tasks/models.py` & `mp-api-0.9.1/src/mp_api/routes/tasks/models.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/tasks/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/tasks/resources.py` & `mp-api-0.9.1/src/mp_api/routes/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/tasks/utils.py` & `mp-api-0.9.1/src/mp_api/routes/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/thermo/client.py` & `mp-api-0.9.1/src/mp_api/routes/thermo/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         material_ids: Optional[List[str]] = None,
         chemsys_formula: Optional[str] = None,
         nelements: Optional[Tuple[int, int]] = None,
         is_stable: Optional[bool] = None,
         total_energy: Optional[Tuple[float, float]] = None,
         formation_energy: Optional[Tuple[float, float]] = None,
         energy_above_hull: Optional[Tuple[float, float]] = None,
-        equillibrium_reaction_energy: Optional[Tuple[float, float]] = None,
+        equilibrium_reaction_energy: Optional[Tuple[float, float]] = None,
         uncorrected_energy: Optional[Tuple[float, float]] = None,
         sort_field: Optional[str] = None,
         ascending: Optional[bool] = None,
         num_chunks: Optional[int] = None,
         chunk_size: int = 1000,
         all_fields: bool = True,
         fields: Optional[List[str]] = None,
@@ -39,15 +39,15 @@
                 or formula including anonomyzed formula
                 or wild cards (e.g., Fe2O3, ABO3, Si*).
             nelements (Tuple[int,int]): Minimum and maximum number of elements in the material to consider.
             is_stable (bool): Whether the material is stable.
             total_energy (Tuple[float,float]): Minimum and maximum corrected total energy in eV/atom to consider.
             formation_energy (Tuple[float,float]): Minimum and maximum formation energy in eV/atom to consider.
             energy_above_hull (Tuple[float,float]): Minimum and maximum energy above the hull in eV/atom to consider.
-            equillibrium_reaction_energy (Tuple[float,float]): Minimum and maximum equilibrium reaction energy
+            equilibrium_reaction_energy (Tuple[float,float]): Minimum and maximum equilibrium reaction energy
                 in eV/atom to consider.
             uncorrected_energy (Tuple[float,float]): Minimum and maximum uncorrected total
                 energy in eV/atom to consider.
             sort_field (str): Field used to sort results.
             ascending (bool): Whether sorting should be in ascending order.
             num_chunks (int): Maximum number of chunks of data to yield. None will yield all possible.
             chunk_size (int): Number of data entries per chunk.
@@ -81,15 +81,15 @@
         if ascending is not None:
             query_params.update({"ascending": ascending})
 
         name_dict = {
             "total_energy": "energy_per_atom",
             "formation_energy": "formation_energy_per_atom",
             "energy_above_hull": "energy_above_hull",
-            "equillibrium_reaction_energy": "equillibrium_reaction_energy_per_atom",
+            "equilibrium_reaction_energy": "equilibrium_reaction_energy_per_atom",
             "uncorrected_energy": "uncorrected_energy_per_atom",
         }
 
         for param, value in locals().items():
             if "energy" in param and value:
                 query_params.update(
                     {
```

### Comparing `mp-api-0.9.0/src/mp_api/routes/thermo/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/thermo/resources.py` & `mp-api-0.9.1/src/mp_api/routes/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/xas/client.py` & `mp-api-0.9.1/src/mp_api/routes/xas/client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/xas/query_operators.py` & `mp-api-0.9.1/src/mp_api/routes/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api/routes/xas/resources.py` & `mp-api-0.9.1/src/mp_api/routes/xas/resources.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/src/mp_api.egg-info/PKG-INFO` & `mp-api-0.9.1/src/mp_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mp-api
-Version: 0.9.0
+Version: 0.9.1
 Summary: API Server for the Materials Project
 Home-page: https://github.com/materialsproject/api
 Author: The Materials Project
 Author-email: feedback@materialsproject.org
 License: modified BSD
 Description: # The Materials Project API
```

### Comparing `mp-api-0.9.0/src/mp_api.egg-info/SOURCES.txt` & `mp-api-0.9.1/src/mp_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/test_files/Si_mp_149.cif` & `mp-api-0.9.1/test_files/Si_mp_149.cif`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/test_files/calcs_reversed_mp_1031016.json` & `mp-api-0.9.1/test_files/calcs_reversed_mp_1031016.json`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/test_files/materials_Li_Fe_V.json` & `mp-api-0.9.1/test_files/materials_Li_Fe_V.json`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/test_files/synth_doc.json` & `mp-api-0.9.1/test_files/synth_doc.json`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/test_files/synth_doc_adaptor.json` & `mp-api-0.9.1/test_files/synth_doc_adaptor.json`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/test_files/synth_doc_adaptor_synpro.json` & `mp-api-0.9.1/test_files/synth_doc_adaptor_synpro.json`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/test_files/tasks_Li_Fe_V.json` & `mp-api-0.9.1/test_files/tasks_Li_Fe_V.json`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/_consumer/test_query_operators.py` & `mp-api-0.9.1/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/charge_density/test_query_operators.py` & `mp-api-0.9.1/tests/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/core/test_client.py` & `mp-api-0.9.1/tests/core/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/core/test_mapi.py` & `mp-api-0.9.1/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/dielectric/test_client.py` & `mp-api-0.9.1/tests/dielectric/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/dielectric/test_query_operators.py` & `mp-api-0.9.1/tests/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/elasticity/test_client.py` & `mp-api-0.9.1/tests/elasticity/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/elasticity/test_query_operators.py` & `mp-api-0.9.1/tests/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/electrodes/test_client.py` & `mp-api-0.9.1/tests/electrodes/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/electrodes/test_query_operators.py` & `mp-api-0.9.1/tests/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/electronic_structure/test_client.py` & `mp-api-0.9.1/tests/electronic_structure/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,25 +96,24 @@
                 assert (
                     doc[project_field if project_field is not None else param]
                     is not None
                 )
 
 
 bs_custom_field_tests = {
-    "path_type": BSPathType.setyawan_curtarolo,
     "magnetic_ordering": Ordering.FM,
     "is_metal": True,
     "is_gap_direct": True,
     "efermi": (0, 100),
     "band_gap": (0, 5),
 }
 
 bs_sub_doc_fields = ["bandstructure"]
 
-bs_alt_name_dict = {"path_type": "setyawan_curtarolo"}  # type: dict
+bs_alt_name_dict = {}  # type: dict
 
 
 @pytest.fixture
 def bs_rester():
     rester = BandStructureRester()
     yield rester
     rester.session.close()
@@ -135,38 +134,40 @@
         project_field = bs_alt_name_dict.get(param, None)
         q = {
             param: bs_custom_field_tests[param],
             "chunk_size": 1,
             "num_chunks": 1,
         }
         doc = search_method(**q)[0].dict()
+        print(q)
+        print(doc)
         for sub_field in bs_sub_doc_fields:
             if sub_field in doc:
                 doc = doc[sub_field]
 
         if param != "path_type":
             doc = doc["setyawan_curtarolo"]
 
+        print("=====")
+        print(doc)
+
         assert doc[project_field if project_field is not None else param] is not None
 
 
 dos_custom_field_tests = {
-    "projection_type": DOSProjectionType.total,
     "magnetic_ordering": Ordering.FM,
     "efermi": (0, 100),
     "band_gap": (0, 5),
 }
 
 dos_excluded_params = ["orbital", "element"]
 
 dos_sub_doc_fields = ["dos"]
 
-dos_alt_name_dict = {
-    "projection_type": "total",
-}  # type: dict
+dos_alt_name_dict = {}  # type: dict
 
 
 @pytest.fixture
 def dos_rester():
     rester = DosRester()
     yield rester
     rester.session.close()
```

### Comparing `mp-api-0.9.0/tests/electronic_structure/test_query_operators.py` & `mp-api-0.9.1/tests/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/eos/test_client.py` & `mp-api-0.9.1/tests/eos/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/grain_boundary/test_client.py` & `mp-api-0.9.1/tests/grain_boundary/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/grain_boundary/test_query_operators.py` & `mp-api-0.9.1/tests/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/magnetism/test_client.py` & `mp-api-0.9.1/tests/magnetism/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/magnetism/test_query_operators.py` & `mp-api-0.9.1/tests/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/materials/test_client.py` & `mp-api-0.9.1/tests/materials/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/materials/test_query_operators.py` & `mp-api-0.9.1/tests/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/materials/test_utils.py` & `mp-api-0.9.1/tests/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/molecules/test_client.py` & `mp-api-0.9.1/tests/molecules/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/molecules/test_query_operators.py` & `mp-api-0.9.1/tests/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/mpcomplete/test_query_operators.py` & `mp-api-0.9.1/tests/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/oxidation_states/test_query_operators.py` & `mp-api-0.9.1/tests/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/piezo/test_client.py` & `mp-api-0.9.1/tests/piezo/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/piezo/test_query_operators.py` & `mp-api-0.9.1/tests/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/robocrys/test_client.py` & `mp-api-0.9.1/tests/robocrys/test_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 @pytest.fixture
 def rester():
     rester = RobocrysRester()
     yield rester
     rester.session.close()
 
 
+@pytest.mark.xfail  # temp
 @pytest.mark.skipif(
     os.environ.get("MP_API_KEY", None) is None, reason="No API key found."
 )
 def test_client(rester):
     # Get specific search method
     search_method = None
     for entry in inspect.getmembers(rester, predicate=inspect.ismethod):
```

### Comparing `mp-api-0.9.0/tests/robocrys/test_query_operators.py` & `mp-api-0.9.1/tests/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/substrates/test_client.py` & `mp-api-0.9.1/tests/substrates/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/substrates/test_query_operators.py` & `mp-api-0.9.1/tests/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/summary/test_query_operators.py` & `mp-api-0.9.1/tests/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/surface_properties/test_client.py` & `mp-api-0.9.1/tests/surface_properties/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/surface_properties/test_query_operators.py` & `mp-api-0.9.1/tests/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/synthesis/test_adaptor.py` & `mp-api-0.9.1/tests/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/synthesis/test_adaptor_synpro.py` & `mp-api-0.9.1/tests/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/synthesis/test_client.py` & `mp-api-0.9.1/tests/synthesis/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/synthesis/test_query_operators.py` & `mp-api-0.9.1/tests/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/synthesis/test_utils.py` & `mp-api-0.9.1/tests/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/tasks/test_client.py` & `mp-api-0.9.1/tests/tasks/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/tasks/test_query_operators.py` & `mp-api-0.9.1/tests/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/tasks/test_utils.py` & `mp-api-0.9.1/tests/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/test_client.py` & `mp-api-0.9.1/tests/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 key_only_resters = {
     "phonon": "mp-11703",
     "similarity": "mp-149",
     "doi": "mp-149",
     "wulff": "mp-149",
     "charge_density": "mp-1936745",
-    "robocrys": "mp-149",
+    "provenance": "mp-149",
 }
 
 search_only_resters = [
     "grain_boundary",
     "electronic_structure_bandstructure",
     "electronic_structure_dos",
     "substrates",
     "synthesis",
 ]
 
 special_resters = [
     "charge_density",
 ]
 
-ignore_generic = ["provenance"]  # temp
+ignore_generic = ["robocrys"]  # temp
 
 
 mpr = MPRester()
 
 
 @pytest.mark.skipif(
     os.environ.get("MP_API_KEY", None) is None, reason="No API key found."
```

### Comparing `mp-api-0.9.0/tests/test_mprester.py` & `mp-api-0.9.1/tests/test_mprester.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     def test_get_database_version(self, mpr):
         db_version = mpr.get_database_version()
         assert db_version == MAPISettings().db_version
 
     def test_get_materials_id_from_task_id(self, mpr):
         assert mpr.get_materials_id_from_task_id("mp-540081") == "mp-19017"
 
-    @pytest.mark.xfail  # temp xfail while data is fixed
     def test_get_materials_id_references(self, mpr):
         data = mpr.get_materials_id_references("mp-123")
         assert len(data) > 5
 
     def test_get_materials_ids_doc(self, mpr):
         mpids = mpr.get_materials_ids("Al2O3")
         random.shuffle(mpids)
@@ -182,15 +181,15 @@
         assert mo_s3_112[0]["gb_energy"] == pytest.approx(0.4796547330588574)
         assert mo_s3_112[0]["w_sep"] == pytest.approx(6.318144)
 
     def test_get_wulff_shape(self, mpr):
         ws = mpr.get_wulff_shape("mp-126")
         assert isinstance(ws, WulffShape)
 
-    @pytest.mark.xfail  # temp xfail while data is fixed
+    @pytest.mark.xfail  # temporary until api deploy
     def test_query(self, mpr):
 
         excluded_params = [
             "sort_field",
             "ascending",
             "chunk_size",
             "num_chunks",
@@ -217,14 +216,15 @@
             "surface_energy_anisotropy": "surface_anisotropy",
         }  # type: dict
 
         custom_field_tests = {
             "material_ids": ["mp-149"],
             "chemsys_formula": "SiO2",
             "exclude_elements": ["Si"],
+            "possible_species": ["O2-"],
             "crystal_system": CrystalSystem.cubic,
             "spacegroup_number": 38,
             "spacegroup_symbol": "Amm2",
             "magnetic_ordering": Ordering.FM,
             "has_props": ["dielectric"],
             "theoretical": True,
             "has_reconstructed": False,
```

### Comparing `mp-api-0.9.0/tests/thermo/test_client.py` & `mp-api-0.9.1/tests/thermo/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 excluded_params = [
     "sort_field",
     "ascending",
     "chunk_size",
     "num_chunks",
     "all_fields",
     "fields",
-    "equillibrium_reaction_energy",
+    "equilibrium_reaction_energy",
 ]
 
 sub_doc_fields = []  # type: list
 
 alt_name_dict = {
     "chemsys_formula": "formula_pretty",
     "material_ids": "material_id",
     "total_energy": "energy_per_atom",
     "formation_energy": "formation_energy_per_atom",
     "uncorrected_energy": "uncorrected_energy_per_atom",
+    "equilibirum_reaction_energy": "equilibirum_reaction_energy_per_atom",
 }  # type: dict
 
 custom_field_tests = {
     "material_ids": ["mp-149"],
     "chemsys_formula": "Si-O",
 }  # type: dict
```

### Comparing `mp-api-0.9.0/tests/xas/test_client.py` & `mp-api-0.9.1/tests/xas/test_client.py`

 * *Files identical despite different names*

### Comparing `mp-api-0.9.0/tests/xas/test_query_operators.py` & `mp-api-0.9.1/tests/xas/test_query_operators.py`

 * *Files identical despite different names*

