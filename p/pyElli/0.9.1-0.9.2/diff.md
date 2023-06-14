# Comparing `tmp/pyElli-0.9.1.tar.gz` & `tmp/pyElli-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyElli-0.9.1.tar", last modified: Mon Nov 15 10:06:38 2021, max compression
+gzip compressed data, was "pyElli-0.9.2.tar", last modified: Tue Nov 23 13:37:34 2021, max compression
```

## Comparing `pyElli-0.9.1.tar` & `pyElli-0.9.2.tar`

### file list

```diff
@@ -1,117 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.552113 pyElli-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-11-15 10:06:29.000000 pyElli-0.9.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.528113 pyElli-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.540113 pyElli-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2021-11-15 10:06:29.000000 pyElli-0.9.1/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (121)      963 2021-11-15 10:06:29.000000 pyElli-0.9.1/.github/workflows/build-docker.yml
--rw-r--r--   0 runner    (1001) docker     (121)      798 2021-11-15 10:06:29.000000 pyElli-0.9.1/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2021-11-15 10:06:29.000000 pyElli-0.9.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      569 2021-11-15 10:06:29.000000 pyElli-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      490 2021-11-15 10:06:29.000000 pyElli-0.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-11-15 10:06:29.000000 pyElli-0.9.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)      750 2021-11-15 10:06:29.000000 pyElli-0.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     4430 2021-11-15 10:06:29.000000 pyElli-0.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-11-15 10:06:29.000000 pyElli-0.9.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)    32473 2021-11-15 10:06:29.000000 pyElli-0.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2021-11-15 10:06:38.552113 pyElli-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2021-11-15 10:06:29.000000 pyElli-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.544113 pyElli-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2021-11-15 10:06:29.000000 pyElli-0.9.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.544113 pyElli-0.9.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-11-15 10:06:29.000000 pyElli-0.9.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-11-15 10:06:29.000000 pyElli-0.9.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-15 10:06:29.000000 pyElli-0.9.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9820 2021-11-15 10:06:29.000000 pyElli-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-11-15 10:06:29.000000 pyElli-0.9.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2021-11-15 10:06:29.000000 pyElli-0.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-11-15 10:06:29.000000 pyElli-0.9.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-11-15 10:06:29.000000 pyElli-0.9.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      303 2021-11-15 10:06:29.000000 pyElli-0.9.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.532113 pyElli-0.9.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.544113 pyElli-0.9.1/examples/Bragg-mirror/
--rw-r--r--   0 runner    (1001) docker     (121)    48875 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Bragg-mirror/Bragg-example.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (121)     1875 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Bragg-mirror/Bragg-example.py
--rw-r--r--   0 runner    (1001) docker     (121)    91509 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Bragg-mirror/validation-Bragg.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (121)     4253 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Bragg-mirror/validation-Bragg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.544113 pyElli-0.9.1/examples/Ellipsometry uniaxial materials/
--rw-r--r--   0 runner    (1001) docker     (121)    60367 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Ellipsometry uniaxial materials/Fujiwara-641.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Ellipsometry uniaxial materials/Fujiwara-641.py
--rw-r--r--   0 runner    (1001) docker     (121)    51179 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Ellipsometry uniaxial materials/Fujiwara-642.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     5982 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Ellipsometry uniaxial materials/Fujiwara-642.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.544113 pyElli-0.9.1/examples/Interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)    56105 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Interfaces/Interferences.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Interfaces/Interferences.py
--rw-r--r--   0 runner    (1001) docker     (121)    84552 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Interfaces/interface-reflection.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2647 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Interfaces/interface-reflection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.544113 pyElli-0.9.1/examples/Liquid crystals/
--rw-r--r--   0 runner    (1001) docker     (121)    79815 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Liquid crystals/cholesteric-example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     4155 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Liquid crystals/cholesteric-example.py
--rw-r--r--   0 runner    (1001) docker     (121)    47268 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Liquid crystals/twisted-nematic.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Liquid crystals/twisted-nematic.py
--rw-r--r--   0 runner    (1001) docker     (121)    41845 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Liquid crystals/validation-cholesteric.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Liquid crystals/validation-cholesteric.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.544113 pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.548113 pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/.ipynb_checkpoints/
--rw-r--r--   0 runner    (1001) docker     (121)     7164 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/.ipynb_checkpoints/SiO2_Si Mueller Matrix-checkpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9764 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/.ipynb_checkpoints/Si_Aspnes-checkpoint.mat
--rw-r--r--   0 runner    (1001) docker     (121)   325221 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/.ipynb_checkpoints/Wafer_MM_70-checkpoint.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11329 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/SiO2_Si Mueller Matrix.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9764 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/Si_Aspnes.mat
--rw-r--r--   0 runner    (1001) docker     (121)   325221 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/Wafer_MM_70.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.548113 pyElli-0.9.1/examples/TiO2 Fit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.548113 pyElli-0.9.1/examples/TiO2 Fit/.ipynb_checkpoints/
--rw-r--r--   0 runner    (1001) docker     (121)    14645 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/TiO2 Fit/.ipynb_checkpoints/TiO2 Multilayerfit-checkpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3444 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/TiO2 Fit/.ipynb_checkpoints/TiO2 Multilayerfit-checkpoint.md
--rw-r--r--   0 runner    (1001) docker     (121)     9764 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/TiO2 Fit/Si_Aspnes.mat
--rw-r--r--   0 runner    (1001) docker     (121)    14645 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/TiO2 Fit/TiO2 Multilayerfit.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3461 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/TiO2 Fit/TiO2 Multilayerfit.md
--rw-r--r--   0 runner    (1001) docker     (121)    36583 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/TiO2 Fit/TiO2_400cycles.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.548113 pyElli-0.9.1/examples/Total internal reflection/
--rw-r--r--   0 runner    (1001) docker     (121)   103247 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Total internal reflection/FrustratedTIR-angle.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (121)     3652 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Total internal reflection/FrustratedTIR-angle.py
--rw-r--r--   0 runner    (1001) docker     (121)    81476 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Total internal reflection/FrustratedTIR-thickness.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (121)     3549 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Total internal reflection/FrustratedTIR-thickness.py
--rw-r--r--   0 runner    (1001) docker     (121)    19784 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Total internal reflection/TIR.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2021-11-15 10:06:29.000000 pyElli-0.9.1/examples/Total internal reflection/TIR.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-11-15 10:06:29.000000 pyElli-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-11-15 10:06:29.000000 pyElli-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2021-11-15 10:06:38.552113 pyElli-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      653 2021-11-15 10:06:29.000000 pyElli-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.532113 pyElli-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.552113 pyElli-0.9.1/src/elli/
--rw-r--r--   0 runner    (1001) docker     (121)      982 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15148 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/dispersions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4271 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.552113 pyElli-0.9.1/src/elli/fitting/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9294 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/fitting/decorator_mmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    11601 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/fitting/decorator_psi_delta.py
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/fitting/params_hist.py
--rw-r--r--   0 runner    (1001) docker     (121)     5982 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/materials.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/materials_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/math.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.552113 pyElli-0.9.1/src/elli/plot/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/plot/mueller_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/plot/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/result.py
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/solver.py
--rw-r--r--   0 runner    (1001) docker     (121)     4807 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/solver2x2.py
--rw-r--r--   0 runner    (1001) docker     (121)    16190 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/solver4x4.py
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/spectraray.py
--rw-r--r--   0 runner    (1001) docker     (121)    13003 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2021-11-15 10:06:29.000000 pyElli-0.9.1/src/elli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.552113 pyElli-0.9.1/src/pyElli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2021-11-15 10:06:38.000000 pyElli-0.9.1/src/pyElli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2021-11-15 10:06:38.000000 pyElli-0.9.1/src/pyElli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 10:06:38.000000 pyElli-0.9.1/src/pyElli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 10:06:38.000000 pyElli-0.9.1/src/pyElli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-11-15 10:06:38.000000 pyElli-0.9.1/src/pyElli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-15 10:06:38.000000 pyElli-0.9.1/src/pyElli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 10:06:38.552113 pyElli-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2021-11-15 10:06:29.000000 pyElli-0.9.1/tests/benchmark_propagators_TiO2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3510 2021-11-15 10:06:29.000000 pyElli-0.9.1/tests/test_bragg_mirror.py
--rw-r--r--   0 runner    (1001) docker     (121)     7437 2021-11-15 10:06:29.000000 pyElli-0.9.1/tests/test_internal_reflection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2021-11-15 10:06:29.000000 pyElli-0.9.1/tests/test_liquid_crystals.py
--rw-r--r--   0 runner    (1001) docker     (121)     5234 2021-11-15 10:06:29.000000 pyElli-0.9.1/tests/test_uniaxial_crystals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2021-11-15 10:06:29.000000 pyElli-0.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.791232 pyElli-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-11-23 13:37:22.000000 pyElli-0.9.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.783232 pyElli-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.783232 pyElli-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2021-11-23 13:37:22.000000 pyElli-0.9.2/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2021-11-23 13:37:22.000000 pyElli-0.9.2/.github/workflows/build-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2021-11-23 13:37:22.000000 pyElli-0.9.2/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2021-11-23 13:37:22.000000 pyElli-0.9.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2021-11-23 13:37:22.000000 pyElli-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2021-11-23 13:37:22.000000 pyElli-0.9.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2021-11-23 13:37:22.000000 pyElli-0.9.2/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-11-23 13:37:22.000000 pyElli-0.9.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2021-11-23 13:37:22.000000 pyElli-0.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4430 2021-11-23 13:37:22.000000 pyElli-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2021-11-23 13:37:22.000000 pyElli-0.9.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)    32473 2021-11-23 13:37:22.000000 pyElli-0.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2922 2021-11-23 13:37:34.791232 pyElli-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2099 2021-11-23 13:37:22.000000 pyElli-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.783232 pyElli-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1154 2021-11-23 13:37:22.000000 pyElli-0.9.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.783232 pyElli-0.9.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-11-23 13:37:22.000000 pyElli-0.9.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-11-23 13:37:22.000000 pyElli-0.9.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-23 13:37:22.000000 pyElli-0.9.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9848 2021-11-23 13:37:22.000000 pyElli-0.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2021-11-23 13:37:22.000000 pyElli-0.9.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2021-11-23 13:37:22.000000 pyElli-0.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-11-23 13:37:22.000000 pyElli-0.9.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2021-11-23 13:37:22.000000 pyElli-0.9.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2021-11-23 13:37:22.000000 pyElli-0.9.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.783232 pyElli-0.9.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.787232 pyElli-0.9.2/examples/Bragg-mirror/
+-rw-r--r--   0 runner    (1001) docker     (121)    48875 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Bragg-mirror/Bragg-example.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1875 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Bragg-mirror/Bragg-example.py
+-rw-r--r--   0 runner    (1001) docker     (121)    91509 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Bragg-mirror/validation-Bragg.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4253 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Bragg-mirror/validation-Bragg.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.787232 pyElli-0.9.2/examples/Ellipsometry uniaxial materials/
+-rw-r--r--   0 runner    (1001) docker     (121)    60367 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Ellipsometry uniaxial materials/Fujiwara-641.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Ellipsometry uniaxial materials/Fujiwara-641.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51179 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Ellipsometry uniaxial materials/Fujiwara-642.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     5982 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Ellipsometry uniaxial materials/Fujiwara-642.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.787232 pyElli-0.9.2/examples/Interfaces/
+-rw-r--r--   0 runner    (1001) docker     (121)    56105 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Interfaces/Interferences.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Interfaces/Interferences.py
+-rw-r--r--   0 runner    (1001) docker     (121)    84552 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Interfaces/interface-reflection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     2647 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Interfaces/interface-reflection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.787232 pyElli-0.9.2/examples/Liquid crystals/
+-rw-r--r--   0 runner    (1001) docker     (121)    79815 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Liquid crystals/cholesteric-example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     4155 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Liquid crystals/cholesteric-example.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47268 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Liquid crystals/twisted-nematic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     2706 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Liquid crystals/twisted-nematic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41845 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Liquid crystals/validation-cholesteric.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     2429 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Liquid crystals/validation-cholesteric.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.787232 pyElli-0.9.2/examples/SiO2_Si Mueller Matrix/
+-rw-r--r--   0 runner    (1001) docker     (121)     7384 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/SiO2_Si Mueller Matrix/SiO2_Si Mueller Matrix.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     9764 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/SiO2_Si Mueller Matrix/Si_Aspnes.mat
+-rw-r--r--   0 runner    (1001) docker     (121)   325221 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/SiO2_Si Mueller Matrix/Wafer_MM_70.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.787232 pyElli-0.9.2/examples/TiO2 Fit/
+-rw-r--r--   0 runner    (1001) docker     (121)     9764 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/TiO2 Fit/Si_Aspnes.mat
+-rw-r--r--   0 runner    (1001) docker     (121)    10513 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/TiO2 Fit/TiO2 Multilayerfit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     3452 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/TiO2 Fit/TiO2 Multilayerfit.md
+-rw-r--r--   0 runner    (1001) docker     (121)    36583 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/TiO2 Fit/TiO2_400cycles.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.787232 pyElli-0.9.2/examples/Total internal reflection/
+-rw-r--r--   0 runner    (1001) docker     (121)   103247 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Total internal reflection/FrustratedTIR-angle.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3652 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Total internal reflection/FrustratedTIR-angle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    81476 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Total internal reflection/FrustratedTIR-thickness.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3549 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Total internal reflection/FrustratedTIR-thickness.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19784 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Total internal reflection/TIR.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2021-11-23 13:37:22.000000 pyElli-0.9.2/examples/Total internal reflection/TIR.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2021-11-23 13:37:22.000000 pyElli-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-11-23 13:37:22.000000 pyElli-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-11-23 13:37:34.795233 pyElli-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2021-11-23 13:37:22.000000 pyElli-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.783232 pyElli-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.791232 pyElli-0.9.2/src/elli/
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15148 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/dispersions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4270 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.791232 pyElli-0.9.2/src/elli/fitting/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5233 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/fitting/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11485 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/fitting/decorator_mmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13532 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/fitting/decorator_psi_delta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3607 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/fitting/params_hist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8189 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/materials.py
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/materials_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3021 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/math.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.791232 pyElli-0.9.2/src/elli/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3043 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/plot/mueller_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2909 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/plot/structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3295 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2353 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/solver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4806 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/solver2x2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16190 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/solver4x4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3070 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/spectraray.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13003 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2506 2021-11-23 13:37:22.000000 pyElli-0.9.2/src/elli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.791232 pyElli-0.9.2/src/pyElli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2922 2021-11-23 13:37:34.000000 pyElli-0.9.2/src/pyElli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2893 2021-11-23 13:37:34.000000 pyElli-0.9.2/src/pyElli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-23 13:37:34.000000 pyElli-0.9.2/src/pyElli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-23 13:37:34.000000 pyElli-0.9.2/src/pyElli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2021-11-23 13:37:34.000000 pyElli-0.9.2/src/pyElli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-23 13:37:34.000000 pyElli-0.9.2/src/pyElli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 13:37:34.791232 pyElli-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     4040 2021-11-23 13:37:22.000000 pyElli-0.9.2/tests/benchmark_propagators_TiO2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3510 2021-11-23 13:37:22.000000 pyElli-0.9.2/tests/test_bragg_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7437 2021-11-23 13:37:22.000000 pyElli-0.9.2/tests/test_internal_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2842 2021-11-23 13:37:22.000000 pyElli-0.9.2/tests/test_liquid_crystals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5298 2021-11-23 13:37:22.000000 pyElli-0.9.2/tests/test_uniaxial_crystals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2182 2021-11-23 13:37:22.000000 pyElli-0.9.2/tox.ini
```

### Comparing `pyElli-0.9.1/.coveragerc` & `pyElli-0.9.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/.github/workflows/benchmark.yml` & `pyElli-0.9.2/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/.github/workflows/build-docker.yml` & `pyElli-0.9.2/.github/workflows/build-docker.yml`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/.github/workflows/pytest.yml` & `pyElli-0.9.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/.github/workflows/python-publish.yml` & `pyElli-0.9.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/.gitignore` & `pyElli-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/CHANGELOG.md` & `pyElli-0.9.2/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## Version 0.9.2
+- Fitting decorator buttons (fit, undo, redo)
+- Data export for decorators
+- Changed file loading to -pi, pi delta convention
+- Fixed Jones vector default
+- Included more documentation
+
 ## Version 0.9.1
 - Automated build of Docker images
 - Benchmarking setup
 - Added more documentation
 - Renamed a lot of functions for PEP8 compliance
 - More bugfixes
```

### Comparing `pyElli-0.9.1/CONTRIBUTING.md` & `pyElli-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/LICENSE.txt` & `pyElli-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/PKG-INFO` & `pyElli-0.9.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,21 @@
-Metadata-Version: 2.1
-Name: pyElli
-Version: 0.9.1
-Summary: Python implementation of Berremans 4x4 matrix method
-Home-page: https://github.com/PyEllips/pyElli/
-Author: dobener
-Author-email: florian.dobener@physik.uni-giessen.de
-License: GPL-3.0-or-later
-Project-URL: Documentation, https://pyelli.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/PyEllips/pyElli/
-Project-URL: Download, https://github.com/PyEllips/pyElli/releases
-Project-URL: Changelog, https://github.com/PyEllips/pyElli/blob/master/CHANGELOG.rst
-Project-URL: Tracker, https://github.com/PyEllips/pyElli/issues
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: PLOT
-Provides-Extra: testing
-License-File: LICENSE.txt
-
-[![Pytest](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml/badge.svg)](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml) [![Documentation Status](https://readthedocs.org/projects/pyelli/badge/?version=latest)](https://pyelli.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/pyElli)](https://pypi.org/project/pyElli/)
+[![Pytest](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml/badge.svg)](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml) [![Documentation Status](https://readthedocs.org/projects/pyelli/badge/?version=latest)](https://pyelli.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/pyElli)](https://pypi.org/project/pyElli/) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5702469.svg)](https://doi.org/10.5281/zenodo.5702469)
 
 
 # pyElli
 PyElli is a numerical solver for spectral ellipsometry employing well-known 2x2 and 4x4 algorithms.
 It is intended for a broad case of problems including simple fitting of layered structures, anisotropic layers and any other light interaction with layered 1D structures.
 It serves as a system for the day to day ellipsometry task at hand and makes fitting a breeze.
 
 ## Features
 - A multitude of models to approximate the dielectric function of your material.
 - Build up your structure easily from materials and layers.
-- Simulate reflectiona and transmission spectra, ellipsometric parameters and Mueller matrices.
+- Simulate reflection and transmission spectra, ellipsometric parameters and Mueller matrices.
 - Utilities to quickly convert, plot and fit your measurement data.
-- Powerfull when necessary, editable and expandeble.
+- Powerful when necessary, editable and expandable.
 
 ## How to get it
 The installers for all releases are available at the [Python Package Index (PyPI)](https://pypi.org/project/pyElli/).
 
 To install run:
 ```sh
 pip install pyElli
@@ -44,16 +23,20 @@
 
 A complete environment for pyElli is also available as a [Docker Container](https://hub.docker.com/r/domna/pyelli).
 From a running Docker installation simply run:
 ```sh
 docker pull domna/pyelli
 ```
 
-The source code is hosted on [GitHub](https://github.com/PyEllips/pyElli), to install from source run:
+To install the latest development version use:
+```sh
+pip install git+https://github.com/PyEllips/pyElli.git
+```
+
+The source code is hosted on [GitHub](https://github.com/PyEllips/pyElli), to manually install from source, download and run inside the downloaded folder:
 ```sh
 python setup.py install
 ```
 
 ## Acknowledgements
 - Based on Olivier Castany's [Berreman4x4](https://github.com/Berreman4x4/Berreman4x4)
 - Solver2x2 based on Steve Byrnes's [tmm](https://github.com/sbyrnes321/tmm)
-
```

### Comparing `pyElli-0.9.1/README.md` & `pyElli-0.9.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,42 @@
-[![Pytest](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml/badge.svg)](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml) [![Documentation Status](https://readthedocs.org/projects/pyelli/badge/?version=latest)](https://pyelli.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/pyElli)](https://pypi.org/project/pyElli/)
+Metadata-Version: 2.1
+Name: pyElli
+Version: 0.9.2
+Summary: Python implementation of Berremans 4x4 matrix method
+Home-page: https://github.com/PyEllips/pyElli/
+Author: dobener
+Author-email: florian.dobener@physik.uni-giessen.de
+License: GPL-3.0-or-later
+Project-URL: Documentation, https://pyelli.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/PyEllips/pyElli/
+Project-URL: Download, https://github.com/PyEllips/pyElli/releases
+Project-URL: Changelog, https://github.com/PyEllips/pyElli/blob/master/CHANGELOG.md
+Project-URL: Tracker, https://github.com/PyEllips/pyElli/issues
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: PLOT
+Provides-Extra: testing
+License-File: LICENSE.txt
+
+[![Pytest](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml/badge.svg)](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml) [![Documentation Status](https://readthedocs.org/projects/pyelli/badge/?version=latest)](https://pyelli.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/pyElli)](https://pypi.org/project/pyElli/) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5702469.svg)](https://doi.org/10.5281/zenodo.5702469)
 
 
 # pyElli
 PyElli is a numerical solver for spectral ellipsometry employing well-known 2x2 and 4x4 algorithms.
 It is intended for a broad case of problems including simple fitting of layered structures, anisotropic layers and any other light interaction with layered 1D structures.
 It serves as a system for the day to day ellipsometry task at hand and makes fitting a breeze.
 
 ## Features
 - A multitude of models to approximate the dielectric function of your material.
 - Build up your structure easily from materials and layers.
-- Simulate reflectiona and transmission spectra, ellipsometric parameters and Mueller matrices.
+- Simulate reflection and transmission spectra, ellipsometric parameters and Mueller matrices.
 - Utilities to quickly convert, plot and fit your measurement data.
-- Powerfull when necessary, editable and expandeble.
+- Powerful when necessary, editable and expandable.
 
 ## How to get it
 The installers for all releases are available at the [Python Package Index (PyPI)](https://pypi.org/project/pyElli/).
 
 To install run:
 ```sh
 pip install pyElli
@@ -23,15 +44,22 @@
 
 A complete environment for pyElli is also available as a [Docker Container](https://hub.docker.com/r/domna/pyelli).
 From a running Docker installation simply run:
 ```sh
 docker pull domna/pyelli
 ```
 
-The source code is hosted on [GitHub](https://github.com/PyEllips/pyElli), to install from source run:
+To install the latest development version use:
+```sh
+pip install git+https://github.com/PyEllips/pyElli.git
+```
+
+The source code is hosted on [GitHub](https://github.com/PyEllips/pyElli), to manually install from source, download and run inside the downloaded folder:
 ```sh
 python setup.py install
 ```
 
 ## Acknowledgements
 - Based on Olivier Castany's [Berreman4x4](https://github.com/Berreman4x4/Berreman4x4)
-- Solver2x2 based on Steve Byrnes's [tmm](https://github.com/sbyrnes321/tmm)
+- Solver2x2 based on Steve Byrnes's [tmm](https://github.com/sbyrnes321/tmm)
+
+
```

### Comparing `pyElli-0.9.1/docs/Makefile` & `pyElli-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/docs/conf.py` & `pyElli-0.9.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
 source_suffix = [".rst", '.md']
 
+autoclass_content = 'both'
+
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
```

### Comparing `pyElli-0.9.1/docs/index.rst` & `pyElli-0.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Bragg-mirror/Bragg-example.ipynb` & `pyElli-0.9.2/examples/Bragg-mirror/Bragg-example.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Bragg-mirror/Bragg-example.py` & `pyElli-0.9.2/examples/Bragg-mirror/Bragg-example.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Bragg-mirror/validation-Bragg.ipynb` & `pyElli-0.9.2/examples/Bragg-mirror/validation-Bragg.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Bragg-mirror/validation-Bragg.py` & `pyElli-0.9.2/examples/Bragg-mirror/validation-Bragg.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Ellipsometry uniaxial materials/Fujiwara-641.ipynb` & `pyElli-0.9.2/examples/Ellipsometry uniaxial materials/Fujiwara-641.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Ellipsometry uniaxial materials/Fujiwara-641.py` & `pyElli-0.9.2/examples/Ellipsometry uniaxial materials/Fujiwara-641.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Ellipsometry uniaxial materials/Fujiwara-642.ipynb` & `pyElli-0.9.2/examples/Ellipsometry uniaxial materials/Fujiwara-642.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Ellipsometry uniaxial materials/Fujiwara-642.py` & `pyElli-0.9.2/examples/Ellipsometry uniaxial materials/Fujiwara-642.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Interfaces/Interferences.ipynb` & `pyElli-0.9.2/examples/Interfaces/Interferences.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Interfaces/Interferences.py` & `pyElli-0.9.2/examples/Interfaces/Interferences.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Interfaces/interface-reflection.ipynb` & `pyElli-0.9.2/examples/Interfaces/interface-reflection.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Interfaces/interface-reflection.py` & `pyElli-0.9.2/examples/Interfaces/interface-reflection.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Liquid crystals/cholesteric-example.ipynb` & `pyElli-0.9.2/examples/Liquid crystals/cholesteric-example.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Liquid crystals/cholesteric-example.py` & `pyElli-0.9.2/examples/Liquid crystals/cholesteric-example.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Liquid crystals/twisted-nematic.ipynb` & `pyElli-0.9.2/examples/Liquid crystals/twisted-nematic.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Liquid crystals/twisted-nematic.py` & `pyElli-0.9.2/examples/Liquid crystals/twisted-nematic.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Liquid crystals/validation-cholesteric.ipynb` & `pyElli-0.9.2/examples/Liquid crystals/validation-cholesteric.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Liquid crystals/validation-cholesteric.py` & `pyElli-0.9.2/examples/Liquid crystals/validation-cholesteric.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/.ipynb_checkpoints/SiO2_Si Mueller Matrix-checkpoint.ipynb` & `pyElli-0.9.2/examples/SiO2_Si Mueller Matrix/SiO2_Si Mueller Matrix.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9724776195200302%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'source': ['import elli']}, 1: {'execution_count': 2, "*

 * *            '\'source\': ["MM = elli.SpectraRay.read_mmatrix(\'Wafer_MM_70.txt\').loc[210:820]"]}, '*

 * *            "2: {'execution_count': 3, 'source': {insert: [(0, 'params = elli.ParamsHist()\\n')], "*

 * *            "delete: [0]}}, 3: {'execution_count': 4, 'outputs': {0: {'data': "*

 * *            "{'application/vnd.jupyter.widget-view+json': {'model_id': "*

 * *            "'7869aa4a5e2a4d669019f040ba1222e9'}}}}, 'source': […]*

```diff
@@ -1,119 +1,119 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 65,
+            "execution_count": 1,
             "id": "55bce57a-ddc5-4088-97c2-e34587a9094e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import berreman4x4 as bm"
+                "import elli"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 66,
+            "execution_count": 2,
             "id": "d5099d9f-a817-4384-8b1a-3b14b8648c01",
             "metadata": {},
             "outputs": [],
             "source": [
-                "MM = bm.SpectraRay.read_mmatrix('Wafer_MM_70.txt').loc[210:820]"
+                "MM = elli.SpectraRay.read_mmatrix('Wafer_MM_70.txt').loc[210:820]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 67,
+            "execution_count": 3,
             "id": "fb3b5352-2dc5-4421-a97a-32e965d865a9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "params = bm.ParamsHist()\n",
+                "params = elli.ParamsHist()\n",
                 "params.add('SiO2_n0', value=1.452, min=-100, max=100, vary=True)\n",
                 "params.add('SiO2_n1', value=36.0, min=-40000, max=40000, vary=True)\n",
                 "params.add('SiO2_n2', value=0, min=-40000, max=40000, vary=True)\n",
                 "params.add('SiO2_k0', value=0, min=-100, max=100, vary=True)\n",
                 "params.add('SiO2_k1', value=0, min=-40000, max=40000, vary=True)\n",
                 "params.add('SiO2_k2', value=0, min=-40000, max=40000, vary=True)\n",
                 "params.add('SiO2_d', value=120, min=0, max=40000, vary=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 68,
+            "execution_count": 4,
             "id": "bad60bc6-3d81-47ef-9742-35cbdb7473b9",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "4090ba1c042e4f96b56be71f3097a755",
+                            "model_id": "7869aa4a5e2a4d669019f040ba1222e9",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "VBox(children=(HBox(children=(BoundedFloatText(value=1.452, description='SiO2_n0', min=-100.0), BoundedFloatTe\u2026"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "@bm.fit_mueller_matrix(MM, params, display_single=False, sharex=True, full_scale=False)\n",
+                "@elli.fit_mueller_matrix(MM, params, display_single=False, sharex=True, full_scale=False)\n",
                 "def model(lbda, params):\n",
-                "    sr = bm.SpectraRay('./')\n",
-                "    Si = bm.IsotropicMaterial(sr.loadDispersionTable('Si_Aspnes.mat'))\n",
+                "    sr = elli.SpectraRay('./')\n",
+                "    Si = elli.IsotropicMaterial(sr.loadDispersionTable('Si_Aspnes.mat'))\n",
                 "\n",
-                "    SiO2 = bm.IsotropicMaterial(bm.DispersionCauchy(params['SiO2_n0'],\n",
+                "    SiO2 = elli.IsotropicMaterial(elli.DispersionCauchy(params['SiO2_n0'],\n",
                 "                                                    params['SiO2_n1'],\n",
                 "                                                    params['SiO2_n2'],\n",
                 "                                                    params['SiO2_k0'],\n",
                 "                                                    params['SiO2_k1'],\n",
                 "                                                    params['SiO2_k2']))\n",
                 "\n",
-                "    Layer = [bm.Layer(SiO2, params['SiO2_d'])]\n",
+                "    Layer = [elli.Layer(SiO2, params['SiO2_d'])]\n",
                 "\n",
-                "    return bm.Structure(bm.AIR, Layer, Si).evaluate(lbda, 70, solver=bm.Solver4x4, propagator=bm.PropagatorEig())"
+                "    return elli.Structure(elli.AIR, Layer, Si).evaluate(lbda, 70, solver=elli.Solver4x4, propagator=elli.PropagatorEig())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 69,
+            "execution_count": 5,
             "id": "dc1ca09c-b0a6-4ce5-8715-fed86f1da48f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<h2>Fit Statistics</h2><table><tr><td>fitting method</td><td>leastsq</td><td></td></tr><tr><td># function evals</td><td>98</td><td></td></tr><tr><td># data points</td><td>22336</td><td></td></tr><tr><td># variables</td><td>7</td><td></td></tr><tr><td>chi-square</td><td> 4.15193667</td><td></td></tr><tr><td>reduced chi-square</td><td> 1.8594e-04</td><td></td></tr><tr><td>Akaike info crit.</td><td>-191860.730</td><td></td></tr><tr><td>Bayesian info crit.</td><td>-191804.632</td><td></td></tr></table><h2>Variables</h2><table><tr><th> name </th><th> value </th><th> standard error </th><th> relative error </th><th> initial value </th><th> min </th><th> max </th><th> vary </th></tr><tr><td> SiO2_n0 </td><td>  1.46444761 </td><td>  7.0599e-04 </td><td> (0.05%) </td><td> 1.452 </td><td> -100.000000 </td><td>  100.000000 </td><td> True </td></tr><tr><td> SiO2_n1 </td><td> -0.13383336 </td><td>  0.58947808 </td><td> (440.46%) </td><td> 36.0 </td><td> -40000.0000 </td><td>  40000.0000 </td><td> True </td></tr><tr><td> SiO2_n2 </td><td>  15.9280047 </td><td>  0.28218991 </td><td> (1.77%) </td><td> 0 </td><td> -40000.0000 </td><td>  40000.0000 </td><td> True </td></tr><tr><td> SiO2_k0 </td><td>  0.01718283 </td><td>  6.4320e-04 </td><td> (3.74%) </td><td> 0 </td><td> -100.000000 </td><td>  100.000000 </td><td> True </td></tr><tr><td> SiO2_k1 </td><td> -24.0903682 </td><td>  1.03845809 </td><td> (4.31%) </td><td> 0 </td><td> -40000.0000 </td><td>  40000.0000 </td><td> True </td></tr><tr><td> SiO2_k2 </td><td>  9.17505029 </td><td>  0.41326998 </td><td> (4.50%) </td><td> 0 </td><td> -40000.0000 </td><td>  40000.0000 </td><td> True </td></tr><tr><td> SiO2_d </td><td>  104.067145 </td><td>  0.10335035 </td><td> (0.10%) </td><td> 120 </td><td>  0.00000000 </td><td>  40000.0000 </td><td> True </td></tr></table><h2>Correlations (unreported correlations are < 0.100)</h2><table><tr><td>SiO2_k1</td><td>SiO2_k2</td><td>-0.9764</td></tr><tr><td>SiO2_k0</td><td>SiO2_k1</td><td>-0.9640</td></tr><tr><td>SiO2_n0</td><td>SiO2_d</td><td>-0.9557</td></tr><tr><td>SiO2_n1</td><td>SiO2_n2</td><td>-0.9513</td></tr><tr><td>SiO2_k0</td><td>SiO2_d</td><td>0.9464</td></tr><tr><td>SiO2_n0</td><td>SiO2_k0</td><td>-0.9044</td></tr><tr><td>SiO2_k0</td><td>SiO2_k2</td><td>0.8935</td></tr><tr><td>SiO2_k1</td><td>SiO2_d</td><td>-0.8400</td></tr><tr><td>SiO2_n0</td><td>SiO2_k1</td><td>0.8028</td></tr><tr><td>SiO2_k2</td><td>SiO2_d</td><td>0.7319</td></tr><tr><td>SiO2_n0</td><td>SiO2_k2</td><td>-0.6995</td></tr><tr><td>SiO2_n1</td><td>SiO2_d</td><td>-0.2971</td></tr><tr><td>SiO2_n1</td><td>SiO2_k0</td><td>-0.2812</td></tr><tr><td>SiO2_n1</td><td>SiO2_k1</td><td>0.2496</td></tr><tr><td>SiO2_n1</td><td>SiO2_k2</td><td>-0.2175</td></tr><tr><td>SiO2_n0</td><td>SiO2_n2</td><td>0.2059</td></tr></table>"
+                            "<h2>Fit Statistics</h2><table><tr><td>fitting method</td><td>leastsq</td><td></td></tr><tr><td># function evals</td><td>107</td><td></td></tr><tr><td># data points</td><td>22336</td><td></td></tr><tr><td># variables</td><td>7</td><td></td></tr><tr><td>chi-square</td><td> 3.00724141</td><td></td></tr><tr><td>reduced chi-square</td><td> 1.3468e-04</td><td></td></tr><tr><td>Akaike info crit.</td><td>-199065.245</td><td></td></tr><tr><td>Bayesian info crit.</td><td>-199009.148</td><td></td></tr></table><h2>Variables</h2><table><tr><th> name </th><th> value </th><th> standard error </th><th> relative error </th><th> initial value </th><th> min </th><th> max </th><th> vary </th></tr><tr><td> SiO2_n0 </td><td>  1.45271092 </td><td>  5.7283e-04 </td><td> (0.04%) </td><td> 1.452 </td><td> -100.000000 </td><td>  100.000000 </td><td> True </td></tr><tr><td> SiO2_n1 </td><td>  30.7219120 </td><td>  0.55071825 </td><td> (1.79%) </td><td> 36.0 </td><td> -40000.0000 </td><td>  40000.0000 </td><td> True </td></tr><tr><td> SiO2_n2 </td><td>  3.41046425 </td><td>  0.25306938 </td><td> (7.42%) </td><td> 0 </td><td> -40000.0000 </td><td>  40000.0000 </td><td> True </td></tr><tr><td> SiO2_k0 </td><td>  0.00393829 </td><td>  5.7854e-04 </td><td> (14.69%) </td><td> 0 </td><td> -100.000000 </td><td>  100.000000 </td><td> True </td></tr><tr><td> SiO2_k1 </td><td> -6.96288298 </td><td>  0.91853048 </td><td> (13.19%) </td><td> 0 </td><td> -40000.0000 </td><td>  40000.0000 </td><td> True </td></tr><tr><td> SiO2_k2 </td><td>  3.16088017 </td><td>  0.36345646 </td><td> (11.50%) </td><td> 0 </td><td> -40000.0000 </td><td>  40000.0000 </td><td> True </td></tr><tr><td> SiO2_d </td><td>  103.560409 </td><td>  0.08979888 </td><td> (0.09%) </td><td> 120 </td><td>  0.00000000 </td><td>  40000.0000 </td><td> True </td></tr></table><h2>Correlations (unreported correlations are < 0.100)</h2><table><tr><td>SiO2_k1</td><td>SiO2_k2</td><td>-0.9755</td></tr><tr><td>SiO2_k0</td><td>SiO2_k1</td><td>-0.9639</td></tr><tr><td>SiO2_n1</td><td>SiO2_n2</td><td>-0.9509</td></tr><tr><td>SiO2_k0</td><td>SiO2_d</td><td>0.9506</td></tr><tr><td>SiO2_n0</td><td>SiO2_d</td><td>-0.9496</td></tr><tr><td>SiO2_n0</td><td>SiO2_k0</td><td>-0.9026</td></tr><tr><td>SiO2_k0</td><td>SiO2_k2</td><td>0.8907</td></tr><tr><td>SiO2_k1</td><td>SiO2_d</td><td>-0.8461</td></tr><tr><td>SiO2_n0</td><td>SiO2_k1</td><td>0.8035</td></tr><tr><td>SiO2_k2</td><td>SiO2_d</td><td>0.7348</td></tr><tr><td>SiO2_n0</td><td>SiO2_k2</td><td>-0.6978</td></tr><tr><td>SiO2_n1</td><td>SiO2_d</td><td>-0.4581</td></tr><tr><td>SiO2_n1</td><td>SiO2_k0</td><td>-0.4355</td></tr><tr><td>SiO2_n1</td><td>SiO2_k1</td><td>0.3877</td></tr><tr><td>SiO2_n1</td><td>SiO2_k2</td><td>-0.3367</td></tr><tr><td>SiO2_n2</td><td>SiO2_d</td><td>0.2265</td></tr><tr><td>SiO2_n2</td><td>SiO2_k0</td><td>0.2153</td></tr><tr><td>SiO2_n2</td><td>SiO2_k1</td><td>-0.1916</td></tr><tr><td>SiO2_n2</td><td>SiO2_k2</td><td>0.1664</td></tr><tr><td>SiO2_n0</td><td>SiO2_n1</td><td>0.1663</td></tr></table>"
                         ],
                         "text/plain": [
-                            "<lmfit.minimizer.MinimizerResult at 0x24dde4b87c8>"
+                            "<lmfit.minimizer.MinimizerResult at 0x28891ca4670>"
                         ]
                     },
-                    "execution_count": 69,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model.fit()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 70,
+            "execution_count": 6,
             "id": "71878507-d611-4507-a011-f5b9029001e9",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "7743f46526df4258909384d5e672645d",
+                            "model_id": "1508bca945114e18b0f11ad3af3c608b",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "FigureWidget({\n",
                             "    'data': [{'line': {'color': '#636EFA', 'dash': 'solid'},\n",
                             "              'name': 'M11 ',\n",
@@ -127,35 +127,35 @@
             "source": [
                 "model.plot(full_scale=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "86384356-dfdb-4033-946f-976620006609",
+            "id": "7de31826-3e98-4ade-9359-01ae9239b849",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python (elli)",
             "language": "python",
-            "name": "python3"
+            "name": "myenv"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.12"
+            "version": "3.9.7"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/.ipynb_checkpoints/Si_Aspnes-checkpoint.mat` & `pyElli-0.9.2/examples/SiO2_Si Mueller Matrix/Si_Aspnes.mat`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/.ipynb_checkpoints/Wafer_MM_70-checkpoint.txt` & `pyElli-0.9.2/examples/SiO2_Si Mueller Matrix/Wafer_MM_70.txt`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/SiO2_Si Mueller Matrix/Si_Aspnes.mat` & `pyElli-0.9.2/examples/TiO2 Fit/Si_Aspnes.mat`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/TiO2 Fit/.ipynb_checkpoints/TiO2 Multilayerfit-checkpoint.md` & `pyElli-0.9.2/examples/TiO2 Fit/TiO2 Multilayerfit.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,37 @@
     formats: ipynb,md
     text_representation:
       extension: .md
       format_name: markdown
       format_version: '1.3'
       jupytext_version: 1.11.4
   kernelspec:
-    display_name: Python 3 (ipykernel)
+    display_name: Python (elli)
     language: python
-    name: python3
+    name: myenv
 ---
 
 ```python
-import berreman4x4 as bm
+import elli
 ```
 
 # Load data
 Load data collected with Sentech Ellipsometer and cut the spectral range (to use Si Aspnes file)
 
 The sample is an ALD grown TiO2 sample (with 400 cycles) on commercially available SiO2 / Si substrate.
 
 ```python
-tss = bm.SpectraRay.read_psi_delta_file('TiO2_400cycles.txt').loc[400:800]
-ρ = bm.SpectraRay.read_rho('TiO2_400cycles.txt').loc[400:800]
+tss = elli.SpectraRay.read_psi_delta_file('TiO2_400cycles.txt').loc[400:800]
+ρ = elli.SpectraRay.read_rho('TiO2_400cycles.txt').loc[400:800]
 ```
 
 # Estimate Parameters and build model
 
 ```python
-params = bm.ParamsHist()
+params = elli.ParamsHist()
 params.add('SiO2_n0', value=1.452, min=-100, max=100, vary=False)
 params.add('SiO2_n1', value=36.0, min=-40000, max=40000, vary=False)
 params.add('SiO2_n2', value=0, min=-40000, max=40000, vary=False)
 params.add('SiO2_k0', value=0, min=-100, max=100, vary=False)
 params.add('SiO2_k1', value=0, min=-40000, max=40000, vary=False)
 params.add('SiO2_k2', value=0, min=-40000, max=40000, vary=False)
 params.add('SiO2_d', value=276.36, min=0, max=40000, vary=False)
@@ -46,36 +46,36 @@
 params.add('TiO2_k1', value=0, min=-40000, max=40000, vary=False)
 params.add('TiO2_k2', value=0, min=-40000, max=40000, vary=False)
 
 params.add('TiO2_d', value=20, min=0, max=40000, vary=True)
 ```
 
 ```python
-@bm.fit(tss, params)
+@elli.fit(tss, params)
 def model(lbda, params):
-    sr = bm.SpectraRay('./')
-    Si = bm.IsotropicMaterial(sr.loadDispersionTable('Si_Aspnes.mat'))
+    sr = elli.SpectraRay('./')
+    Si = elli.IsotropicMaterial(sr.loadDispersionTable('Si_Aspnes.mat'))
 
-    SiO2 = bm.IsotropicMaterial(bm.DispersionCauchy(params['SiO2_n0'], 
+    SiO2 = elli.IsotropicMaterial(elli.DispersionCauchy(params['SiO2_n0'], 
                                                     params['SiO2_n1'], 
                                                     params['SiO2_n2'], 
                                                     params['SiO2_k0'], 
                                                     params['SiO2_k1'], 
                                                     params['SiO2_k2']))
-    TiO2 = bm.IsotropicMaterial(bm.DispersionCauchy(params['TiO2_n0'], 
+    TiO2 = elli.IsotropicMaterial(elli.DispersionCauchy(params['TiO2_n0'], 
                                                     params['TiO2_n1'], 
                                                     params['TiO2_n2'], 
                                                     params['TiO2_k0'], 
                                                     params['TiO2_k1'], 
                                                     params['TiO2_k2']))
     
-    Layer = [bm.Layer(TiO2, params['TiO2_d']), 
-             bm.Layer(SiO2, params['SiO2_d'])]
+    Layer = [elli.Layer(TiO2, params['TiO2_d']), 
+             elli.Layer(SiO2, params['SiO2_d'])]
     
-    return bm.Structure(bm.AIR, Layer, Si).evaluate(lbda, 70, solver=bm.Solver2x2)
+    return elli.Structure(elli.AIR, Layer, Si).evaluate(lbda, 70, solver=elli.Solver2x2)
     # Alternative: Use 4x4 Solver with scipy propagator
     # return bm.Structure(bm.AIR, Layer, Si).evaluate(lbda, 70, solver=bm.Solver4x4, propagator=bm.PropagatorExpmScipy())
 
     # Alternative: Use 4x4 Solver with faster PyTorch propagator (needs Pytorch to be installed)
     # return bm.Structure(bm.AIR, Layer, Si).evaluate(lbda, 70, solver=bm.Solver4x4, propagator=bm.PropagatorExpmTorch())
 ```
```

### Comparing `pyElli-0.9.1/examples/TiO2 Fit/TiO2_400cycles.txt` & `pyElli-0.9.2/examples/TiO2 Fit/TiO2_400cycles.txt`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Total internal reflection/FrustratedTIR-angle.ipynb` & `pyElli-0.9.2/examples/Total internal reflection/FrustratedTIR-angle.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Total internal reflection/FrustratedTIR-angle.py` & `pyElli-0.9.2/examples/Total internal reflection/FrustratedTIR-angle.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Total internal reflection/FrustratedTIR-thickness.ipynb` & `pyElli-0.9.2/examples/Total internal reflection/FrustratedTIR-thickness.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Total internal reflection/FrustratedTIR-thickness.py` & `pyElli-0.9.2/examples/Total internal reflection/FrustratedTIR-thickness.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Total internal reflection/TIR.ipynb` & `pyElli-0.9.2/examples/Total internal reflection/TIR.ipynb`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/examples/Total internal reflection/TIR.py` & `pyElli-0.9.2/examples/Total internal reflection/TIR.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/setup.cfg` & `pyElli-0.9.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/PyEllips/pyElli/
 project_urls = 
 	Documentation = https://pyelli.readthedocs.io/en/latest/
 	Source = https://github.com/PyEllips/pyElli/
 	Download = https://github.com/PyEllips/pyElli/releases
-	Changelog = https://github.com/PyEllips/pyElli/blob/master/CHANGELOG.rst
+	Changelog = https://github.com/PyEllips/pyElli/blob/master/CHANGELOG.md
 	Tracker = https://github.com/PyEllips/pyElli/issues
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
```

### Comparing `pyElli-0.9.1/setup.py` & `pyElli-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/src/elli/__init__.py` & `pyElli-0.9.2/src/elli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/src/elli/dispersions.py` & `pyElli-0.9.2/src/elli/dispersions.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/src/elli/experiment.py` & `pyElli-0.9.2/src/elli/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     structure = None
     jones_vector = None
     stokes_vector = None
     theta_i = None
     lbda = None
 
-    def __init__(self, structure: "Structure", lbda: npt.ArrayLike, theta_i: float, vector: npt.ArrayLike = [1, 0, -1, 0]) -> None:
+    def __init__(self, structure: "Structure", lbda: npt.ArrayLike, theta_i: float, vector: npt.ArrayLike = [1, 0, 1, 0]) -> None:
         """Creates a virtual experiment to simulate the behavior of a structure.
         
         Args:
             structure (Structure): Structure object to evaluate.
             lbda (npt.ArrayLike): Single value or array of wavelengths (in nm).
             theta_i (float): Incident angle (in degrees).
             vector (npt.ArrayLike, optional): Jones or Stokes vector of incident light. Defaults to [1, 0, -1, 0].
```

### Comparing `pyElli-0.9.1/src/elli/fitting/decorator_mmatrix.py` & `pyElli-0.9.2/src/elli/fitting/decorator_mmatrix.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,195 +1,262 @@
 """Decorator functions for convenient fitting of Mueller matrices"""
 # Encoding: utf-8
+from typing import Callable
 from ipywidgets import widgets
 from IPython.display import display
 import pandas as pd
 import numpy.typing as npt
 from lmfit import minimize, Parameters
 from lmfit.minimizer import MinimizerResult
 import plotly.graph_objects as go
-from typing import Callable
 from ..result import Result
 from ..plot.mueller_matrix import plot_mmatrix
+from .params_hist import ParamsHist
+from .decorator import FitDecorator
+
 
-def mmatrix_to_dataframe(exp_df:pd.DataFrame, mueller_matrix:npt.NDArray) -> pd.DataFrame:
+def mmatrix_to_dataframe(exp_df: pd.DataFrame,
+                         mueller_matrix: npt.NDArray,
+                         identifier:str=None) -> pd.DataFrame:
     """Reshape a numpy 4x4 array containing mueller matrix elements
     to a dataframe with columns Mxy. The index labels for each column
     are taken from the provided exp_df.
 
     Args:
         exp_df (pd.DataFrame): The experimental dataframe providing the index and columns for
                                the newly generated dataframe.
         mueller_matrix (npt.NDArray): Data to be reshaped into a dataframe
+        identifier (str, optional):
+            An identifier to append to each column name, in the form
+            Mxy_<identifier>, where Mxy is the old column name.
+            Defaults to None.
 
     Returns:
         pd.DataFrame: Contains the data from mueller_matrix in the shape of exp_df
     """
-    mueller_df = pd.DataFrame(index=exp_df.index, columns=exp_df.columns, dtype='float64')
+    if identifier is not None:
+        columns = [f'{c}_{identifier}' for c in exp_df.columns]
+    else:
+        columns = exp_df.columns
+    mueller_df = pd.DataFrame(
+        index=exp_df.index, columns=columns, dtype='float64')
     mueller_df.values[:] = mueller_matrix.reshape(-1, 16)
 
     return mueller_df
 
-class FitMuellerMatrix():
+
+class FitMuellerMatrix(FitDecorator):
     """A class to fit mueller matrices to experimental data"""
 
-    def update_params(self, change:dict):
-        """Update plot after a change of fitting parameters
+    def update_selection(self, _: dict = None) -> None:
+        """Update plot after selection of displayed data
 
         Args:
-            change (dict): A dictionary containing the ipywidgets change event
+            _ (dict, optional): No function. Just for compliance with ABC.
         """
-        self.params[change.owner.description].value = change.new
-
         with self.fig.batch_update():
             model_df = mmatrix_to_dataframe(self.exp_mm,
                                             self.model(self.exp_mm.index.values,
                                                        self.params).mueller_matrix)
 
             for i, melem in enumerate(model_df):
                 self.fig.data[2*i+1].y = model_df[melem]
 
-    def create_widgets(self):
+    def create_widgets(self) -> None:
         """Create ipywidgets for parameter estimation"""
-        widget_list = []
+        self.param_widgets = {}
         for param in self.params.valuesdict():
             curr_widget = widgets.BoundedFloatText(self.params[param],
                                                    min=self.params[param].min,
                                                    max=self.params[param].max,
                                                    description=param,
                                                    continuous_update=False)
             curr_widget.observe(self.update_params, names=('value', 'owner'))
-            widget_list.append(curr_widget)
+            self.param_widgets[param] = curr_widget
 
-        display(widgets.VBox([widgets.HBox(widget_list,
+        fit_button = widgets.Button(description='Fit')
+        fit_button.on_click(lambda _: self.fit_button_clicked())
+        button_list = [fit_button]
+
+        if isinstance(self.params, ParamsHist):
+            undo_button = widgets.Button(description='Undo')
+            undo_button.on_click(self.re_undo_button_clicked)
+            redo_button = widgets.Button(description='Redo')
+            redo_button.on_click(self.re_undo_button_clicked)
+
+            button_list.append(undo_button)
+            button_list.append(redo_button)
+
+        display(widgets.VBox([widgets.HBox(list(self.param_widgets.values()) +
+                                           button_list,
                                            layout=widgets.Layout(width='100%',
                                                                  display='inline-flex',
                                                                  flex_flow='row wrap')),
                               self.fig]))
 
     def fit_function(self,
-                     params:Parameters,
-                     lbda:npt.NDArray,
+                     params: Parameters,
+                     lbda: npt.NDArray,
                      mueller_matrix: pd.DataFrame) -> npt.NDArray:
         """The fit function to minimize the fitting problem
 
         Args:
             params (Parameters): The lmfit fitting Parameters to construct the simulation
             lbda (npt.NDArray): Wavelengths in nm
             mueller_matrix (pd.DataFrame): The experimental data to compare to the fitted model
 
         Returns:
-            npt.NDArray: Residual between the calculation with current parameters and experimental data
+            npt.NDArray: Residual between the calculation
+                with current parameters and experimental data
         """
         return mueller_matrix.values.reshape(-1, 4, 4) - self.model(lbda, params).mueller_matrix
 
-    def fit(self, method:str='leastsq') -> MinimizerResult:
+    def fit(self, method: str = 'leastsq') -> MinimizerResult:
         """Execute lmfit with the current fitting parameters
 
         Args:
-            method (str, optional): The fitting method to use. Any method supported by scipys curve_fit is allowed.
-                                    Defaults to 'leastsq'.
+            method (str, optional): The fitting method to use.
+                Any method supported by scipys curve_fit is allowed.
+                Defaults to 'leastsq'.
 
         Returns:
             Result: The fitting result
-        """        
+        """
         res = minimize(self.fit_function,
                        self.params,
                        args=(self.exp_mm.index.values, self.exp_mm),
                        method=method)
 
         self.fitted_params = res.params
         return res
 
-    def get_fit_data(self) -> pd.DataFrame:
-        """Gets the fit results as dataframe
+    def get_model_data(self,
+                       params:Parameters=None,
+                       append_exp_data=False) -> pd.DataFrame:
+        """Gets the data from the provided model with the provided parameters.
+        If no parameters are provided, the fitted parameters are used
+        (which default to the initial parameters if no fit has been triggered).
+
+        Args:
+            params (Parameters, optional): 
+                The parameters to calculate the model with. 
+                If not provided, the fitted parameters are used.
+                Defaults to None.
+            append_exp_data (bool, optional):
+                Appends the experimental data if set to True.
+                Defaults to False.
 
         Returns:
-            pd.DataFrame: The fit results
-        """        
+            pd.DataFrame: The model results
+        """
+        if params is None:
+            fit_result = self.model(self.exp_mm.index.values, self.fitted_params)
+            desc = 'fit'
+        else:
+            fit_result = self.model(self.exp_mm.index.values, params)
+            desc = 'model'
+
+        if append_exp_data:
+            return pd.concat([self.exp_mm,
+                              mmatrix_to_dataframe(self.exp_mm,
+                                                   fit_result.mueller_matrix,
+                                                   identifier=desc)], axis=1)
+
         return mmatrix_to_dataframe(self.exp_mm,
-                                    self.model(self.exp_mm.index.values,
-                                                self.fitted_params).mueller_matrix)
+                                    fit_result.mueller_matrix,
+                                    identifier=desc)
 
     def plot(self, **kwargs) -> go.Figure:
         """Plot the fit results
 
         Args:
-            **display_single (bool): Returns a figure containing a single graph, if set to true. Returns a grid of figures otherwise.
+            **display_single (bool):
+                Returns a figure containing a single graph, if set to true.
+                Returns a grid of figures otherwise.
             **sharex (bool): Ties the zoom of the x-axes together for grid view.
             **full_scale (bool): Sets the y-axis scale to [-1, 1] if set to True.
 
         Returns:
             go.Figure: The figure containing the data
-        """        
+        """
         fit_result = mmatrix_to_dataframe(self.exp_mm,
                                           self.model(self.exp_mm.index.values,
                                                      self.fitted_params).mueller_matrix)
 
         return plot_mmatrix([self.exp_mm, fit_result],
-                single=self.display_single
-                    if kwargs.get('display_single') is None else kwargs.get('display_single'),
-                sharex=self.sharex
-                    if kwargs.get('sharex') is None else kwargs.get('sharex'),
-                full_scale=self.full_scale
-                    if kwargs.get('full_scale') is None else kwargs.get('full_scale'))
+                            single=self.display_single
+                            if kwargs.get('display_single') is None else kwargs.get('display_single'),
+                            sharex=self.sharex
+                            if kwargs.get('sharex') is None else kwargs.get('sharex'),
+                            full_scale=self.full_scale
+                            if kwargs.get('full_scale') is None else kwargs.get('full_scale'))
 
     def __init__(self,
-                 exp_mm:pd.DataFrame,
-                 params:Parameters,
-                 model:Callable[[npt.NDArray, Parameters], Result],
-                 **kwargs):
+                 exp_mm: pd.DataFrame,
+                 params: Parameters,
+                 model: Callable[[npt.NDArray, Parameters], Result],
+                 **kwargs) -> None:
         """Intialize the mueller matrix fitting class
 
         Args:
             exp_mm (pd.DataFrame): The dataframe containing an experimental mueller matrix.
                                    It should contain 16 columns with labels Mxy,
                                    where xy are the matrix positions.
             params (Parameters): Fitting start parameters
-            model (Callable[[npt.NDArray, Parameters], Result]): A function taking wavelengths as first parameter
-                                                                 and fitting parameters as second,
-                                                                 which returns a pyEllis Result object.
-                                                                 This function contains the actual model which should be fitted
-
-            **display_single (bool): Returns a figure containing a single graph, if set to true. Returns a grid of figures otherwise.
+            model (Callable[[npt.NDArray, Parameters], Result]):
+                A function taking wavelengths as first parameter
+                and fitting parameters as second,
+                which returns a pyEllis Result object.
+                This function contains the actual model which should be fitted
+
+            **display_single (bool):
+                Returns a figure containing a single graph, if set to true.
+                Returns a grid of figures otherwise.
             **sharex (bool): Ties the zoom of the x-axes together for grid view.
             **full_scale (bool): Sets the y-axis scale to [-1, 1] if set to True.
-        """        
+        """
+        super().__init__()
         self.exp_mm = exp_mm
         self.params = params
         self.fitted_params = params.copy()
         self.model = model
         self.display_single = kwargs.get('display_single')
         self.sharex = kwargs.get('sharex')
         self.full_scale = kwargs.get('full_scale')
+        self.param_widgets = {}
 
-        model_df = mmatrix_to_dataframe(exp_mm, model(exp_mm.index.values, params).mueller_matrix)
+        model_df = mmatrix_to_dataframe(exp_mm, model(
+            exp_mm.index.values, params).mueller_matrix)
         self.fig = plot_mmatrix([exp_mm,
                                  model_df],
-                                 single=self.display_single,
-                                 sharex=self.sharex,
-                                 full_scale=self.full_scale)
+                                single=self.display_single,
+                                sharex=self.sharex,
+                                full_scale=self.full_scale)
 
         self.create_widgets()
 
-def fit_mueller_matrix(exp_mm:pd.DataFrame,
-                       params:Parameters,
+
+def fit_mueller_matrix(exp_mm: pd.DataFrame,
+                       params: Parameters,
                        **kwargs) -> Callable[[npt.NDArray, Parameters], Result]:
     """A parameters decorator for fitting mueller matrices. Displays an ipywidget float box for
     each fitting parameter and an interactive plot to estimate parameters.
 
     Args:
         exp_mm (pd.DataFrame): The dataframe containing an experimental mueller matrix.
                                It should contain 16 columns with labels Mxy,
                                where xy are the matrix positions.
         params (Parameters): Fitting start parameters
-        **display_single (bool): Returns a figure containing a single graph, if set to true. Returns a grid of figures otherwise.
+        **display_single (bool):
+            Returns a figure containing a single graph, if set to true.
+            Returns a grid of figures otherwise.
         **sharex (bool): Ties the zoom of the x-axes together for grid view.
         **full_scale (bool): Sets the y-axis scale to [-1, 1] if set to True.
 
     Returns:
-        Callable[[npt.NDArray, Parameters], Result]: A function taking wavelengths as first parameter and fitting parameters as second,
-                                                     which returns a pyEllis Result object.
-                                                     This function contains the actual model which should be fitted and is automatically
-                                                     provided when used as a decorator.
-    """    
+        Callable[[npt.NDArray, Parameters], Result]:
+            A function taking wavelengths as first parameter and fitting parameters as second,
+            which returns a pyEllis Result object.
+            This function contains the actual model which should be fitted and is automatically
+            provided when used as a decorator.
+    """
     return lambda model: FitMuellerMatrix(exp_mm, params, model, **kwargs)
```

### Comparing `pyElli-0.9.1/src/elli/fitting/decorator_psi_delta.py` & `pyElli-0.9.2/src/elli/fitting/decorator_psi_delta.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """Decorator functions for convenient fitting"""
 # Encoding: utf-8
+from typing import Callable
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
 import plotly.graph_objects as go
 from lmfit import minimize, Parameters
 from ipywidgets import widgets
 from IPython.display import display
-import numpy.typing as npt
-from typing import Callable
 from ..result import Result
-from ..utils import calcPseudoDiel, calc_rho
+from ..utils import calc_pseudo_diel, calc_rho
+from .params_hist import ParamsHist
+from .decorator import FitDecorator
 
-class FitRho():
+
+class FitRho(FitDecorator):
     """A class to fit psi/delta or rho based ellipsometry data with two degress of freedom"""
 
-    def set_psi_delta(self, update_exp:bool=False, update_names:bool=False) -> None:
+    def set_psi_delta(self, update_exp: bool = False, update_names: bool = False) -> None:
         """Sets Plot to Psi/Delta values
 
         Args:
-            update_exp (bool, optional): Flag to change the experimental data as well. Defaults to False.
-            update_names (bool, optional): Flag to change the label names. Defaults to False.
+            update_exp (bool, optional):
+                Flag to change the experimental data as well. Defaults to False.
+            update_names (bool, optional):
+                Flag to change the label names. Defaults to False.
         """
         data = self.model(self.exp_data.index, self.params)
         self.fig.update_layout(yaxis_title="Ψ/Δ (°)")
         self.fig.data[2].y = data.psi
         self.fig.data[3].y = data.delta
 
         if update_exp:
@@ -32,20 +37,22 @@
 
         if update_names:
             self.fig.data[0].name = 'Ψ'
             self.fig.data[1].name = 'Δ'
             self.fig.data[2].name = 'Ψ_tmm'
             self.fig.data[3].name = 'Δ_tmm'
 
-    def set_rho(self, update_exp:bool=False, update_names:bool=False) -> None:
+    def set_rho(self, update_exp: bool = False, update_names: bool = False) -> None:
         """Sets Plot to Rho values
 
         Args:
-            update_exp (bool, optional): Flag to change the experimental data as well. Defaults to False.
-            update_names (bool, optional): Flag to change the label names. Defaults to False.
+            update_exp (bool, optional):
+                Flag to change the experimental data as well. Defaults to False.
+            update_names (bool, optional):
+                Flag to change the label names. Defaults to False.
         """
         data = self.model(self.exp_data.index, self.params)
         self.fig.update_layout(yaxis_title="ρ")
         self.fig.data[2].y = data.rho.real
         self.fig.data[3].y = data.rho.imag
 
         if update_exp:
@@ -55,205 +62,251 @@
 
         if update_names:
             self.fig.data[0].name = 'ρr'
             self.fig.data[1].name = 'ρi'
             self.fig.data[2].name = 'ρr_tmm'
             self.fig.data[3].name = 'ρi_tmm'
 
-    def set_pseudo_diel(self, update_exp:bool=False, update_names:bool=False):
+    def set_pseudo_diel(self, update_exp: bool = False, update_names: bool = False) -> None:
         """Sets Plot to Pseudo Dielectric function values
 
         Args:
             update_exp (bool, optional): Flag to change the experimental data as well.
                                          Defaults to False.
             update_names (bool, optional): Flag to change the label names.
                                            Defaults to False.
         """
         data = self.model(self.exp_data.index, self.params)
-        peps = calcPseudoDiel(pd.DataFrame(data.rho, index=self.exp_data.index).iloc[:, 0],
-                                          self.angle)
+        peps = calc_pseudo_diel(pd.DataFrame(data.rho, index=self.exp_data.index).iloc[:, 0],
+                                self.angle)
         self.fig.update_layout(yaxis_title="ϵ")
         self.fig.data[2].y = peps.loc[:, 'ϵ1']
         self.fig.data[3].y = peps.loc[:, 'ϵ2']
 
         if update_exp:
-            exp_peps = calcPseudoDiel(calc_rho(self.exp_data), self.angle)
+            exp_peps = calc_pseudo_diel(calc_rho(self.exp_data), self.angle)
             self.fig.data[0].y = exp_peps.loc[:, 'ϵ1']
             self.fig.data[1].y = exp_peps.loc[:, 'ϵ2']
 
         if update_names:
             self.fig.data[0].name = 'ϵ1'
             self.fig.data[1].name = 'ϵ2'
             self.fig.data[2].name = 'ϵ1_tmm'
             self.fig.data[3].name = 'ϵ2_tmm'
 
-    def update_params(self, change:dict, selected:dict):
-        """Update plot after a change of fitting parameters
-
-        Args:
-            change (dict): A dictionary containing the ipywidgets change event
-            selected (dict): The selected value of the data display dropdown widget
-        """        
-        self.params[change.owner.description].value = change.new
-
-        with self.fig.batch_update():
-            update = self.update_dict.get(selected.value)
-            if update is not None:
-                update()
-
-    def update_selection(self, change:dict):
+    def update_selection(self, change: dict = None) -> None:
         """Update plot after selection of displayed data
 
         Args:
-            change (dict): A dictionary containing the ipywidgets change event
+            change (dict, optional): A dictionary containing the ipywidgets change event
         """
         with self.fig.batch_update():
-            update = self.update_dict.get(change.new)
+            update = self.update_dict.get(
+                change.new if change is not None else self.selector.value
+            )
             if update is not None:
                 update(update_exp=True, update_names=True)
 
-    def create_widgets(self):
+    def create_widgets(self) -> None:
         """Create ipywidgets for parameter estimation"""
-        widget_list = []
+        self.param_widgets = {}
+        self.selector = widgets.Dropdown(
+            options=['Psi/Delta', 'Rho', 'Pseudo Diel.'],
+            value='Psi/Delta',
+            description='Display: ',
+            disabled=False
+        )
+        self.selector.observe(self.update_selection, names='value')
+
         for param in self.params.valuesdict():
             curr_widget = widgets.BoundedFloatText(self.params[param],
                                                    min=self.params[param].min,
                                                    max=self.params[param].max,
                                                    description=param,
                                                    continuous_update=False)
-            curr_widget.observe(lambda x: self.update_params(x, selector), names=('value', 'owner'))
-            widget_list.append(curr_widget)
+            curr_widget.observe(self.update_params, names='value')
+            self.param_widgets[param] = curr_widget
 
-        selector = widgets.Dropdown(
-            options=['Psi/Delta', 'Rho', 'Pseudo Diel.'],
-            value='Psi/Delta',
-            description='Display: ',
-            disabled=False
-        )
-        selector.observe(self.update_selection, names='value')
-        widget_list.append(selector)
+        fit_button = widgets.Button(description='Fit')
+        fit_button.on_click(lambda _: self.fit_button_clicked())
+        button_list = [self.selector, fit_button]
+
+        if isinstance(self.params, ParamsHist):
+            undo_button = widgets.Button(description='Undo')
+            undo_button.on_click(self.re_undo_button_clicked)
+            redo_button = widgets.Button(description='Redo')
+            redo_button.on_click(self.re_undo_button_clicked)
 
-        display(widgets.VBox([widgets.HBox(widget_list,
+            button_list.append(undo_button)
+            button_list.append(redo_button)
+
+        display(widgets.VBox([widgets.HBox(list(self.param_widgets.values()) +
+                                           button_list,
                                            layout=widgets.Layout(width='100%',
                                                                  display='inline-flex',
                                                                  flex_flow='row wrap')),
                               self.fig]))
 
     def fit_function(self,
-                     params:Parameters,
-                     lbda:npt.NDArray,
-                     rhor:npt.NDArray,
-                     rhoi:npt.NDArray) -> npt.NDArray:
+                     params: Parameters,
+                     lbda: npt.NDArray,
+                     rhor: npt.NDArray,
+                     rhoi: npt.NDArray) -> npt.NDArray:
         """The fit function to minimize the fitting problem
 
         Args:
             params (Parameters): The lmfit fitting Parameters to construct the simulation
             lbda (npt.NDArray): Wavelengths in nm
             rhor (npt.NDArray): The real part of the experimental rho
             rhoi (npt.NDArray): The imaginary part of the experimental rho
 
         Returns:
-            npt.NDArray: Residual between the calculation with current parameters and experimental data
-        """                
+            npt.NDArray:
+                Residual between the calculation with current parameters and experimental data
+        """
         result = self.model(lbda, params)
 
         resid_rhor = rhor - result.rho.real
         resid_rhoi = rhoi - result.rho.imag
 
         return np.concatenate((resid_rhor, resid_rhoi))
 
     def fit(self, method='leastsq'):
         """Execute lmfit with the current fitting parameters
 
         Args:
-            method (str, optional): The fitting method to use. Any method supported by scipys curve_fit is allowed.
+            method (str, optional): The fitting method to use.
+                                    Any method supported by scipys curve_fit is allowed.
                                     Defaults to 'leastsq'.
 
         Returns:
             Result: The fitting result
         """
         rho = calc_rho(self.exp_data)
         res = minimize(self.fit_function,
                        self.params,
                        args=(rho.index.to_numpy(), rho.values.real, rho.values.imag),
                        method=method)
 
         self.fitted_params = res.params
         return res
 
-    def plot(self):
+    def plot(self) -> go.Figure:
         """Plot the fit results as Psi/Delta"""
         fit_result = self.model(self.exp_data.index.to_numpy(), self.fitted_params)
 
         return go.FigureWidget(pd.concat([self.exp_data,
-                                            pd.DataFrame({'Ψ_fit': fit_result.psi,
+                                          pd.DataFrame({'Ψ_fit': fit_result.psi,
                                                         'Δ_fit': fit_result.delta},
-                                                        index=self.exp_data.index)]
-                                            ).plot())
+                                                       index=self.exp_data.index)]
+                                         ).plot())
 
-    def plot_rho(self):
+    def plot_rho(self) -> go.Figure:
         """Plot the fit results as Rho"""
         rho = calc_rho(self.exp_data)
         fit_result = self.model(rho.index.to_numpy(), self.fitted_params)
 
         return go.FigureWidget(pd.DataFrame({'ρr': rho.apply(lambda x: x.real),
                                              'ρi': rho.apply(lambda x: x.imag),
                                              'ρcr': fit_result.rho.real,
                                              'ρci': fit_result.rho.imag},
-                                             index=rho.index).plot())
+                                            index=rho.index).plot())
+
+    def get_model_data(self,
+                       params:Parameters=None,
+                       append_exp_data=False) -> pd.DataFrame:     
+        """Gets the data from the provided modle with the provided parameters.
+        If no parameters are provided, the fitted parameters are used
+        (which default to the initial parameters if no fit has been triggered).
+
+        Args:
+            params (Parameters, optional): 
+                The parameters to calculate the model with. 
+                If not provided, the fitted parameters are used.
+                Defaults to None.
+            append_exp_data (bool, optional):
+                Appends the experimental data if set to True.
+                Defaults to False.
+
+        Returns:
+            pd.DataFrame: The model results
+        """
+        if params is None:
+            fit_result = self.model(self.exp_data.index.to_numpy(), self.fitted_params)
+            desc = 'fit'
+        else:
+            fit_result = self.model(self.exp_data.index.to_numpy(), params)
+            desc = 'model'
+
+        if append_exp_data:
+            return pd.concat([self.exp_data,
+                              pd.DataFrame({f'Ψ_{desc}': fit_result.psi,
+                                            f'Δ_{desc}': fit_result.delta},
+                                            index=self.exp_data.index)], axis=1)
+
+        return pd.DataFrame({f'Ψ_{desc}': fit_result.psi,
+                             f'Δ_{desc}': fit_result.delta},
+                             index=self.exp_data.index)
 
     def __init__(self,
-                 exp_data:pd.DataFrame,
-                 params:Parameters,
-                 model:Callable[[npt.NDArray, Parameters], Result],
-                 angle:float = 70):
+                 exp_data: pd.DataFrame,
+                 params: Parameters,
+                 model: Callable[[npt.NDArray, Parameters], Result],
+                 angle: float = 70) -> None:
         """Intialize the psi/delta fitting class
 
         Args:
             exp_data (pd.DataFrame): The dataframe containing an experimental mueller matrix.
                                      It should contain 2 columns with labels Ψ and Δ.
             params (Parameters): Fitting start parameters
-            model (Callable[[npt.NDArray, Parameters], Result]): A function taking wavelengths as first parameter and fitting parameters as second,
-                                                     which returns a pyEllis Result object.
-                                                     This function contains the actual model which should be fitted.
-            angle (float, optional): The angle of incident of the measurement. 
+            model (Callable[[npt.NDArray, Parameters], Result]):
+                A function taking wavelengths as first parameter and fitting parameters as second,
+                which returns a pyEllis Result object.
+                This function contains the actual model which should be fitted.
+            angle (float, optional): The angle of incident of the measurement.
                                      Used to calculate the Pseudo-Dielectric function.
                                      Defaults to 70.
-        """        
+        """
+        super().__init__()
         self.model = model
         self.exp_data = exp_data
         self.params = params
         self.fitted_params = params.copy()
         self.angle = angle
+        self.param_widgets = {}
+        self.selector = widgets.Dropdown()
+        self.last_params = None
         self.fig = go.FigureWidget(pd.concat([exp_data,
-                    pd.DataFrame({'Ψ_tmm': model(exp_data.index, params).psi,
-                                 'Δ_tmm': model(exp_data.index, params).delta},
-                                 index=exp_data.index)]).plot(backend='plotly'))
+                                              pd.DataFrame({'Ψ_tmm': model(exp_data.index, params).psi,
+                                                            'Δ_tmm': model(exp_data.index, params).delta},
+                                                           index=exp_data.index)]).plot(backend='plotly'))
         self.fig.update_layout(yaxis_title="Ψ/Δ (°)", xaxis_title="Wavelength (nm)")
 
         self.update_dict = {'Psi/Delta': self.set_psi_delta,
                             'Rho': self.set_rho,
                             'Pseudo Diel.': self.set_pseudo_diel}
 
         self.create_widgets()
 
-def fit(exp_data:pd.DataFrame,
-        params:Parameters,
-        angle:float = 70) -> Callable[[npt.NDArray, Parameters], Result]:
+
+def fit(exp_data: pd.DataFrame,
+        params: Parameters,
+        angle: float = 70) -> Callable[[npt.NDArray, Parameters], Result]:
     """A parameters decorator for fitting psi/delta valus. Displays an ipywidget float box for
     each fitting parameter and an interactive plot to estimate parameters.
 
     Args:
         exp_data (pd.DataFrame): The dataframe containing an experimental mueller matrix.
                                  It should contain 2 columns with labels Ψ and Δ.
         params (Parameters): Fitting start parameters
-        angle (float, optional): The angle of incident of the measurement. 
+        angle (float, optional): The angle of incident of the measurement.
                                  Used to calculate the Pseudo-Dielectric function.
                                  Defaults to 70.
 
     Returns:
-        Callable[[npt.NDArray, Parameters], Result]: A function taking wavelengths as first parameter and fitting parameters as second,
-                                                     which returns a pyEllis Result object.
-                                                     This function contains the actual model which should be fitted and is automatically
-                                                     provided when used as a decorator.
-    """        
+        Callable[[npt.NDArray, Parameters], Result]:
+            fitting parameters as second,
+            which returns a pyEllis Result object.
+            This function contains the actual model which should be fitted and is automatically
+            provided when used as a decorator.
+    """
     return lambda model: FitRho(exp_data, params, model, angle)
```

### Comparing `pyElli-0.9.1/src/elli/fitting/params_hist.py` & `pyElli-0.9.2/src/elli/fitting/params_hist.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """ParmsHist provides a wrapper around lmfit.Parameters
 to keep track of the changes made to the parameters."""
 # Encoding: utf-8
 import copy
 from typing import List
 from lmfit import Parameters
 
+
 class ParamsHist(Parameters):
     """A wrapper around lmfit.Parameters to keep track of the changes made to the parameters."""
-    _history = []
-    _max_length = 50
 
-    def _clone_and_append(self):
-        if len(self._history) >= self._max_length:
-            self._history = self._history[1:]
-        clone = copy.deepcopy(self)
-        self.history.append(clone)
+    def __init__(self) -> None:
+        super().__init__()
+        self._history = []
+        self._max_length = 50
 
     @property
     def history(self) -> List[Parameters]:
         """Gets the entire history
 
         Returns:
             List[Parameters]: The history
         """
         return self._history
 
-    def clear_history(self):
+    def clear_history(self) -> None:
         """Clears the parameters history"""
         self._history = []
 
     @property
     def history_len(self) -> int:
         """The current length of the history
 
@@ -44,15 +42,15 @@
 
         Returns:
             int: The maximum length of the history
         """
         return self._max_length
 
     @max_history_len.setter
-    def max_history_len(self, history_len:int):
+    def max_history_len(self, history_len: int) -> None:
         """Sets the maximum history length. If the current
         history length is greater than the new history length the history
         gets truncated.
 
         Args:
             history_len (int): The new history length
 
@@ -64,33 +62,57 @@
 
         if history_len < 1:
             raise ValueError('History length must be greater than 0')
 
         self._history = self._history[-history_len:]
         self._max_length = history_len
 
-    def revert(self, hist_pos:int):
-        """Reverts to an older history version
+    def revert(self, hist_pos: int) -> None:
+        """Reverts to an older history version and keeps the entire history.
 
         Args:
             hist_pos (int): The history position to revert to.
         """
-        self.update(self._history[hist_pos])
+        if len(self._history) > (hist_pos % len(self._history)):
+            self.update(self._history[hist_pos])
+
+    def pop(self):
+        """Gets to the previous history version and deletes the current element."""
+        if len(self._history) > 0:
+            curr_params = self.copy()
+            self.update(self._history[-1])
+            self._history = self._history[:-1]
+
+            return curr_params
+        return None
 
-    def update_value(self, key:str, value:float):
+    def update_value(self, key: str, value: float) -> None:
         """Updates a parameter and keeps track of the change in history
 
         Args:
             key (str): The key to be updated
             value (float): The value the key should be updated to
         """
-        self._clone_and_append()
-        super(ParamsHist, self).__getitem__(key).value = value
+        self.commit()
+        super().__getitem__(key).value = value
 
-    def tracked_add(self, *args, **kwargs):
+    def update_params(self, parameters) -> None:
+        """Updates the current paramters from a lmfit parameters object.
+
+        Args:
+            parameters (lmfit.Parameters):
+                The lmfit paramters object to update the values from.
+        """
+        self.commit()
+        self.update(parameters)
+
+    def tracked_add(self, *args, **kwargs) -> None:
         """Adds a parameter and keeps track of the change in history"""
-        self._clone_and_append()
-        super(ParamsHist, self).add(*args, **kwargs)
+        self.commit()
+        super().add(*args, **kwargs)
 
-    def commit(self):
-        """Saves the current parameter set to history."""        
-        self._clone_and_append()
+    def commit(self) -> None:
+        """Saves the current parameter set to history."""
+        if len(self._history) >= self._max_length:
+            self._history = self._history[1:]
+        clone = copy.deepcopy(self)
+        self.history.append(clone)
```

### Comparing `pyElli-0.9.1/src/elli/materials.py` & `pyElli-0.9.2/src/elli/materials.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,57 +5,75 @@
 import numpy.typing as npt
 from numpy.lib.scimath import sqrt
 
 from .dispersions import DispersionLaw
 
 
 class Material(ABC):
-    """Base class for materials (abstract class).
-
-    Method that should be implemented in derived classes:
-    * get_tensor(lbda) : returns the permittivity tensor for wavelength 'lbda'.
+    """Base class for materials (abstract).
     """
 
     @abstractmethod
     def get_tensor(self, lbda: npt.ArrayLike) -> npt.NDArray:
+        """Gets the permittivity tensor of the marterial for wavelength 'lbda'.
+
+        Args:
+            lbda (npt.ArrayLike): Single value or array of wavelengths (in nm).
+
+        Returns:
+            npt.NDArray: Permittivity tensor.
+        """
         pass
 
     def get_refractive_index(self, lbda: npt.ArrayLike) -> npt.NDArray:
-        """Returns refractive index for wavelength 'lbda'."""
+        """Gets the refractive index tensor for wavelength 'lbda'.
+
+        Args:
+            lbda (npt.ArrayLike): Single value or array of wavelengths (in nm).
+
+        Returns:
+            npt.NDArray: Refractive index tensor.
+        """
         return sqrt(self.get_tensor(lbda))
 
 
 class SingleMaterial(Material):
-    """Base class for single materials (abstract class).
-
-    Method that should be implemented in derived classes:
-    * get_tensor(lbda) : returns the permittivity tensor for wavelength 'lbda'.
+    """Base class for non mixed materials (abstract).
     """
 
     law_x = None
     law_y = None
     law_z = None
     rotated = False
     rotation_matrix = None
 
     @abstractmethod
     def set_dispersion(self) -> None:
-        """Creates a new material -- abstract class"""
-        raise NotImplementedError("Should be implemented in derived classes")
+        """Sets dipsersion relation of the material.
+        """
+        pass
 
     def set_rotation(self, r: npt.NDArray) -> None:
-        """Rotates the Material.
+        """Sets rotation of the Material.
 
-        'r' : rotation matrix (from rotation_Euler() or others)
-        """
+        Args:
+            r (npt.NDArray): rotation matrix (from rotation_Euler() or others)
+        """       
         self.rotated = True
         self.rotation_matrix = r
 
     def get_tensor(self, lbda: npt.ArrayLike) -> npt.NDArray:
-        """Returns permittivity tensor matrix for the desired wavelength."""
+        """Gets the permittivity tensor of the marterial for wavelength 'lbda'.
+
+        Args:
+            lbda (npt.ArrayLike): Single value or array of wavelengths (in nm).
+
+        Returns:
+            npt.NDArray: Permittivity tensor.
+        """
         # Check for shape of lbda
         shape = np.shape(lbda)
         if shape == ():
             i = 1
         else:
             i = shape[0]
 
@@ -73,114 +91,164 @@
         return epsilon
 
 
 class IsotropicMaterial(SingleMaterial):
     """Isotropic material."""
 
     def __init__(self, law: DispersionLaw) -> None:
-        """Creates isotropic material with dispersion law.
+        """Creates isotropic material with a dispersion law.
 
-        'law' : Dispersion law object
+        Args:
+            law (DispersionLaw): Dispersion relation of all three crystal directions.
         """
         self.set_dispersion(law)
 
     def set_dispersion(self, law: DispersionLaw) -> None:
+        """Sets dipsersion relation of the isotropic material.
+
+        Args:
+            law (DispersionLaw): Dispersion relation of all three crystal directions.
+        """
         self.law_x = law
         self.law_y = law
         self.law_z = law
 
 
 class UniaxialMaterial(SingleMaterial):
     """Uniaxial material."""
 
     def __init__(self, law_o: DispersionLaw, law_e: DispersionLaw) -> None:
-        """Creates a uniaxial material with dispersion law.
+        """Creates a uniaxial material with two dispersion laws.
 
-        'law_o' : dispersion law for ordinary crystal axes (x and y direction)
-        'law_o' : dispersion law for extraordinary crystal axis (z direction)
+        Args:
+            law_o (DispersionLaw): Dispersion relation for ordinary crystal axes (x and y direction).
+            law_e (DispersionLaw): Dispersion relation for extraordinary crystal axis (z direction).
         """
         self.set_dispersion(law_o, law_e)
 
     def set_dispersion(self, law_o: DispersionLaw, law_e: DispersionLaw) -> None:
+        """Sets dipsersion relations of the uniaxial material.
+
+        Args:
+            law_o (DispersionLaw): Dispersion relation for ordinary crystal axes (x and y direction).
+            law_e (DispersionLaw): Dispersion relation for extraordinary crystal axis (z direction).
+        """
         self.law_x = law_o
         self.law_y = law_o
         self.law_z = law_e
 
 
 class BiaxialMaterial(SingleMaterial):
     """Biaxial material."""
 
     def __init__(self, law_x: DispersionLaw, law_y: DispersionLaw, law_z: DispersionLaw) -> None:
-        """Creates a biaxial material with dispersion law.
+        """Creates a biaxial material with three dispersion laws.
 
-        'law_x' : dispersion law for x axis
-        'law_y' : dispersion law for y axis
-        'law_z' : dispersion law for z axis
+        Args:
+            law_x (DispersionLaw): Dispersion relation for x crystal axes.
+            law_y (DispersionLaw): Dispersion relation for y crystal axes.
+            law_z (DispersionLaw): Dispersion relation for z crystal axes.
         """
         self.set_dispersion(law_x, law_y, law_z)
 
     def set_dispersion(self, law_x: DispersionLaw, law_y: DispersionLaw, law_z: DispersionLaw) -> None:
+        """Sets dipsersion relations of the biaxial material.
+
+        Args:
+            law_x (DispersionLaw): Dispersion relation for x crystal axes.
+            law_y (DispersionLaw): Dispersion relation for y crystal axes.
+            law_z (DispersionLaw): Dispersion relation for z crystal axes.
+        """
         self.law_x = law_x
         self.law_y = law_y
         self.law_z = law_z
 
 
 class MixtureMaterial(Material):
-    """Abstract Class for mixed materials"""
+    """Abstract Class for mixed materials."""
 
     host_material = None
     guest_material = None
     fraction = None
 
     def __init__(self, host_material: Material, guest_material: Material, fraction: float) -> None:
-        """Creates a material mixture from two materials
+        """Creates a material mixture from two materials.
 
-        'host_material': Host Material
-        'guest_material': Material incorporated in the host
-        'fraction' : Fraction of the guest material (Range 0 - 1) 
+        Args:
+            host_material (Material): Host Material.
+            guest_material (Material): Material incorporated in the host.
+            fraction (float): Fraction of the guest material (Range 0 - 1).
         """
         self.set_constituents(host_material, guest_material)
         self.set_fraction(fraction)
 
     def set_constituents(self, host_material: Material, guest_material: Material) -> None:
-        """ Sets Materials in the mixture
-        'host_material': Host Material
-        'guest_material': Material incorporated in the host
+        """Sets Materials in the mixture.
+
+        Args:
+            host_material (Material): Host Material.
+            guest_material (Material): Material incorporated in the host.
         """
         self.host_material = host_material
         self.guest_material = guest_material
 
     def set_fraction(self, fraction: float) -> None:
-        """ Sets fraction and checks if fraction is in range from 0 to 1.
-        'fraction' : Fraction of the guest material (Range 0 - 1)
+        """Sets fraction and checks if fraction is in range from 0 to 1.
+
+        Args:
+            fraction (float): Fraction of the guest material (Range 0 - 1).
         """
         if not 0 <= fraction <= 1:
             raise ValueError('Fractions not in range from 0 to 1')
 
         self.fraction = fraction
 
     @abstractmethod
     def get_tensor(self, lbda: npt.ArrayLike) -> npt.NDArray:
+        """Gets the permittivity tensor of the marterial for wavelength 'lbda'.
+
+        Args:
+            lbda (npt.ArrayLike): Single value or array of wavelengths (in nm).
+
+        Returns:
+            npt.NDArray: Permittivity tensor.
+        """
         pass
 
 
 class VCAMaterial(MixtureMaterial):
     """Mixture Material approximated with a simple virtual crystal like average."""
 
     def get_tensor(self, lbda: npt.ArrayLike) -> npt.NDArray:
+        """Gets the permittivity tensor of the marterial for wavelength 'lbda'.
+
+        Args:
+            lbda (npt.ArrayLike): Single value or array of wavelengths (in nm).
+
+        Returns:
+            npt.NDArray: Permittivity tensor.
+        """
         epsilon = self.host_material.get_tensor(lbda) * (1 - self.fraction) \
             + self.guest_material.get_tensor(lbda) * self.fraction
         return epsilon
 
 
 class MaxwellGarnetEMA(MixtureMaterial):
     """Mixture Material approximated with the Maxwell Garnet formula.
        It is valid for spherical inclusions with small volume fraction.
     """
 
     def get_tensor(self, lbda: npt.ArrayLike) -> npt.NDArray:
+        """Gets the permittivity tensor of the marterial for wavelength 'lbda'.
+
+        Args:
+            lbda (npt.ArrayLike): Single value or array of wavelengths (in nm).
+
+        Returns:
+            npt.NDArray: Permittivity tensor.
+        """
         e_h = self.host_material.get_tensor(lbda)
         e_g = self.guest_material.get_tensor(lbda)
 
         epsilon = e_h * (2 * self.fraction * (e_g - e_h) + e_g + 2 * e_h) \
             / (2 * e_h + e_g - self.fraction * (e_g - e_h))
         return epsilon
```

### Comparing `pyElli-0.9.1/src/elli/math.py` & `pyElli-0.9.2/src/elli/math.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/src/elli/plot/mueller_matrix.py` & `pyElli-0.9.2/src/elli/plot/mueller_matrix.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/src/elli/plot/structure.py` & `pyElli-0.9.2/src/elli/plot/structure.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/src/elli/result.py` & `pyElli-0.9.2/src/elli/result.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/src/elli/solver.py` & `pyElli-0.9.2/src/elli/solver.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/src/elli/solver2x2.py` & `pyElli-0.9.2/src/elli/solver2x2.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             return None
         return self._rtotp / self._rtots
 
     @property
     def delta(self):
         if self._rtotp is None or self._rtots is None:
             return None
-        return -np.angle(-self._rtotp / self._rtots, deg=True)
+        return -np.angle(self._rtotp / self._rtots, deg=True)
 
     @property
     def R(self):
         return np.abs(self._rtotp + self._rtots)
 
     def list_snell(self, n_list):
         angles = arcsin(n_list[0] * np.sin(np.deg2rad(self.theta_i)) / n_list)
```

### Comparing `pyElli-0.9.1/src/elli/solver4x4.py` & `pyElli-0.9.2/src/elli/solver4x4.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/src/elli/spectraray.py` & `pyElli-0.9.2/src/elli/spectraray.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,48 +9,53 @@
 
     def __init__(self, path: str) -> None:
         self.spectraray_path = path
 
     def loadDispersionTable(self, fname: str) -> DispersionTableEpsilon:
         start = 0
         stop = 0
-        with open(self.spectraray_path + fname, 'r') as f:
-            line = f.readline()
+        with open(self.spectraray_path + fname, 'r', encoding='utf8') as file:
+            line = file.readline()
             cnt = 0
             while line:
                 if line.strip() == 'Begin of array':
                     start = cnt + 1
                 if line.strip() == 'End of array':
                     stop = cnt
-                line = f.readline()
+                line = file.readline()
                 cnt += 1
 
                 if line.startswith('Units='):
                     x_unit = line.split('=')[1].split(',')[0]
 
         df = pd.read_csv(self.spectraray_path + fname,
                          delim_whitespace=True,
                          skiprows=start, nrows=stop-start,
                          index_col=0, usecols=[0, 1, 2],
                          names=[x_unit, 'ϵ1', 'ϵ2'])
 
         if x_unit == 'Wavelength':
             return DispersionTableEpsilon(df.index, df.loc[:, 'ϵ1'] + 1j * df.iloc[:, 'ϵ2'])
-        elif x_unit == 'eV':
-            return DispersionTableEpsilon(SpectraRay.eV2nm(df.index), df.loc[:, 'ϵ1'] + 1j * df.loc[:, 'ϵ2'])
+        return DispersionTableEpsilon(SpectraRay.eV2nm(df.index), df.loc[:, 'ϵ1'] + 1j * df.loc[:, 'ϵ2'])
 
     @staticmethod
     def read_psi_delta_file(fname: str, decimal: str = '.') -> pd.DataFrame:
-        return pd.read_csv(fname,
-                           index_col=0,
-                           sep=r'\s+',
-                           decimal=decimal,
-                           usecols=[0, 1, 2],
-                           names=['Wavelength', 'Ψ', 'Δ'],
-                           skiprows=1)
+        psi_delta = pd.read_csv(fname,
+                                index_col=0,
+                                sep=r'\s+',
+                                decimal=decimal,
+                                usecols=[0, 1, 2],
+                                names=['Wavelength', 'Ψ', 'Δ'],
+                                skiprows=1)
+
+        psi_delta.loc[:,'Δ'] = psi_delta.loc[:,'Δ'].where(
+            psi_delta.loc[:,'Δ'] <= 180, psi_delta.loc[:,'Δ'] - 360
+        )
+
+        return psi_delta
 
     @staticmethod
     def read_mmatrix(fname: str, decimal: str = '.') -> pd.DataFrame:
         """Read a Mueller matrix from a Sentech ASCII file.
         Save the file in SpectraRay under Save As -> Ascii (.txt)"""
         mueller_matrix = pd.read_csv(fname,
                                      sep=r'\s+',
```

### Comparing `pyElli-0.9.1/src/elli/structure.py` & `pyElli-0.9.2/src/elli/structure.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/src/elli/utils.py` & `pyElli-0.9.2/src/elli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Encoding: utf-8
 import pandas as pd
 import numpy as np
 import scipy.constants as sc
 from numpy.lib.scimath import sqrt
 
-def calcPseudoDiel(rho, angle: float, output: str = 'eps') -> pd.DataFrame:
+def calc_pseudo_diel(rho, angle: float, output: str = 'eps') -> pd.DataFrame:
     """Calculates the pseudo dielectric function of a measurement from rho.
 
     Args:
-        rho (pandas.DataFrame): Measurement DataFrame containing rho as complex number as column and wavelength as index
+        rho (pandas.DataFrame):
+            Measurement DataFrame containing rho as complex number as column and wavelength as index
         angle (float): Angle of measurement in degree
         output (str, optional): Output format for dielectric function.
             'n': refractive index,
             'eps': Dielectic function as two-column pandas.DataFrame,
             'epsi': Dielectric function as imaginary number.
             Defaults to 'eps'.
 
@@ -31,15 +32,16 @@
         return eps
 
     return pd.concat({'ϵ1': eps.apply(lambda x: x.real),
                       'ϵ2': eps.apply(lambda x: x.imag)}, axis=1)
 
 
 def calc_rho(psi_delta: pd.DataFrame) -> pd.DataFrame:
-    """Calculate rho from a Psi-Delta DataFrame. The Psi-Delta DataFrame should be structured as follows:
+    """Calculate rho from a Psi-Delta DataFrame.
+            The Psi-Delta DataFrame should be structured as follows:
         index: Wavelength
         column 'Ψ': Psi from measurement
         column 'Δ': Delta from measurement
 
         This format is as returned from SpectraRay.read_psi_delta_file(...).
 
     Args:
```

### Comparing `pyElli-0.9.1/src/pyElli.egg-info/PKG-INFO` & `pyElli-0.9.2/src/pyElli.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: pyElli
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python implementation of Berremans 4x4 matrix method
 Home-page: https://github.com/PyEllips/pyElli/
 Author: dobener
 Author-email: florian.dobener@physik.uni-giessen.de
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://pyelli.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/PyEllips/pyElli/
 Project-URL: Download, https://github.com/PyEllips/pyElli/releases
-Project-URL: Changelog, https://github.com/PyEllips/pyElli/blob/master/CHANGELOG.rst
+Project-URL: Changelog, https://github.com/PyEllips/pyElli/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/PyEllips/pyElli/issues
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: PLOT
 Provides-Extra: testing
 License-File: LICENSE.txt
 
-[![Pytest](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml/badge.svg)](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml) [![Documentation Status](https://readthedocs.org/projects/pyelli/badge/?version=latest)](https://pyelli.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/pyElli)](https://pypi.org/project/pyElli/)
+[![Pytest](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml/badge.svg)](https://github.com/PyEllips/pyElli/actions/workflows/pytest.yml) [![Documentation Status](https://readthedocs.org/projects/pyelli/badge/?version=latest)](https://pyelli.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/pyElli)](https://pypi.org/project/pyElli/) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5702469.svg)](https://doi.org/10.5281/zenodo.5702469)
 
 
 # pyElli
 PyElli is a numerical solver for spectral ellipsometry employing well-known 2x2 and 4x4 algorithms.
 It is intended for a broad case of problems including simple fitting of layered structures, anisotropic layers and any other light interaction with layered 1D structures.
 It serves as a system for the day to day ellipsometry task at hand and makes fitting a breeze.
 
 ## Features
 - A multitude of models to approximate the dielectric function of your material.
 - Build up your structure easily from materials and layers.
-- Simulate reflectiona and transmission spectra, ellipsometric parameters and Mueller matrices.
+- Simulate reflection and transmission spectra, ellipsometric parameters and Mueller matrices.
 - Utilities to quickly convert, plot and fit your measurement data.
-- Powerfull when necessary, editable and expandeble.
+- Powerful when necessary, editable and expandable.
 
 ## How to get it
 The installers for all releases are available at the [Python Package Index (PyPI)](https://pypi.org/project/pyElli/).
 
 To install run:
 ```sh
 pip install pyElli
@@ -44,16 +44,22 @@
 
 A complete environment for pyElli is also available as a [Docker Container](https://hub.docker.com/r/domna/pyelli).
 From a running Docker installation simply run:
 ```sh
 docker pull domna/pyelli
 ```
 
-The source code is hosted on [GitHub](https://github.com/PyEllips/pyElli), to install from source run:
+To install the latest development version use:
+```sh
+pip install git+https://github.com/PyEllips/pyElli.git
+```
+
+The source code is hosted on [GitHub](https://github.com/PyEllips/pyElli), to manually install from source, download and run inside the downloaded folder:
 ```sh
 python setup.py install
 ```
 
 ## Acknowledgements
 - Based on Olivier Castany's [Berreman4x4](https://github.com/Berreman4x4/Berreman4x4)
 - Solver2x2 based on Steve Byrnes's [tmm](https://github.com/sbyrnes321/tmm)
 
+
```

### Comparing `pyElli-0.9.1/src/pyElli.egg-info/SOURCES.txt` & `pyElli-0.9.2/src/pyElli.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .coveragerc
 .gitignore
 .readthedocs.yml
+.zenodo.json
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 Dockerfile
 LICENSE.txt
 README.md
 pyproject.toml
@@ -43,23 +44,18 @@
 examples/Liquid crystals/twisted-nematic.ipynb
 examples/Liquid crystals/twisted-nematic.py
 examples/Liquid crystals/validation-cholesteric.ipynb
 examples/Liquid crystals/validation-cholesteric.py
 examples/SiO2_Si Mueller Matrix/SiO2_Si Mueller Matrix.ipynb
 examples/SiO2_Si Mueller Matrix/Si_Aspnes.mat
 examples/SiO2_Si Mueller Matrix/Wafer_MM_70.txt
-examples/SiO2_Si Mueller Matrix/.ipynb_checkpoints/SiO2_Si Mueller Matrix-checkpoint.ipynb
-examples/SiO2_Si Mueller Matrix/.ipynb_checkpoints/Si_Aspnes-checkpoint.mat
-examples/SiO2_Si Mueller Matrix/.ipynb_checkpoints/Wafer_MM_70-checkpoint.txt
 examples/TiO2 Fit/Si_Aspnes.mat
 examples/TiO2 Fit/TiO2 Multilayerfit.ipynb
 examples/TiO2 Fit/TiO2 Multilayerfit.md
 examples/TiO2 Fit/TiO2_400cycles.txt
-examples/TiO2 Fit/.ipynb_checkpoints/TiO2 Multilayerfit-checkpoint.ipynb
-examples/TiO2 Fit/.ipynb_checkpoints/TiO2 Multilayerfit-checkpoint.md
 examples/Total internal reflection/FrustratedTIR-angle.ipynb
 examples/Total internal reflection/FrustratedTIR-angle.py
 examples/Total internal reflection/FrustratedTIR-thickness.ipynb
 examples/Total internal reflection/FrustratedTIR-thickness.py
 examples/Total internal reflection/TIR.ipynb
 examples/Total internal reflection/TIR.py
 src/elli/__init__.py
@@ -72,14 +68,15 @@
 src/elli/solver.py
 src/elli/solver2x2.py
 src/elli/solver4x4.py
 src/elli/spectraray.py
 src/elli/structure.py
 src/elli/utils.py
 src/elli/fitting/__init__.py
+src/elli/fitting/decorator.py
 src/elli/fitting/decorator_mmatrix.py
 src/elli/fitting/decorator_psi_delta.py
 src/elli/fitting/params_hist.py
 src/elli/plot/__init__.py
 src/elli/plot/mueller_matrix.py
 src/elli/plot/structure.py
 src/pyElli.egg-info/PKG-INFO
```

### Comparing `pyElli-0.9.1/tests/benchmark_propagators_TiO2.py` & `pyElli-0.9.2/tests/benchmark_propagators_TiO2.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/tests/test_bragg_mirror.py` & `pyElli-0.9.2/tests/test_bragg_mirror.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/tests/test_internal_reflection.py` & `pyElli-0.9.2/tests/test_internal_reflection.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/tests/test_liquid_crystals.py` & `pyElli-0.9.2/tests/test_liquid_crystals.py`

 * *Files identical despite different names*

### Comparing `pyElli-0.9.1/tests/test_uniaxial_crystals.py` & `pyElli-0.9.2/tests/test_uniaxial_crystals.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,20 +88,22 @@
                        [0,         0,          n_x,     n_x]]],
                       dtype=np.complex128)
 
         np.testing.assert_array_almost_equal(self.Lt, lt, decimal=3)
 
     def test_transition_matrix_with_halfspace(self):
         # Fujiwara Original
-        tmatrix = np.array([[[-1.946 - 1j*3.588, 1.668 - 1j*1.548, 0.273 + 1j * 0.03, 0.63 - 1j*0.148],
+        tmatrix = np.array([[[-1.946 - 1j*3.588, 1.668 - 1j*1.548,
+                                0.273 + 1j * 0.03, 0.63 - 1j*0.148],
                             [1.614 + 1j*1.679, -1.989 + 1j*3.435, -
                                 0.301 - 1j*0.064, -0.861 - 1j*0.101],
                             [0.065 - 1j*0.086, 0.039 + 1j*0.097, -
                                 0.71 - 1j*3.486, -0.003 - 1j*1.266],
-                            [0.167 + 1j*0.403, -0.593 - 1j*0.386, -0.369 + 1j*1.199, -1.66 + 1j * 3.094]]])
+                            [0.167 + 1j*0.403, -0.593 - 1j*0.386,
+                                -0.369 + 1j*1.199, -1.66 + 1j * 3.094]]])
 
         np.testing.assert_array_almost_equal(
             self.Li @ self.Tp @ self.Lt, tmatrix, decimal=1)
 
     def test_jones_calculation(self):
         jones_matrix = np.array([[[-0.311 - 0.161j, -0.107 - 0.002j],
                                   [0.042 - 0.036j, -0.551 + 0.151j]]])
```

### Comparing `pyElli-0.9.1/tox.ini` & `pyElli-0.9.2/tox.ini`

 * *Files identical despite different names*

